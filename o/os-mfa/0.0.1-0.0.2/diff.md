# Comparing `tmp/os-mfa-0.0.1.tar.gz` & `tmp/os-mfa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-mfa-0.0.1.tar", last modified: Sun Apr 30 10:02:43 2023, max compression
+gzip compressed data, was "os-mfa-0.0.2.tar", last modified: Sun Apr 30 13:45:14 2023, max compression
```

## Comparing `os-mfa-0.0.1.tar` & `os-mfa-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 10:02:43.121470 os-mfa-0.0.1/
--rw-r--r--   0 simon     (1000) simon     (1000)     1060 2023-04-30 09:59:27.000000 os-mfa-0.0.1/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)     9138 2023-04-30 10:02:43.121470 os-mfa-0.0.1/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     8599 2023-04-30 10:00:36.000000 os-mfa-0.0.1/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 10:02:43.121470 os-mfa-0.0.1/os_mfa/
--rw-r--r--   0 simon     (1000) simon     (1000)       22 2023-04-30 09:52:50.000000 os-mfa-0.0.1/os_mfa/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1763 2023-04-30 09:55:50.000000 os-mfa-0.0.1/os_mfa/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4641 2023-04-30 09:52:50.000000 os-mfa-0.0.1/os_mfa/config_helpers.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 10:02:43.121470 os-mfa-0.0.1/os_mfa.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     9138 2023-04-30 10:02:43.000000 os-mfa-0.0.1/os_mfa.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      349 2023-04-30 10:02:43.000000 os-mfa-0.0.1/os_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-04-30 10:02:43.000000 os-mfa-0.0.1/os_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       48 2023-04-30 10:02:43.000000 os-mfa-0.0.1/os_mfa.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       29 2023-04-30 10:02:43.000000 os-mfa-0.0.1/os_mfa.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-04-30 10:02:43.000000 os-mfa-0.0.1/os_mfa.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)     1160 2023-04-30 09:57:37.000000 os-mfa-0.0.1/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-30 10:02:43.121470 os-mfa-0.0.1/setup.cfg
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 10:02:43.121470 os-mfa-0.0.1/tests/
--rw-r--r--   0 simon     (1000) simon     (1000)     1106 2023-04-30 09:40:55.000000 os-mfa-0.0.1/tests/test_create_long_term_config.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1220 2023-04-30 09:40:47.000000 os-mfa-0.0.1/tests/test_create_token_config.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1060 2023-04-30 09:59:27.000000 os-mfa-0.0.2/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)     7230 2023-04-30 13:45:14.461474 os-mfa-0.0.2/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     6691 2023-04-30 13:25:11.000000 os-mfa-0.0.2/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/os_mfa/
+-rw-r--r--   0 simon     (1000) simon     (1000)       22 2023-04-30 13:44:34.000000 os-mfa-0.0.2/os_mfa/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1763 2023-04-30 09:55:50.000000 os-mfa-0.0.2/os_mfa/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     4996 2023-04-30 13:35:30.000000 os-mfa-0.0.2/os_mfa/config_helpers.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/os_mfa.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7230 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      358 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       48 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       59 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-04-30 13:45:14.000000 os-mfa-0.0.2/os_mfa.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)     1273 2023-04-30 13:44:32.000000 os-mfa-0.0.2/pyproject.toml
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-30 13:45:14.461474 os-mfa-0.0.2/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-30 13:35:56.000000 os-mfa-0.0.2/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-30 13:45:14.461474 os-mfa-0.0.2/tests/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1107 2023-04-30 12:54:26.000000 os-mfa-0.0.2/tests/test_create_long_term_config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1221 2023-04-30 12:54:26.000000 os-mfa-0.0.2/tests/test_create_token_config.py
```

### Comparing `os-mfa-0.0.1/LICENSE` & `os-mfa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `os-mfa-0.0.1/PKG-INFO` & `os-mfa-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,196 +1,227 @@
 Metadata-Version: 2.1
 Name: os-mfa
-Version: 0.0.1
+Version: 0.0.2
 Summary: A minimal utility for managing cli authentication with openstack more securely and conveniently
 Author-email: Simon Merrick <s.m3rrick@gmail.com>
 Project-URL: Homepage, https://github.com/iokiwi/os-mfa
 Keywords: openstack,mfa,auth
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# OS-MFA: Easily manage one or more openstack credentials for command line and programmatic access
+# os-mfa
 
-os-mfa makes using MFA with cli/programmatic authentication with OpenStack easier and more secure by combining the convenience of durable authentication session persistence with better credential management hygiene though automatically managing the lifecycle of authentication tokens in the `clouds.yaml` file.
+Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](broamski/aws-mfa)
 
-Inspired by https://github.com/broamski/aws-mfa
+## What problem does os-mfa solve?
 
-Note: This is currently a proof of concept/Work in progress. Pull requests welcome.
+First some quick background. OpenStack provides two main methods of setting credentials for programmatic authentication:
 
-## In this README
+**A) [Environment variables set via 'openrc.sh' files](https://docs.openstack.org/newton/user-guide/common/cli-set-environment-variables-using-openstack-rc.html)**
 
-* [The Problems this project aims to Address](#the-problems-this-project-aims-to-address)
-* [Installation](#installation)
-  * [Linux](#linux)
-  * [macOS](#macos)
-  * [Windows](#windows)
-* [Quick Start](#quick-start)
-* [How it Works](#how-it-works)
+* 🛡️ Avoids storing passwords in plaintext on disk 👍<br>
+* 🤦 Session credentials are lost if you close or restart your terminal window 👎<br>
+* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎<br>
+* 💔 Not compatible with windows clients 👎<br>
 
-## The Problem(s) this project aims to address
+**B) [clouds.yaml configuration files](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files)**
 
-Openstack provides several methods for configuring authentication for its SDK's and clients including CLI arguments, environment variables and a [clouds.yaml](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files) file.
+ * 🌏 Are accessible in every terminal session 👍
+ * 💪 Are durable to restarts/shutdowns 👍
+ * 💗 Compatible and consistent user experience across platforms 👍
+ * 🙈 Encourages credentials to be stored in plain text 👎
+ * ⌛ Tokens expire after 12 hours and need to be manually refreshed and updated in clouds.yaml 👎
 
-### 1. Using openrc files/environment variables is not durable across terminal sessions
+As we can see both have advantages and disadvantages. But what if we could have the best parts of both options?
 
-For some reason the preferred / default authentication method users are steered towards is using openrc files - non-trivial bash files which set environment variables in your shell session.
+**🌈 os-mfa 🦄 leverages the convenience and durability of using `clouds.yaml` and automates the secure management of credentials and tokens**
 
-Using environment variables to persist your authentication session is not durable across terminal instances or restarts. If you open a new terminal for any reason you will need to re authenticate there with your username, password and MFA token. This becomes very tiresome very quickly.
+ * 🛡️ Avoids storing passwords in plaintext on disk 👍
+ * 🌏 Session credentials are accessible in all terminals sessions 👍
+ * 💪 Are durable to restarts/shutdowns 👍
+ * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
+ * 🤝 Ensures native compatibility with the OpenStack ecosystem 👍
+ * 💗 Compatible and consistent user experience across platforms 👍
 
-### 2. Using clouds.yaml does not work nicely with token authentication or MFA
+## Quick start
 
-Openstack does provide a better, more persisted, authentication mechanism by way of the [clouds.yaml](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files) configuration file.
+Install os-mfa
 
-Switching sessions is then simplified by referencing the cloud config name from `clouds.yaml
-  * Using an cli argument (`--os-cloud=<name>`) 
-  * Setting the `OS_CLOUD` environment variable inline (E.g `OS_CLOUD=<name> <command>`)
-  * Exporting `OS_CLOUD` environnement variable to used by all future commands in that session (`export OS_CLOUD=<name>`)
+```bash
+pip install -U os-mfa
+```
 
