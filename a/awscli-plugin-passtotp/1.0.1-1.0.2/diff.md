# Comparing `tmp/awscli_plugin_passtotp-1.0.1.tar.gz` & `tmp/awscli_plugin_passtotp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awscli_plugin_passtotp-1.0.1.tar", max compression
+gzip compressed data, was "awscli_plugin_passtotp-1.0.2.tar", max compression
```

## Comparing `awscli_plugin_passtotp-1.0.1.tar` & `awscli_plugin_passtotp-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1466 2023-03-19 23:16:29.047018 awscli_plugin_passtotp-1.0.1/README.md
--rw-r--r--   0        0        0      443 2023-03-19 23:16:29.047018 awscli_plugin_passtotp-1.0.1/awscli_plugin_passtotp/__init__.py
--rw-r--r--   0        0        0      292 2023-03-19 23:16:29.047018 awscli_plugin_passtotp-1.0.1/awscli_plugin_passtotp/boto_plugin.py
--rw-r--r--   0        0        0     2361 2023-03-19 23:16:29.047018 awscli_plugin_passtotp-1.0.1/awscli_plugin_passtotp/commands.py
--rw-r--r--   0        0        0     1234 2023-03-19 23:16:29.047018 awscli_plugin_passtotp-1.0.1/awscli_plugin_passtotp/prompter.py
--rw-r--r--   0        0        0      761 2023-03-19 23:16:29.047018 awscli_plugin_passtotp-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2584 1970-01-01 00:00:00.000000 awscli_plugin_passtotp-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1864 2023-04-30 10:44:29.990061 awscli_plugin_passtotp-1.0.2/README
+-rw-r--r--   0        0        0      443 2023-04-30 09:44:14.523909 awscli_plugin_passtotp-1.0.2/awscli_plugin_passtotp/__init__.py
+-rw-r--r--   0        0        0      292 2023-04-30 09:44:14.524193 awscli_plugin_passtotp-1.0.2/awscli_plugin_passtotp/boto_plugin.py
+-rw-r--r--   0        0        0     2361 2023-04-30 09:44:14.524522 awscli_plugin_passtotp-1.0.2/awscli_plugin_passtotp/commands.py
+-rw-r--r--   0        0        0     1234 2023-04-30 09:44:14.524916 awscli_plugin_passtotp-1.0.2/awscli_plugin_passtotp/prompter.py
+-rw-r--r--   0        0        0      712 2023-04-30 10:57:28.175055 awscli_plugin_passtotp-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 awscli_plugin_passtotp-1.0.2/PKG-INFO
```

### Comparing `awscli_plugin_passtotp-1.0.1/awscli_plugin_passtotp/commands.py` & `awscli_plugin_passtotp-1.0.2/awscli_plugin_passtotp/commands.py`

 * *Files identical despite different names*

### Comparing `awscli_plugin_passtotp-1.0.1/awscli_plugin_passtotp/prompter.py` & `awscli_plugin_passtotp-1.0.2/awscli_plugin_passtotp/prompter.py`

 * *Files identical despite different names*

### Comparing `awscli_plugin_passtotp-1.0.1/PKG-INFO` & `awscli_plugin_passtotp-1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: awscli-plugin-passtotp
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
-Home-page: https://github.com/someone-stole-my-name/awscli-plugin-passtotp
+Home-page: https://git.segundo.io/awscli-plugin-passtotp
 License: GPL-3.0-or-later
 Keywords: aws,aws-cli,boto3,pass,pass-otp
 Author: Christian Segundo
 Author-email: christian@segundo.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -15,65 +15,94 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: botocore (>=1.14.14,<2.0.0)
