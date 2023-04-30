# Comparing `tmp/csle_attacker-0.1.9.tar.gz` & `tmp/csle_attacker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attacker-0.1.9.tar", last modified: Tue Mar 21 08:09:25 2023, max compression
+gzip compressed data, was "csle_attacker-0.2.0.tar", last modified: Sun Apr 30 12:36:30 2023, max compression
```

## Comparing `csle_attacker-0.1.9.tar` & `csle_attacker-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:25.989220 csle_attacker-0.1.9/
--rw-rw-r--   0 kim       (1000) kim       (1000)      659 2023-03-21 08:09:25.989220 csle_attacker-0.1.9/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3922 2023-01-03 16:53:36.000000 csle_attacker-0.1.9/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-02-11 20:28:41.000000 csle_attacker-0.1.9/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1218 2023-03-21 08:09:25.989220 csle_attacker-0.1.9/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:25.985220 csle_attacker-0.1.9/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:25.985220 csle_attacker-0.1.9/src/csle_attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_attacker-0.1.9/src/csle_attacker/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      941 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/attacker.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:25.989220 csle_attacker-0.1.9/src/csle_attacker/emulation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      994 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/attacker_stopping_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11411 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/emulated_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11560 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/exploit_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4676 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/post_exploit_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5951 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/recon_middleware.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:25.989220 csle_attacker-0.1.9/src/csle_attacker/emulation/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    42067 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/util/exploit_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7585 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/util/nikto_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    34189 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/util/nmap_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    29810 2022-11-28 13:03:16.000000 csle_attacker-0.1.9/src/csle_attacker/emulation/util/shell_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:25.985220 csle_attacker-0.1.9/src/csle_attacker.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      659 2023-03-21 08:09:25.000000 csle_attacker-0.1.9/src/csle_attacker.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      916 2023-03-21 08:09:25.000000 csle_attacker-0.1.9/src/csle_attacker.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:25.000000 csle_attacker-0.1.9/src/csle_attacker.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:55.000000 csle_attacker-0.1.9/src/csle_attacker.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      177 2023-03-21 08:09:25.000000 csle_attacker-0.1.9/src/csle_attacker.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       14 2023-03-21 08:09:25.000000 csle_attacker-0.1.9/src/csle_attacker.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:30.308505 csle_attacker-0.2.0/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      659 2023-04-30 12:36:30.308505 csle_attacker-0.2.0/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3922 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1218 2023-04-30 12:36:30.308505 csle_attacker-0.2.0/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:30.304505 csle_attacker-0.2.0/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:30.304505 csle_attacker-0.2.0/src/csle_attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-04-30 12:35:57.000000 csle_attacker-0.2.0/src/csle_attacker/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      941 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/attacker.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:30.308505 csle_attacker-0.2.0/src/csle_attacker/emulation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      994 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/attacker_stopping_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11411 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/emulated_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11560 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/exploit_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4676 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/post_exploit_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5951 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/recon_middleware.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:30.308505 csle_attacker-0.2.0/src/csle_attacker/emulation/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    45611 2023-04-18 12:47:39.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/util/exploit_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7585 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/util/nikto_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34189 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/util/nmap_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    29810 2023-03-28 14:03:22.000000 csle_attacker-0.2.0/src/csle_attacker/emulation/util/shell_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-04-30 12:36:30.304505 csle_attacker-0.2.0/src/csle_attacker.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      659 2023-04-30 12:36:29.000000 csle_attacker-0.2.0/src/csle_attacker.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      916 2023-04-30 12:36:30.000000 csle_attacker-0.2.0/src/csle_attacker.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-04-30 12:36:29.000000 csle_attacker-0.2.0/src/csle_attacker.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:55.000000 csle_attacker-0.2.0/src/csle_attacker.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      177 2023-04-30 12:36:30.000000 csle_attacker-0.2.0/src/csle_attacker.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       14 2023-04-30 12:36:30.000000 csle_attacker-0.2.0/src/csle_attacker.egg-info/top_level.txt
```

### Comparing `csle_attacker-0.1.9/PKG-INFO` & `csle_attacker-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_attacker
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.1.9/README.md` & `csle_attacker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/pyproject.toml` & `csle_attacker-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/setup.cfg` & `csle_attacker-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-common>=0.1.9
+	csle-common>=0.2.0
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_attacker-0.1.9/src/csle_attacker/attacker.py` & `csle_attacker-0.2.0/src/csle_attacker/attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/attacker_stopping_middleware.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/attacker_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/emulated_attacker.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/emulated_attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/exploit_middleware.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/post_exploit_middleware.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/post_exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/recon_middleware.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/recon_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/util/exploit_util.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/util/exploit_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,16 @@
                 jump_connection = ConnectionUtil.find_jump_host_connection(ip=ip, s=s)
                 for i in range(constants.ENV_CONSTANTS.ATTACKER_RETRY_SAMBACRY):
                     cost = 0
                     cmd = a.cmds[0]
                     cmd = cmd.format(ip)
                     outdata, errdata, total_time = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
