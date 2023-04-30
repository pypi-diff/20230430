# Comparing `tmp/django_object_safety-1.2.3.tar.gz` & `tmp/django_object_safety-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-1.2.3.tar", max compression
+gzip compressed data, was "django_object_safety-2.0.0.tar", max compression
```

## Comparing `django_object_safety-1.2.3.tar` & `django_object_safety-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1081 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/LICENSE
--rw-r--r--   0        0        0      129 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/README.md
--rw-r--r--   0        0        0      697 2023-04-29 22:35:53.446472 django_object_safety-1.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.2.3/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.3/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.2.3/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.2.3/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.2.3/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/models.py
--rw-r--r--   0        0        0    18774 2023-04-29 22:35:46.702479 django_object_safety-1.2.3/safety/shortcuts.py
--rw-r--r--   0        0        0     9846 2023-04-29 13:05:50.477556 django_object_safety-1.2.3/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.3/safety/views.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/README.md
+-rw-r--r--   0        0        0      698 2023-04-30 15:51:21.188514 django_object_safety-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-2.0.0/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-2.0.0/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-2.0.0/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-2.0.0/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-29 13:05:50.477556 django_object_safety-2.0.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0     2599 2023-04-30 15:51:21.188514 django_object_safety-2.0.0/safety/migrations/0009_alter_objectgroup_permissions_and_more.py
+-rw-r--r--   0        0        0      667 2023-04-30 15:51:21.188514 django_object_safety-2.0.0/safety/migrations/0010_alter_objectgroupuser_options_and_more.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-2.0.0/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     3256 2023-04-30 15:51:21.188514 django_object_safety-2.0.0/safety/models.py
+-rw-r--r--   0        0        0    19955 2023-04-30 15:51:21.188514 django_object_safety-2.0.0/safety/shortcuts.py
+-rw-r--r--   0        0        0     9852 2023-04-30 15:51:21.188514 django_object_safety-2.0.0/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-2.0.0/safety/views.py
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 django_object_safety-2.0.0/PKG-INFO
```

### Comparing `django_object_safety-1.2.3/LICENSE` & `django_object_safety-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.3/pyproject.toml` & `django_object_safety-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "1.2.3"
+version = "2.0.0"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/en/latest/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
 packages = [{ include = "safety" }]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = ">3.5"
+python = ">=3.7"
 django = ">3.2"
 
 [tool.poetry.group.dev.dependencies]
 build = "^0.10.0"
 
 
 [build-system]
```

### Comparing `django_object_safety-1.2.3/safety/migrations/0001_initial.py` & `django_object_safety-2.0.0/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.3/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-2.0.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.3/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-2.0.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.3/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-2.0.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.3/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-2.0.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.3/safety/models.py` & `django_object_safety-2.0.0/safety/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     permission = models.ForeignKey('auth.Permission', on_delete=models.CASCADE, verbose_name=_('Permission'))
 
     to = GenericForeignKey('to_ct', 'to_id')
     to_id = models.CharField(_('Target ID'), max_length=255)
     to_ct = models.ForeignKey('contenttypes.ContentType', on_delete=models.CASCADE, verbose_name=_('Content Type'),
                               limit_choices_to={'model__in': ('user', 'group')}, related_name='entity_of')
 
-    object_id = models.IntegerField(_('Object ID'))
+    object_id = models.IntegerField(_('Object ID'), null=True)
     object_ct = models.ForeignKey('contenttypes.ContentType', on_delete=models.CASCADE,
-                                  verbose_name=_('Target Content Type'), related_name='object_of')
+                                  verbose_name=_('Target Content Type'), related_name='object_of', blank=True,
+                                  null=True)
     object = GenericForeignKey('object_ct', 'object_id')
 
     class Meta:
         unique_together = (('to_ct', 'to_id', 'permission', 'object_ct', 'object_id'),)
         abstract = True
 
     def __str__(self):
@@ -30,37 +31,57 @@
 
 
 class ObjectPermission(AbstractObjectPermission):
     class Meta(AbstractObjectPermission.Meta):
         verbose_name = _('User Object Permission')
         verbose_name_plural = _('User Object Permissions')
 