-However using `clouds.yaml` files also has some drawbacks.
+Download `clouds.yaml` file from your OpenStack dashboard. For example
 
-* It discourages token based authorization as tokens expire after 12 hours requiring users to constantly manually update clouds.yaml with new tokens.
-* It discourages the use of MFA which requires token based authorization.
-* It encourages storing usernames and passwords in clear text in a file on your machine as this is less friction than using token based authorization.
+ 1. Click API Access https://dashboard.catalystcloud.nz/project/api_access/
+ 2. Click **Download OpenStack RC File** on the top right
+ 3. Select **OpenStack clouds.yaml File** from the drop down
 
-## Best of both worlds: Convenience + Hygiene with os-mfa
 
-This openstack MFA helper combines the convenience of durable authentication session persistence with better security hygiene by utilizing `clouds.yaml` and automatically managing the lifecycle of tokens in the config file allowing users to keep passwords out of their `clouds.yaml` file.
 
-## Quick Start
+Place the file in your current working directory (`.`) or an alternate [location described by the docs](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#clouds-yaml)
 
-1. Obtain a `clouds.yaml` file from the cloud dashboard. For catalyst cloud:
-    * Go to https://dashboard.cloud.catalyst.net.nz/project/api_access/
-    * Hover over `Download OpenStack RC File` on the top right
-    * Click the `OpenStack clouds.yml file`
+Linux
+  * `~/.config/openstack/clouds.yaml`
+  * `/etc/openstack/clouds.yaml`
 
-2. Place your `clouds.yaml` file in one of the following locations detailed in the [upstream docs](https://docs.openstack.org/python-openstackclient/latest/cli/man/openstack.html#config-files)
-    * `./clouds.yaml`
-    * `~/config/openstack/clouds.yaml`
-    * `/etc/openstack/clouds.yaml`
+Windows
+  * `C:\Users\you\.config\openstack\clouds.yaml`
+  * `C:\ProgramData\openstack\clouds.yaml`
 
-3. E.g. Assign and export your config name as the OS_CLOUD environment variable
+E.g.
 
-    ```bash
-    $ export OS_CLOUD=catalystcloud
-    ```
+```yaml
+# /home/john/clouds.yaml
+clouds:
+  catalystcloud:
+    auth:
+      auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
+      project_id: 33735662374f4b7a9621631f2e7e5e15
+      project_name: acme-incorporated
+      user_domain_name: Default
+      username: john.smith@acme.com
+      password: 1ns3curE123!
+    identity_api_version: 3
+    interface: public
+    region_name: nz-hlz-1
+```
 
-4. Authenticate using `os-mfa`
+Run os-mfa
 
-    ```bash
-    $ os-mfa
+```bash
+$ export OS_CLOUD=catalystcloud
+```
+```bash
+$ os-mfa
+Authenticating 'john.smith@example.com' in project 'john-smith'
+Enter Password:
+MFA Code (Press enter to skip): 654321
+Getting token...
+```
 
-    Authenticating 'john.smith@example.com' in project 'john-smith'
-    Enter Password:
-    TOTP (press enter to skip): 654321
-    ```
+```
+$ openstack network list
++--------------------------------------+------------+--------------------------------------------+
+| ID                                   | Name       | Subnets                                    |
++--------------------------------------+------------+--------------------------------------------+
+| f10ad6de-a26d-4c29-8c64-2a7418d47f8f | public-net | 5063aab1-aa08-48b2-b81d-730ac732fc51,      |
+|                                      |            | 8a7fe804-7fbe-43d0-aa1d-cfa03034ef22,      |
+|                                      |            | a1549e09-4176-4322-860c-cadc68608b48       |
++--------------------------------------+------------+--------------------------------------------+
+```
 
-5. Happy OpenStacking
-    ```bash
-    $ openstack server list
-    +---------------+---------------+--------+---------------+---------------+---------+
-    | ID            | Name          | Status | Networks      | Image         | Flavor  |
-    +---------------+---------------+--------+---------------+---------------+---------+
-    | a5d3814a-4f6e | proxy-server- | ACTIVE | proxy-        | N/A (booted   | c1.c1r1 |
-    | -493f-aa03-ac | yohjuqh5vzhm  |        | network-lju2p | from volume)  |         |
-    | 13fdb9a860    |               |        | kokjtsh=10.0. |               |         |
-    |               |               |        | 0.4, 103.***. |               |         |
-    |               |               |        | ***.***       |               |         |
-    +---------------+---------------+--------+---------------+---------------+---------+
-    ```
-## How it works
+If you close/restart or start a new terminal window, resume your openstack session simply by exporting `$OS_CLOUD` again.
 
-With os-mfa we introduce the concept of a "Long Term" configuration, distinguished by a suffix of `-long-term`, which is a copy of the original config that does not contain any secretes such as passwords or tokens.
+```bash
+export OS_CLOUD=catalystcloud
+```
 
-os-mfa will assume ownership and manage the lifecycle of the original config, which we will refer to as the "Ephemeral" config going forward.
+## What happened when we ran os-mfa?
 
-The Long Term and Ephemeral configs are described as follows.
+os-mfa created a *"long-term"* configuration without any passwords or secrets.
 
-|Long Term|Ephemeral|
-|---|---|
-|Managed by you, the user|Managed by os-mfa|
-|Contains project information. Does not contain any secrets|Contains project information + temporary authentication token|
-|Used as basis to create an Ephemeral config but is otherwise ignored|Used by SDK's and clients for authentication|
-|Has a suffix of `-long-term`|Does not have a suffix|
-|Manual changes will be passed on to the Ephemeral config|Manual changes will be overwritten|
+ * *"long-term"* configurations are distinguished with a suffix of `-long-term`
+ * We do not use the long term configs with the openstack client tools.
+ 
+The long term config used as a foundation for authentication by os-mfa which then:
 
-The "Long Term" and "Ephemeral" configs coexist in the same clouds.yaml file. For example: Here's an annotated example of a `clouds.yaml` file with a Long Term and Ephemeral config.
+1) Prompts the user for their password and totp token
+
+2) Swaps the password and totp for an openstack auth token
+
+3) Updates the original configuration to use the new token for authentication
+
+The resulting clouds.yaml should look like this
 
 ```yaml
+# /home/john/clouds.yaml
 clouds:
-    # Managed by os-mfa, Ephemeral.
-    catalystcloud:
-        auth_type: token # Managed by os-mfa
-        auth:
-            auth_url: https://api.nz-hlz-1.catalystcloud.io:5000 # Inherited
-            project_id: 33735662374f4b7a9621631f2e7e5e15         # Inherited
-            project_name: john-smith    # Inherited
-            token: gAAAAABjrN[...]e6vqt # Ephemeral, Managed by os-mfa
-        region_name: nz-hlz-1           # Inherited
-        interface: public               # Inherited
-        identity_api_version: 3         # Inherited
-
-    # Managed by you - the user.
-    catalystcloud-long-term:
-        auth:
-            auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
-            username: john.smith@example.com
-            project_id: 33735662374f4b7a9621631f2e7e5e15
-            project_name: john-smith
-            user_domain_name: Default
-        region_name: nz-hlz-1
-        interface: public
-        identity_api_version: 3
+  catalystcloud:
+    auth:
+      auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
+      project_id: 33735662374f4b7a9621631f2e7e5e15
+      project_name: acme-incorporated
+      token: gAAAAABkTkGx4Dah37lkiGTSEe3-r[...]9dQCVTBRsKjg6NFIYgMYRdAk7TTvIPOaaOE
+    identity_api_version: 3
+    interface: public
+    region_name: nz-hlz-1
+  catalystcloud-long-term:
+    auth:
+      auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
+      project_id: 33735662374f4b7a9621631f2e7e5e15
+      project_name: acme-incorporated
+      user_domain_name: Default
+      username: john.smith@acme.com
+    identity_api_version: 3
+    interface: public
+    region_name: nz-hlz-1
+
 ```
 