+                    Logger.__call__().get_logger().warning(
+                        f"Samba command: {cmd}, out: {outdata.decode()}, err: {errdata.decode()}")
 
                     # Parse result and check outcome
                     exploit_successful = (constants.SAMBA.ALREADY_EXISTS in outdata.decode() or
                                           (constants.SAMBA.ERROR not in outdata.decode() and
                                            constants.SAMBA.ERROR not in errdata.decode() and
                                            constants.SAMBA.AUTH_OK in outdata.decode()))
 
@@ -62,14 +64,17 @@
             except Exception as e:
                 Logger.__call__().get_logger().warning(
                     f"There was an error executing the sambacry exploit: {str(e)} {repr(e)}")
 
         # Parse Result
         if exploit_successful:
 
+            Logger.__call__().get_logger().info(f"The SambaCry exploit against machine: {target_machine.ips[0]} "
+                                                f"was successful, cmd: {a.cmds[0].format(target_machine.ips[0])}")
+
             # Exploit successful
             credential = Credential(username=constants.SAMBA.BACKDOOR_USER, pw=constants.SAMBA.BACKDOOR_PW,
                                     port=constants.SSH.DEFAULT_PORT, protocol=TransportProtocol.TCP,
                                     service=constants.SSH.SERVICE_NAME)
             vuln = EmulationVulnerabilityObservationState(
                 name=constants.EXPLOIT_VULNERABILITES.SAMBACRY_EXPLOIT,
                 cvss=constants.EXPLOIT_VULNERABILITES.SAMBACRY_CVSS,
@@ -87,14 +92,17 @@
             target_machine.cve_vulns.append(vuln)
 
             # Measure  cost and alerts
             cost += float(total_time)
 
             EmulationUtil.log_measured_action_time(total_time=total_time, action=a,
                                                    emulation_env_config=s.emulation_env_config)
+        else:
+            Logger.__call__().get_logger().info(f"The SambaCry exploit against machine: {target_machine.ips[0]} "
+                                                f"was unsuccessful")
 
         target_machine.sambacry_tried = True
         attacker_machine_observations = EnvDynamicsUtil.merge_new_obs_with_old(
             s.attacker_obs_state.machines, [target_machine.copy()],
             emulation_env_config=s.emulation_env_config, action=a)
         s_prime = s
         s_prime.attacker_obs_state.machines = attacker_machine_observations
@@ -120,15 +128,16 @@
                     # Try execute exploit from jumphost
                     cost = 0
                     cmd = a.cmds[0]
                     cmd = cmd.format(constants.SHELLSHOCK.BACKDOOR_USER, constants.SHELLSHOCK.BACKDOOR_PW,
                                      constants.SHELLSHOCK.BACKDOOR_USER, ip)
                     outdata, errdata, total_time = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
-
+                    Logger.__call__().get_logger().info(f"Shellshock cmd: {cmd}, out: {outdata.decode()}, "
+                                                        f"err:{errdata.decode()}")
                     cmd = a.cmds[1]
                     cmd = cmd.format(constants.SHELLSHOCK.BACKDOOR_USER, constants.SHELLSHOCK.BACKDOOR_PW, a.ips)
                     outdata1, errdata1, total_time1 = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
                     total_time = total_time + total_time1
 
                     # Parse Result
@@ -149,14 +158,17 @@
                     break
             except Exception as e:
                 Logger.__call__().get_logger().warning(f"There was an error executing the shellshock exploit: "
                                                        f"{str(e)}, {repr(e)}")
 
         if exploit_successful:
 
+            Logger.__call__().get_logger().info(f"The Shellshock exploit against machine: {target_machine.ips[0]} "
+                                                f"was successful")
+
             # Exploit successful
             credential = Credential(username=constants.SHELLSHOCK.BACKDOOR_USER,
                                     pw=constants.SHELLSHOCK.BACKDOOR_PW,
                                     port=constants.SSH.DEFAULT_PORT, protocol=TransportProtocol.TCP,
                                     service=constants.SSH.SERVICE_NAME)
             vuln = EmulationVulnerabilityObservationState(
                 name=constants.EXPLOIT_VULNERABILITES.SHELLSHOCK_EXPLOIT,
@@ -170,14 +182,17 @@
             target_machine.shell_access = True
             target_machine.untried_credentials = True
             target_machine.shell_access_credentials.append(credential)
             target_machine.backdoor_credentials.append(credential)
             target_machine.backdoor_tried = True
             target_machine.backdoor_installed = True
             target_machine.cve_vulns.append(vuln)
+        else:
+            Logger.__call__().get_logger().info(f"The Shellshock exploit against machine: {target_machine.ips[0]} "
+                                                f"was unsuccessful")
 
         # Measure  cost and alerts
         cost += float(total_time)
 
         EmulationUtil.log_measured_action_time(total_time=total_time, action=a,
                                                emulation_env_config=s.emulation_env_config)
 
@@ -237,14 +252,16 @@
             try:
                 jump_connection = ConnectionUtil.find_jump_host_connection(ip=ip, s=s)
                 for i in range(constants.ENV_CONSTANTS.ATTACKER_RETRY_DVWA_SQL_INJECTION):
                     cmd = a.cmds[0]
                     cmd = cmd + " " + ip
                     outdata, errdata, total_time = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
+                    Logger.__call__().get_logger().info(f"Sql injeciton cmd: {cmd}, out: {outdata.decode()}, "
+                                                        f"err:{errdata.decode()}")
 
                     # Parse Result
                     exploit_successful = False
                     dir = "/home/" + jump_connection.credential.username + "/"
                     try:
                         exploit_result = ExploitUtil.read_dvwa_sql_injection_result(conn=jump_connection.conn,
                                                                                     dir=dir)
@@ -259,14 +276,16 @@
                     except Exception as e:
                         Logger.__call__().get_logger().warning(
                             f"There was an error executing the SQL injection exploit: {str(e)}, {repr(e)}")
                         exploit_successful = False
                         pw = "-"
 
                     if exploit_successful:
+                        Logger.__call__().get_logger().info(f"SQL injection against: {target_machine.ips[0]} "
+                                                            f"was successful")
                         ExploitUtil.remove_dvwa_sql_injection_result(conn=jump_connection.conn,
                                                                      dir=dir)
                         # Exploit successful
                         credential = Credential(username=constants.DVWA_SQL_INJECTION.EXPLOIT_USER,
                                                 pw=pw,
                                                 port=constants.SSH.DEFAULT_PORT, protocol=TransportProtocol.TCP,
                                                 service=constants.SSH.SERVICE_NAME)
@@ -287,14 +306,16 @@
                         target_machine.backdoor_installed = True
                         target_machine.cve_vulns.append(vuln)
 
                         # Measure  cost and alerts
                         cost += float(total_time)
                         break
                     else:
+                        Logger.__call__().get_logger().info(f"SQL injection against: {target_machine.ips[0]} "
+                                                            f"was not successful")
                         time.sleep(constants.ENV_CONSTANTS.ATTACKER_RETRY_DVWA_SQL_INJECTION)
 
                 if exploit_successful:
                     break
             except Exception as e:
                 Logger.__call__().get_logger().warning(
                     f"There was an error executing the SQL injection exploit: {e}, {repr(e)}")
@@ -360,15 +381,16 @@
                 jump_connection = ConnectionUtil.find_jump_host_connection(ip=ip, s=s)
                 for i in range(constants.ENV_CONSTANTS.ATTACKER_RETRY_CVE_2015_3306):
                     cost = 0
                     cmd = a.cmds[0]
                     cmd = cmd.format(a.ips)
                     outdata, errdata, total_time = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
-
+                    Logger.__call__().get_logger().info(f"CVE-2015-3306, cmd: {cmd}, out: {outdata.decode()}, "
+                                                        f"err: {errdata.decode()}")
                     proxy_conn = EmulationConnectionObservationState(
                         conn=jump_connection.conn, credential=jump_connection.credential,
                         root=True, port=constants.SSH.DEFAULT_PORT, service=constants.SSH.SERVICE_NAME,
                         proxy=None, ip=s.emulation_env_config.containers_config.agent_ip)
 
                     exploit_successful = ExploitUtil.check_if_rce_exploit_succeeded(
                         user=constants.CVE_2015_3306.BACKDOOR_USER, pw=constants.CVE_2015_3306.BACKDOOR_PW,
@@ -382,15 +404,16 @@
                 if exploit_successful:
                     break
             except Exception as e:
                 Logger.__call__().get_logger().warning(
                     f"There was an error executing the CVE-2015-3306 exploit: {e}, {repr(e)}")
 
         if exploit_successful:
-
+            Logger.__call__().get_logger().info(f"CVE-2015-3306 against target: {target_machine.ips[0]} "
+                                                f"was successful")
             # Exploit successful
             credential = Credential(username=constants.CVE_2015_3306.BACKDOOR_USER,
                                     pw=constants.CVE_2015_3306.BACKDOOR_PW,
                                     port=constants.SSH.DEFAULT_PORT, protocol=TransportProtocol.TCP,
                                     service=constants.SSH.SERVICE_NAME)
             vuln = EmulationVulnerabilityObservationState(
                 name=constants.EXPLOIT_VULNERABILITES.CVE_2015_3306,
@@ -404,14 +427,17 @@
             target_machine.shell_access = True
             target_machine.untried_credentials = True
             target_machine.shell_access_credentials.append(credential)
             target_machine.backdoor_credentials.append(credential)
             target_machine.backdoor_tried = True
             target_machine.backdoor_installed = True
             target_machine.cve_vulns.append(vuln)
+        else:
+            Logger.__call__().get_logger().info(f"CVE-2015-3306 against target: {target_machine.ips[0]} "
+                                                f"was not successful")
 
         # Measure  cost and alerts
         cost += float(total_time)
 
         EmulationUtil.log_measured_action_time(total_time=total_time, action=a,
                                                emulation_env_config=s.emulation_env_config)
         target_machine.cve_2015_3306_tried = True
@@ -442,14 +468,16 @@
                 jump_connection = ConnectionUtil.find_jump_host_connection(ip=ip, s=s)
                 for i in range(constants.ENV_CONSTANTS.ATTACKER_RETRY_CVE_2015_1427):
                     cost = 0
                     cmd = a.cmds[0]
                     cmd = cmd.format(a.ips)
                     outdata, errdata, total_time = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
+                    Logger.__call__().get_logger().info(f"CVE-2015-1427 cmd:{cmd}, out:{outdata.decode()}, "
+                                                        f"err: {errdata.decode()}")
 
                     # Parse Result
                     proxy_conn = EmulationConnectionObservationState(
                         conn=jump_connection.conn, credential=jump_connection.credential,
                         root=True, port=constants.SSH.DEFAULT_PORT, service=constants.SSH.SERVICE_NAME,
                         proxy=None, ip=s.emulation_env_config.containers_config.agent_ip)
 
@@ -465,14 +493,16 @@
                 if exploit_successful:
                     break
             except Exception as e:
                 Logger.__call__().get_logger().warning(
                     f"There was an error executing the CVE-2015-1427 exploit: {e}, {repr(e)}")
 
         if exploit_successful:
+            Logger.__call__().get_logger().info(f"CVE-2015-1427 against target: {target_machine.ips[0]} was successful")
+
             # Exploit successful
             credential = Credential(username=constants.CVE_2015_1427.BACKDOOR_USER,
                                     pw=constants.CVE_2015_1427.BACKDOOR_PW,
                                     port=constants.SSH.DEFAULT_PORT, protocol=TransportProtocol.TCP,
                                     service=constants.SSH.SERVICE_NAME)
             vuln = EmulationVulnerabilityObservationState(
                 name=constants.EXPLOIT_VULNERABILITES.CVE_2015_1427,
@@ -486,14 +516,17 @@
             target_machine.shell_access = True
             target_machine.untried_credentials = True
             target_machine.shell_access_credentials.append(credential)
             target_machine.backdoor_credentials.append(credential)
             target_machine.backdoor_tried = True
             target_machine.backdoor_installed = True
             target_machine.cve_vulns.append(vuln)
+        else:
+            Logger.__call__().get_logger().info(f"CVE-2015-1427 against target: {target_machine.ips[0]} "
+                                                f"was not successful")
 
         # Measure  cost and alerts
         cost += float(total_time)
         EmulationUtil.log_measured_action_time(total_time=total_time, action=a,
                                                emulation_env_config=s.emulation_env_config)
         target_machine.cve_2015_1427_tried = True
 
@@ -524,14 +557,16 @@
                                                                            emulation_env_config=s.emulation_env_config)
                 for i in range(constants.ENV_CONSTANTS.ATTACKER_RETRY_CVE_2016_10033):
                     cost = 0
                     cmd = a.cmds[0]
                     cmd = cmd.format(a.ips)
                     outdata, errdata, total_time = EmulationUtil.execute_ssh_cmd(
                         cmd=cmd, conn=jump_connection.conn)
+                    Logger.__call__().get_logger().info(f"CVE-2016-10033 cmd:{cmd}, out: {outdata.decode()}, "
+                                                        f"err: {errdata.decode()}")
 
                     # Parse Result
                     proxy_conn = EmulationConnectionObservationState(
                         conn=jump_connection.conn, credential=jump_connection.credential,
                         root=True, port=constants.SSH.DEFAULT_PORT, service=constants.SSH.SERVICE_NAME,
                         proxy=None, ip=s.emulation_env_config.containers_config.agent_ip)
 
@@ -547,14 +582,16 @@
                 if exploit_successful:
                     break
             except Exception as e:
                 Logger.__call__().get_logger().warning(
                     f"There was an exception executing exploit CVE-2016-10033: {e}, {repr(e)}")
 
         if exploit_successful:
+            Logger.__call__().get_logger().info(f"CVE-2016-10033 against {target_machine.ips[0]} was succcessful")
+
             # Exploit successful
             credential = Credential(username=constants.CVE_2016_10033.BACKDOOR_USER,
                                     pw=constants.CVE_2016_10033.BACKDOOR_PW,
                                     port=constants.SSH.DEFAULT_PORT, protocol=TransportProtocol.TCP,
                                     service=constants.SSH.SERVICE_NAME)
             vuln = EmulationVulnerabilityObservationState(
                 name=constants.EXPLOIT_VULNERABILITES.CVE_2016_10033,
@@ -568,14 +605,16 @@
             target_machine.shell_access = True
             target_machine.untried_credentials = True
             target_machine.shell_access_credentials.append(credential)
             target_machine.backdoor_credentials.append(credential)
             target_machine.backdoor_tried = True
             target_machine.backdoor_installed = True
             target_machine.cve_vulns.append(vuln)
+        else:
+            Logger.__call__().get_logger().info(f"CVE-2016-10033 against {target_machine.ips[0]} was not succcessful")
 
         # Measure  cost and alerts
         cost += float(total_time)
         EmulationUtil.log_measured_action_time(total_time=total_time, action=a,
                                                emulation_env_config=s.emulation_env_config)
 
         target_machine.cve_2016_10033_tried = True
@@ -639,14 +678,15 @@
                                 port=constants.SSH.DEFAULT_PORT,
                                 target_ip=ip, proxy_conn=proxy_conn)
                         except Exception as e:
                             Logger.__call__().get_logger().warning("CVE-2010-0426 error:{}".format(str(e)))
                             e_succ = False
 
                         if e_succ:
+                            Logger.__call__().get_logger().info("CVE-2010-0426 was succcessful")
                             root_credential = Credential(
                                 username=constants.CVE_2010_0426.BACKDOOR_USER,
                                 pw=constants.CVE_2010_0426.BACKDOOR_PW, port=constants.SSH.DEFAULT_PORT,
                                 protocol=TransportProtocol.TCP, service=constants.SSH.SERVICE_NAME)
                             root_connection = EmulationUtil.setup_custom_connection(
                                 user=constants.CVE_2010_0426.BACKDOOR_USER, pw=constants.CVE_2010_0426.BACKDOOR_PW,
                                 source_ip=s.emulation_env_config.containers_config.agent_ip,
@@ -667,14 +707,15 @@
                             result.shell_access = True
                             result.logged_in = True
                             result.root = True
                             result.ssh_connections.append(root_connection)
                             service = constants.SSH.SERVICE_NAME
                             break
                         else:
+                            Logger.__call__().get_logger().info("CVE-2010-0426 against was not succcessful")
                             time.sleep(constants.ENV_CONSTANTS.ATTACKER_CVE_2010_0426_SLEEP_RETRY)
                     if e_succ:
                         break
                 except Exception as e:
                     Logger.__call__().get_logger().warning(
                         f"Exception occurred during execution of exploit CVE-2010-0426, {str(e)}, {repr(e)}")
 
@@ -747,14 +788,15 @@
                             port=constants.SSH.DEFAULT_PORT,
                             target_ip=ip, proxy_conn=proxy_conn)
                     except Exception as e:
                         Logger.__call__().get_logger().warning(f"CVE-2015-5602 error:{str(e)}, {repr(e)}")
                         e_succ = False
 
                     if e_succ:
+                        Logger.__call__().get_logger().info("CVE-2015-5602 was succcessful")
                         root_credential = Credential(username=constants.CVE_2015_5602.BACKDOOR_USER,
                                                      pw=constants.CVE_2015_5602.BACKDOOR_PW,
                                                      port=constants.SSH.DEFAULT_PORT,
                                                      protocol=TransportProtocol.TCP,
                                                      service=constants.SSH.SERVICE_NAME)
                         root_connection = EmulationUtil.setup_custom_connection(
                             user=constants.CVE_2015_5602.BACKDOOR_USER, pw=constants.CVE_2015_5602.BACKDOOR_PW,
```

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/util/nikto_util.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/util/nikto_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/util/nmap_util.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/util/nmap_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker/emulation/util/shell_util.py` & `csle_attacker-0.2.0/src/csle_attacker/emulation/util/shell_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.1.9/src/csle_attacker.egg-info/PKG-INFO` & `csle_attacker-0.2.0/src/csle_attacker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-attacker
-Version: 0.1.9
+Version: 0.2.0
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.1.9/src/csle_attacker.egg-info/SOURCES.txt` & `csle_attacker-0.2.0/src/csle_attacker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