-Project-URL: Documentation, https://github.com/someone-stole-my-name/awscli-plugin-passtotp/blob/master/README.md
-Project-URL: Repository, https://github.com/someone-stole-my-name/awscli-plugin-passtotp
-Description-Content-Type: text/markdown
-
-# AWS CLI MFA with pass-otp made easy
-
-This plugin enables aws-cli to directly talk to [pass](https://www.passwordstore.org/)
-to acquire an OATH-TOTP code using the [pass-otp](https://github.com/tadfisher/pass-otp) extension.
-
-## Installation
-
-`awscli-plugin-passtotp` can be installed from PyPI:
-```sh
-$ pip install awscli-plugin-passtotp
-```
-
-It's also possible to install it just for your user in case you don't have
-permission to install packages system-wide:
-```sh
-$ pip install --user awscli-plugin-passtotp
-```
-
-### Configure AWS CLI
-
-To enable the plugin, add this to your `~/.aws/config`:
-```ini
-[plugins]
-# If using aws-cli v2 you must specify the path to where the package was installed.
-# Use `pip show awscli-plugin-passtotp | grep Location:` to find the right location.
-cli_legacy_plugin_path = /foo/bar/lib/python3.9/site-packages/
-
-passtotp = awscli_plugin_passtotp
-```
-
-Also make sure to specify a path to a file in your password-store in the profiles managed by pass:
-```ini
-[profile myprofile]
-role_arn = arn:aws:iam::...
-mfa_serial = arn:aws:iam::...
-mfa_path = foo/aws/bar
-...
-```
-
-## Usage
-
-Just use the `aws` command with a custom role and the plugin will do the rest:
-
-```sh
-$ aws s3 ls --profile myprofile
-2013-07-11 17:08:50 mybucket
-2013-07-24 14:55:44 mybucket2
-```
+Project-URL: Documentation, https://git.segundo.io/awscli-plugin-passtotp/tree/README
+Project-URL: Repository, https://git.segundo.io/awscli-plugin-passtotp
+Description-Content-Type: text/plain
 
----
+awscli-plugin-passtotp
+======================
 
-## Acknowledgements
-* Thanks to [@tommie-lie](https://github.com/tommie-lie) for [awscli-plugin-yubikeytotp](https://github.com/tommie-lie/awscli-plugin-yubikeytotp)
+This plugin enables aws-cli to directly talk to pass to acquire an
+OATH-TOTP code using the pass-otp extension.
+
+Dependencies
+------------
+
+* pass
+* pass-otp
+* python
+* aws-cli
+
+Installation
+------------
+
+Building and installing awscli-plugin-passtotp requires a working
+Python 3 installation.
+
+a) To install it from a cloned repository:
+
+    $ python3 -m pip install .
+
+b) You can also install it directly from PyPi like this:
+
+    $ python3 -m pip install awscli-plugin-passtotp
+
+Enabling the plugin
+-------------------
+
+A new entry to the plugins section in your config (~/.aws/config)
+must be added to enable the plugin:
+
+    [plugins]
+    passtotp = awscli_plugin_passtotp
+
+If using aws-cli version 2 you must specify the path to where the
+package was installed. You can use the following command to find
+the right location:
+
+    $ pip show awscli-plugin-passtotp | grep Location:
+
+And then add the following to your config (~/.aws/config):
+
+    [plugins]
+    cli_legacy_plugin_path = /usr/local/lib/python3.10/dist-packages
+    passtotp = awscli_plugin_passtotp
+
+AWS CLI configuration
+---------------------
+
+Specify a path to a file in your passord-store in the profiles where
+you want to use the plugin.
+
+    [profile bar]
+    mfa_path = foo/aws/bar
+    ...
+
+You can ensure you have a working pass-otp entry by running:
+
+    $ pass otp foo/aws/bar
+
+Where 'foo/aws/bar' is an entry added by 'pass otp', eg:
+
+    $ pass otp insert foo/aws/bar
+
+Usage
+-----
+
+Just use the aws command with a custom role and the plugin will
+obtain the TOTP token from pass:
+
+    $ aws s3 ls --profile myprofile
+    2013-07-11 17:08:50 mybucket
+    2013-07-24 14:55:44 mybucket2
+
+Acknowledgements
+----------------
+
+This plugin was primarily based off the work of tommie-lie in
+https://github.com/tommie-lie/awscli-plugin-yubikeytotp
```