-Just the same as openstack sdk's and clients, os-mfa finds your cloud.yaml file by checking the following locations in order:
+## Going further
 
-  * Current directory (`./clouds.yaml`)
-  * `~/config/openstack/clouds.yaml`
-  * `/etc/openstack/clouds.yaml`
 
-We specify which config we are working with by setting the `OS_CLOUD` environment variable.
+### Switching between multiple cloud accounts and sessions
 
-```bash
-export OS_CLOUD=catalystcloud
+```yaml
+clouds:
+  project1-long-term:
+    region: nz-hlz-1
+    auth:
+        project_name: project1
+        username: john.smith@acme.com
+        # ...
+  project2-long-term:
+    region: nz-por-1
+    auth:
+        project_name: project2
+        username: john.smith@acme.com
+        # ...
 ```
 
-When we run os-mfa, it will check our `clouds.yaml` file for a long term profile called `<OS_CLOUD>-long-term`. E.g. `catalystcloud-long-term`.
+After running os-mfa once for each project you can switch between them 
 
-If a long term config does not exist, os-mfa will try to create a default long term config for us based on the original config and sanitized of sensitive values.
+```
+OS_CLOUD=project1
+OS_CLOUD=project2
+```
 
-Once os-mfa finds (or creates) the Long Term Config os-mfa will then:
+## Contributing
 
- 1. Read the project information from the long term config `<OS_CLOUD>-long-term`
- 2. Prompt for your secret credentials (password, MFA code)
- 3. Swap your credentials (username, password and MFA code) for an authorized token
- 4. Create/update a token based Ephemeral configuration in your `clouds.yaml` named `<OS_CLOUD>`
+Nothing special to report, just raise a PR
 
-## Run tests
+### Run tests
 
 ```
 python -m unittest discover
 ```
 
-## Building Package
+### Building Package
 
 Source: https://realpython.com/pypi-publish-python-package/
 
 ```
