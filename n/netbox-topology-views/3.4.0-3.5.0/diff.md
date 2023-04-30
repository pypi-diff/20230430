# Comparing `tmp/netbox-topology-views-3.4.0.tar.gz` & `tmp/netbox-topology-views-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-topology-views-3.4.0.tar", last modified: Fri Apr 28 14:09:41 2023, max compression
+gzip compressed data, was "netbox-topology-views-3.5.0.tar", last modified: Sun Apr 30 18:15:10 2023, max compression
```

## Comparing `netbox-topology-views-3.4.0.tar` & `netbox-topology-views-3.5.0.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views/api/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/migrations/0002_individualoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.006084 netbox-topology-views-3.4.0/netbox_topology_views/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.006084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.018084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/database.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/
--rw-r--r--   0 runner    (1001) docker     (123)   349261 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.010084 netbox-topology-views-3.4.0/netbox_topology_views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/images.html
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/individual_options.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/site_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/toasts.html
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31580 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/netbox_topology_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:09:41.014084 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-28 14:09:40.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-28 14:09:41.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:09:40.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 14:09:40.000000 netbox-topology-views-3.4.0/netbox_topology_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 14:09:41.034084 netbox-topology-views-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-28 14:09:29.000000 netbox-topology-views-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/0002_individualoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.742385 netbox-topology-views-3.5.0/netbox_topology_views/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.742385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   349737 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.742385 netbox-topology-views-3.5.0/netbox_topology_views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/individual_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/site_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/toasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31247 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/setup.py
```

### Comparing `netbox-topology-views-3.4.0/LICENSE` & `netbox-topology-views-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/PKG-INFO` & `netbox-topology-views-3.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.4.0
+Version: 3.5.0
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -110,31 +110,33 @@
 
 ## Use
 
 Go to the plugins tab in the navbar and click topology or go to `$NETBOX_URL/plugins/netbox_topology_views/` to view your topologies
 
 Select your options for the topology view:
 
