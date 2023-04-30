# Comparing `tmp/bodhi_messages-7.1.1.tar.gz` & `tmp/bodhi_messages-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_messages-7.1.1.tar", max compression
+gzip compressed data, was "bodhi_messages-7.2.0.tar", max compression
```

## Comparing `bodhi_messages-7.1.1.tar` & `bodhi_messages-7.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    18018 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/COPYING
--rw-r--r--   0        0        0       97 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/README.rst
--rw-r--r--   0        0        0      906 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/bodhi/messages/__init__.py
--rw-r--r--   0        0        0      793 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/bodhi/messages/schemas/__init__.py
--rw-r--r--   0        0        0     9240 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/bodhi/messages/schemas/base.py
--rw-r--r--   0        0        0     5116 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/bodhi/messages/schemas/buildroot_override.py
--rw-r--r--   0        0        0    11249 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/bodhi/messages/schemas/compose.py
--rw-r--r--   0        0        0     3783 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/bodhi/messages/schemas/errata.py
--rw-r--r--   0        0        0    28720 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/bodhi/messages/schemas/update.py
--rw-r--r--   0        0        0     1271 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/bodhi/messages/utils.py
--rw-r--r--   0        0        0     3548 2023-03-18 09:16:08.000000 bodhi_messages-7.1.1/pyproject.toml
--rw-r--r--   0        0        0      788 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2713 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/tests/test_base.py
--rw-r--r--   0        0        0     3500 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/tests/test_buildroot_override.py
--rw-r--r--   0        0        0     6651 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/tests/test_compose.py
--rw-r--r--   0        0        0     5321 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/tests/test_errata.py
--rw-r--r--   0        0        0    38664 2023-03-05 14:50:21.000000 bodhi_messages-7.1.1/tests/test_update.py
--rw-r--r--   0        0        0     1960 2022-12-23 15:08:00.000000 bodhi_messages-7.1.1/tests/utils.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 bodhi_messages-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18018 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/COPYING
+-rw-r--r--   0        0        0       97 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/README.rst
+-rw-r--r--   0        0        0      906 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/bodhi/messages/__init__.py
+-rw-r--r--   0        0        0      793 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/__init__.py
+-rw-r--r--   0        0        0     9240 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/base.py
+-rw-r--r--   0        0        0     5116 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/buildroot_override.py
+-rw-r--r--   0        0        0    11249 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/compose.py
+-rw-r--r--   0        0        0     3783 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/errata.py
+-rw-r--r--   0        0        0    30333 2023-04-29 13:40:09.000000 bodhi_messages-7.2.0/bodhi/messages/schemas/update.py
+-rw-r--r--   0        0        0     1271 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/bodhi/messages/utils.py
+-rw-r--r--   0        0        0     3618 2023-04-30 06:59:12.000000 bodhi_messages-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0      788 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2713 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_base.py
+-rw-r--r--   0        0        0     3500 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_buildroot_override.py
+-rw-r--r--   0        0        0     6651 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_compose.py
+-rw-r--r--   0        0        0     5321 2023-04-29 08:18:48.000000 bodhi_messages-7.2.0/tests/test_errata.py
+-rw-r--r--   0        0        0    43182 2023-04-29 13:40:09.000000 bodhi_messages-7.2.0/tests/test_update.py
+-rw-r--r--   0        0        0     1960 2023-04-29 08:07:12.000000 bodhi_messages-7.2.0/tests/utils.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 bodhi_messages-7.2.0/PKG-INFO
```

### Comparing `bodhi_messages-7.1.1/COPYING` & `bodhi_messages-7.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/__init__.py` & `bodhi_messages-7.2.0/bodhi/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/schemas/__init__.py` & `bodhi_messages-7.2.0/bodhi/messages/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/schemas/base.py` & `bodhi_messages-7.2.0/bodhi/messages/schemas/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/schemas/buildroot_override.py` & `bodhi_messages-7.2.0/bodhi/messages/schemas/buildroot_override.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/schemas/compose.py` & `bodhi_messages-7.2.0/bodhi/messages/schemas/compose.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/schemas/errata.py` & `bodhi_messages-7.2.0/bodhi/messages/schemas/errata.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/bodhi/messages/schemas/update.py` & `bodhi_messages-7.2.0/bodhi/messages/schemas/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,14 +356,61 @@
         """
         return (
             f"{self.agent_name} edited {self.update.alias} "
             f"adding {len(self.body['new_bugs'])} new bugs"
         )
 
 
+class UpdateEditV2(UpdateEditV1):
+    """
+    Sent when an update is edited. Newer version.
+
+    Has 'new_builds' and 'removed_builds' properties.
+    """
+
+    # mypy infers that lots of the things we touch below should be
+    # collections of strings and doesn't like us doing unexpected
+    # things to them, so the typing.Any shuts it up
+    body_schema: typing.Any = copy.deepcopy(UpdateEditV1.body_schema)
+    body_schema['properties']['new_builds'] = {
+        'type': 'array',
+        'description': 'An array of build NVRs that have been added to the update',
+        'items': {
+            'type': 'string',
+            'description': 'A build NVR'
+        }
+    }
+    body_schema['properties']['removed_builds'] = {
+        'type': 'array',
+        'description': 'An array of build NVRs that have been removed from the update',
+        'items': {
+            'type': 'string',
+            'description': 'A build NVR'
+        }
+    }
+    body_schema['required'].extend(('new_builds', 'removed_builds'))
+
+    def __str__(self) -> str:
+        """
+        Return a human-readable representation of this message.
+
+        This should provide a detailed representation of the message, much like the body
+        of an email.
+
+        Returns:
+            A human readable representation of this message.
+        """
+        return (
+            f"{self.agent_name} edited {self.update.alias} "
+            f"adding {len(self.body['new_bugs'])} new bug(s), "
+            f"adding {len(self.body['new_builds'])} build(s), and "
+            f"removing {len(self.body['removed_builds'])} build(s)"
+        )
+
+
 class UpdateEjectV1(UpdateMessage):
     """Sent when an update is ejected from the push."""
 
     body_schema = {
         'id': f'{SCHEMA_URL}/v1/bodhi.update.eject#',
         '$schema': 'http://json-schema.org/draft-04/schema#',
         'description': 'Schema for message sent when an update is ejected from a compose',
```

### Comparing `bodhi_messages-7.1.1/bodhi/messages/utils.py` & `bodhi_messages-7.2.0/bodhi/messages/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/pyproject.toml` & `bodhi_messages-7.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-messages"
-version = "7.1.1"
+version = "7.2.0"
 description = "JSON schema for messages sent by Bodhi"
 readme = "README.rst"
 authors = ["Fedora Infrastructure Team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 repository = "https://github.com/fedora-infra/bodhi"
 homepage = "https://bodhi.fedoraproject.org"
 keywords = ["fedora", "fedora-messaging"]
@@ -54,14 +54,15 @@
 "bodhi.repo.done.v1" = "bodhi.messages.schemas.compose:RepoDoneV1"
 "bodhi.update.comment.v1" = "bodhi.messages.schemas.update:UpdateCommentV1"
 "bodhi.update.complete.stable.v1" = "bodhi.messages.schemas.update:UpdateCompleteStableV1"
 "bodhi.update.complete.testing.v1" = "bodhi.messages.schemas.update:UpdateCompleteTestingV1"
 "bodhi.update.status.testing.v1" = "bodhi.messages.schemas.update:UpdateReadyForTestingV1"
 "bodhi.update.status.testing.v2" = "bodhi.messages.schemas.update:UpdateReadyForTestingV2"
 "bodhi.update.edit.v1" = "bodhi.messages.schemas.update:UpdateEditV1"
+"bodhi.update.edit.v2" = "bodhi.messages.schemas.update:UpdateEditV2"
 "bodhi.update.eject.v1" = "bodhi.messages.schemas.update:UpdateEjectV1"
 "bodhi.update.karma.threshold.v1" = "bodhi.messages.schemas.update:UpdateKarmaThresholdV1"
 "bodhi.update.request.revoke.v1" = "bodhi.messages.schemas.update:UpdateRequestRevokeV1"
 "bodhi.update.request.stable.v1" = "bodhi.messages.schemas.update:UpdateRequestStableV1"
 "bodhi.update.request.testing.v1" = "bodhi.messages.schemas.update:UpdateRequestTestingV1"
 "bodhi.update.request.unpush.v1" = "bodhi.messages.schemas.update:UpdateRequestUnpushV1"
 "bodhi.update.request.obsolete.v1" = "bodhi.messages.schemas.update:UpdateRequestObsoleteV1"
```

### Comparing `bodhi_messages-7.1.1/tests/__init__.py` & `bodhi_messages-7.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/tests/test_base.py` & `bodhi_messages-7.2.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/tests/test_buildroot_override.py` & `bodhi_messages-7.2.0/tests/test_buildroot_override.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/tests/test_compose.py` & `bodhi_messages-7.2.0/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/tests/test_errata.py` & `bodhi_messages-7.2.0/tests/test_errata.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/tests/test_update.py` & `bodhi_messages-7.2.0/tests/test_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 """Unit tests for the update message schemas."""
 
 
 from bodhi.messages.schemas.base import BuildV1, ReleaseV1, UpdateV1, UserV1
 from bodhi.messages.schemas.update import (UpdateCommentV1,
                                            UpdateCompleteStableV1,
                                            UpdateCompleteTestingV1,
-                                           UpdateEditV1, UpdateEjectV1,
+                                           UpdateEditV1,
+                                           UpdateEditV2,
+                                           UpdateEjectV1,
                                            UpdateKarmaThresholdV1,
                                            UpdateReadyForTestingV1,
                                            UpdateReadyForTestingV2,
                                            UpdateRequestObsoleteV1,
                                            UpdateRequestRevokeV1,
                                            UpdateRequestStableV1,
                                            UpdateRequestTestingV1,
@@ -709,14 +711,115 @@
                 "update": {
                     "close_bugs": True,
                     "pushed": False,
                     "require_testcases": True,
                     "critpath": False,
                     "stable_karma": 3,
                     "date_pushed": None,
+                    "requirements": "rpmlint",
+                    "severity": "unspecified",
+                    "title": "tzdata-2014i-1.fc19",
+                    "suggest": "unspecified",
+                    "require_bugs": True,
+                    "comments": [
+                        {
+                            "bug_feedback": [],
+                            "user_id": 1681,
+                            "timestamp": "2015-01-28 03:02:44",
+                            "testcase_feedback": [],
+                            "karma_critpath": 0,
+                            "update": 54046,
+                            "update_id": 54046,
+                            "karma": 0,
+                            "anonymous": False,
+                            "text": "ralph edited this update. ",
+                            "id": 484236,
+                            "user": {
+                                "buildroot_overrides": [],
+                                "name": "bodhi",
+                                "avatar": None
+                            }
+                        }
+                    ],
+                    "date_approved": None,
+                    "type": "enhancement",
+                    "status": "pending",
+                    "date_submitted": "2014-10-29 20:02:57",
+                    "unstable_karma": -3,
+                    "user": {
+                        "buildroot_overrides": [],
+                        "name": "ralph",
+                        "avatar": None
+                    },
+                    "locked": False,
+                    "builds": [
+                        {
+                            "override": None,
+                            "nvr": "tzdata-2014i-1.fc19"
+                        }
+                    ],
+                    "date_modified": "2015-01-28 03:02:55",
+                    "notes": "the update notes go here...",
+                    "request": "testing",
+                    "bugs": [],
+                    "alias": 'FEDORA-2019-7dbbb74a13',
+                    "karma": 0,
+                    "release": {
+                        "dist_tag": "f19",
+                        "name": "F19",
+                        "testing_tag": "f19-updates-testing",
+                        "pending_stable_tag": "f19-updates-pending",
+                        "long_name": "Fedora 19",
+                        "state": "disabled",
+                        "version": None,
+                        "override_tag": "f19-override",
+                        "branch": None,
+                        "id_prefix": "FEDORA",
+                        "pending_testing_tag": "f19-updates-testing-pending",
+                        "stable_tag": "f19-updates",
+                        "candidate_tag": "f19-updates-candidate"
+                    }
+                },
+                "agent": "ralph"
+            }
+        )
+        check_message(msg, expected)
+
+    def test_edit_v2(self):
+        expected = {
+            "topic": "bodhi.update.edit",
+            "summary": "ralph edited FEDORA-2019-7dbbb74a13",
+            "__str__": ("ralph edited FEDORA-2019-7dbbb74a13 adding 2 new bug(s), "
+                        "adding 1 build(s), and removing 1 build(s)"),
+            "app_icon": "https://apps.fedoraproject.org/img/icons/bodhi.png",
+            "app_name": "bodhi",
+            "url": "https://bodhi.fedoraproject.org/updates/FEDORA-2019-7dbbb74a13",
+            "agent_avatar": (
+                "https://seccdn.libravatar.org/avatar/"
+                "9c9f7784935381befc302fe3c814f9136e7a33953d0318761669b8643f4df55c"
+                "?s=64&d=retro"
+            ),
+            "new_bugs": [1708925, 1706626],
+            "usernames": ["ralph"],
+            "packages": ["tzdata"],
+            'update': UpdateV1('FEDORA-2019-7dbbb74a13', [BuildV1('tzdata-2014i-1.fc19')],
+                               UserV1('ralph'), 'pending', 'testing', ReleaseV1('F19'))
+        }
+        msg = UpdateEditV2(
+            body={
+                "new_bugs": [1708925, 1706626],
+                "new_builds": ["tzdata-2014i-1.fc19"],
+                "removed_builds": ["tzdata-2014h-1.fc19"],
+                "update": {
+                    "close_bugs": True,
+                    "pushed": False,
+                    "require_testcases": True,
+                    "critpath": False,
+                    "stable_karma": 3,
+                    "date_pushed": None,
                     "requirements": "rpmlint",
                     "severity": "unspecified",
                     "title": "tzdata-2014i-1.fc19",
                     "suggest": "unspecified",
                     "require_bugs": True,
                     "comments": [
                         {
```

### Comparing `bodhi_messages-7.1.1/tests/utils.py` & `bodhi_messages-7.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_messages-7.1.1/PKG-INFO` & `bodhi_messages-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-messages
-Version: 7.1.1
+Version: 7.2.0
 Summary: JSON schema for messages sent by Bodhi
 Home-page: https://bodhi.fedoraproject.org
 License: GPL-2.0-or-later
 Keywords: fedora,fedora-messaging
 Author: Fedora Infrastructure Team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
```