-python -m pip install pip-tools
+python -m pip install pip-tools build twine bumpver
 pip-compile pyproject.toml
-```
-
-## TODO:
-
- * [/] TBH I am probably going to port this back to python
- * [/] Alert if no clouds.yaml found
- * [/] Better error message if OS_CLOUD not set
- * Non-interactive mode
- * Sanitize long-term config better
- * Store and check expiry of token
-    * Only reauthenticate if token is not valid
-    * -f, --force cli option to force authentication
+python -m build
+twine check dist/*
+twine upload -r testpypi dist/*
+twine upload dist/*
+```
+
+## TODO
+
+ * ☑️ TBH I am probably going to port this back to python
+ * ☑️ Alert if no clouds.yaml found
+ * ☑️ Better error message if OS_CLOUD not set
+ * ☑️ CI/CD
+ * 🟦 Non-interactive mode
+ * 🟦 Sanitize long-term config better
+ * 🟦 Store and check expiry of token
+    * 🟦 Only reauthenticate if token is not valid
+    * 🟦 -f, --force cli option to force authentication
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `os-mfa-0.0.1/README.md` & `os-mfa-0.0.2/os_mfa.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,181 +1,227 @@
-# OS-MFA: Easily manage one or more openstack credentials for command line and programmatic access
+Metadata-Version: 2.1
+Name: os-mfa
+Version: 0.0.2
+Summary: A minimal utility for managing cli authentication with openstack more securely and conveniently
+Author-email: Simon Merrick <s.m3rrick@gmail.com>
+Project-URL: Homepage, https://github.com/iokiwi/os-mfa
+Keywords: openstack,mfa,auth
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# os-mfa
+
+Convenient and secure OpenStack authentication and credential management inspired by [broamski/aws-mfa](broamski/aws-mfa)
+
+## What problem does os-mfa solve?
+
+First some quick background. OpenStack provides two main methods of setting credentials for programmatic authentication:
+
+**A) [Environment variables set via 'openrc.sh' files](https://docs.openstack.org/newton/user-guide/common/cli-set-environment-variables-using-openstack-rc.html)**
+
+* 🛡️ Avoids storing passwords in plaintext on disk 👍<br>
+* 🤦 Session credentials are lost if you close or restart your terminal window 👎<br>
+* 🔒 Sessions can't be shared/accessed across multiple terminal sessions 👎<br>
+* 💔 Not compatible with windows clients 👎<br>
+
+**B) [clouds.yaml configuration files](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files)**
+
+ * 🌏 Are accessible in every terminal session 👍
+ * 💪 Are durable to restarts/shutdowns 👍
+ * 💗 Compatible and consistent user experience across platforms 👍
+ * 🙈 Encourages credentials to be stored in plain text 👎
+ * ⌛ Tokens expire after 12 hours and need to be manually refreshed and updated in clouds.yaml 👎
+
+As we can see both have advantages and disadvantages. But what if we could have the best parts of both options?
+
+**🌈 os-mfa 🦄 leverages the convenience and durability of using `clouds.yaml` and automates the secure management of credentials and tokens**
+
+ * 🛡️ Avoids storing passwords in plaintext on disk 👍
+ * 🌏 Session credentials are accessible in all terminals sessions 👍
+ * 💪 Are durable to restarts/shutdowns 👍
+ * 🔀 Trivially switch between multiple authenticated OpenStack sessions 👍
+ * 🤝 Ensures native compatibility with the OpenStack ecosystem 👍
+ * 💗 Compatible and consistent user experience across platforms 👍
 
-os-mfa makes using MFA with cli/programmatic authentication with OpenStack easier and more secure by combining the convenience of durable authentication session persistence with better credential management hygiene though automatically managing the lifecycle of authentication tokens in the `clouds.yaml` file.
+## Quick start
 
-Inspired by https://github.com/broamski/aws-mfa
+Install os-mfa
 
-Note: This is currently a proof of concept/Work in progress. Pull requests welcome.
-
-## In this README
-
-* [The Problems this project aims to Address](#the-problems-this-project-aims-to-address)
-* [Installation](#installation)
-  * [Linux](#linux)
-  * [macOS](#macos)
-  * [Windows](#windows)
-* [Quick Start](#quick-start)
-* [How it Works](#how-it-works)
+```bash
+pip install -U os-mfa
+```
 
-## The Problem(s) this project aims to address
+Download `clouds.yaml` file from your OpenStack dashboard. For example
 
-Openstack provides several methods for configuring authentication for its SDK's and clients including CLI arguments, environment variables and a [clouds.yaml](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files) file.
+ 1. Click API Access https://dashboard.catalystcloud.nz/project/api_access/
+ 2. Click **Download OpenStack RC File** on the top right
+ 3. Select **OpenStack clouds.yaml File** from the drop down
 
-### 1. Using openrc files/environment variables is not durable across terminal sessions
 
-For some reason the preferred / default authentication method users are steered towards is using openrc files - non-trivial bash files which set environment variables in your shell session.
 
-Using environment variables to persist your authentication session is not durable across terminal instances or restarts. If you open a new terminal for any reason you will need to re authenticate there with your username, password and MFA token. This becomes very tiresome very quickly.
+Place the file in your current working directory (`.`) or an alternate [location described by the docs](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#clouds-yaml)
 
-### 2. Using clouds.yaml does not work nicely with token authentication or MFA
+Linux
+  * `~/.config/openstack/clouds.yaml`
+  * `/etc/openstack/clouds.yaml`
 
-Openstack does provide a better, more persisted, authentication mechanism by way of the [clouds.yaml](https://docs.openstack.org/python-openstackclient/latest/configuration/index.html#configuration-files) configuration file.
+Windows
+  * `C:\Users\you\.config\openstack\clouds.yaml`
+  * `C:\ProgramData\openstack\clouds.yaml`
 
-Switching sessions is then simplified by referencing the cloud config name from `clouds.yaml
-  * Using an cli argument (`--os-cloud=<name>`) 
-  * Setting the `OS_CLOUD` environment variable inline (E.g `OS_CLOUD=<name> <command>`)
-  * Exporting `OS_CLOUD` environnement variable to used by all future commands in that session (`export OS_CLOUD=<name>`)
+E.g.
 