-![selection_options](https://user-images.githubusercontent.com/20901110/220410144-5633d24c-6383-4cba-8d6d-ba77ef3d3cdd.png)
+![topology_options](https://user-images.githubusercontent.com/20901110/235302073-234c3ef7-2c2b-4d0c-a674-9909d490d7ea.png)
 
 <dl>
     <dt>Save Coordinates</dt>
     <dd>Save the coordinates of devices in the topology view.</dd>
     <dt>Show Unconnected</dt>
     <dd>Show devices that have no connections or for which no connection is displayed. This option depends on other parameters like 'Show Cables' and 'Show Logical Connections'.</dd>
-    <dt>Show Circuit Terminations</dt>
-    <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Cables</dt>
     <dd>Show connections between interfaces, front / rear ports, etc., that are connected with one or more cables. These connections are displayed as solid lines in the color of the cable.</dd> 
     <dt>Show Logical Connections</dt>
     <dd>Show logical connections between interfaces (referred to as Interface Connections in NetBox) in the topology view. Where the path between
         interfaces includes multiple cables (e.g., via patch panels), only the end interface connections are shown, not the 
         intermediate front / rear port connections, etc. This is similar to what was referred to as 'end-to-end' connections in previous versions. These connections are displayed as yellow dotted lines.</dd>
     <dt>Show redundant Cable and Locigal Connection</dt>
     <dd>Shows a logical connection (in addition to a cable), even if a cable is directly connected. Leaving this option disabled prevents that redundant display. This option only has an effect if 'Show Logical Connections' is activated.</dd>
+    <dt>Show Neighbors</dt>
+    <dd>Adds neighbors to the filter result set automatically. Link peers will be added if 'Show Cables' is ticked, far-end terminations will be added if 'Show Logical Connections' is ticked.</dd>
+    <dt>Show Circuit Terminations</dt>
+    <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Power Feeds</dt>
     <dd>Displays connections between power outlets and power ports. These connections are displayed as solid lines in the color of the cable. This option depends on 'Show Cables'.</dd>
     <dt>Show Wireless Links</dt>
     <dd>Displays wireless connections. These connections are displayed as blue dotted lines.</dd>
 </dl>
     
 ### Update
@@ -161,16 +163,7 @@
  + dcim | site | view
  + dcim | device role | view
  + dcim | device role | add
  + dcim | device role | change
 
  To view `/plugins/netbox_topology-views/individualoptions`:
  + netbox topology views | individualoptions | change
-
- ## Icons info
-
-Power icons created by [Freepik - Flaticon](https://www.flaticon.com/free-icons/power).
-
-Power icons created by [Flat Icons - Flaticon](https://www.flaticon.com/free-icons/power)
-
-Provider icons created by [Good Ware - Flaticon](https://www.flaticon.com/free-icons/provider)
-
```

### Comparing `netbox-topology-views-3.4.0/README.md` & `netbox-topology-views-3.5.0/netbox_topology_views.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: netbox-topology-views
+Version: 3.5.0
+Summary: An NetBox plugin to create Topology maps
+Home-page: https://github.com/mattieserver/netbox-topology-views
+Author: Mattijs Vanhaverbeke
+License: Apache 2.0
+Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
+Keywords: netbox-plugin
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Netbox Topology Views Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-topology-views) ![Downloads](https://img.shields.io/pypi/dm/netbox-topology-views)
 
 Create topology views/maps from your devices in netbox.
 The connections are based on the cables you created in netbox.
 Support to filter on name, site, tag and device role.
@@ -95,31 +110,33 @@
 
 ## Use
 
 Go to the plugins tab in the navbar and click topology or go to `$NETBOX_URL/plugins/netbox_topology_views/` to view your topologies
 
 Select your options for the topology view:
 
-![selection_options](https://user-images.githubusercontent.com/20901110/220410144-5633d24c-6383-4cba-8d6d-ba77ef3d3cdd.png)
+![topology_options](https://user-images.githubusercontent.com/20901110/235302073-234c3ef7-2c2b-4d0c-a674-9909d490d7ea.png)
 
 <dl>
     <dt>Save Coordinates</dt>
     <dd>Save the coordinates of devices in the topology view.</dd>
     <dt>Show Unconnected</dt>
     <dd>Show devices that have no connections or for which no connection is displayed. This option depends on other parameters like 'Show Cables' and 'Show Logical Connections'.</dd>
-    <dt>Show Circuit Terminations</dt>
-    <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Cables</dt>
     <dd>Show connections between interfaces, front / rear ports, etc., that are connected with one or more cables. These connections are displayed as solid lines in the color of the cable.</dd> 
     <dt>Show Logical Connections</dt>
     <dd>Show logical connections between interfaces (referred to as Interface Connections in NetBox) in the topology view. Where the path between
         interfaces includes multiple cables (e.g., via patch panels), only the end interface connections are shown, not the 
         intermediate front / rear port connections, etc. This is similar to what was referred to as 'end-to-end' connections in previous versions. These connections are displayed as yellow dotted lines.</dd>
     <dt>Show redundant Cable and Locigal Connection</dt>
     <dd>Shows a logical connection (in addition to a cable), even if a cable is directly connected. Leaving this option disabled prevents that redundant display. This option only has an effect if 'Show Logical Connections' is activated.</dd>
+    <dt>Show Neighbors</dt>
+    <dd>Adds neighbors to the filter result set automatically. Link peers will be added if 'Show Cables' is ticked, far-end terminations will be added if 'Show Logical Connections' is ticked.</dd>
+    <dt>Show Circuit Terminations</dt>
+    <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Power Feeds</dt>
     <dd>Displays connections between power outlets and power ports. These connections are displayed as solid lines in the color of the cable. This option depends on 'Show Cables'.</dd>
     <dt>Show Wireless Links</dt>
     <dd>Displays wireless connections. These connections are displayed as blue dotted lines.</dd>
 </dl>
     
 ### Update
@@ -146,16 +163,7 @@
  + dcim | site | view
  + dcim | device role | view
  + dcim | device role | add
  + dcim | device role | change
 
  To view `/plugins/netbox_topology-views/individualoptions`:
  + netbox topology views | individualoptions | change
-
- ## Icons info
-
-Power icons created by [Freepik - Flaticon](https://www.flaticon.com/free-icons/power).
-
-Power icons created by [Flat Icons - Flaticon](https://www.flaticon.com/free-icons/power)
-
-Provider icons created by [Good Ware - Flaticon](https://www.flaticon.com/free-icons/provider)
-
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/__init__.py` & `netbox-topology-views-3.5.0/netbox_topology_views/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class TopologyViewsConfig(PluginConfig):
     name = "netbox_topology_views"
     verbose_name = "Topology views"
     description = "An plugin to render topology maps"
-    version = "3.4.0"
+    version = "3.5.0"
     author = "Mattijs Vanhaverbeke"
     author_email = "author@example.com"
     base_url = "netbox_topology_views"
     required_settings = []
     default_settings = {
         "static_image_directory": "netbox_topology_views/img",
         "allow_coordinates_saving": False,
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/api/serializers.py` & `netbox-topology-views-3.5.0/netbox_topology_views/api/serializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,8 +21,9 @@
     class Meta:
         model = DeviceRole
         fields = ("name", "slug", "color", "vm_role", "description")
 
 class IndividualOptionsSerializer(NetBoxModelSerializer):
     class Meta:
         model = IndividualOptions
-        fields = ("ignore_cable_type", "show_unconnected", "show_cables", "show_logical_connections", "show_single_cable_logical_conns", "show_circuit", "show_power", "show_wireless", "draw_default_layout")
+        fields = ("ignore_cable_type", "show_unconnected", "show_cables", "show_logical_connections", "show_single_cable_logical_conns", "show_neighbors", "show_circuit", "show_power", "show_wireless", "draw_default_layout")
+
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/filters.py` & `netbox-topology-views-3.5.0/netbox_topology_views/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/forms.py` & `netbox-topology-views-3.5.0/netbox_topology_views/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,18 @@
             None,
             (
                 "q",
                 "filter_id",
                 "save_coords",
                 "show_unconnected",
                 "show_cables",
-                "show_circuit",
                 "show_logical_connections",
                 "show_single_cable_logical_conns",
+                "show_neighbors",
+                "show_circuit",
                 "show_power",
                 "show_wireless",
             ),
         ),
         (
             None,
             (
@@ -114,47 +115,51 @@
         required=False,
         disabled=(not settings.PLUGINS_CONFIG["netbox_topology_views"]["allow_coordinates_saving"] or settings.PLUGINS_CONFIG["netbox_topology_views"]["always_save_coordinates"]),
         initial=(settings.PLUGINS_CONFIG["netbox_topology_views"]["always_save_coordinates"])
     )
     show_unconnected = forms.BooleanField(
         label=_("Show Unconnected"), required=False, initial=False
     )
+    show_cables = forms.BooleanField(
+        label =_("Show Cables"), required=False, initial=False
+    )
     show_logical_connections = forms.BooleanField(
         label =_("Show Logical Connections"), required=False, initial=False
     )
     show_single_cable_logical_conns = forms.BooleanField(
         label =_("Show redundant Cable and Locigal Connection"), required=False, initial=False
     )
-    show_cables = forms.BooleanField(
-        label =_("Show Cables"), required=False, initial=False
-    )
-    show_wireless = forms.BooleanField(
-        label =_("Show Wireless Links"), required=False, initial=False
+    show_neighbors = forms.BooleanField(
+        label =_("Show Neighbors"), required=False, initial=False
     )
     show_circuit = forms.BooleanField(
         label=_("Show Circuit Terminations"), required=False, initial=False
     )
     show_power = forms.BooleanField(
         label=_("Show Power Feeds"), required=False, initial=False
     )
+    show_wireless = forms.BooleanField(
+        label =_("Show Wireless Links"), required=False, initial=False
+    )
 
 class IndividualOptionsForm(NetBoxModelForm):
     fieldsets = (
         (
             None,
             (
                 "user_id",
                 "ignore_cable_type",
                 "preselected_device_roles",
                 "preselected_tags",
                 "show_unconnected",
                 "show_cables",
-                "show_circuit",
                 "show_logical_connections",
                 "show_single_cable_logical_conns",
+                "show_neighbors",
+                "show_circuit",
                 "show_power",
                 "show_wireless",
                 "draw_default_layout",
             ),
         ),
     )
 
@@ -211,14 +216,22 @@
         required = False,
         initial=False,
         help_text=_("Shows a logical connection (in addition to a cable), "
             "even if a cable is directly connected. Leaving this option "
             "disabled prevents that redundant display. This option only "
             "has an effect if 'Show Logical Connections' is activated.")
     )
+    show_neighbors = forms.BooleanField(
+        label =_("Show Neighbors"), 
+        required=False, 
+        initial=False,
+        help_text=_("Adds neighbors to the filter result set automatically. "
+            "Link peers will be added if 'Show Cables' is ticked, far-end "
+            "terminations will be added if 'Show Logical Connections' is ticked.")
+    )
     show_circuit = forms.BooleanField(
         label=_("Show Circuit Terminations"), 
         required=False, 
         initial=False,
         help_text=_("Displays connections between circuit terminations. "
             "These connections are displayed as blue dashed lines.")
     )
@@ -244,9 +257,10 @@
         help_text=_("Enable this option if you want to draw the topology on "
             "the initial load (when you go to the topology plugin page).")
     )
 
     class Meta:
         model = IndividualOptions
         fields = [
-            'user_id', 'ignore_cable_type', 'preselected_device_roles', 'preselected_tags', 'show_unconnected', 'show_cables', 'show_logical_connections', 'show_single_cable_logical_conns', 'show_circuit', 'show_power', 'show_wireless', 'draw_default_layout'
-        ]
+            'user_id', 'ignore_cable_type', 'preselected_device_roles', 'preselected_tags', 'show_unconnected', 'show_cables', 'show_logical_connections', 'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 'show_wireless', 'draw_default_layout'
+        ]
+
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/migrations/0001_initial.py` & `netbox-topology-views-3.5.0/netbox_topology_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/migrations/0002_individualoptions.py` & `netbox-topology-views-3.5.0/netbox_topology_views/migrations/0002_individualoptions.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/models.py` & `netbox-topology-views-3.5.0/netbox_topology_views/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,17 @@
     )
     show_logical_connections = models.BooleanField(
         default=False
     )
     show_single_cable_logical_conns = models.BooleanField(
         default=False
     )
+    show_neighbors = models.BooleanField(
+        default=False
+    )
     show_circuit = models.BooleanField(
         default=False
     )
     show_power = models.BooleanField(
         default=False
     )
     show_wireless = models.BooleanField(
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/navigation.py` & `netbox-topology-views-3.5.0/netbox_topology_views/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/signals.py` & `netbox-topology-views-3.5.0/netbox_topology_views/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/database.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/router.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/server.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/app.js` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -58,15 +58,15 @@
                 } catch (h) {
                     s(h)
                 }
             },
             a = d => d.done ? i(d.value) : Promise.resolve(d.value).then(o, r);
         a((t = t.apply(n, e)).next())
     });
-    var si = ei((ja, ii) => {
+    var si = ei((Va, ii) => {
         typeof ii != "undefined" && (ii.exports = ne);
 
         function ne(n) {
             if (n) return Ln(n)
         }
 
         function Ln(n) {
@@ -427,15 +427,15 @@
                         T.pushRun(m, E), T.mergeRuns(), _ -= E, m += E
                     } while (_ !== 0);
                     T.forceMergeRuns()
                 }
             }
         })
     });
-    var oo = ei((fd, so) => {
+    var oo = ei((gd, so) => {
         so.exports = io()
     });
     var Ps = ti(si());
 
     function fe() {
         return fe = Object.assign || function(n) {
             for (var e = 1; e < arguments.length; e++) {
@@ -1406,15 +1406,15 @@
                     recognizers: _s.concat()
                 }, i))
             };
             return n.VERSION = "2.0.17-rc", n.DIRECTION_ALL = es, n.DIRECTION_DOWN = Qe, n.DIRECTION_LEFT = dt, n.DIRECTION_RIGHT = ht, n.DIRECTION_UP = lt, n.DIRECTION_HORIZONTAL = pe, n.DIRECTION_VERTICAL = He, n.DIRECTION_NONE = Pt, n.DIRECTION_DOWN = Qe, n.INPUT_START = ee, n.INPUT_MOVE = Re, n.INPUT_END = K, n.INPUT_CANCEL = se, n.STATE_POSSIBLE = Nt, n.STATE_BEGAN = le, n.STATE_CHANGED = et, n.STATE_ENDED = Oe, n.STATE_RECOGNIZED = ve, n.STATE_CANCELLED = gt, n.STATE_FAILED = ge, n.Manager = Cs, n.Input = $e, n.TouchAction = is, n.TouchInput = ci, n.MouseInput = ui, n.PointerEventInput = ls, n.TouchMouseInput = fs, n.SingleTouchInput = wr, n.Recognizer = mt, n.AttrRecognizer = tt, n.Tap = fi, n.Pan = pi, n.Swipe = ms, n.Pinch = ys, n.Rotate = bs, n.Press = vs, n.on = ut, n.off = ft, n.each = be, n.merge = Er, n.extend = ks, n.bindFn = Ss, n.assign = Ae, n.inherit = xr, n.bindFn = Ss, n.prefixed = Ot, n.toArray = pt, n.inArray = We, n.uniqueArray = li, n.splitStr = ct, n.boolOrFn = Dt, n.hasParent = di, n.addEventListeners = ut, n.removeEventListeners = ft, n.defaults = Ae({}, ws, {
                 preset: _s
             }), n
         }(),
-        Wa = Os.defaults,
+        qa = Os.defaults,
         Is = Os;
     var gi = Symbol("DELETE");
 
     function Ms(n, ...e) {
         return Ds({}, n, ...e)
     }
 
@@ -13183,22 +13183,36 @@
 
     function La() {
         let n = kn.querySelector("canvas"),
             e = document.createElement("a"),
             t = n.toDataURL(Aa);
         e.href = t, e.download = "topology", document.body.appendChild(e), e.click(), document.body.removeChild(e)
     }
-    var Ra = new MutationObserver(n => n.forEach(e => {
+    var Ra = document.querySelector("#btnDownloadXml");
+    Ra.addEventListener("click", n => {
+        Ha()
+    });
+
+    function Ha() {
+        let n = document.createElement("a");
+        fetch("/api/plugins/netbox_topology_views/xml-export/?" + new URLSearchParams(window.location.search)).then(e => e.text()).then(e => {
+            var t = new Blob([e], {
+                type: "text/plain"
+            });
+            n.setAttribute("href", window.URL.createObjectURL(t)), n.setAttribute("download", "topology.xml"), n.dataset.downloadurl = ["text/plain", n.download, n.href].join(":"), n.click()
+        })
+    }
+    var ja = new MutationObserver(n => n.forEach(e => {
         if (!Ge || e.type !== "attributes" || e.attributeName !== "data-netbox-color-mode" || !(e.target instanceof HTMLElement)) return;
         let {
             netboxColorMode: t
         } = e.target.dataset;
         qi.nodes.font.color = t === "dark" ? "#fff" : "#000", Ge.setOptions(qi)
     }));
-    Ra.observe(document.documentElement, {
+    ja.observe(document.documentElement, {
         attributes: !0,
         attributeFilter: ["data-netbox-color-mode"]
     });
 })();
 /*! Hammer.JS - v2.0.17-rc - 2019-12-16
  * http://naver.github.io/egjs
  *
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map` & `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html` & `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 <link rel="stylesheet" href="{% static 'netbox_topology_views/css/app.css' %}">
 
 <div class="modal-header">
     <h5 class="modal-title">Topology Views</h5>
     <div class="controls">
     	<div class="control-group">
 			{% block extra_controls %}{% endblock %}
+			<a id="btnDownloadXml" class="btn btn-sm btn-info" href="#">
+				<i class="mdi mdi-download"></i>
+				Download XML
+			</a>
 			<a id="btnDownloadImage" class="btn btn-sm btn-info" href="#">
 				<i class="mdi mdi-download"></i>
-				Download
+				Download PNG
 			</a>
             <a class="btn  btn-sm btn-danger" data-bs-dismiss="modal">
                 <i class="mdi mdi-close-thick"></i>
                 Close
             </a>
     	</div>
 	</div>
@@ -32,8 +36,8 @@
     }
 </style>
 
 <script type="text/javascript">
     const brokenImage = '{{ broken_image }}';
     const topologyData = {{ topology_data | safe }};
 </script>
-<script src="{% static 'netbox_topology_views/js/app.js' %}?ver={{ epoch }} " defer></script>
+<script src="{% static 'netbox_topology_views/js/app.js' %}?ver={{ epoch }} " defer></script>
```

#### html2text {}

```diff
@@ -1,7 +1,10 @@
 {% load static %}
 
 ** Topology Views **
 {% block extra_controls %}{% endblock %}
- Download
+ Download_XML
+
+ Download_PNG
 
  Close
+
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/images.html` & `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/images.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/index.html` & `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 <link rel="stylesheet" href="{% static 'netbox_topology_views/css/app.css' %}">
 {% endblock %} 
 
 {% block controls %}
   <div class="controls">
     	<div class="control-group">
 			{% block extra_controls %}{% endblock %}
+			<a id="btnDownloadXml" class="btn btn-sm btn-info" href="#">
+				<i class="mdi mdi-download"></i>
+				Download XML
+			</a>
 			<a id="btnDownloadImage" class="btn btn-sm btn-info" href="#">
 				<i class="mdi mdi-download"></i>
-				Download
+				Download PNG
 			</a>
     	</div>
 	</div>
 {% endblock controls %}
 
 {% block tabs %}
 	<ul class="nav nav-tabs px-3">
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 {% extends 'base/layout.html' %} {% load buttons %} {% load render_table from
 django_tables2 %} {% load static %} {% load perms %} {% load helpers %} {%
 block title %}Topology Views{% endblock %} {% block head %}
 
  {% endblock %} {% block controls %}
 {% block extra_controls %}{% endblock %}
- Download
+ Download_XML
+
+ Download_PNG
 {% endblock controls %} {% block tabs %}
     * {% block tab_items %}
     *  Network
     * {% if filter_form %}
     *  Filters {% if filter_form %}{% badge filter_form.changed_data|length
       bg_color="blue" %}{% endif %}
     * {% endif %} {% endblock tab_items %}
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/templates/netbox_topology_views/toasts.html` & `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/toasts.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/urls.py` & `netbox-topology-views-3.5.0/netbox_topology_views/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views/views.py` & `netbox-topology-views-3.5.0/netbox_topology_views/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from functools import reduce
 from typing import DefaultDict, Dict, Optional, Union
 import time
+from itertools import chain
 
 from utilities.htmx import is_htmx
 from circuits.models import Circuit, CircuitTermination
 from dcim.models import (
     Cable,
     CableTermination,
     Device,
@@ -34,14 +35,16 @@
 from netbox_topology_views.models import RoleImage, IndividualOptions
 from netbox_topology_views.utils import (
     CONF_IMAGE_DIR,
     find_image_url,
     get_model_role,
     get_model_slug,
     image_static_url,
+    LinePattern,
+    get_query_settings
 )
 
 
 
 def get_image_for_entity(entity: Union[Device, Circuit, PowerPanel, PowerFeed]):
     is_device = isinstance(entity, Device)
     query = (
@@ -194,32 +197,33 @@
         else termination_b["termination_device_name"]
     )
 
     edge = {}
     edge["id"] = edge_id
     edge["from"] = termination_a["device_id"]
     edge["to"] = termination_b["device_id"]
+    edge["color"] = '#2b7ce9'
     title = "Cable"
 
     if circuit is not None:
         edge["dashes"] = True
         title = f"Circuit provider: {circuit['provider_name']}<br>Termination"
 
     elif wireless is not None:
-        edge["dashes"] = [2, 10, 2, 10]
+        edge["dashes"] = LinePattern().wireless
         title = "Wireless Connection"
 
     elif power is not None:
-        edge["dashes"] = [5, 5, 3, 3]
+        edge["dashes"] = LinePattern().power
         title = "Power Connection"
 
     elif interface is not None:
         title = "Interface Connection"
         edge["width"] = 3
-        edge["dashes"] = [1, 10, 1, 10]
+        edge["dashes"] = LinePattern().logical
         edge["color"] = '#f1c232'
         edge["href"] = interface.get_absolute_url() + "trace"
         
     edge[
         "title"
     ] = f"{title} between<br>{cable_a_dev_name} [{cable_a_name}]<br>{cable_b_dev_name} [{cable_b_name}]"
 
@@ -256,14 +260,15 @@
     individualOptions: IndividualOptions,
     show_unconnected: bool,
     save_coords: bool,
     show_cables: bool,
     show_circuit: bool,
     show_logical_connections: bool,
     show_single_cable_logical_conns: bool,
+    show_neighbors: bool,
     show_power: bool,
     show_wireless: bool,
 ):
     
     supported_termination_types = []
     for t in IndividualOptions.CHOICES:
         supported_termination_types.append(t[1])
@@ -283,14 +288,39 @@
     interface_ids = DefaultDict(dict)
 
     ignore_cable_type = individualOptions.ignore_cable_type
 
     device_ids = [d.pk for d in queryset]
     site_ids = [d.site_id for d in queryset]
 
+    if show_neighbors:
+        interfaces = Interface.objects.filter(
+            Q(device_id__in=device_ids)
+        )
+        frontports = FrontPort.objects.filter(
+            Q(device_id__in=device_ids)
+        )
+        rearports = RearPort.objects.filter(
+            Q(device_id__in=device_ids)
+        )
+
+        ports = chain(interfaces, frontports, rearports)
+        for port in ports:
+            for link_peer in port.link_peers:
+                if link_peer.device.id not in device_ids:
+                    device_ids.append(link_peer.device.id)
+
+        if show_logical_connections:
+            path_complete_interfaces = Interface.objects.filter(
+                Q(_path__is_complete=True) & Q(device_id__in=device_ids)
+            )
+            for path_complete_interface in path_complete_interfaces:
+                for connected_endpoint in path_complete_interface.connected_endpoints:
+                    device_ids.append(connected_endpoint.device.id)
+
     if show_circuit:
         circuit_terminations = CircuitTermination.objects.filter(
             Q(site_id__in=site_ids) | Q(provider_network__isnull=False)
         ).prefetch_related("provider_network", "circuit")
         for circuit_termination in circuit_terminations:
             circuit_termination: CircuitTermination
             if (
@@ -592,73 +622,30 @@
         topo_data = None
 
         individualOptions, created = IndividualOptions.objects.get_or_create(
             user_id=request.user.id,
         )
 
         if request.GET:
-            save_coords = False
-            if "save_coords" in request.GET:
-                if request.GET["save_coords"] == "on":
-                    save_coords = True
-            # General options overrides
-            if save_coords == True and settings.PLUGINS_CONFIG["netbox_topology_views"]["allow_coordinates_saving"] == False:
-                save_coords = False
-                messages.warning(request, "Coordinate saving not allowed. Setting has been overridden")
-            elif settings.PLUGINS_CONFIG["netbox_topology_views"]["always_save_coordinates"] == True:
-                save_coords = True
-
-            # Individual options
-            show_unconnected = False
-            if "show_unconnected" in request.GET:
-                if request.GET["show_unconnected"] == "on":
-                    show_unconnected = True
-
-            show_power = False
-            if "show_power" in request.GET:
-                if request.GET["show_power"] == "on":
-                    show_power = True
-
-            show_circuit = False
-            if "show_circuit" in request.GET:
-                if request.GET["show_circuit"] == "on":
-                    show_circuit = True
-
-            show_logical_connections = False
-            if "show_logical_connections" in request.GET:
-                if request.GET["show_logical_connections"] == "on" :
-                    show_logical_connections = True
-
-            show_single_cable_logical_conns = False
-            if "show_single_cable_logical_conns" in request.GET:
-                if request.GET["show_single_cable_logical_conns"] == "on" :
-                    show_single_cable_logical_conns = True
-
-            show_cables = False
-            if "show_cables" in request.GET:
-                if request.GET["show_cables"] == "on" :
-                    show_cables = True
-
-            show_wireless = False
-            if "show_wireless" in request.GET:
-                if request.GET["show_wireless"] == "on" :
-                    show_wireless = True
 
+            save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, show_neighbors = get_query_settings(request)
+            
             if not "draw_init" in request.GET or "draw_init" in request.GET and request.GET["draw_init"].lower() == "true":
                 topo_data = get_topology_data(
-                    self.queryset,
-                    individualOptions,
-                    show_unconnected,
-                    save_coords,
-                    show_cables,
-                    show_circuit,
-                    show_logical_connections,
-                    show_single_cable_logical_conns,
-                    show_power,
-                    show_wireless,
+                    queryset=self.queryset,
+                    individualOptions=individualOptions,
+                    save_coords=save_coords,
+                    show_unconnected=show_unconnected,
+                    show_cables=show_cables,
+                    show_logical_connections=show_logical_connections,
+                    show_single_cable_logical_conns=show_single_cable_logical_conns,
+                    show_neighbors=show_neighbors,
+                    show_circuit=show_circuit,
+                    show_power=show_power,
+                    show_wireless=show_wireless,
                 )
             
         else:
             # No GET-Request in URL. We most likely came here from the navigation menu.
             preselected_device_roles = IndividualOptions.objects.get(id=individualOptions.id).preselected_device_roles.all().values_list('id', flat=True)
             preselected_tags = IndividualOptions.objects.get(id=individualOptions.id).preselected_tags.all().values_list(Lower('name'), flat=True)
 
@@ -666,14 +653,15 @@
             q.setlist("device_role_id", list(preselected_device_roles))
             q.setlist("tag", list(preselected_tags))
 
             if individualOptions.show_unconnected: q['show_unconnected'] = "on"
             if individualOptions.show_cables: q['show_cables'] = "on"
             if individualOptions.show_logical_connections: q['show_logical_connections'] = "on"
             if individualOptions.show_single_cable_logical_conns: q['show_single_cable_logical_conns'] = "on"
+            if individualOptions.show_neighbors: q['show_neighbors'] = "on"
             if individualOptions.show_circuit: q['show_circuit'] = "on"
             if individualOptions.show_power: q['show_power'] = "on"
             if individualOptions.show_wireless: q['show_wireless'] = "on"
             if individualOptions.draw_default_layout: 
                 q['draw_init'] = "true"
             else:
                 q['draw_init'] = "false"
@@ -686,26 +674,26 @@
             return render(
                 request,
                 "netbox_topology_views/htmx_topology.html",
                 {
                     "filter_form": DeviceFilterForm(request.GET, label_suffix=""),
                     "topology_data": json.dumps(topo_data),
                     "broken_image": find_image_url("role-unknown"),
-                    "epoch": int(time.time()),
+                    "epoch": int(time.time())
                 },
             )
 
         return render(
             request,
             "netbox_topology_views/index.html",
             {
                 "filter_form": DeviceFilterForm(request.GET, label_suffix=""),
                 "topology_data": json.dumps(topo_data),
                 "broken_image": find_image_url("role-unknown"),
-                "model": self.model,
+                "model": self.model
             },
         )
 
 
 CONFIG = settings.PLUGINS_CONFIG["netbox_topology_views"]
 ADDITIONAL_ROLES = (PowerPanel, PowerFeed, Circuit)
 
@@ -788,14 +776,15 @@
                 'ignore_cable_type': tuple(queryset.ignore_cable_type.translate({ord(i): None for i in '[]\''}).split(', ')),
                 'preselected_device_roles': IndividualOptions.objects.get(id=queryset.id).preselected_device_roles.all(),
                 'preselected_tags': IndividualOptions.objects.get(id=queryset.id).preselected_tags.all(),
                 'show_unconnected': queryset.show_unconnected,
                 'show_cables': queryset.show_cables, 
                 'show_logical_connections': queryset.show_logical_connections,
                 'show_single_cable_logical_conns': queryset.show_single_cable_logical_conns,
+                'show_neighbors': queryset.show_neighbors,
                 'show_circuit': queryset.show_circuit,
                 'show_power': queryset.show_power,
                 'show_wireless': queryset.show_wireless,
                 'draw_default_layout': queryset.draw_default_layout,
             },
         )
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views.egg-info/PKG-INFO` & `netbox-topology-views-3.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: netbox-topology-views
-Version: 3.4.0
-Summary: An NetBox plugin to create Topology maps
-Home-page: https://github.com/mattieserver/netbox-topology-views
-Author: Mattijs Vanhaverbeke
-License: Apache 2.0
-Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
-Keywords: netbox-plugin
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Netbox Topology Views Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-topology-views) ![Downloads](https://img.shields.io/pypi/dm/netbox-topology-views)
 
 Create topology views/maps from your devices in netbox.
 The connections are based on the cables you created in netbox.
 Support to filter on name, site, tag and device role.
@@ -110,31 +95,33 @@
 
 ## Use
 
 Go to the plugins tab in the navbar and click topology or go to `$NETBOX_URL/plugins/netbox_topology_views/` to view your topologies
 
 Select your options for the topology view:
 
-![selection_options](https://user-images.githubusercontent.com/20901110/220410144-5633d24c-6383-4cba-8d6d-ba77ef3d3cdd.png)
+![topology_options](https://user-images.githubusercontent.com/20901110/235302073-234c3ef7-2c2b-4d0c-a674-9909d490d7ea.png)
 
 <dl>
     <dt>Save Coordinates</dt>
     <dd>Save the coordinates of devices in the topology view.</dd>
     <dt>Show Unconnected</dt>
     <dd>Show devices that have no connections or for which no connection is displayed. This option depends on other parameters like 'Show Cables' and 'Show Logical Connections'.</dd>
-    <dt>Show Circuit Terminations</dt>
-    <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Cables</dt>
     <dd>Show connections between interfaces, front / rear ports, etc., that are connected with one or more cables. These connections are displayed as solid lines in the color of the cable.</dd> 
     <dt>Show Logical Connections</dt>
     <dd>Show logical connections between interfaces (referred to as Interface Connections in NetBox) in the topology view. Where the path between
         interfaces includes multiple cables (e.g., via patch panels), only the end interface connections are shown, not the 
         intermediate front / rear port connections, etc. This is similar to what was referred to as 'end-to-end' connections in previous versions. These connections are displayed as yellow dotted lines.</dd>
     <dt>Show redundant Cable and Locigal Connection</dt>
     <dd>Shows a logical connection (in addition to a cable), even if a cable is directly connected. Leaving this option disabled prevents that redundant display. This option only has an effect if 'Show Logical Connections' is activated.</dd>
+    <dt>Show Neighbors</dt>
+    <dd>Adds neighbors to the filter result set automatically. Link peers will be added if 'Show Cables' is ticked, far-end terminations will be added if 'Show Logical Connections' is ticked.</dd>
+    <dt>Show Circuit Terminations</dt>
+    <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Power Feeds</dt>
     <dd>Displays connections between power outlets and power ports. These connections are displayed as solid lines in the color of the cable. This option depends on 'Show Cables'.</dd>
     <dt>Show Wireless Links</dt>
     <dd>Displays wireless connections. These connections are displayed as blue dotted lines.</dd>
 </dl>
     
 ### Update
@@ -161,16 +148,7 @@
  + dcim | site | view
  + dcim | device role | view
  + dcim | device role | add
  + dcim | device role | change
 
  To view `/plugins/netbox_topology-views/individualoptions`:
  + netbox topology views | individualoptions | change
-
- ## Icons info
-
-Power icons created by [Freepik - Flaticon](https://www.flaticon.com/free-icons/power).
-
-Power icons created by [Flat Icons - Flaticon](https://www.flaticon.com/free-icons/power)
-
-Provider icons created by [Good Ware - Flaticon](https://www.flaticon.com/free-icons/provider)
-
```

### Comparing `netbox-topology-views-3.4.0/netbox_topology_views.egg-info/SOURCES.txt` & `netbox-topology-views-3.5.0/netbox_topology_views.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 netbox_topology_views.egg-info/top_level.txt
 netbox_topology_views/api/__init__.py
 netbox_topology_views/api/serializers.py
 netbox_topology_views/api/urls.py
 netbox_topology_views/api/views.py
 netbox_topology_views/migrations/0001_initial.py
 netbox_topology_views/migrations/0002_individualoptions.py
+netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
 netbox_topology_views/migrations/__init__.py
 netbox_topology_views/static/netbox_topology_views/css/app.css
 netbox_topology_views/static/netbox_topology_views/css/vendor.css
 netbox_topology_views/static/netbox_topology_views/img/LICENSE
 netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
 netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
 netbox_topology_views/static/netbox_topology_views/img/backup.svg
```