-        swappable = 'SAFETY_OBJECT_PERMISSION_MODEL'
+
+class AbstractObjectGroupUser(models.Model):
+    """
+    Intermediary model allowing storage of metadata in an object group that differs between users.
+    """
+
+    group = models.ForeignKey('safety.ObjectGroup', on_delete=models.CASCADE, verbose_name=_('Group'))
+
+    user = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE, verbose_name=_('User'))
+
+    class Meta:
+        abstract = True
+        unique_together = (('group', 'user'),)
+
+    def __str__(self):
+        return f'{self.user} is in {self.group}'
+
+
+class ObjectGroupUser(AbstractObjectGroupUser):
+    class Meta(AbstractObjectGroupUser.Meta):
+        abstract = False
+        verbose_name = _('Object Group User')
+        verbose_name_plural = _('Object Group Users')
 
 
 class AbstractObjectGroup(models.Model):
     """
     A group of permissions for an object.
     """
 
     name = models.CharField(_('Name'), max_length=255)
-    users = models.ManyToManyField(settings.AUTH_USER_MODEL, verbose_name=_('Users'))
-    permissions = models.ManyToManyField('auth.Permission', verbose_name=_('Permissions'))
+    permissions = models.ManyToManyField('auth.Permission', verbose_name=_('Permissions'), blank=True)
+    users = models.ManyToManyField(settings.AUTH_USER_MODEL, through=ObjectGroupUser, verbose_name=_('Users'))
 
     target = GenericForeignKey('target_ct', 'target_id')
     target_id = models.IntegerField(_('Target ID'), null=True)
     target_ct = models.ForeignKey('contenttypes.ContentType', on_delete=models.CASCADE,
-                                  verbose_name=_('Target Content Type'))
+                                  verbose_name=_('Target Content Type'), related_name='obj_group_target_ct_of')
 
     class Meta:
         abstract = True
 
     def __str__(self):
         return self.name
 
 
 class ObjectGroup(AbstractObjectGroup):
     class Meta:
         verbose_name = _('Permission Group')
         verbose_name_plural = _('Permission Groups')
-
-        swappable = 'SAFETY_OBJECT_GROUP_MODEL'
```

### Comparing `django_object_safety-1.2.3/safety/shortcuts.py` & `django_object_safety-2.0.0/safety/shortcuts.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from operator import concat
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Permission, Group
 from django.contrib.contenttypes.models import ContentType
 
-from safety.models import ObjectPermission, ObjectGroup
+from safety.models import ObjectPermission, ObjectGroup, ObjectGroupUser
 
 
 def get_object_permission_model(obj=None):
     """
     Retrieves the object permission model. If obj is provided, the Meta class of
     that object will be checked for a custom object permission model.
 
@@ -20,15 +20,17 @@
     Returns:
         An instance of an object permission model.
     """
 
     # pylint: disable-next=protected-access
     # noinspection PyProtectedMember
     if obj and hasattr(obj._meta, 'object_permission_model'):
-        return obj.object_permission_model
+        # pylint: disable-next=protected-access
+        # noinspection PyProtectedMember
+        return obj._meta.object_permission_model
 
     return ContentType.objects.get_model(settings.SAFETY_OBJECT_PERMISSION_MODEL) \
         if hasattr(settings, 'SAFETY_OBJECT_PERMISSION_MODEL') \
         else ObjectPermission
 
 
 def get_object_group_model(obj=None):
@@ -40,22 +42,42 @@
         obj: The model class or instance to check for a custom Object Group model.
     Returns:
         An instance of an Object Group model.
     """
 
     # pylint: disable-next=protected-access
     # noinspection PyProtectedMember
-    if obj and hasattr(obj._meta, 'object_permission_model'):
-        return obj.object_group_model
+    if obj and hasattr(obj._meta, 'object_group_model'):
+        # pylint: disable-next=protected-access
+        # noinspection PyProtectedMember
+        return obj._meta.object_group_model
 
     return ContentType.objects.get_model(settings.SAFETY_PERMISSION_GROUP_MODEL) \
         if hasattr(settings, 'SAFETY_OBJECT_GROUP_MODEL') \
         else ObjectGroup
 
 
+def get_object_group_user_model(obj=None):
+    """
+    Retrieves the object group user intermediary model. If obj is provided,
+    the Meta class of that object will be checked for a per object model.
+    """
+
+    # pylint: disable-next=protected-access
+    # noinspection PyProtectedMember
+    if obj and hasattr(obj._meta, 'object_group_user_model'):
+        # pylint: disable-next=protected-access
+        # noinspection PyProtectedMember
+        return obj._meta.object_group_user_model
+
+    return ContentType.objects.get_model(settings.SAFETY_OBJECT_GROUP_USER_MODEL) \
+        if hasattr(settings, 'SAFETY_OBJECT_GROUP_USER_MODEL') \
+        else ObjectGroupUser
+
+
 def has_perm(entities: list, perm: str, obj=None, content_type=None) -> bool:
     """
     Return True if the user has the specified permission. If obj is provided,
     the permission must be checked against obj. If the permission does not
     exist, return False.
 
     Args:
@@ -91,17 +113,22 @@
         if isinstance(entity, get_user_model()):
             all_have_perm = get_object_permission_model(obj).objects.filter(permission=permission, to_id=entity.id,
                                                                             to_ct=ContentType.objects.get_for_model(
                                                                                 entity),
                                                                             object_id=obj.id).exists()
             # Check the PermissionGroup object
             if not all_have_perm:
-                all_have_perm = get_object_group_model().objects.filter(target_id=obj.id,
-                                                                        permissions__in=[permission],
-                                                                        users__in=[entity]).exists()
+                # links = ObjectPermissionLink.objects.filter(
+                #     permission_id=permission.id,
+                #     permission_ct=ContentType.objects.get_for_model(permission)
+                # )
+
+                all_have_perm = get_object_group_model(obj).objects.filter(target_id=obj.id,
+                                                                           permissions__in=[permission],
+                                                                           users__in=[entity]).exists()
         elif isinstance(entity, Group):
             all_have_perm = get_object_permission_model(obj).objects.filter(permission=permission, to_id=entity.id,
                                                                             to_ct=ContentType.objects.get_for_model(
                                                                                 entity),
                                                                             object_id=obj.id).exists()
 
     return all_have_perm
@@ -268,15 +295,16 @@
             reduce(concat,
                    [[permission.codename for permission in group.permissions] for group in entity.groups]
                    )
         )
 
     return get_perms(entity, obj) + [perm.permission.codename for perm in get_object_group_model(obj).objects.filter(
         users__in=[entity],
-        object=obj,
+        target_id=obj.id,
+        target_ct=ContentType.objects.get_for_model(obj)
     )]
 
 
 def get_users_with_perms(perms, obj=None, content_type=None, with_group_users=False) -> \
         list[get_user_model()]:
     """
     Get all users that have the specified permission(s).
@@ -436,15 +464,16 @@
 
     ct = ContentType.objects.get_for_model(obj)
 
     perm_group = get_object_group_model().objects.create(name=name, target_id=obj.id,
                                                          target_ct=ct)
 
     for permission in permissions:
-        perm_group.permissions.add(Permission.objects.get_or_create(codename=permission, content_type=ct)[0].id)
+        perm = Permission.objects.get_or_create(codename=permission, content_type=ct)[0]
+        perm_group.permissions.add(perm)
 
     return perm_group
 
 
 def delete_object_group(name: str, obj) -> bool:
     """
     Remove an object group.
@@ -477,14 +506,15 @@
 
     Returns:
         bool: True if the user was added to the group, otherwise False.
     """
 
     get_object_group_model().objects.get(name=name, target_id=obj.id,
                                          target_ct=ContentType.objects.get_for_model(obj)).users.add(user)
+
     return True
 
 
 def remove_user_from_object_group(user: get_user_model(), name: str, obj) -> bool:
     """
     Remove a user from an object group.
```

### Comparing `django_object_safety-1.2.3/safety/tests.py` & `django_object_safety-2.0.0/safety/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
         self.assertQuerySetEqual(get_users_with_perms("view_fakepost", self.posts[0]), [self.users[0], self.users[1]])
 
     def test_get_users_with_perms_global(self):
         set_perm(self.users[0], "view_fakepost", content_type=self.fake_post_ct)
         set_perm(self.users[1], "view_fakepost", content_type=self.fake_post_ct)
 
-        self.assertListEqual(get_users_with_perms("view_fakepost", content_type=self.fake_post_ct),
+        self.assertListEqual(list(get_users_with_perms("view_fakepost", content_type=self.fake_post_ct)),
                              [self.users[0], self.users[1]])
 
     def test_get_users_with_group_perms(self):
         create_object_group("editors", ["view_fakepost"], self.posts[0])
         add_user_to_object_group(self.users[0], "editors", self.posts[0])
 
         self.assertListEqual(get_users_with_perms("view_fakepost", self.posts[0], with_group_users=True),
```

### Comparing `django_object_safety-1.2.3/PKG-INFO` & `django_object_safety-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 1.2.3
+Version: 2.0.0
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/en/latest/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
-Requires-Python: >3.5
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django (>3.2)
 Project-URL: Repository, https://github.com/williammferreira/django-object-safety/
```