-However using `clouds.yaml` files also has some drawbacks.
+```yaml
+# /home/john/clouds.yaml
+clouds:
+  catalystcloud:
+    auth:
+      auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
+      project_id: 33735662374f4b7a9621631f2e7e5e15
+      project_name: acme-incorporated
+      user_domain_name: Default
+      username: john.smith@acme.com
+      password: 1ns3curE123!
+    identity_api_version: 3
+    interface: public
+    region_name: nz-hlz-1
+```
 
-* It discourages token based authorization as tokens expire after 12 hours requiring users to constantly manually update clouds.yaml with new tokens.
-* It discourages the use of MFA which requires token based authorization.
-* It encourages storing usernames and passwords in clear text in a file on your machine as this is less friction than using token based authorization.
+Run os-mfa
 
-## Best of both worlds: Convenience + Hygiene with os-mfa
+```bash
+$ export OS_CLOUD=catalystcloud
+```
+```bash
+$ os-mfa
+Authenticating 'john.smith@example.com' in project 'john-smith'
+Enter Password:
+MFA Code (Press enter to skip): 654321
+Getting token...
+```
 
-This openstack MFA helper combines the convenience of durable authentication session persistence with better security hygiene by utilizing `clouds.yaml` and automatically managing the lifecycle of tokens in the config file allowing users to keep passwords out of their `clouds.yaml` file.
+```
+$ openstack network list
++--------------------------------------+------------+--------------------------------------------+
+| ID                                   | Name       | Subnets                                    |
++--------------------------------------+------------+--------------------------------------------+
+| f10ad6de-a26d-4c29-8c64-2a7418d47f8f | public-net | 5063aab1-aa08-48b2-b81d-730ac732fc51,      |
+|                                      |            | 8a7fe804-7fbe-43d0-aa1d-cfa03034ef22,      |
+|                                      |            | a1549e09-4176-4322-860c-cadc68608b48       |
++--------------------------------------+------------+--------------------------------------------+
+```
 
-## Quick Start
+If you close/restart or start a new terminal window, resume your openstack session simply by exporting `$OS_CLOUD` again.
 
-1. Obtain a `clouds.yaml` file from the cloud dashboard. For catalyst cloud:
-    * Go to https://dashboard.cloud.catalyst.net.nz/project/api_access/
-    * Hover over `Download OpenStack RC File` on the top right
-    * Click the `OpenStack clouds.yml file`
+```bash
+export OS_CLOUD=catalystcloud
+```
 
-2. Place your `clouds.yaml` file in one of the following locations detailed in the [upstream docs](https://docs.openstack.org/python-openstackclient/latest/cli/man/openstack.html#config-files)
-    * `./clouds.yaml`
-    * `~/config/openstack/clouds.yaml`
-    * `/etc/openstack/clouds.yaml`
+## What happened when we ran os-mfa?
 
-3. E.g. Assign and export your config name as the OS_CLOUD environment variable
+os-mfa created a *"long-term"* configuration without any passwords or secrets.
 
-    ```bash
-    $ export OS_CLOUD=catalystcloud
-    ```
+ * *"long-term"* configurations are distinguished with a suffix of `-long-term`
+ * We do not use the long term configs with the openstack client tools.
+ 
+The long term config used as a foundation for authentication by os-mfa which then:
 
-4. Authenticate using `os-mfa`
+1) Prompts the user for their password and totp token
 
-    ```bash
-    $ os-mfa
+2) Swaps the password and totp for an openstack auth token
 
-    Authenticating 'john.smith@example.com' in project 'john-smith'
-    Enter Password:
-    TOTP (press enter to skip): 654321
-    ```
+3) Updates the original configuration to use the new token for authentication
 
-5. Happy OpenStacking
-    ```bash
-    $ openstack server list
-    +---------------+---------------+--------+---------------+---------------+---------+
-    | ID            | Name          | Status | Networks      | Image         | Flavor  |
-    +---------------+---------------+--------+---------------+---------------+---------+
-    | a5d3814a-4f6e | proxy-server- | ACTIVE | proxy-        | N/A (booted   | c1.c1r1 |
-    | -493f-aa03-ac | yohjuqh5vzhm  |        | network-lju2p | from volume)  |         |
-    | 13fdb9a860    |               |        | kokjtsh=10.0. |               |         |
-    |               |               |        | 0.4, 103.***. |               |         |
-    |               |               |        | ***.***       |               |         |
-    +---------------+---------------+--------+---------------+---------------+---------+
-    ```
-## How it works
+The resulting clouds.yaml should look like this
 
-With os-mfa we introduce the concept of a "Long Term" configuration, distinguished by a suffix of `-long-term`, which is a copy of the original config that does not contain any secretes such as passwords or tokens.
+```yaml
+# /home/john/clouds.yaml
+clouds:
+  catalystcloud:
+    auth:
+      auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
+      project_id: 33735662374f4b7a9621631f2e7e5e15
+      project_name: acme-incorporated
+      token: gAAAAABkTkGx4Dah37lkiGTSEe3-r[...]9dQCVTBRsKjg6NFIYgMYRdAk7TTvIPOaaOE
+    identity_api_version: 3
+    interface: public
+    region_name: nz-hlz-1
+  catalystcloud-long-term:
+    auth:
+      auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
+      project_id: 33735662374f4b7a9621631f2e7e5e15
+      project_name: acme-incorporated
+      user_domain_name: Default
+      username: john.smith@acme.com
+    identity_api_version: 3
+    interface: public
+    region_name: nz-hlz-1
 
-os-mfa will assume ownership and manage the lifecycle of the original config, which we will refer to as the "Ephemeral" config going forward.
+```
 
-The Long Term and Ephemeral configs are described as follows.
+## Going further
 
-|Long Term|Ephemeral|
-|---|---|
-|Managed by you, the user|Managed by os-mfa|
-|Contains project information. Does not contain any secrets|Contains project information + temporary authentication token|
-|Used as basis to create an Ephemeral config but is otherwise ignored|Used by SDK's and clients for authentication|
-|Has a suffix of `-long-term`|Does not have a suffix|
-|Manual changes will be passed on to the Ephemeral config|Manual changes will be overwritten|
 
-The "Long Term" and "Ephemeral" configs coexist in the same clouds.yaml file. For example: Here's an annotated example of a `clouds.yaml` file with a Long Term and Ephemeral config.
+### Switching between multiple cloud accounts and sessions
 
 ```yaml
 clouds:
-    # Managed by os-mfa, Ephemeral.
-    catalystcloud:
-        auth_type: token # Managed by os-mfa
-        auth:
-            auth_url: https://api.nz-hlz-1.catalystcloud.io:5000 # Inherited
-            project_id: 33735662374f4b7a9621631f2e7e5e15         # Inherited
-            project_name: john-smith    # Inherited
-            token: gAAAAABjrN[...]e6vqt # Ephemeral, Managed by os-mfa
-        region_name: nz-hlz-1           # Inherited
-        interface: public               # Inherited
-        identity_api_version: 3         # Inherited
-
-    # Managed by you - the user.
-    catalystcloud-long-term:
-        auth:
-            auth_url: https://api.nz-hlz-1.catalystcloud.io:5000
-            username: john.smith@example.com
-            project_id: 33735662374f4b7a9621631f2e7e5e15
-            project_name: john-smith
-            user_domain_name: Default
-        region_name: nz-hlz-1
-        interface: public
-        identity_api_version: 3
+  project1-long-term:
+    region: nz-hlz-1
+    auth:
+        project_name: project1
+        username: john.smith@acme.com
+        # ...
+  project2-long-term:
+    region: nz-por-1
+    auth:
+        project_name: project2
+        username: john.smith@acme.com
+        # ...
 ```
 
-Just the same as openstack sdk's and clients, os-mfa finds your cloud.yaml file by checking the following locations in order:
+After running os-mfa once for each project you can switch between them 
 
-  * Current directory (`./clouds.yaml`)
-  * `~/config/openstack/clouds.yaml`
-  * `/etc/openstack/clouds.yaml`
-
-We specify which config we are working with by setting the `OS_CLOUD` environment variable.
-
-```bash
-export OS_CLOUD=catalystcloud
+```
+OS_CLOUD=project1
+OS_CLOUD=project2
 ```
 
-When we run os-mfa, it will check our `clouds.yaml` file for a long term profile called `<OS_CLOUD>-long-term`. E.g. `catalystcloud-long-term`.
-
-If a long term config does not exist, os-mfa will try to create a default long term config for us based on the original config and sanitized of sensitive values.
-
-Once os-mfa finds (or creates) the Long Term Config os-mfa will then:
+## Contributing
 
- 1. Read the project information from the long term config `<OS_CLOUD>-long-term`
- 2. Prompt for your secret credentials (password, MFA code)
- 3. Swap your credentials (username, password and MFA code) for an authorized token
- 4. Create/update a token based Ephemeral configuration in your `clouds.yaml` named `<OS_CLOUD>`
+Nothing special to report, just raise a PR
 
-## Run tests
+### Run tests
 
 ```
 python -m unittest discover
 ```
 
-## Building Package
+### Building Package
 
 Source: https://realpython.com/pypi-publish-python-package/
 
 ```
-python -m pip install pip-tools
+python -m pip install pip-tools build twine bumpver
 pip-compile pyproject.toml
-```
-
-## TODO:
-
- * [/] TBH I am probably going to port this back to python
- * [/] Alert if no clouds.yaml found
- * [/] Better error message if OS_CLOUD not set
- * Non-interactive mode
- * Sanitize long-term config better
- * Store and check expiry of token
-    * Only reauthenticate if token is not valid
-    * -f, --force cli option to force authentication
+python -m build
+twine check dist/*
+twine upload -r testpypi dist/*
+twine upload dist/*
+```
+
+## TODO
+
+ * ☑️ TBH I am probably going to port this back to python
+ * ☑️ Alert if no clouds.yaml found
+ * ☑️ Better error message if OS_CLOUD not set
+ * ☑️ CI/CD
+ * 🟦 Non-interactive mode
+ * 🟦 Sanitize long-term config better
+ * 🟦 Store and check expiry of token
+    * 🟦 Only reauthenticate if token is not valid
+    * 🟦 -f, --force cli option to force authentication
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `os-mfa-0.0.1/os_mfa/__main__.py` & `os-mfa-0.0.2/os_mfa/__main__.py`

 * *Files identical despite different names*

### Comparing `os-mfa-0.0.1/os_mfa/config_helpers.py` & `os-mfa-0.0.2/os_mfa/config_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from pathlib import Path
 
 from getpass import getpass
 
 import requests
 
+PASSWORD = None
+
 
 class ConfigManager:
     def __init__(self, config_path: str):
         self.config_path = config_path
         self.config = dict()
 
     @classmethod
@@ -97,14 +99,16 @@
     )
     return r.headers.get("x-subject-token")
 
 
 def create_long_term_config(config: dict) -> dict:
     """takes a config and returns a long term config with no secrets"""
 
+    global PASSWORD
+
     config = copy.deepcopy(config)
 
     # username = config["auth"].get("username")
     # if username is None:
     #     save = input("Would you like to save your username? [Y/n]").strip()
     #     if save == "" or save.lower().startswith("y"):
     #         username = input("Username:").strip()
@@ -113,14 +117,15 @@
     if "auth_type" in config:
         del config["auth_type"]
 
     if "token" in config["auth"]:
         del config["auth"]["token"]
 
     if "password" in config["auth"]:
+        PASSWORD = config["auth"]["password"]
         del config["auth"]["password"]
 
     return config
 
 
 def create_token_config(long_term_config: dict, token: str) -> dict:
     token_config = copy.deepcopy(long_term_config)
@@ -138,20 +143,31 @@
 def get_token_config(config: dict) -> dict:
     """takes a long-term-config and generates a token based config"""
 
     config = copy.deepcopy(config)
 
     username = config["auth"].get("username")
     if username is None:
-        username = input("Username:").strip()
+        username = input("Username: ").strip()
         # save = input("Would you like to save your username for next time? [y/N]: ").strip()
         # if save == "" or save.lower().startswith("y"):
         #     # Do something
         #     pass
 
-    password = getpass(f"Password for {username}:")
-    totp = input("MFA Temporary Password (Press enter to skip):").strip()
+    print(
+        "Authenticating '{}' in project '{}'".format(
+            username, config["auth"]["project_name"]
+        )
+    )
+
+    # Prompt for password unless we already have it from converting to long-term config
+    if PASSWORD is None:
+        password = getpass(f"Enter Password: ")
+    else:
+        password = PASSWORD
+
+    totp = input("MFA Code (Press enter to skip): ").strip()
     password = password + totp
 
     print("Getting token...")
     token = get_token(config["auth"], password)
     return create_token_config(config, token)
```

### Comparing `os-mfa-0.0.1/pyproject.toml` & `os-mfa-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os-mfa"
-version = "0.0.1"
+version = "0.0.2"
 description = "A minimal utility for managing cli authentication with openstack more securely and conveniently"
 readme = "README.md"
 authors = [{ name = "Simon Merrick", email = "s.m3rrick@gmail.com" }]
 # license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -18,26 +18,38 @@
 dependencies = [
     "requests",
     "PyYaml"
 ]
 requires-python = ">= 3.6"
 
 [project.optional-dependencies]
-dev = ["black"]
+dev = ["black", "bumpver", "pip-tools", "twine", "build"]
 
 [project.urls]
 Homepage = "https://github.com/iokiwi/os-mfa"
 
 [project.scripts]
 os-mfa = "os_mfa.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.1"
+current_version = "0.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
-commit_message  = "Bump version {old_version} -> {new_version}"
-commit          = true
-tag             = true
-push            = false
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = true
 
 [tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"os_mfa/__init__.py" = ["{version}"]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+]
+"setup.py" = [
+    "{version}",
+    "{pep440_version}",
+]
+"README.md" = [
+    "{version}",
+    "{pep440_version}",
+]
+"os_mfa/__init__.py" = [
+    "{version}"
+]
```

### Comparing `os-mfa-0.0.1/tests/test_create_long_term_config.py` & `os-mfa-0.0.2/tests/test_create_long_term_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from os_mfa.config_helpers import create_long_term_config
 
-class TestCreateLongTermConfig(unittest.TestCase):
 
+class TestCreateLongTermConfig(unittest.TestCase):
     def setUp(self):
         self.config = {
             "auth": {
                 "auth_url": "https://api.nz-hlz-1.catalystcloud.io:5000",
                 "project_id": "1238a098c1273d409812409812",
                 "project_name": "john-doe",
                 "user_domain_name": "Default",
@@ -23,9 +23,10 @@
 
     def test_create_long_term_config(self):
         long_term_config = create_long_term_config(self.config)
         self.assertFalse("password" in long_term_config["auth"])
         self.assertFalse("token" in long_term_config["auth"])
         self.assertFalse("auth_type" in long_term_config)
 
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `os-mfa-0.0.1/tests/test_create_token_config.py` & `os-mfa-0.0.2/tests/test_create_token_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from os_mfa.config_helpers import create_token_config
 
-class TestCreateLongTermConfig(unittest.TestCase):
 
+class TestCreateLongTermConfig(unittest.TestCase):
     def setUp(self):
         self.config = {
             "auth": {
                 "auth_url": "https://api.nz-hlz-1.catalystcloud.io:5000",
                 "project_id": "1238a098c1273d409812409812",
                 "project_name": "john-doe",
                 "user_domain_name": "Default",
@@ -25,9 +25,10 @@
         token_config = create_token_config(self.config, token)
         self.assertFalse("password" in token_config["auth"])
         self.assertFalse("user_domain_name" in token_config["auth"])
         self.assertFalse("username" in token_config["auth"])
         self.assertEqual(token_config["auth_type"], "token")
         self.assertEqual(token_config["auth"]["token"], token)
 
+
 if __name__ == "__main__":
     unittest.main()
```

