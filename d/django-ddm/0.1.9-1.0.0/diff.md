# Comparing `tmp/django-ddm-0.1.9.tar.gz` & `tmp/django-ddm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ddm-0.1.9.tar", last modified: Tue May  3 09:29:21 2022, max compression
+gzip compressed data, was "django-ddm-1.0.0.tar", last modified: Sun Apr 30 14:03:35 2023, max compression
```

## Comparing `django-ddm-0.1.9.tar` & `django-ddm-1.0.0.tar`

### file list

```diff
@@ -1,172 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:06.000000 django-ddm-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-03 09:29:06.000000 django-ddm-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-05-03 09:29:21.079122 django-ddm-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      640 2022-05-03 09:29:06.000000 django-ddm-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    11947 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/migrations/0002_alter_donationproject_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/migrations/0003_auto_20220429_1154.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/migrations/0004_auto_20220502_1810.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/migrations/0005_alter_donationproject_public_key.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/models/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6553 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/models/data_donations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/models/encryption.py
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/models/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     8843 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/models/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/static/ddm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/css/
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/css/public-base.css
--rw-r--r--   0 runner    (1001) docker     (121)     9287 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/css/questionnaire.css
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/css/research-interface-base.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/img/
--rw-r--r--   0 runner    (1001) docker     (121)    27639 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/img/glow background.png
--rw-r--r--   0 runner    (1001) docker     (121)    78886 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/img/ikmz_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9846 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/img/surquest.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9758 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/img/surquest_v0-2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7867 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/img/surquest_v0-2_icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)    89143 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/img/uzh_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/js/bootstrap4/
--rw-r--r--   0 runner    (1001) docker     (121)    80927 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/bootstrap4/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/delete-responses.js
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/file-download.js
--rw-r--r--   0 runner    (1001) docker     (121)     8479 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/file-upload.js
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/multistep-form.js
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/questionnaire-admin.js
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/questionnaire-structure.js
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/js/questionnaire-tools.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/vue/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/vue/css/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/css/vue_questionnaire.css
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/css/vue_uploader.css
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/static/ddm/vue/js/
--rw-r--r--   0 runner    (1001) docker     (121)   230294 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/js/chunk-vendors.js
--rw-r--r--   0 runner    (1001) docker     (121)    12202 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/js/vue_questionnaire.js
--rw-r--r--   0 runner    (1001) docker     (121)    15320 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/js/vue_uploader.js
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/static/ddm/vue/webpack-stats.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/templates/ddm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/templates/ddm/admin/
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/templates/ddm/admin/controls/
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/controls/button_add_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/controls/button_add_question.html
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/controls/button_add_trigger.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.071122 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/base_delete_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/base_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/form_field.html
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/form_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/inline_form.html
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/forms/list_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.067122 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/level_0_header.html
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/level_1_questionnaires.html
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/level_2_questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/level_3_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/level_4_question.html
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/navigation/side_navigation/level_5_question_item.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/admin/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/pages/create.html
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/pages/delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/pages/update.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/create.html
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/external_variables_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/general_settings.html
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/questionnaire_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/responses.html
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/structure.html
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/trigger_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questionnaires/uploaded_data.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/admin/questions/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questions/create.html
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questions/filters.html
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/questions/update.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/admin/triggers/
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/triggers/create.html
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/admin/triggers/update.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/project_admin/
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/project_admin/blueprint/
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/blueprint/create.html
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/blueprint/delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/blueprint/edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/blueprint/list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/project_admin/generic/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/generic/page_with_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/project_admin/instructions/
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/instructions/create.html
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/instructions/delete.html
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/instructions/edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/instructions/list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/create.html
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/delete.html
--rw-r--r--   0 runner    (1001) docker     (121)     2847 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/detail.html
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/edit.html
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.075122 django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/create.html
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/delete.html
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/edit.html
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/edit_set.html
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/ddm/templates/ddm/public/
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/public/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/public/data_donation.html
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/public/end.html
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/public/entry_page.html
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/public/questionnaire.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/admission.html
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/already_completed.html
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/base_questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/continuation.html
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/display.html
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/inactive.html
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/templates/ddm/questionnaire/thankyou.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/ddm/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/tests/encryption.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    14212 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/ddm/views/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/data_donation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4852 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/ddm/views/project_admin/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/project_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7313 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/project_admin/data_donations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1885 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/project_admin/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/project_admin/questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (121)     3381 2022-05-03 09:29:06.000000 django-ddm-0.1.9/ddm/views/questionnaire.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/django_ddm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-05-03 09:29:20.000000 django-ddm-0.1.9/django_ddm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5495 2022-05-03 09:29:21.000000 django-ddm-0.1.9/django_ddm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 09:29:20.000000 django-ddm-0.1.9/django_ddm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-05-03 09:29:20.000000 django-ddm-0.1.9/django_ddm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-05-03 09:29:20.000000 django-ddm-0.1.9/django_ddm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-03 09:29:06.000000 django-ddm-0.1.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-05-03 09:29:06.000000 django-ddm-0.1.9/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 09:29:21.079122 django-ddm-0.1.9/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-05-03 09:29:06.000000 django-ddm-0.1.9/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-05-03 09:29:06.000000 django-ddm-0.1.9/docs/source/for_developers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-05-03 09:29:06.000000 django-ddm-0.1.9/docs/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-05-03 09:29:06.000000 django-ddm-0.1.9/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-05-03 09:29:21.079122 django-ddm-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-03 09:29:06.000000 django-ddm-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.487769 django-ddm-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-04-30 14:03:06.000000 django-ddm-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-30 14:03:06.000000 django-ddm-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-30 14:03:35.487769 django-ddm-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-30 14:03:06.000000 django-ddm-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.439768 django-ddm-1.0.0/ddm/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.439768 django-ddm-1.0.0/ddm/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.447769 django-ddm-1.0.0/ddm/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0002_alter_donationproject_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0003_auto_20220429_1154.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0004_auto_20220502_1810.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0005_alter_donationproject_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0006_auto_20220617_1433.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0007_auto_20220621_1136.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0008_auto_20220623_2142.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0009_auto_20220629_1641.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0010_auto_20220629_1651.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0011_auto_20220830_1047.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0012_auto_20220921_1634.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0013_auto_20220922_1324.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0014_auto_20220922_1640.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0015_auto_20220923_1055.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0016_auto_20220928_1344.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0017_alter_processingrule_comparison_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0018_auto_20220929_1308.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0019_auto_20221212_2121.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0020_auto_20221216_1428.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0021_auto_20221222_0925.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0022_auto_20230103_1433.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0023_auto_20230104_1325.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0024_customtoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0025_rename_customtoken_projectaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0026_exceptionlogentry_raised_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0027_auto_20230110_1738.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0028_auto_20230112_1140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0029_rename_eventlog_eventlogentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0030_auto_20230120_1746.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0031_auto_20230122_1828.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0032_auto_20230130_1733.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0033_participant_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0034_auto_20230210_1148.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0035_auto_20230217_1552.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0036_alter_processingrule_replacement_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0037_auto_20230227_1117.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0038_auto_20230308_1619.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0039_alter_donationblueprint_json_extraction_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0040_participant_current_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0041_auto_20230429_1258.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/0042_auto_20230429_2215.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.447769 django-ddm-1.0.0/ddm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/questions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/models/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/static/ddm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.447769 django-ddm-1.0.0/ddm/static/ddm/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.447769 django-ddm-1.0.0/ddm/static/ddm/css/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    95510 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/bootstrap/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/bootstrap/bootstrap-table-filter-control.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/bootstrap/bootstrap-table.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   163873 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/bootstrap/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   451427 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/bootstrap/bootstrap.min.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/ddm-base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/public-base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/questionnaire.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/css/research-interface-base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/static/ddm/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.455768 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/
+-rw-r--r--   0 runner    (1001) docker     (123)   141076 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   142312 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141236 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   143208 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141680 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   143484 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   137076 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   140544 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   142396 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141700 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   144764 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   139168 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   139928 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   142832 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/NunitoSans-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/NunitoSans/OFL.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.459769 django-ddm-1.0.0/ddm/static/ddm/fonts/bootstrap-icons/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/fonts/bootstrap-icons/bootstrap-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.459769 django-ddm-1.0.0/ddm/static/ddm/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/img/ddl_favicon_black.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.459769 django-ddm-1.0.0/ddm/static/ddm/img/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/img/logos/DDM_Logo_Schwarz.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    52227 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/img/logos/Example Logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.459769 django-ddm-1.0.0/ddm/static/ddm/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/blueprint-edit-ui-helpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.459769 django-ddm-1.0.0/ddm/static/ddm/js/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)   905032 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/bokeh/bokeh-3.0.3.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.463769 django-ddm-1.0.0/ddm/static/ddm/js/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)    32448 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/bootstrap/bootstrap-table-export.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62303 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/bootstrap/bootstrap-table-filter-control.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   135874 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/bootstrap/bootstrap-table.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78129 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/bootstrap/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/delete-data.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/download-data.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.463769 django-ddm-1.0.0/ddm/static/ddm/js/filesaver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/filesaver/FileSaver.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/filesaver/FileSaver.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.463769 django-ddm-1.0.0/ddm/static/ddm/js/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    89942 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/jquery/jquery-3.6.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    77666 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/jquery/tableExport.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/processing-rule-modal.js
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/js/project-admin-base.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.463769 django-ddm-1.0.0/ddm/static/ddm/vue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.463769 django-ddm-1.0.0/ddm/static/ddm/vue/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/vue/css/vue_questionnaire.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/vue/css/vue_uploader.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/vue/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/vue/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.467769 django-ddm-1.0.0/ddm/static/ddm/vue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   346341 2023-04-30 14:03:06.000000 django-ddm-1.0.0/ddm/static/ddm/vue/js/chunk-vendors.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1715448 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/static/ddm/vue/js/chunk-vendors.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/static/ddm/vue/js/vue_questionnaire.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44767 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/static/ddm/vue/js/vue_questionnaire.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    42634 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/static/ddm/vue/js/vue_uploader.js
+-rw-r--r--   0 runner    (1001) docker     (123)   116001 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/static/ddm/vue/js/vue_uploader.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/static/ddm/vue/webpack-stats.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/ddm/templates/ddm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.467769 django-ddm-1.0.0/ddm/templates/ddm/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.471769 django-ddm-1.0.0/ddm/templates/ddm/admin/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/auth/confirm_profile.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/auth/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/auth/login_oidc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/auth/no_permission.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.471769 django-ddm-1.0.0/ddm/templates/ddm/admin/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/components/form_field_basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/components/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/components/info_modal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.471769 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.471769 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/donation_blueprint/
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/donation_blueprint/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/donation_blueprint/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/donation_blueprint/edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.471769 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/file_uploader/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/file_uploader/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/file_uploader/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/file_uploader/edit.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.471769 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/instructions/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/instructions/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/instructions/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/instructions/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/processing_rule_modal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.475769 django-ddm-1.0.0/ddm/templates/ddm/admin/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/generic/page_with_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.475769 django-ddm-1.0.0/ddm/templates/ddm/admin/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/edit-briefing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/edit-debriefing.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/logs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.475769 django-ddm-1.0.0/ddm/templates/ddm/admin/project/project_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/project_logs/event_log.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/project_logs/exception_log.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/project_logs/overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/project/token.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.479769 django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/edit_set.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.479769 django-ddm-1.0.0/ddm/templates/ddm/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/public/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/public/briefing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/public/continuation_not_found.html
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/public/data_donation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/public/debriefing.html
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templates/ddm/public/questionnaire.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.479769 django-ddm-1.0.0/ddm/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/templatetags/ddm_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/ddm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/performance_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_admin_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_participation_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/ddm/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/ddm/views/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/admin/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/admin/data_donations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/admin/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/admin/questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-04-30 14:03:07.000000 django-ddm-1.0.0/ddm/views/participation_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/django_ddm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-30 14:03:35.000000 django-ddm-1.0.0/django_ddm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-04-30 14:03:35.000000 django-ddm-1.0.0/django_ddm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 14:03:35.000000 django-ddm-1.0.0/django_ddm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-30 14:03:35.000000 django-ddm-1.0.0/django_ddm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-30 14:03:35.000000 django-ddm-1.0.0/django_ddm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/antora-playbook-local.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/antora-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/antora.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    29611 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/asciidoctor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.435768 django-ddm-1.0.0/docs/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/docs/modules/ROOT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.483769 django-ddm-1.0.0/docs/modules/ROOT/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/images/ddl_favicon_black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.487769 django-ddm-1.0.0/docs/modules/ROOT/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.487769 django-ddm-1.0.0/docs/modules/ROOT/pages/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/components/footer.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/components/header.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/components/scripts.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/for_admins.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/for_developers.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/for_participants.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)    33019 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/for_researchers.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/index.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/issues.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topic_references.adoc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.487769 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/continuation.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/customize_admin_templates.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/customize_ckeditor_configs.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/encryption.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/exception_logging.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/internationalization.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/modules/ROOT/pages/topics/user_authentication.adoc
+-rw-r--r--   0 runner    (1001) docker     (123)   160664 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 14:03:35.487769 django-ddm-1.0.0/docs/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    58412 2023-04-30 14:03:07.000000 django-ddm-1.0.0/docs/ui/ui-bundle.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-30 14:03:35.487769 django-ddm-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 14:03:07.000000 django-ddm-1.0.0/setup.py
```

### Comparing `django-ddm-0.1.9/PKG-INFO` & `django-ddm-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: django-ddm
-Version: 0.1.9
+Version: 1.0.0
 Summary: A Django app to setup data donation projects.
 Home-page: https://github.com/uzh/ddm
 Author: Nico Pfiffner
 Author-email: n.pfiffner@ikmz.uzh.ch
-License: MIT
-Project-URL: Documentation, https://data-donation-module.readthedocs.io/
+License: GPLv3
+Project-URL: Documentation, https://uzh.github.io/ddm/
 Project-URL: Website, https://datadonation.uzh.ch
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 # Data Donation Module (ddm)
 
 > **_NOTE:_**  This package is currently under active development.
 
 **DDM** (Data Donation Module) is a Django application that helps researchers to
 setup data donation projects and to collect data donations for academic research.
 
 This is part of a larger initiative from the University of Zurich and the Digital
 Society Initiative to strengthen the exchange about the topic of data donations and
 promote this data collection approach. For more information, visit https://datadonation.uzh.ch.
 
-Documentation: https://data-donation-module.readthedocs.io/en/latest/ \
+Documentation: https://uzh.github.io/ddm/ddm/main/index.html \
 PyPi: https://pypi.org/project/django-ddm/
-
-
```

### Comparing `django-ddm-0.1.9/README.md` & `django-ddm-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 **DDM** (Data Donation Module) is a Django application that helps researchers to
 setup data donation projects and to collect data donations for academic research.
 
 This is part of a larger initiative from the University of Zurich and the Digital
 Society Initiative to strengthen the exchange about the topic of data donations and
 promote this data collection approach. For more information, visit https://datadonation.uzh.ch.
 
-Documentation: https://data-donation-module.readthedocs.io/en/latest/ \
+Documentation: https://uzh.github.io/ddm/ddm/main/index.html \
 PyPi: https://pypi.org/project/django-ddm/
```

### Comparing `django-ddm-0.1.9/ddm/migrations/0001_initial.py` & `django-ddm-1.0.0/ddm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ddm-0.1.9/ddm/migrations/0003_auto_20220429_1154.py` & `django-ddm-1.0.0/ddm/migrations/0003_auto_20220429_1154.py`

 * *Files identical despite different names*

### Comparing `django-ddm-0.1.9/ddm/migrations/0004_auto_20220502_1810.py` & `django-ddm-1.0.0/ddm/migrations/0004_auto_20220502_1810.py`

 * *Files identical despite different names*

### Comparing `django-ddm-0.1.9/ddm/static/ddm/css/public-base.css` & `django-ddm-1.0.0/ddm/static/ddm/css/public-base.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .public-header {
-    height: 120px;
+    height: 100%;
     padding-top: 10px;
     padding-bottom: 10px;
     border-bottom: 1px solid #ddd;
     margin-bottom: 40px;
 }
 
 .public-footer {
@@ -17,35 +17,40 @@
     font-size: 0.8rem !important;
     text-decoration: none;
 }
 
 .flow-btn {
     background-color: black;
     font-size: 1.1rem;
-    min-width: 15%;
+    min-width: 140px;
     float: right;
-    color: white;
+    color: white !important;
     transition: none;
     line-height: 1.5;
     text-align: center;
     text-decoration: none;
+    margin-top: 20px;
     padding: .375rem;
     border-radius: .25rem;
     border: none;
 }
 .flow-btn:hover {
     background-color: #2f2f2f;
-    color: white;
+    color: white !important;
 }
 
-.text-orange {
-    color: #de5300;
+a {
+    color: #0068b3;
 }
-.text-orange:hover {
-    color: #ff5f00;
+a:hover {
+    color: #00518d !important;
+}
+
+.text-red {
+    color: #ab0000;
 }
 .bg-success-light {
     background-color: #55ff5517;
 }
 .consent-checkbox {
     width: 1.3rem;
     height: 1.3rem;
@@ -54,15 +59,14 @@
     background-color: #198754;
     border-color: #198754;
 }
 .upload-other {
     cursor: pointer;
     color: #7f887f;
     text-decoration: none;
-    margin-left: 3rem;
 }
 .upload-other:hover {
     color: #5a5f5a;
 }
 .select-file-btn {
     background: #eaeaea;
     line-height: 1;
@@ -73,7 +77,13 @@
     margin-left: 2rem;
     padding: 0.4rem;
     border-radius: 0.25rem;
 }
 .select-file-btn:hover {
     background: #d5d5d5;
 }
+.modal-close {
+    font-size: 0.8rem;
+}
+#briefing-consent-answer label {
+    cursor: pointer;
+}
```

### Comparing `django-ddm-0.1.9/ddm/static/ddm/img/surquest_v0-2_icon.svg` & `django-ddm-1.0.0/ddm/static/ddm/img/ddl_favicon_black.svg`

 * *Files 24% similar despite different names*

```diff
@@ -2,491 +2,530 @@
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
 00000070: 0a0a 3c73 7667 0a20 2020 786d 6c6e 733a  ..<svg.   xmlns:
-00000080: 6f73 623d 2268 7474 703a 2f2f 7777 772e  osb="http://www.
-00000090: 6f70 656e 7377 6174 6368 626f 6f6b 2e6f  openswatchbook.o
-000000a0: 7267 2f75 7269 2f32 3030 392f 6f73 6222  rg/uri/2009/osb"
-000000b0: 0a20 2020 786d 6c6e 733a 6463 3d22 6874  .   xmlns:dc="ht
-000000c0: 7470 3a2f 2f70 7572 6c2e 6f72 672f 6463  tp://purl.org/dc
-000000d0: 2f65 6c65 6d65 6e74 732f 312e 312f 220a  /elements/1.1/".
-000000e0: 2020 2078 6d6c 6e73 3a63 633d 2268 7474     xmlns:cc="htt
-000000f0: 703a 2f2f 6372 6561 7469 7665 636f 6d6d  p://creativecomm
-00000100: 6f6e 732e 6f72 672f 6e73 2322 0a20 2020  ons.org/ns#".   
-00000110: 786d 6c6e 733a 7264 663d 2268 7474 703a  xmlns:rdf="http:
-00000120: 2f2f 7777 772e 7733 2e6f 7267 2f31 3939  //www.w3.org/199
-00000130: 392f 3032 2f32 322d 7264 662d 7379 6e74  9/02/22-rdf-synt
-00000140: 6178 2d6e 7323 220a 2020 2078 6d6c 6e73  ax-ns#".   xmlns
-00000150: 3a73 7667 3d22 6874 7470 3a2f 2f77 7777  :svg="http://www
-00000160: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-00000170: 220a 2020 2078 6d6c 6e73 3d22 6874 7470  ".   xmlns="http
-00000180: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
-00000190: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
-000001a0: 3a78 6c69 6e6b 3d22 6874 7470 3a2f 2f77  :xlink="http://w
-000001b0: 7777 2e77 332e 6f72 672f 3139 3939 2f78  ww.w3.org/1999/x
-000001c0: 6c69 6e6b 220a 2020 2078 6d6c 6e73 3a73  link".   xmlns:s
-000001d0: 6f64 6970 6f64 693d 2268 7474 703a 2f2f  odipodi="http://
-000001e0: 736f 6469 706f 6469 2e73 6f75 7263 6566  sodipodi.sourcef
-000001f0: 6f72 6765 2e6e 6574 2f44 5444 2f73 6f64  orge.net/DTD/sod
-00000200: 6970 6f64 692d 302e 6474 6422 0a20 2020  ipodi-0.dtd".   
-00000210: 786d 6c6e 733a 696e 6b73 6361 7065 3d22  xmlns:inkscape="
-00000220: 6874 7470 3a2f 2f77 7777 2e69 6e6b 7363  http://www.inksc
-00000230: 6170 652e 6f72 672f 6e61 6d65 7370 6163  ape.org/namespac
-00000240: 6573 2f69 6e6b 7363 6170 6522 0a20 2020  es/inkscape".   
-00000250: 7769 6474 683d 2232 3639 2e30 3038 3739  width="269.00879
-00000260: 220a 2020 2068 6569 6768 743d 2232 3639  ".   height="269
-00000270: 2e30 3038 3739 220a 2020 2076 6965 7742  .00879".   viewB
-00000280: 6f78 3d22 3020 3020 3731 2e31 3735 3234  ox="0 0 71.17524
-00000290: 3720 3731 2e31 3735 3234 3922 0a20 2020  7 71.175249".   
-000002a0: 7665 7273 696f 6e3d 2231 2e31 220a 2020  version="1.1".  
-000002b0: 2069 643d 2273 7667 3822 0a20 2020 696e   id="svg8".   in
-000002c0: 6b73 6361 7065 3a76 6572 7369 6f6e 3d22  kscape:version="
-000002d0: 302e 3932 2e33 2028 3234 3035 3534 362c  0.92.3 (2405546,
-000002e0: 2032 3031 382d 3033 2d31 3129 220a 2020   2018-03-11)".  
-000002f0: 2073 6f64 6970 6f64 693a 646f 636e 616d   sodipodi:docnam
-00000300: 653d 2273 7572 7175 6573 745f 7630 2d32  e="surquest_v0-2
-00000310: 2e73 7667 223e 0a20 203c 6465 6673 0a20  .svg">.  <defs. 
-00000320: 2020 2020 6964 3d22 6465 6673 3222 3e0a      id="defs2">.
-00000330: 2020 2020 3c6c 696e 6561 7247 7261 6469      <linearGradi
-00000340: 656e 740a 2020 2020 2020 2069 6e6b 7363  ent.       inksc
-00000350: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
-00000360: 6179 7322 0a20 2020 2020 2020 6964 3d22  ays".       id="
-00000370: 6c69 6e65 6172 4772 6164 6965 6e74 3438  linearGradient48
-00000380: 3436 223e 0a20 2020 2020 203c 7374 6f70  46">.      <stop
-00000390: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-000003a0: 2273 746f 702d 636f 6c6f 723a 2332 6338  "stop-color:#2c8
-000003b0: 3961 303b 7374 6f70 2d6f 7061 6369 7479  9a0;stop-opacity
-000003c0: 3a31 3b22 0a20 2020 2020 2020 2020 6f66  :1;".         of
-000003d0: 6673 6574 3d22 3022 0a20 2020 2020 2020  fset="0".       
-000003e0: 2020 6964 3d22 7374 6f70 3438 3432 2220    id="stop4842" 
-000003f0: 2f3e 0a20 2020 2020 203c 7374 6f70 0a20  />.      <stop. 
-00000400: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-00000410: 3438 3530 220a 2020 2020 2020 2020 206f  4850".         o
-00000420: 6666 7365 743d 2231 220a 2020 2020 2020  ffset="1".      
-00000430: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
-00000440: 6f6c 6f72 3a23 3634 3839 6434 3b73 746f  olor:#6489d4;sto
-00000450: 702d 6f70 6163 6974 793a 3122 202f 3e0a  p-opacity:1" />.
-00000460: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00000470: 6965 6e74 3e0a 2020 2020 3c6c 696e 6561  ient>.    <linea
-00000480: 7247 7261 6469 656e 740a 2020 2020 2020  rGradient.      
-00000490: 2069 6e6b 7363 6170 653a 636f 6c6c 6563   inkscape:collec
-000004a0: 743d 2261 6c77 6179 7322 0a20 2020 2020  t="always".     
-000004b0: 2020 6964 3d22 6c69 6e65 6172 4772 6164    id="linearGrad
-000004c0: 6965 6e74 3437 3939 223e 0a20 2020 2020  ient4799">.     
-000004d0: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
-000004e0: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
-000004f0: 723a 2335 6664 3362 633b 7374 6f70 2d6f  r:#5fd3bc;stop-o
-00000500: 7061 6369 7479 3a31 3b22 0a20 2020 2020  pacity:1;".     
-00000510: 2020 2020 6f66 6673 6574 3d22 3022 0a20      offset="0". 
-00000520: 2020 2020 2020 2020 6964 3d22 7374 6f70          id="stop
-00000530: 3437 3935 2220 2f3e 0a20 2020 2020 203c  4795" />.      <
-00000540: 7374 6f70 0a20 2020 2020 2020 2020 6964  stop.         id
-00000550: 3d22 7374 6f70 3438 3130 220a 2020 2020  ="stop4810".    
-00000560: 2020 2020 206f 6666 7365 743d 2231 220a       offset="1".
-00000570: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00000580: 7374 6f70 2d63 6f6c 6f72 3a23 3566 6433  stop-color:#5fd3
-00000590: 6438 3b73 746f 702d 6f70 6163 6974 793a  d8;stop-opacity:
-000005a0: 3122 202f 3e0a 2020 2020 3c2f 6c69 6e65  1" />.    </line
-000005b0: 6172 4772 6164 6965 6e74 3e0a 2020 2020  arGradient>.    
-000005c0: 3c6c 696e 6561 7247 7261 6469 656e 740a  <linearGradient.
-000005d0: 2020 2020 2020 2069 643d 226c 696e 6561         id="linea
-000005e0: 7247 7261 6469 656e 7432 3334 3222 0a20  rGradient2342". 
-000005f0: 2020 2020 2020 6f73 623a 7061 696e 743d        osb:paint=
-00000600: 2273 6f6c 6964 223e 0a20 2020 2020 203c  "solid">.      <
-00000610: 7374 6f70 0a20 2020 2020 2020 2020 7374  stop.         st
-00000620: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
-00000630: 2330 3030 3030 303b 7374 6f70 2d6f 7061  #000000;stop-opa
-00000640: 6369 7479 3a31 3b22 0a20 2020 2020 2020  city:1;".       
-00000650: 2020 6f66 6673 6574 3d22 3022 0a20 2020    offset="0".   
-00000660: 2020 2020 2020 6964 3d22 7374 6f70 3233        id="stop23
-00000670: 3430 2220 2f3e 0a20 2020 203c 2f6c 696e  40" />.    </lin
-00000680: 6561 7247 7261 6469 656e 743e 0a20 2020  earGradient>.   
-00000690: 203c 6c69 6e65 6172 4772 6164 6965 6e74   <linearGradient
-000006a0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-000006b0: 3a63 6f6c 6c65 6374 3d22 616c 7761 7973  :collect="always
-000006c0: 220a 2020 2020 2020 2078 6c69 6e6b 3a68  ".       xlink:h
-000006d0: 7265 663d 2223 6c69 6e65 6172 4772 6164  ref="#linearGrad
-000006e0: 6965 6e74 3437 3939 220a 2020 2020 2020  ient4799".      
-000006f0: 2069 643d 226c 696e 6561 7247 7261 6469   id="linearGradi
-00000700: 656e 7434 3830 3322 0a20 2020 2020 2020  ent4803".       
-00000710: 6772 6164 6965 6e74 556e 6974 733d 2275  gradientUnits="u
-00000720: 7365 7253 7061 6365 4f6e 5573 6522 0a20  serSpaceOnUse". 
-00000730: 2020 2020 2020 7831 3d22 3430 2e35 3232        x1="40.522
-00000740: 3330 3522 0a20 2020 2020 2020 7931 3d22  305".       y1="
-00000750: 3830 2e39 3033 3436 3522 0a20 2020 2020  80.903465".     
-00000760: 2020 7832 3d22 3330 2e39 3237 3139 3122    x2="30.927191"
-00000770: 0a20 2020 2020 2020 7932 3d22 3830 2e37  .       y2="80.7
-00000780: 3935 3235 2220 2f3e 0a20 2020 203c 6c69  9525" />.    <li
-00000790: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
-000007a0: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
-000007b0: 6c65 6374 3d22 616c 7761 7973 220a 2020  lect="always".  
-000007c0: 2020 2020 2078 6c69 6e6b 3a68 7265 663d       xlink:href=
-000007d0: 2223 6c69 6e65 6172 4772 6164 6965 6e74  "#linearGradient
-000007e0: 3438 3436 220a 2020 2020 2020 2069 643d  4846".       id=
-000007f0: 226c 696e 6561 7247 7261 6469 656e 7431  "linearGradient1
-00000800: 3437 3222 0a20 2020 2020 2020 6772 6164  472".       grad
-00000810: 6965 6e74 556e 6974 733d 2275 7365 7253  ientUnits="userS
-00000820: 7061 6365 4f6e 5573 6522 0a20 2020 2020  paceOnUse".     
-00000830: 2020 6772 6164 6965 6e74 5472 616e 7366    gradientTransf
-00000840: 6f72 6d3d 226d 6174 7269 7828 302e 3831  orm="matrix(0.81
-00000850: 3335 3437 3336 2c30 2c30 2c30 2e38 3133  354736,0,0,0.813
-00000860: 3534 3733 362c 2d32 392e 3036 3430 3831  54736,-29.064081
-00000870: 2c31 382e 3235 3835 3931 2922 0a20 2020  ,18.258591)".   
-00000880: 2020 2020 7831 3d22 3239 2e35 3133 3338      x1="29.51338
-00000890: 220a 2020 2020 2020 2079 313d 2237 322e  ".       y1="72.
-000008a0: 3036 3232 3032 220a 2020 2020 2020 2078  062202".       x
-000008b0: 323d 2234 322e 3138 3930 3638 220a 2020  2="42.189068".  
-000008c0: 2020 2020 2079 323d 2237 322e 3036 3232       y2="72.0622
-000008d0: 3032 2220 2f3e 0a20 2020 203c 6c69 6e65  02" />.    <line
-000008e0: 6172 4772 6164 6965 6e74 0a20 2020 2020  arGradient.     
-000008f0: 2020 696e 6b73 6361 7065 3a63 6f6c 6c65    inkscape:colle
-00000900: 6374 3d22 616c 7761 7973 220a 2020 2020  ct="always".    
-00000910: 2020 2078 6c69 6e6b 3a68 7265 663d 2223     xlink:href="#
-00000920: 6c69 6e65 6172 4772 6164 6965 6e74 3437  linearGradient47
-00000930: 3939 220a 2020 2020 2020 2069 643d 226c  99".       id="l
-00000940: 696e 6561 7247 7261 6469 656e 7431 3437  inearGradient147
-00000950: 3422 0a20 2020 2020 2020 6772 6164 6965  4".       gradie
-00000960: 6e74 556e 6974 733d 2275 7365 7253 7061  ntUnits="userSpa
-00000970: 6365 4f6e 5573 6522 0a20 2020 2020 2020  ceOnUse".       
-00000980: 6772 6164 6965 6e74 5472 616e 7366 6f72  gradientTransfor
-00000990: 6d3d 226d 6174 7269 7828 302e 3831 3335  m="matrix(0.8135
-000009a0: 3437 3336 2c30 2c30 2c30 2e38 3133 3534  4736,0,0,0.81354
-000009b0: 3733 362c 2d32 392e 3036 3430 3831 2c31  736,-29.064081,1
-000009c0: 382e 3235 3835 3931 2922 0a20 2020 2020  8.258591)".     
-000009d0: 2020 7831 3d22 3430 2e35 3232 3330 3522    x1="40.522305"
-000009e0: 0a20 2020 2020 2020 7931 3d22 3830 2e39  .       y1="80.9
-000009f0: 3033 3436 3522 0a20 2020 2020 2020 7832  03465".       x2
-00000a00: 3d22 3330 2e39 3237 3139 3122 0a20 2020  ="30.927191".   
-00000a10: 2020 2020 7932 3d22 3830 2e37 3935 3235      y2="80.79525
-00000a20: 2220 2f3e 0a20 203c 2f64 6566 733e 0a20  " />.  </defs>. 
-00000a30: 203c 736f 6469 706f 6469 3a6e 616d 6564   <sodipodi:named
-00000a40: 7669 6577 0a20 2020 2020 6964 3d22 6261  view.     id="ba
-00000a50: 7365 220a 2020 2020 2070 6167 6563 6f6c  se".     pagecol
-00000a60: 6f72 3d22 2366 6666 6666 6622 0a20 2020  or="#ffffff".   
-00000a70: 2020 626f 7264 6572 636f 6c6f 723d 2223    bordercolor="#
-00000a80: 3636 3636 3636 220a 2020 2020 2062 6f72  666666".     bor
-00000a90: 6465 726f 7061 6369 7479 3d22 312e 3022  deropacity="1.0"
-00000aa0: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
-00000ab0: 6167 656f 7061 6369 7479 3d22 302e 3022  ageopacity="0.0"
-00000ac0: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
-00000ad0: 6167 6573 6861 646f 773d 2232 220a 2020  ageshadow="2".  
-00000ae0: 2020 2069 6e6b 7363 6170 653a 7a6f 6f6d     inkscape:zoom
-00000af0: 3d22 3122 0a20 2020 2020 696e 6b73 6361  ="1".     inksca
-00000b00: 7065 3a63 783d 222d 3334 2e35 3630 3238  pe:cx="-34.56028
-00000b10: 3822 0a20 2020 2020 696e 6b73 6361 7065  8".     inkscape
-00000b20: 3a63 793d 2232 3436 2e30 3131 3834 220a  :cy="246.01184".
-00000b30: 2020 2020 2069 6e6b 7363 6170 653a 646f       inkscape:do
-00000b40: 6375 6d65 6e74 2d75 6e69 7473 3d22 6d6d  cument-units="mm
-00000b50: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000b60: 6375 7272 656e 742d 6c61 7965 723d 2267  current-layer="g
-00000b70: 3236 3038 220a 2020 2020 2073 686f 7767  2608".     showg
-00000b80: 7269 643d 2266 616c 7365 220a 2020 2020  rid="false".    
-00000b90: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-00000ba0: 2d77 6964 7468 3d22 3234 3030 220a 2020  -width="2400".  
-00000bb0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-00000bc0: 6f77 2d68 6569 6768 743d 2231 3237 3122  ow-height="1271"
-00000bd0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-00000be0: 696e 646f 772d 783d 2232 3339 3122 0a20  indow-x="2391". 
-00000bf0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-00000c00: 646f 772d 793d 222d 3922 0a20 2020 2020  dow-y="-9".     
-00000c10: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-00000c20: 6d61 7869 6d69 7a65 643d 2231 220a 2020  maximized="1".  
-00000c30: 2020 2066 6974 2d6d 6172 6769 6e2d 746f     fit-margin-to
-00000c40: 703d 2230 220a 2020 2020 2066 6974 2d6d  p="0".     fit-m
-00000c50: 6172 6769 6e2d 6c65 6674 3d22 3022 0a20  argin-left="0". 
-00000c60: 2020 2020 6669 742d 6d61 7267 696e 2d72      fit-margin-r
-00000c70: 6967 6874 3d22 3022 0a20 2020 2020 6669  ight="0".     fi
-00000c80: 742d 6d61 7267 696e 2d62 6f74 746f 6d3d  t-margin-bottom=
-00000c90: 2230 220a 2020 2020 2073 6361 6c65 2d78  "0".     scale-x
-00000ca0: 3d22 302e 3822 0a20 2020 2020 696e 6b73  ="0.8".     inks
-00000cb0: 6361 7065 3a70 6167 6563 6865 636b 6572  cape:pagechecker
-00000cc0: 626f 6172 643d 2274 7275 6522 0a20 2020  board="true".   
-00000cd0: 2020 756e 6974 733d 2270 7822 0a20 2020    units="px".   
-00000ce0: 2020 696e 6b73 6361 7065 3a73 686f 7770    inkscape:showp
-00000cf0: 6167 6573 6861 646f 773d 2266 616c 7365  ageshadow="false
-00000d00: 220a 2020 2020 2073 686f 7762 6f72 6465  ".     showborde
-00000d10: 723d 2266 616c 7365 220a 2020 2020 2073  r="false".     s
-00000d20: 686f 7767 7569 6465 733d 2266 616c 7365  howguides="false
-00000d30: 2220 2f3e 0a20 203c 6d65 7461 6461 7461  " />.  <metadata
-00000d40: 0a20 2020 2020 6964 3d22 6d65 7461 6461  .     id="metada
-00000d50: 7461 3522 3e0a 2020 2020 3c72 6466 3a52  ta5">.    <rdf:R
-00000d60: 4446 3e0a 2020 2020 2020 3c63 633a 576f  DF>.      <cc:Wo
-00000d70: 726b 0a20 2020 2020 2020 2020 7264 663a  rk.         rdf:
-00000d80: 6162 6f75 743d 2222 3e0a 2020 2020 2020  about="">.      
-00000d90: 2020 3c64 633a 666f 726d 6174 3e69 6d61    <dc:format>ima
-00000da0: 6765 2f73 7667 2b78 6d6c 3c2f 6463 3a66  ge/svg+xml</dc:f
-00000db0: 6f72 6d61 743e 0a20 2020 2020 2020 203c  ormat>.        <
-00000dc0: 6463 3a74 7970 650a 2020 2020 2020 2020  dc:type.        
-00000dd0: 2020 2072 6466 3a72 6573 6f75 7263 653d     rdf:resource=
-00000de0: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
-00000df0: 2f64 632f 6463 6d69 7479 7065 2f53 7469  /dc/dcmitype/Sti
-00000e00: 6c6c 496d 6167 6522 202f 3e0a 2020 2020  llImage" />.    
-00000e10: 2020 2020 3c64 633a 7469 746c 653e 3c2f      <dc:title></
-00000e20: 6463 3a74 6974 6c65 3e0a 2020 2020 2020  dc:title>.      
-00000e30: 3c2f 6363 3a57 6f72 6b3e 0a20 2020 203c  </cc:Work>.    <
-00000e40: 2f72 6466 3a52 4446 3e0a 2020 3c2f 6d65  /rdf:RDF>.  </me
-00000e50: 7461 6461 7461 3e0a 2020 3c67 0a20 2020  tadata>.  <g.   
-00000e60: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00000e70: 3d22 4562 656e 6520 3122 0a20 2020 2020  ="Ebene 1".     
-00000e80: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
-00000e90: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
-00000ea0: 6964 3d22 6c61 7965 7231 220a 2020 2020  id="layer1".    
-00000eb0: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
-00000ec0: 736c 6174 6528 2d31 3937 2e31 3138 3239  slate(-197.11829
-00000ed0: 2c31 3237 2e34 3330 3333 2922 3e0a 2020  ,127.43033)">.  
-00000ee0: 2020 3c74 6578 740a 2020 2020 2020 2078    <text.       x
-00000ef0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
-00000f00: 7665 220a 2020 2020 2020 2073 7479 6c65  ve".       style
-00000f10: 3d22 666f 6e74 2d73 7479 6c65 3a6e 6f72  ="font-style:nor
-00000f20: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
-00000f30: 6e6f 726d 616c 3b66 6f6e 742d 7369 7a65  normal;font-size
-00000f40: 3a31 302e 3538 3333 3333 3032 7078 3b6c  :10.58333302px;l
-00000f50: 696e 652d 6865 6967 6874 3a31 2e32 353b  ine-height:1.25;
-00000f60: 666f 6e74 2d66 616d 696c 793a 7361 6e73  font-family:sans
-00000f70: 2d73 6572 6966 3b6c 6574 7465 722d 7370  -serif;letter-sp
-00000f80: 6163 696e 673a 3070 783b 776f 7264 2d73  acing:0px;word-s
-00000f90: 7061 6369 6e67 3a30 7078 3b66 696c 6c3a  pacing:0px;fill:
-00000fa0: 2330 3030 3030 303b 6669 6c6c 2d6f 7061  #000000;fill-opa
-00000fb0: 6369 7479 3a31 3b73 7472 6f6b 653a 6e6f  city:1;stroke:no
-00000fc0: 6e65 3b73 7472 6f6b 652d 7769 6474 683a  ne;stroke-width:
-00000fd0: 302e 3236 3435 3833 3332 220a 2020 2020  0.26458332".    
-00000fe0: 2020 2078 3d22 3730 2e36 3831 3534 3922     x="70.681549"
-00000ff0: 0a20 2020 2020 2020 793d 2231 3034 2e36  .       y="104.6
-00001000: 3130 3132 220a 2020 2020 2020 2069 643d  1012".       id=
-00001010: 2274 6578 7438 3137 223e 3c74 7370 616e  "text817"><tspan
-00001020: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-00001030: 6469 3a72 6f6c 653d 226c 696e 6522 0a20  di:role="line". 
-00001040: 2020 2020 2020 2020 6964 3d22 7473 7061          id="tspa
-00001050: 6e38 3135 220a 2020 2020 2020 2020 2078  n815".         x
-00001060: 3d22 3730 2e36 3831 3534 3922 0a20 2020  ="70.681549".   
-00001070: 2020 2020 2020 793d 2231 3134 2e32 3635        y="114.265
-00001080: 3632 220a 2020 2020 2020 2020 2073 7479  62".         sty
-00001090: 6c65 3d22 7374 726f 6b65 2d77 6964 7468  le="stroke-width
-000010a0: 3a30 2e32 3634 3538 3333 3222 202f 3e3c  :0.26458332" /><
-000010b0: 2f74 6578 743e 0a20 2020 203c 670a 2020  /text>.    <g.  
-000010c0: 2020 2020 2069 643d 2267 3236 3038 223e       id="g2608">
-000010d0: 0a20 2020 2020 203c 7265 6374 0a20 2020  .      <rect.   
-000010e0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-000010f0: 6c3a 2330 3031 3131 633b 6669 6c6c 2d6f  l:#00111c;fill-o
-00001100: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00001110: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
-00001120: 683a 302e 3633 3430 3737 3835 3b73 7472  h:0.63407785;str
-00001130: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00001140: 2020 2020 2020 2020 793d 222d 3132 372e          y="-127.
-00001150: 3433 3033 3322 0a20 2020 2020 2020 2020  43033".         
-00001160: 783d 2231 3937 2e31 3138 3239 220a 2020  x="197.11829".  
-00001170: 2020 2020 2020 2068 6569 6768 743d 2237         height="7
-00001180: 312e 3137 3532 3422 0a20 2020 2020 2020  1.17524".       
-00001190: 2020 7769 6474 683d 2237 312e 3137 3532    width="71.1752
-000011a0: 3422 0a20 2020 2020 2020 2020 6964 3d22  4".         id="
-000011b0: 7265 6374 3337 3637 2d35 2d36 3122 202f  rect3767-5-61" /
-000011c0: 3e0a 2020 2020 2020 3c67 0a20 2020 2020  >.      <g.     
-000011d0: 2020 2020 7472 616e 7366 6f72 6d3d 226d      transform="m
-000011e0: 6174 7269 7828 322e 3431 3931 3332 392c  atrix(2.4191329,
-000011f0: 302c 302c 322e 3431 3931 3332 392c 3233  0,0,2.4191329,23
-00001200: 332e 3532 3530 342c 2d32 3931 2e30 3939  3.52504,-291.099
-00001210: 3436 2922 0a20 2020 2020 2020 2020 6964  46)".         id
-00001220: 3d22 6738 3937 2d33 2d33 3522 3e0a 2020  ="g897-3-35">.  
-00001230: 2020 2020 2020 3c72 6563 740a 2020 2020        <rect.    
-00001240: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00001250: 3d22 7363 616c 6528 2d31 2c31 2922 0a20  ="scale(-1,1)". 
-00001260: 2020 2020 2020 2020 2020 7374 796c 653d            style=
-00001270: 2266 696c 6c3a 7572 6c28 236c 696e 6561  "fill:url(#linea
-00001280: 7247 7261 6469 656e 7431 3437 3229 3b66  rGradient1472);f
-00001290: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-000012a0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-000012b0: 2d77 6964 7468 3a30 2e32 3836 3933 3935  -width:0.2869395
-000012c0: 393b 7374 726f 6b65 2d6f 7061 6369 7479  9;stroke-opacity
-000012d0: 3a31 220a 2020 2020 2020 2020 2020 2069  :1".           i
-000012e0: 643d 2272 6563 7433 3830 312d 312d 3922  d="rect3801-1-9"
-000012f0: 0a20 2020 2020 2020 2020 2020 7769 6474  .           widt
-00001300: 683d 2231 312e 3734 3138 3236 220a 2020  h="11.741826".  
-00001310: 2020 2020 2020 2020 2068 6569 6768 743d           height=
-00001320: 2237 2e32 3535 3238 3632 220a 2020 2020  "7.2552862".    
-00001330: 2020 2020 2020 2078 3d22 2d35 2e30 3533         x="-5.053
-00001340: 3534 3838 220a 2020 2020 2020 2020 2020  5488".          
-00001350: 2079 3d22 3733 2e32 3536 3935 3822 202f   y="73.256958" /
-00001360: 3e0a 2020 2020 2020 2020 3c72 6563 740a  >.        <rect.
-00001370: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
-00001380: 666f 726d 3d22 7363 616c 6528 2d31 2c31  form="scale(-1,1
-00001390: 2922 0a20 2020 2020 2020 2020 2020 7374  )".           st
-000013a0: 796c 653d 226f 7061 6369 7479 3a31 3b66  yle="opacity:1;f
-000013b0: 696c 6c3a 7572 6c28 236c 696e 6561 7247  ill:url(#linearG
-000013c0: 7261 6469 656e 7431 3437 3429 3b66 696c  radient1474);fil
-000013d0: 6c2d 6f70 6163 6974 793a 313b 6669 6c6c  l-opacity:1;fill
-000013e0: 2d72 756c 653a 6e6f 6e7a 6572 6f3b 7374  -rule:nonzero;st
-000013f0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-00001400: 2d77 6964 7468 3a30 2e32 3837 3837 3039  -width:0.2878709
-00001410: 343b 7374 726f 6b65 2d6f 7061 6369 7479  4;stroke-opacity
-00001420: 3a30 220a 2020 2020 2020 2020 2020 2069  :0".           i
-00001430: 643d 2272 6563 7433 3830 312d 382d 322d  d="rect3801-8-2-
-00001440: 3622 0a20 2020 2020 2020 2020 2020 7769  6".           wi
-00001450: 6474 683d 2231 312e 3935 3930 3539 220a  dth="11.959059".
-00001460: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-00001470: 743d 2237 2e31 3639 3831 3531 220a 2020  t="7.1698151".  
-00001480: 2020 2020 2020 2020 2078 3d22 2d36 2e30           x="-6.0
-00001490: 3131 3532 3939 220a 2020 2020 2020 2020  115299".        
-000014a0: 2020 2079 3d22 3830 2e37 3635 3431 3922     y="80.765419"
-000014b0: 202f 3e0a 2020 2020 2020 2020 3c72 6563   />.        <rec
-000014c0: 740a 2020 2020 2020 2020 2020 2074 7261  t.           tra
-000014d0: 6e73 666f 726d 3d22 7363 616c 6528 2d31  nsform="scale(-1
-000014e0: 2c31 2922 0a20 2020 2020 2020 2020 2020  ,1)".           
-000014f0: 7374 796c 653d 2266 696c 6c3a 2366 6666  style="fill:#fff
-00001500: 6666 663b 7374 726f 6b65 3a6e 6f6e 653b  fff;stroke:none;
-00001510: 7374 726f 6b65 2d77 6964 7468 3a30 2e31  stroke-width:0.1
-00001520: 3933 3531 3238 363b 7374 726f 6b65 2d6f  9351286;stroke-o
-00001530: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00001540: 2020 2020 2069 643d 2272 6563 7433 3736       id="rect376
-00001550: 392d 362d 372d 362d 3422 0a20 2020 2020  9-6-7-6-4".     
-00001560: 2020 2020 2020 7769 6474 683d 2231 322e        width="12.
-00001570: 3639 3938 3122 0a20 2020 2020 2020 2020  69981".         
-00001580: 2020 6865 6967 6874 3d22 312e 3530 3637    height="1.5067
-00001590: 3537 3522 0a20 2020 2020 2020 2020 2020  575".           
-000015a0: 783d 222d 362e 3031 3135 3239 3922 0a20  x="-6.0115299". 
-000015b0: 2020 2020 2020 2020 2020 793d 2238 372e            y="87.
-000015c0: 3235 3134 3732 2220 2f3e 0a20 2020 2020  251472" />.     
-000015d0: 2020 203c 7265 6374 0a20 2020 2020 2020     <rect.       
-000015e0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-000015f0: 2366 6666 6666 663b 7374 726f 6b65 3a6e  #ffffff;stroke:n
-00001600: 6f6e 653b 7374 726f 6b65 2d77 6964 7468  one;stroke-width
-00001610: 3a30 2e31 3632 3738 3431 343b 7374 726f  :0.16278414;stro
-00001620: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00001630: 2020 2020 2020 2020 2069 643d 2272 6563           id="rec
-00001640: 7433 3736 392d 392d 372d 312d 3522 0a20  t3769-9-7-1-5". 
-00001650: 2020 2020 2020 2020 2020 7769 6474 683d            width=
-00001660: 2238 2e39 3836 3733 3036 220a 2020 2020  "8.9867306".    
-00001670: 2020 2020 2020 2068 6569 6768 743d 2231         height="1
-00001680: 2e35 3036 3735 3735 220a 2020 2020 2020  .5067575".      
-00001690: 2020 2020 2078 3d22 3739 2e37 3731 3522       x="79.7715"
-000016a0: 0a20 2020 2020 2020 2020 2020 793d 222d  .           y="-
-000016b0: 362e 3638 3832 3738 3222 0a20 2020 2020  6.6882782".     
-000016c0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-000016d0: 226d 6174 7269 7828 302c 312c 312c 302c  "matrix(0,1,1,0,
-000016e0: 302c 3029 2220 2f3e 0a20 2020 2020 2020  0,0)" />.       
-000016f0: 203c 7265 6374 0a20 2020 2020 2020 2020   <rect.         
-00001700: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
-00001710: 6666 6666 663b 7374 726f 6b65 3a6e 6f6e  fffff;stroke:non
-00001720: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
-00001730: 2e31 3033 3837 3433 333b 7374 726f 6b65  .10387433;stroke
-00001740: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00001750: 2020 2020 2020 2069 643d 2272 6563 7433         id="rect3
-00001760: 3736 392d 392d 302d 342d 3522 0a20 2020  769-9-0-4-5".   
-00001770: 2020 2020 2020 2020 7769 6474 683d 2233          width="3
-00001780: 2e36 3539 3236 3637 220a 2020 2020 2020  .6592667".      
-00001790: 2020 2020 2068 6569 6768 743d 2231 2e35       height="1.5
-000017a0: 3036 3735 3735 220a 2020 2020 2020 2020  067575".        
-000017b0: 2020 2078 3d22 3732 2e32 3931 3531 3922     x="72.291519"
-000017c0: 0a20 2020 2020 2020 2020 2020 793d 222d  .           y="-
-000017d0: 362e 3638 3837 3432 3622 0a20 2020 2020  6.6887426".     
-000017e0: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-000017f0: 226d 6174 7269 7828 302c 312c 312c 302c  "matrix(0,1,1,0,
-00001800: 302c 3029 2220 2f3e 0a20 2020 2020 2020  0,0)" />.       
-00001810: 203c 7265 6374 0a20 2020 2020 2020 2020   <rect.         
-00001820: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
-00001830: 6666 6666 663b 7374 726f 6b65 3a6e 6f6e  fffff;stroke:non
-00001840: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
-00001850: 2e31 3033 3837 3433 333b 7374 726f 6b65  .10387433;stroke
-00001860: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00001870: 2020 2020 2020 2069 643d 2272 6563 7433         id="rect3
-00001880: 3736 392d 392d 302d 312d 302d 3222 0a20  769-9-0-1-0-2". 
-00001890: 2020 2020 2020 2020 2020 7769 6474 683d            width=
-000018a0: 2233 2e36 3539 3236 3637 220a 2020 2020  "3.6592667".    
-000018b0: 2020 2020 2020 2068 6569 6768 743d 2231         height="1
-000018c0: 2e35 3036 3735 3735 220a 2020 2020 2020  .5067575".      
-000018d0: 2020 2020 2078 3d22 3835 2e30 3938 3935       x="85.09895
-000018e0: 3322 0a20 2020 2020 2020 2020 2020 793d  3".           y=
-000018f0: 2234 2e35 3034 3737 3237 220a 2020 2020  "4.5047727".    
-00001900: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-00001910: 3d22 6d61 7472 6978 2830 2c31 2c31 2c30  ="matrix(0,1,1,0
-00001920: 2c30 2c30 2922 202f 3e0a 2020 2020 2020  ,0,0)" />.      
-00001930: 2020 3c72 6563 740a 2020 2020 2020 2020    <rect.        
-00001940: 2020 2079 3d22 3930 2e31 3938 3136 3622     y="90.198166"
-00001950: 0a20 2020 2020 2020 2020 2020 783d 222d  .           x="-
-00001960: 312e 3436 3035 3432 3122 0a20 2020 2020  1.4605421".     
-00001970: 2020 2020 2020 6865 6967 6874 3d22 322e        height="2.
-00001980: 3234 3433 3334 3522 0a20 2020 2020 2020  2443345".       
-00001990: 2020 2020 7769 6474 683d 2232 2e32 3434      width="2.244
-000019a0: 3333 3435 220a 2020 2020 2020 2020 2020  3345".          
-000019b0: 2069 643d 2272 6563 7434 3732 352d 362d   id="rect4725-6-
-000019c0: 3422 0a20 2020 2020 2020 2020 2020 7374  4".           st
-000019d0: 796c 653d 2266 696c 6c3a 2366 6666 6666  yle="fill:#fffff
-000019e0: 663b 7374 726f 6b65 3a6e 6f6e 653b 7374  f;stroke:none;st
-000019f0: 726f 6b65 2d77 6964 7468 3a30 2e31 3732  roke-width:0.172
-00001a00: 3634 3130 383b 7374 726f 6b65 2d6f 7061  64108;stroke-opa
-00001a10: 6369 7479 3a31 2220 2f3e 0a20 2020 2020  city:1" />.     
-00001a20: 2020 203c 7265 6374 0a20 2020 2020 2020     <rect.       
-00001a30: 2020 2020 7472 616e 7366 6f72 6d3d 2273      transform="s
-00001a40: 6361 6c65 282d 312c 3129 220a 2020 2020  cale(-1,1)".    
-00001a50: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00001a60: 6c6c 3a23 6666 6666 6666 3b73 7472 6f6b  ll:#ffffff;strok
-00001a70: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00001a80: 6474 683a 302e 3138 3837 3332 3731 3b73  dth:0.18873271;s
-00001a90: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00001aa0: 0a20 2020 2020 2020 2020 2020 6964 3d22  .           id="
-00001ab0: 7265 6374 3337 3639 2d36 2d33 2d36 3222  rect3769-6-3-62"
-00001ac0: 0a20 2020 2020 2020 2020 2020 7769 6474  .           widt
-00001ad0: 683d 2231 322e 3038 3031 3431 220a 2020  h="12.080141".  
-00001ae0: 2020 2020 2020 2020 2068 6569 6768 743d           height=
-00001af0: 2231 2e35 3036 3735 3735 220a 2020 2020  "1.5067575".    
-00001b00: 2020 2020 2020 2078 3d22 2d36 2e30 3131         x="-6.011
-00001b10: 3532 3939 220a 2020 2020 2020 2020 2020  5299".          
-00001b20: 2079 3d22 3739 2e37 3731 3522 202f 3e0a   y="79.7715" />.
-00001b30: 2020 2020 2020 2020 3c72 6563 740a 2020          <rect.  
-00001b40: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00001b50: 6669 6c6c 3a23 6666 6666 6666 3b73 7472  fill:#ffffff;str
-00001b60: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-00001b70: 7769 6474 683a 302e 3135 3038 3433 3437  width:0.15084347
-00001b80: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00001b90: 3122 0a20 2020 2020 2020 2020 2020 6964  1".           id
-00001ba0: 3d22 7265 6374 3337 3639 2d39 2d31 2d38  ="rect3769-9-1-8
-00001bb0: 220a 2020 2020 2020 2020 2020 2077 6964  ".           wid
-00001bc0: 7468 3d22 372e 3731 3636 3832 3422 0a20  th="7.7166824". 
-00001bd0: 2020 2020 2020 2020 2020 6865 6967 6874            height
-00001be0: 3d22 312e 3530 3637 3537 3522 0a20 2020  ="1.5067575".   
-00001bf0: 2020 2020 2020 2020 783d 2237 322e 3239          x="72.29
-00001c00: 3135 3237 220a 2020 2020 2020 2020 2020  1527".          
-00001c10: 2079 3d22 342e 3530 3437 3732 3722 0a20   y="4.5047727". 
-00001c20: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-00001c30: 6f72 6d3d 226d 6174 7269 7828 302c 312c  orm="matrix(0,1,
-00001c40: 312c 302c 302c 3029 2220 2f3e 0a20 2020  1,0,0,0)" />.   
-00001c50: 2020 2020 203c 7265 6374 0a20 2020 2020       <rect.     
-00001c60: 2020 2020 2020 7472 616e 7366 6f72 6d3d        transform=
-00001c70: 2273 6361 6c65 282d 312c 3129 220a 2020  "scale(-1,1)".  
-00001c80: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00001c90: 6669 6c6c 3a23 6666 6666 6666 3b73 7472  fill:#ffffff;str
-00001ca0: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-00001cb0: 7769 6474 683a 302e 3139 3331 3039 3536  width:0.19310956
-00001cc0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00001cd0: 3122 0a20 2020 2020 2020 2020 2020 6964  1".           id
-00001ce0: 3d22 7265 6374 3337 3639 2d37 2d38 220a  ="rect3769-7-8".
-00001cf0: 2020 2020 2020 2020 2020 2077 6964 7468             width
-00001d00: 3d22 3132 2e36 3436 3932 3822 0a20 2020  ="12.646928".   
-00001d10: 2020 2020 2020 2020 6865 6967 6874 3d22          height="
-00001d20: 312e 3530 3637 3537 3522 0a20 2020 2020  1.5067575".     
-00001d30: 2020 2020 2020 783d 222d 352e 3935 3831        x="-5.9581
-00001d40: 3835 3222 0a20 2020 2020 2020 2020 2020  852".           
-00001d50: 793d 2237 322e 3239 3135 3139 2220 2f3e  y="72.291519" />
-00001d60: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
-00001d70: 2020 3c72 6563 740a 2020 2020 2020 2020    <rect.        
-00001d80: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
-00001d90: 6978 2830 2e37 3037 3130 3637 382c 302e  ix(0.70710678,0.
-00001da0: 3730 3731 3036 3738 2c30 2e37 3037 3130  70710678,0.70710
-00001db0: 3637 382c 2d30 2e37 3037 3130 3637 382c  678,-0.70710678,
-00001dc0: 302c 3029 220a 2020 2020 2020 2020 2079  0,0)".         y
-00001dd0: 3d22 3232 372e 3734 3230 3722 0a20 2020  ="227.74207".   
-00001de0: 2020 2020 2020 783d 2231 3130 2e37 3738        x="110.778
-00001df0: 3833 220a 2020 2020 2020 2020 2068 6569  83".         hei
-00001e00: 6768 743d 2233 2e36 3435 3034 3639 220a  ght="3.6450469".
-00001e10: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
-00001e20: 3130 2e36 3632 3632 3122 0a20 2020 2020  10.662621".     
-00001e30: 2020 2020 6964 3d22 7265 6374 3337 3639      id="rect3769
-00001e40: 2d39 2d30 2d31 2d35 2d30 2d37 220a 2020  -9-0-1-5-0-7".  
-00001e50: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00001e60: 6c6c 3a23 6666 6666 6666 3b73 7472 6f6b  ll:#ffffff;strok
-00001e70: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00001e80: 6474 683a 302e 3237 3537 3836 3535 3b73  dth:0.27578655;s
-00001e90: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00001ea0: 202f 3e0a 2020 2020 3c2f 673e 0a20 203c   />.    </g>.  <
-00001eb0: 2f67 3e0a 3c2f 7376 673e 0a              /g>.</svg>.
+00000080: 6463 3d22 6874 7470 3a2f 2f70 7572 6c2e  dc="http://purl.
+00000090: 6f72 672f 6463 2f65 6c65 6d65 6e74 732f  org/dc/elements/
+000000a0: 312e 312f 220a 2020 2078 6d6c 6e73 3a63  1.1/".   xmlns:c
+000000b0: 633d 2268 7474 703a 2f2f 6372 6561 7469  c="http://creati
+000000c0: 7665 636f 6d6d 6f6e 732e 6f72 672f 6e73  vecommons.org/ns
+000000d0: 2322 0a20 2020 786d 6c6e 733a 7264 663d  #".   xmlns:rdf=
+000000e0: 2268 7474 703a 2f2f 7777 772e 7733 2e6f  "http://www.w3.o
+000000f0: 7267 2f31 3939 392f 3032 2f32 322d 7264  rg/1999/02/22-rd
+00000100: 662d 7379 6e74 6178 2d6e 7323 220a 2020  f-syntax-ns#".  
+00000110: 2078 6d6c 6e73 3a73 7667 3d22 6874 7470   xmlns:svg="http
+00000120: 3a2f 2f77 7777 2e77 332e 6f72 672f 3230  ://www.w3.org/20
+00000130: 3030 2f73 7667 220a 2020 2078 6d6c 6e73  00/svg".   xmlns
+00000140: 3d22 6874 7470 3a2f 2f77 7777 2e77 332e  ="http://www.w3.
+00000150: 6f72 672f 3230 3030 2f73 7667 220a 2020  org/2000/svg".  
+00000160: 2078 6d6c 6e73 3a78 6c69 6e6b 3d22 6874   xmlns:xlink="ht
+00000170: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000180: 3139 3939 2f78 6c69 6e6b 220a 2020 2078  1999/xlink".   x
+00000190: 6d6c 6e73 3a73 6f64 6970 6f64 693d 2268  mlns:sodipodi="h
+000001a0: 7474 703a 2f2f 736f 6469 706f 6469 2e73  ttp://sodipodi.s
+000001b0: 6f75 7263 6566 6f72 6765 2e6e 6574 2f44  ourceforge.net/D
+000001c0: 5444 2f73 6f64 6970 6f64 692d 302e 6474  TD/sodipodi-0.dt
+000001d0: 6422 0a20 2020 786d 6c6e 733a 696e 6b73  d".   xmlns:inks
+000001e0: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
+000001f0: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
+00000200: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
+00000210: 6522 0a20 2020 7769 6474 683d 2233 3222  e".   width="32"
+00000220: 0a20 2020 6865 6967 6874 3d22 3332 220a  .   height="32".
+00000230: 2020 2076 6965 7742 6f78 3d22 3020 3020     viewBox="0 0 
+00000240: 382e 3436 3636 3636 3520 382e 3436 3636  8.4666665 8.4666
+00000250: 3637 220a 2020 2076 6572 7369 6f6e 3d22  67".   version="
+00000260: 312e 3122 0a20 2020 6964 3d22 7376 6738  1.1".   id="svg8
+00000270: 3634 220a 2020 2069 6e6b 7363 6170 653a  64".   inkscape:
+00000280: 7665 7273 696f 6e3d 2230 2e39 322e 3320  version="0.92.3 
+00000290: 2832 3430 3535 3436 2c20 3230 3138 2d30  (2405546, 2018-0
+000002a0: 332d 3131 2922 0a20 2020 736f 6469 706f  3-11)".   sodipo
+000002b0: 6469 3a64 6f63 6e61 6d65 3d22 4444 4c5f  di:docname="DDL_
+000002c0: 6661 7669 636f 6e2e 7376 6722 3e0a 2020  favicon.svg">.  
+000002d0: 3c64 6566 730a 2020 2020 2069 643d 2264  <defs.     id="d
+000002e0: 6566 7338 3538 223e 0a20 2020 203c 6c69  efs858">.    <li
+000002f0: 6e65 6172 4772 6164 6965 6e74 0a20 2020  nearGradient.   
+00000300: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
+00000310: 6c65 6374 3d22 616c 7761 7973 220a 2020  lect="always".  
+00000320: 2020 2020 2069 643d 226c 696e 6561 7247       id="linearG
+00000330: 7261 6469 656e 7431 3032 3122 3e0a 2020  radient1021">.  
+00000340: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
+00000350: 2020 2073 7479 6c65 3d22 7374 6f70 2d63     style="stop-c
+00000360: 6f6c 6f72 3a23 6666 6666 6666 3b73 746f  olor:#ffffff;sto
+00000370: 702d 6f70 6163 6974 793a 3022 0a20 2020  p-opacity:0".   
+00000380: 2020 2020 2020 6f66 6673 6574 3d22 3022        offset="0"
+00000390: 0a20 2020 2020 2020 2020 6964 3d22 7374  .         id="st
+000003a0: 6f70 3130 3137 2220 2f3e 0a20 2020 2020  op1017" />.     
+000003b0: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
+000003c0: 6964 3d22 7374 6f70 3130 3536 220a 2020  id="stop1056".  
+000003d0: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
+000003e0: 2e31 3335 3638 3735 3722 0a20 2020 2020  .13568757".     
+000003f0: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
+00000400: 636f 6c6f 723a 2364 6464 6464 643b 7374  color:#dddddd;st
+00000410: 6f70 2d6f 7061 6369 7479 3a30 2e31 3239  op-opacity:0.129
+00000420: 3431 3137 363b 2220 2f3e 0a20 2020 2020  41176;" />.     
+00000430: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
+00000440: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
+00000450: 723a 2330 3030 3030 303b 7374 6f70 2d6f  r:#000000;stop-o
+00000460: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00000470: 2020 206f 6666 7365 743d 2231 220a 2020     offset="1".  
+00000480: 2020 2020 2020 2069 643d 2273 746f 7031         id="stop1
+00000490: 3031 3922 202f 3e0a 2020 2020 3c2f 6c69  019" />.    </li
+000004a0: 6e65 6172 4772 6164 6965 6e74 3e0a 2020  nearGradient>.  
+000004b0: 2020 3c63 6c69 7050 6174 680a 2020 2020    <clipPath.    
+000004c0: 2020 2069 643d 2253 5647 4944 5f32 5f22     id="SVGID_2_"
+000004d0: 3e0a 2020 2020 2020 3c75 7365 0a20 2020  >.      <use.   
+000004e0: 2020 2020 2020 786c 696e 6b3a 6872 6566        xlink:href
+000004f0: 3d22 2353 5647 4944 5f31 5f22 0a20 2020  ="#SVGID_1_".   
+00000500: 2020 2020 2020 7374 796c 653d 226f 7665        style="ove
+00000510: 7266 6c6f 773a 7669 7369 626c 6522 0a20  rflow:visible". 
+00000520: 2020 2020 2020 2020 6964 3d22 7573 6534          id="use4
+00000530: 3122 0a20 2020 2020 2020 2020 783d 2230  1".         x="0
+00000540: 220a 2020 2020 2020 2020 2079 3d22 3022  ".         y="0"
+00000550: 0a20 2020 2020 2020 2020 7769 6474 683d  .         width=
+00000560: 2231 3030 2522 0a20 2020 2020 2020 2020  "100%".         
+00000570: 6865 6967 6874 3d22 3130 3025 2220 2f3e  height="100%" />
+00000580: 0a20 2020 203c 2f63 6c69 7050 6174 683e  .    </clipPath>
+00000590: 0a20 2020 203c 6c69 6e65 6172 4772 6164  .    <linearGrad
+000005a0: 6965 6e74 0a20 2020 2020 2020 696e 6b73  ient.       inks
+000005b0: 6361 7065 3a63 6f6c 6c65 6374 3d22 616c  cape:collect="al
+000005c0: 7761 7973 220a 2020 2020 2020 2069 643d  ways".       id=
+000005d0: 226c 696e 6561 7247 7261 6469 656e 7431  "linearGradient1
+000005e0: 3036 3222 3e0a 2020 2020 2020 3c73 746f  062">.      <sto
+000005f0: 700a 2020 2020 2020 2020 2073 7479 6c65  p.         style
+00000600: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 3030  ="stop-color:#00
+00000610: 3030 3030 3b73 746f 702d 6f70 6163 6974  0000;stop-opacit
+00000620: 793a 313b 220a 2020 2020 2020 2020 206f  y:1;".         o
+00000630: 6666 7365 743d 2230 220a 2020 2020 2020  ffset="0".      
+00000640: 2020 2069 643d 2273 746f 7031 3035 3822     id="stop1058"
+00000650: 202f 3e0a 2020 2020 2020 3c73 746f 700a   />.      <stop.
+00000660: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00000670: 7374 6f70 2d63 6f6c 6f72 3a23 3030 3030  stop-color:#0000
+00000680: 3030 3b73 746f 702d 6f70 6163 6974 793a  00;stop-opacity:
+00000690: 303b 220a 2020 2020 2020 2020 206f 6666  0;".         off
+000006a0: 7365 743d 2231 220a 2020 2020 2020 2020  set="1".        
+000006b0: 2069 643d 2273 746f 7031 3036 3022 202f   id="stop1060" /
+000006c0: 3e0a 2020 2020 3c2f 6c69 6e65 6172 4772  >.    </linearGr
+000006d0: 6164 6965 6e74 3e0a 2020 2020 3c72 6164  adient>.    <rad
+000006e0: 6961 6c47 7261 6469 656e 740a 2020 2020  ialGradient.    
+000006f0: 2020 2069 6e6b 7363 6170 653a 636f 6c6c     inkscape:coll
+00000700: 6563 743d 2261 6c77 6179 7322 0a20 2020  ect="always".   
+00000710: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000720: 236c 696e 6561 7247 7261 6469 656e 7431  #linearGradient1
+00000730: 3032 3122 0a20 2020 2020 2020 6964 3d22  021".       id="
+00000740: 7261 6469 616c 4772 6164 6965 6e74 3130  radialGradient10
+00000750: 3331 2d39 220a 2020 2020 2020 2063 783d  31-9".       cx=
+00000760: 2231 3130 2e31 3339 3722 0a20 2020 2020  "110.1397".     
+00000770: 2020 6379 3d22 3837 2e36 3433 3134 3322    cy="87.643143"
+00000780: 0a20 2020 2020 2020 6678 3d22 3131 302e  .       fx="110.
+00000790: 3133 3937 220a 2020 2020 2020 2066 793d  1397".       fy=
+000007a0: 2238 372e 3634 3331 3433 220a 2020 2020  "87.643143".    
+000007b0: 2020 2072 3d22 3530 2e35 3939 3939 3822     r="50.599998"
+000007c0: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+000007d0: 5472 616e 7366 6f72 6d3d 226d 6174 7269  Transform="matri
+000007e0: 7828 2d31 2e30 3634 3735 3839 2c30 2c30  x(-1.0647589,0,0
+000007f0: 2c2d 312e 3833 3736 3834 322c 3239 352e  ,-1.8376842,295.
+00000800: 3536 3436 2c32 3438 2e36 3630 3431 2922  5646,248.66041)"
+00000810: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00000820: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00000830: 4f6e 5573 6522 202f 3e0a 2020 2020 3c63  OnUse" />.    <c
+00000840: 6c69 7050 6174 680a 2020 2020 2020 2069  lipPath.       i
+00000850: 643d 2253 5647 4944 5f32 5f2d 3522 3e0a  d="SVGID_2_-5">.
+00000860: 2020 2020 2020 3c75 7365 0a20 2020 2020        <use.     
+00000870: 2020 2020 786c 696e 6b3a 6872 6566 3d22      xlink:href="
+00000880: 2353 5647 4944 5f31 5f22 0a20 2020 2020  #SVGID_1_".     
+00000890: 2020 2020 7374 796c 653d 226f 7665 7266      style="overf
+000008a0: 6c6f 773a 7669 7369 626c 6522 0a20 2020  low:visible".   
+000008b0: 2020 2020 2020 6964 3d22 7573 6534 312d        id="use41-
+000008c0: 3522 0a20 2020 2020 2020 2020 783d 2230  5".         x="0
+000008d0: 220a 2020 2020 2020 2020 2079 3d22 3022  ".         y="0"
+000008e0: 0a20 2020 2020 2020 2020 7769 6474 683d  .         width=
+000008f0: 2231 3030 2522 0a20 2020 2020 2020 2020  "100%".         
+00000900: 6865 6967 6874 3d22 3130 3025 2220 2f3e  height="100%" />
+00000910: 0a20 2020 203c 2f63 6c69 7050 6174 683e  .    </clipPath>
+00000920: 0a20 2020 203c 7261 6469 616c 4772 6164  .    <radialGrad
+00000930: 6965 6e74 0a20 2020 2020 2020 696e 6b73  ient.       inks
+00000940: 6361 7065 3a63 6f6c 6c65 6374 3d22 616c  cape:collect="al
+00000950: 7761 7973 220a 2020 2020 2020 2078 6c69  ways".       xli
+00000960: 6e6b 3a68 7265 663d 2223 6c69 6e65 6172  nk:href="#linear
+00000970: 4772 6164 6965 6e74 3130 3231 220a 2020  Gradient1021".  
+00000980: 2020 2020 2069 643d 2272 6164 6961 6c47       id="radialG
+00000990: 7261 6469 656e 7431 3036 362d 3722 0a20  radient1066-7". 
+000009a0: 2020 2020 2020 6772 6164 6965 6e74 556e        gradientUn
+000009b0: 6974 733d 2275 7365 7253 7061 6365 4f6e  its="userSpaceOn
+000009c0: 5573 6522 0a20 2020 2020 2020 6772 6164  Use".       grad
+000009d0: 6965 6e74 5472 616e 7366 6f72 6d3d 226d  ientTransform="m
+000009e0: 6174 7269 7828 2d31 2e30 3634 3735 3839  atrix(-1.0647589
+000009f0: 2c30 2c30 2c2d 312e 3833 3736 3834 322c  ,0,0,-1.8376842,
+00000a00: 3239 352e 3536 3436 2c32 3438 2e36 3630  295.5646,248.660
+00000a10: 3431 2922 0a20 2020 2020 2020 6378 3d22  41)".       cx="
+00000a20: 3131 302e 3133 3937 220a 2020 2020 2020  110.1397".      
+00000a30: 2063 793d 2238 372e 3634 3331 3433 220a   cy="87.643143".
+00000a40: 2020 2020 2020 2066 783d 2231 3130 2e31         fx="110.1
+00000a50: 3339 3722 0a20 2020 2020 2020 6679 3d22  397".       fy="
+00000a60: 3837 2e36 3433 3134 3322 0a20 2020 2020  87.643143".     
+00000a70: 2020 723d 2235 302e 3539 3939 3938 2220    r="50.599998" 
+00000a80: 2f3e 0a20 2020 203c 7261 6469 616c 4772  />.    <radialGr
+00000a90: 6164 6965 6e74 0a20 2020 2020 2020 696e  adient.       in
+00000aa0: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
+00000ab0: 616c 7761 7973 220a 2020 2020 2020 2078  always".       x
+00000ac0: 6c69 6e6b 3a68 7265 663d 2223 6c69 6e65  link:href="#line
+00000ad0: 6172 4772 6164 6965 6e74 3130 3231 220a  arGradient1021".
+00000ae0: 2020 2020 2020 2069 643d 2272 6164 6961         id="radia
+00000af0: 6c47 7261 6469 656e 7431 3036 382d 3522  lGradient1068-5"
+00000b00: 0a20 2020 2020 2020 6772 6164 6965 6e74  .       gradient
+00000b10: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00000b20: 4f6e 5573 6522 0a20 2020 2020 2020 6772  OnUse".       gr
+00000b30: 6164 6965 6e74 5472 616e 7366 6f72 6d3d  adientTransform=
+00000b40: 226d 6174 7269 7828 2d31 2e30 3634 3735  "matrix(-1.06475
+00000b50: 3839 2c30 2c30 2c2d 312e 3833 3736 3834  89,0,0,-1.837684
+00000b60: 322c 3239 352e 3536 3436 2c32 3438 2e36  2,295.5646,248.6
+00000b70: 3630 3431 2922 0a20 2020 2020 2020 6378  6041)".       cx
+00000b80: 3d22 3131 302e 3133 3937 220a 2020 2020  ="110.1397".    
+00000b90: 2020 2063 793d 2238 372e 3634 3331 3433     cy="87.643143
+00000ba0: 220a 2020 2020 2020 2066 783d 2231 3130  ".       fx="110
+00000bb0: 2e31 3339 3722 0a20 2020 2020 2020 6679  .1397".       fy
+00000bc0: 3d22 3837 2e36 3433 3134 3322 0a20 2020  ="87.643143".   
+00000bd0: 2020 2020 723d 2235 302e 3539 3939 3938      r="50.599998
+00000be0: 2220 2f3e 0a20 2020 203c 6c69 6e65 6172  " />.    <linear
+00000bf0: 4772 6164 6965 6e74 0a20 2020 2020 2020  Gradient.       
+00000c00: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
+00000c10: 3d22 616c 7761 7973 220a 2020 2020 2020  ="always".      
+00000c20: 2078 6c69 6e6b 3a68 7265 663d 2223 6c69   xlink:href="#li
+00000c30: 6e65 6172 4772 6164 6965 6e74 3130 3632  nearGradient1062
+00000c40: 220a 2020 2020 2020 2069 643d 226c 696e  ".       id="lin
+00000c50: 6561 7247 7261 6469 656e 7431 3036 342d  earGradient1064-
+00000c60: 3322 0a20 2020 2020 2020 7831 3d22 3230  3".       x1="20
+00000c70: 372e 3937 3136 3622 0a20 2020 2020 2020  7.97166".       
+00000c80: 7931 3d22 3235 2e32 3531 3835 3222 0a20  y1="25.251852". 
+00000c90: 2020 2020 2020 7832 3d22 3230 372e 3233        x2="207.23
+00000ca0: 3231 3622 0a20 2020 2020 2020 7932 3d22  216".       y2="
+00000cb0: 3235 2e31 3033 3935 3122 0a20 2020 2020  25.103951".     
+00000cc0: 2020 6772 6164 6965 6e74 556e 6974 733d    gradientUnits=
+00000cd0: 2275 7365 7253 7061 6365 4f6e 5573 6522  "userSpaceOnUse"
+00000ce0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00000cf0: 2020 2020 2069 643d 2253 5647 4944 5f31       id="SVGID_1
+00000d00: 5f22 0a20 2020 2020 2020 643d 226d 2031  _".       d="m 1
+00000d10: 3834 2e31 2c37 312e 3920 6820 2d36 352e  84.1,71.9 h -65.
+00000d20: 3420 7620 3020 6820 2d35 2e32 2063 202d  4 v 0 h -5.2 c -
+00000d30: 382e 352c 302e 3220 2d31 352e 332c 372e  8.5,0.2 -15.3,7.
+00000d40: 3220 2d31 352e 332c 3135 2e37 2030 2c38  2 -15.3,15.7 0,8
+00000d50: 2e36 2036 2e38 2c31 352e 3520 3135 2e33  .6 6.8,15.5 15.3
+00000d60: 2c31 352e 3720 6820 352e 3220 7620 3020  ,15.7 h 5.2 v 0 
+00000d70: 6820 3438 2e34 2030 2e32 2076 2030 2068  h 48.4 0.2 v 0 h
+00000d80: 2031 362e 3820 6320 382e 352c 2d30 2e32   16.8 c 8.5,-0.2
+00000d90: 2031 352e 332c 2d37 2e32 2031 352e 332c   15.3,-7.2 15.3,
+00000da0: 2d31 352e 3720 302c 2d38 2e35 202d 362e  -15.7 0,-8.5 -6.
+00000db0: 382c 2d31 352e 3420 2d31 352e 332c 2d31  8,-15.4 -15.3,-1
+00000dc0: 352e 3720 7a22 0a20 2020 2020 2020 696e  5.7 z".       in
+00000dd0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00000de0: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
+00000df0: 3e0a 2020 3c2f 6465 6673 3e0a 2020 3c73  >.  </defs>.  <s
+00000e00: 6f64 6970 6f64 693a 6e61 6d65 6476 6965  odipodi:namedvie
+00000e10: 770a 2020 2020 2069 643d 2262 6173 6522  w.     id="base"
+00000e20: 0a20 2020 2020 7061 6765 636f 6c6f 723d  .     pagecolor=
+00000e30: 2223 6666 6666 6666 220a 2020 2020 2062  "#ffffff".     b
+00000e40: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
+00000e50: 3636 3622 0a20 2020 2020 626f 7264 6572  666".     border
+00000e60: 6f70 6163 6974 793d 2231 2e30 220a 2020  opacity="1.0".  
+00000e70: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
+00000e80: 6f70 6163 6974 793d 2230 2e30 220a 2020  opacity="0.0".  
+00000e90: 2020 2069 6e6b 7363 6170 653a 7061 6765     inkscape:page
+00000ea0: 7368 6164 6f77 3d22 3222 0a20 2020 2020  shadow="2".     
+00000eb0: 696e 6b73 6361 7065 3a7a 6f6f 6d3d 2232  inkscape:zoom="2
+00000ec0: 322e 3632 3734 3137 220a 2020 2020 2069  2.627417".     i
+00000ed0: 6e6b 7363 6170 653a 6378 3d22 362e 3134  nkscape:cx="6.14
+00000ee0: 3439 3436 3322 0a20 2020 2020 696e 6b73  49463".     inks
+00000ef0: 6361 7065 3a63 793d 2231 352e 3335 3633  cape:cy="15.3563
+00000f00: 3122 0a20 2020 2020 696e 6b73 6361 7065  1".     inkscape
+00000f10: 3a64 6f63 756d 656e 742d 756e 6974 733d  :document-units=
+00000f20: 226d 6d22 0a20 2020 2020 696e 6b73 6361  "mm".     inksca
+00000f30: 7065 3a63 7572 7265 6e74 2d6c 6179 6572  pe:current-layer
+00000f40: 3d22 6c61 7965 7231 220a 2020 2020 2073  ="layer1".     s
+00000f50: 686f 7767 7269 643d 2266 616c 7365 220a  howgrid="false".
+00000f60: 2020 2020 2075 6e69 7473 3d22 7078 220a       units="px".
+00000f70: 2020 2020 2069 6e6b 7363 6170 653a 736e       inkscape:sn
+00000f80: 6170 2d6e 6f64 6573 3d22 6661 6c73 6522  ap-nodes="false"
+00000f90: 0a20 2020 2020 696e 6b73 6361 7065 3a73  .     inkscape:s
+00000fa0: 6e61 702d 6262 6f78 3d22 6661 6c73 6522  nap-bbox="false"
+00000fb0: 0a20 2020 2020 696e 6b73 6361 7065 3a73  .     inkscape:s
+00000fc0: 6e61 702d 6772 6964 733d 2266 616c 7365  nap-grids="false
+00000fd0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000fe0: 736e 6170 2d74 6f2d 6775 6964 6573 3d22  snap-to-guides="
+00000ff0: 6661 6c73 6522 0a20 2020 2020 696e 6b73  false".     inks
+00001000: 6361 7065 3a73 6e61 702d 6f74 6865 7273  cape:snap-others
+00001010: 3d22 6661 6c73 6522 0a20 2020 2020 696e  ="false".     in
+00001020: 6b73 6361 7065 3a77 696e 646f 772d 7769  kscape:window-wi
+00001030: 6474 683d 2232 3430 3022 0a20 2020 2020  dth="2400".     
+00001040: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
+00001050: 6865 6967 6874 3d22 3132 3731 220a 2020  height="1271".  
+00001060: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+00001070: 6f77 2d78 3d22 3233 3931 220a 2020 2020  ow-x="2391".    
+00001080: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
+00001090: 2d79 3d22 2d39 220a 2020 2020 2069 6e6b  -y="-9".     ink
+000010a0: 7363 6170 653a 7769 6e64 6f77 2d6d 6178  scape:window-max
+000010b0: 696d 697a 6564 3d22 3122 202f 3e0a 2020  imized="1" />.  
+000010c0: 3c6d 6574 6164 6174 610a 2020 2020 2069  <metadata.     i
+000010d0: 643d 226d 6574 6164 6174 6138 3631 223e  d="metadata861">
+000010e0: 0a20 2020 203c 7264 663a 5244 463e 0a20  .    <rdf:RDF>. 
+000010f0: 2020 2020 203c 6363 3a57 6f72 6b0a 2020       <cc:Work.  
+00001100: 2020 2020 2020 2072 6466 3a61 626f 7574         rdf:about
+00001110: 3d22 223e 0a20 2020 2020 2020 203c 6463  ="">.        <dc
+00001120: 3a66 6f72 6d61 743e 696d 6167 652f 7376  :format>image/sv
+00001130: 672b 786d 6c3c 2f64 633a 666f 726d 6174  g+xml</dc:format
+00001140: 3e0a 2020 2020 2020 2020 3c64 633a 7479  >.        <dc:ty
+00001150: 7065 0a20 2020 2020 2020 2020 2020 7264  pe.           rd
+00001160: 663a 7265 736f 7572 6365 3d22 6874 7470  f:resource="http
+00001170: 3a2f 2f70 7572 6c2e 6f72 672f 6463 2f64  ://purl.org/dc/d
+00001180: 636d 6974 7970 652f 5374 696c 6c49 6d61  cmitype/StillIma
+00001190: 6765 2220 2f3e 0a20 2020 2020 2020 203c  ge" />.        <
+000011a0: 6463 3a74 6974 6c65 3e3c 2f64 633a 7469  dc:title></dc:ti
+000011b0: 746c 653e 0a20 2020 2020 203c 2f63 633a  tle>.      </cc:
+000011c0: 576f 726b 3e0a 2020 2020 3c2f 7264 663a  Work>.    </rdf:
+000011d0: 5244 463e 0a20 203c 2f6d 6574 6164 6174  RDF>.  </metadat
+000011e0: 613e 0a20 203c 670a 2020 2020 2069 6e6b  a>.  <g.     ink
+000011f0: 7363 6170 653a 6c61 6265 6c3d 2245 6265  scape:label="Ebe
+00001200: 6e65 2031 220a 2020 2020 2069 6e6b 7363  ne 1".     inksc
+00001210: 6170 653a 6772 6f75 706d 6f64 653d 226c  ape:groupmode="l
+00001220: 6179 6572 220a 2020 2020 2069 643d 226c  ayer".     id="l
+00001230: 6179 6572 3122 0a20 2020 2020 7472 616e  ayer1".     tran
+00001240: 7366 6f72 6d3d 2274 7261 6e73 6c61 7465  sform="translate
+00001250: 2830 2c2d 3238 382e 3533 3333 3129 223e  (0,-288.53331)">
+00001260: 0a20 2020 203c 670a 2020 2020 2020 2069  .    <g.       i
+00001270: 643d 2267 3137 3038 220a 2020 2020 2020  d="g1708".      
+00001280: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
+00001290: 6978 2830 2e33 3135 3933 3934 382c 302c  ix(0.31593948,0,
+000012a0: 302c 302e 3331 3539 3339 3438 2c32 2e34  0,0.31593948,2.4
+000012b0: 3839 3930 3139 2c31 3939 2e36 3434 3138  899019,199.64418
+000012c0: 2922 0a20 2020 2020 2020 7374 796c 653d  )".       style=
+000012d0: 2273 7472 6f6b 652d 7769 6474 683a 332e  "stroke-width:3.
+000012e0: 3136 3531 3633 3034 223e 0a20 2020 2020  16516304">.     
+000012f0: 203c 670a 2020 2020 2020 2020 2069 643d   <g.         id=
+00001300: 2267 3637 220a 2020 2020 2020 2020 2074  "g67".         t
+00001310: 7261 6e73 666f 726d 3d22 6d61 7472 6978  ransform="matrix
+00001320: 2830 2e32 3634 3538 3333 332c 302c 302c  (0.26458333,0,0,
+00001330: 302e 3236 3435 3833 3333 2c2d 3335 2e38  0.26458333,-35.8
+00001340: 3332 3637 352c 3236 392e 3930 3532 3829  32675,269.90528)
+00001350: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+00001360: 3d22 7374 726f 6b65 2d77 6964 7468 3a33  ="stroke-width:3
+00001370: 2e31 3635 3136 3330 3422 3e0a 2020 2020  .16516304">.    
+00001380: 2020 2020 3c64 6566 730a 2020 2020 2020      <defs.      
+00001390: 2020 2020 2069 643d 2264 6566 7333 3922       id="defs39"
+000013a0: 3e0a 2020 2020 2020 2020 2020 3c70 6174  >.          <pat
+000013b0: 680a 2020 2020 2020 2020 2020 2020 2069  h.             i
+000013c0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+000013d0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+000013e0: 2020 2020 2020 2020 2020 2020 2064 3d22               d="
+000013f0: 6d20 3138 342e 312c 3731 2e39 2068 202d  m 184.1,71.9 h -
+00001400: 3635 2e34 2076 2030 2068 202d 352e 3220  65.4 v 0 h -5.2 
+00001410: 6320 2d38 2e35 2c30 2e32 202d 3135 2e33  c -8.5,0.2 -15.3
+00001420: 2c37 2e32 202d 3135 2e33 2c31 352e 3720  ,7.2 -15.3,15.7 
+00001430: 302c 382e 3620 362e 382c 3135 2e35 2031  0,8.6 6.8,15.5 1
+00001440: 352e 332c 3135 2e37 2068 2035 2e32 2076  5.3,15.7 h 5.2 v
+00001450: 2030 2068 2034 382e 3420 302e 3220 7620   0 h 48.4 0.2 v 
+00001460: 3020 6820 3136 2e38 2063 2038 2e35 2c2d  0 h 16.8 c 8.5,-
+00001470: 302e 3220 3135 2e33 2c2d 372e 3220 3135  0.2 15.3,-7.2 15
+00001480: 2e33 2c2d 3135 2e37 2030 2c2d 382e 3520  .3,-15.7 0,-8.5 
+00001490: 2d36 2e38 2c2d 3135 2e34 202d 3135 2e33  -6.8,-15.4 -15.3
+000014a0: 2c2d 3135 2e37 207a 220a 2020 2020 2020  ,-15.7 z".      
+000014b0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000014c0: 3637 3122 202f 3e0a 2020 2020 2020 2020  671" />.        
+000014d0: 3c2f 6465 6673 3e0a 2020 2020 2020 2020  </defs>.        
+000014e0: 3c63 6c69 7050 6174 680a 2020 2020 2020  <clipPath.      
+000014f0: 2020 2020 2069 643d 2263 6c69 7050 6174       id="clipPat
+00001500: 6831 3630 3522 3e0a 2020 2020 2020 2020  h1605">.        
+00001510: 2020 3c75 7365 0a20 2020 2020 2020 2020    <use.         
+00001520: 2020 2020 6865 6967 6874 3d22 3130 3025      height="100%
+00001530: 220a 2020 2020 2020 2020 2020 2020 2077  ".             w
+00001540: 6964 7468 3d22 3130 3025 220a 2020 2020  idth="100%".    
+00001550: 2020 2020 2020 2020 2079 3d22 3022 0a20           y="0". 
+00001560: 2020 2020 2020 2020 2020 2020 783d 2230              x="0
+00001570: 220a 2020 2020 2020 2020 2020 2020 2069  ".             i
+00001580: 643d 2275 7365 3136 3033 220a 2020 2020  d="use1603".    
+00001590: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+000015a0: 6f76 6572 666c 6f77 3a76 6973 6962 6c65  overflow:visible
+000015b0: 220a 2020 2020 2020 2020 2020 2020 2078  ".             x
+000015c0: 6c69 6e6b 3a68 7265 663d 2223 5356 4749  link:href="#SVGI
+000015d0: 445f 315f 2220 2f3e 0a20 2020 2020 2020  D_1_" />.       
+000015e0: 203c 2f63 6c69 7050 6174 683e 0a20 2020   </clipPath>.   
+000015f0: 2020 2020 203c 670a 2020 2020 2020 2020       <g.        
+00001600: 2020 2073 7479 6c65 3d22 6669 6c6c 3a75     style="fill:u
+00001610: 726c 2823 7261 6469 616c 4772 6164 6965  rl(#radialGradie
+00001620: 6e74 3130 3331 2d39 293b 6669 6c6c 2d6f  nt1031-9);fill-o
+00001630: 7061 6369 7479 3a31 3b66 696c 6c2d 7275  pacity:1;fill-ru
+00001640: 6c65 3a6e 6f6e 7a65 726f 3b73 7472 6f6b  le:nonzero;strok
+00001650: 652d 7769 6474 683a 332e 3136 3531 3633  e-width:3.165163
+00001660: 3034 220a 2020 2020 2020 2020 2020 2074  04".           t
+00001670: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
+00001680: 6174 6528 372e 3435 3831 3731 2c36 2e30  ate(7.458171,6.0
+00001690: 3637 3636 3536 2922 0a20 2020 2020 2020  676656)".       
+000016a0: 2020 2020 6964 3d22 6736 352d 302d 3622      id="g65-0-6"
+000016b0: 0a20 2020 2020 2020 2020 2020 636c 6970  .           clip
+000016c0: 2d70 6174 683d 2275 726c 2823 5356 4749  -path="url(#SVGI
+000016d0: 445f 325f 2d35 2922 0a20 2020 2020 2020  D_2_-5)".       
+000016e0: 2020 2020 636c 6173 733d 2273 7430 223e      class="st0">
+000016f0: 0a20 2020 2020 2020 2020 203c 7261 6469  .          <radi
+00001700: 616c 4772 6164 6965 6e74 0a20 2020 2020  alGradient.     
+00001710: 2020 2020 2020 2020 6772 6164 6965 6e74          gradient
+00001720: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
+00001730: 4f6e 5573 6522 0a20 2020 2020 2020 2020  OnUse".         
+00001740: 2020 2020 6772 6164 6965 6e74 5472 616e      gradientTran
+00001750: 7366 6f72 6d3d 2272 6f74 6174 6528 3138  sform="rotate(18
+00001760: 302c 3739 302e 3533 3432 2c2d 3133 3530  0,790.5342,-1350
+00001770: 2e36 3736 3829 220a 2020 2020 2020 2020  .6768)".        
+00001780: 2020 2020 2066 793d 222d 3237 3839 2e30       fy="-2789.0
+00001790: 3736 3222 0a20 2020 2020 2020 2020 2020  762".           
+000017a0: 2020 6678 3d22 3133 3934 2e37 3931 3522    fx="1394.7915"
+000017b0: 0a20 2020 2020 2020 2020 2020 2020 723d  .             r=
+000017c0: 2234 332e 3831 3832 3938 220a 2020 2020  "43.818298".    
+000017d0: 2020 2020 2020 2020 2063 793d 222d 3237           cy="-27
+000017e0: 3839 2e30 3138 3822 0a20 2020 2020 2020  89.0188".       
+000017f0: 2020 2020 2020 6378 3d22 3134 3232 2e39        cx="1422.9
+00001800: 3430 3722 0a20 2020 2020 2020 2020 2020  407".           
+00001810: 2020 6964 3d22 7261 6469 616c 4772 6164    id="radialGrad
+00001820: 6965 6e74 3936 322d 3422 3e0a 2020 2020  ient962-4">.    
+00001830: 2020 2020 2020 2020 3c73 746f 700a 2020          <stop.  
+00001840: 2020 2020 2020 2020 2020 2020 2069 643d               id=
+00001850: 2273 746f 7039 3436 2d37 220a 2020 2020  "stop946-7".    
+00001860: 2020 2020 2020 2020 2020 2073 7479 6c65             style
+00001870: 3d22 7374 6f70 2d63 6f6c 6f72 3a23 4646  ="stop-color:#FF
+00001880: 4646 4646 3b66 696c 6c2d 6f70 6163 6974  FFFF;fill-opacit
+00001890: 793a 313b 6669 6c6c 3a75 726c 2823 7261  y:1;fill:url(#ra
+000018a0: 6469 616c 4772 6164 6965 6e74 3130 3331  dialGradient1031
+000018b0: 2922 0a20 2020 2020 2020 2020 2020 2020  )".             
+000018c0: 2020 6f66 6673 6574 3d22 302e 3334 3038    offset="0.3408
+000018d0: 2220 2f3e 0a20 2020 2020 2020 2020 2020  " />.           
+000018e0: 203c 7374 6f70 0a20 2020 2020 2020 2020   <stop.         
+000018f0: 2020 2020 2020 6964 3d22 7374 6f70 3934        id="stop94
+00001900: 382d 3922 0a20 2020 2020 2020 2020 2020  8-9".           
+00001910: 2020 2020 7374 796c 653d 2273 746f 702d      style="stop-
+00001920: 636f 6c6f 723a 2343 4643 4643 463b 6669  color:#CFCFCF;fi
+00001930: 6c6c 2d6f 7061 6369 7479 3a31 3b66 696c  ll-opacity:1;fil
+00001940: 6c3a 7572 6c28 2372 6164 6961 6c47 7261  l:url(#radialGra
+00001950: 6469 656e 7431 3033 3129 220a 2020 2020  dient1031)".    
+00001960: 2020 2020 2020 2020 2020 206f 6666 7365             offse
+00001970: 743d 2230 2e34 3233 3722 202f 3e0a 2020  t="0.4237" />.  
+00001980: 2020 2020 2020 2020 2020 3c73 746f 700a            <stop.
+00001990: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000019a0: 643d 2273 746f 7039 3530 2d35 220a 2020  d="stop950-5".  
+000019b0: 2020 2020 2020 2020 2020 2020 2073 7479               sty
+000019c0: 6c65 3d22 7374 6f70 2d63 6f6c 6f72 3a23  le="stop-color:#
+000019d0: 3931 3931 3931 3b66 696c 6c2d 6f70 6163  919191;fill-opac
+000019e0: 6974 793a 313b 6669 6c6c 3a75 726c 2823  ity:1;fill:url(#
+000019f0: 7261 6469 616c 4772 6164 6965 6e74 3130  radialGradient10
+00001a00: 3331 2922 0a20 2020 2020 2020 2020 2020  31)".           
+00001a10: 2020 2020 6f66 6673 6574 3d22 302e 3534      offset="0.54
+00001a20: 3222 202f 3e0a 2020 2020 2020 2020 2020  2" />.          
+00001a30: 2020 3c73 746f 700a 2020 2020 2020 2020    <stop.        
+00001a40: 2020 2020 2020 2069 643d 2273 746f 7039         id="stop9
+00001a50: 3532 2d30 220a 2020 2020 2020 2020 2020  52-0".          
+00001a60: 2020 2020 2073 7479 6c65 3d22 7374 6f70       style="stop
+00001a70: 2d63 6f6c 6f72 3a23 3544 3544 3544 3b66  -color:#5D5D5D;f
+00001a80: 696c 6c2d 6f70 6163 6974 793a 313b 6669  ill-opacity:1;fi
+00001a90: 6c6c 3a75 726c 2823 7261 6469 616c 4772  ll:url(#radialGr
+00001aa0: 6164 6965 6e74 3130 3331 2922 0a20 2020  adient1031)".   
+00001ab0: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
+00001ac0: 6574 3d22 302e 3635 3534 2220 2f3e 0a20  et="0.6554" />. 
+00001ad0: 2020 2020 2020 2020 2020 203c 7374 6f70             <stop
+00001ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001af0: 6964 3d22 7374 6f70 3935 342d 3322 0a20  id="stop954-3". 
+00001b00: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00001b10: 796c 653d 2273 746f 702d 636f 6c6f 723a  yle="stop-color:
+00001b20: 2333 3533 3533 353b 6669 6c6c 2d6f 7061  #353535;fill-opa
+00001b30: 6369 7479 3a31 3b66 696c 6c3a 7572 6c28  city:1;fill:url(
+00001b40: 2372 6164 6961 6c47 7261 6469 656e 7431  #radialGradient1
+00001b50: 3033 3129 220a 2020 2020 2020 2020 2020  031)".          
+00001b60: 2020 2020 206f 6666 7365 743d 2230 2e37       offset="0.7
+00001b70: 3630 3922 202f 3e0a 2020 2020 2020 2020  609" />.        
+00001b80: 2020 2020 3c73 746f 700a 2020 2020 2020      <stop.      
+00001b90: 2020 2020 2020 2020 2069 643d 2273 746f           id="sto
+00001ba0: 7039 3536 2d30 220a 2020 2020 2020 2020  p956-0".        
+00001bb0: 2020 2020 2020 2073 7479 6c65 3d22 7374         style="st
+00001bc0: 6f70 2d63 6f6c 6f72 3a23 3138 3138 3138  op-color:#181818
+00001bd0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00001be0: 6669 6c6c 3a75 726c 2823 7261 6469 616c  fill:url(#radial
+00001bf0: 4772 6164 6965 6e74 3130 3331 2922 0a20  Gradient1031)". 
+00001c00: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+00001c10: 6673 6574 3d22 302e 3835 3637 2220 2f3e  fset="0.8567" />
+00001c20: 0a20 2020 2020 2020 2020 2020 203c 7374  .            <st
+00001c30: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+00001c40: 2020 6964 3d22 7374 6f70 3935 382d 3522    id="stop958-5"
+00001c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c60: 7374 796c 653d 2273 746f 702d 636f 6c6f  style="stop-colo
+00001c70: 723a 2330 3630 3630 363b 6669 6c6c 2d6f  r:#060606;fill-o
+00001c80: 7061 6369 7479 3a31 3b66 696c 6c3a 7572  pacity:1;fill:ur
+00001c90: 6c28 2372 6164 6961 6c47 7261 6469 656e  l(#radialGradien
+00001ca0: 7431 3033 3129 220a 2020 2020 2020 2020  t1031)".        
+00001cb0: 2020 2020 2020 206f 6666 7365 743d 2230         offset="0
+00001cc0: 2e39 3339 3522 202f 3e0a 2020 2020 2020  .9395" />.      
+00001cd0: 2020 2020 2020 3c73 746f 700a 2020 2020        <stop.    
+00001ce0: 2020 2020 2020 2020 2020 2069 643d 2273             id="s
+00001cf0: 746f 7039 3630 2d38 220a 2020 2020 2020  top960-8".      
+00001d00: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00001d10: 7374 6f70 2d63 6f6c 6f72 3a23 3030 3030  stop-color:#0000
+00001d20: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
+00001d30: 313b 6669 6c6c 3a75 726c 2823 7261 6469  1;fill:url(#radi
+00001d40: 616c 4772 6164 6965 6e74 3130 3331 2922  alGradient1031)"
+00001d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d60: 6f66 6673 6574 3d22 3122 202f 3e0a 2020  offset="1" />.  
+00001d70: 2020 2020 2020 2020 3c2f 7261 6469 616c          </radial
+00001d80: 4772 6164 6965 6e74 3e0a 2020 2020 2020  Gradient>.      
+00001d90: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00001da0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00001db0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00001dc0: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+00001dd0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00001de0: 3a75 726c 2823 7261 6469 616c 4772 6164  :url(#radialGrad
+00001df0: 6965 6e74 3130 3636 2d37 293b 6669 6c6c  ient1066-7);fill
+00001e00: 2d6f 7061 6369 7479 3a31 3b66 696c 6c2d  -opacity:1;fill-
+00001e10: 7275 6c65 3a6e 6f6e 7a65 726f 3b73 7472  rule:nonzero;str
+00001e20: 6f6b 652d 7769 6474 683a 332e 3136 3531  oke-width:3.1651
+00001e30: 3633 3034 220a 2020 2020 2020 2020 2020  6304".          
+00001e40: 2020 2069 643d 2270 6174 6836 312d 362d     id="path61-6-
+00001e50: 3122 0a20 2020 2020 2020 2020 2020 2020  1".             
+00001e60: 643d 226d 2039 382e 322c 3837 2e37 2063  d="m 98.2,87.7 c
+00001e70: 2030 2c38 2e36 2036 2e38 2c31 352e 3520   0,8.6 6.8,15.5 
+00001e80: 3135 2e33 2c31 352e 3720 7620 3020 4820  15.3,15.7 v 0 H 
+00001e90: 3231 3820 5620 3731 2e39 2048 2031 3133  218 V 71.9 H 113
+00001ea0: 2e35 2076 2030 2043 2031 3035 2c37 322e  .5 v 0 C 105,72.
+00001eb0: 3220 3938 2e32 2c37 392e 3120 3938 2e32  2 98.2,79.1 98.2
+00001ec0: 2c38 372e 3720 5a22 0a20 2020 2020 2020  ,87.7 Z".       
+00001ed0: 2020 2020 2020 636c 6173 733d 2273 7431        class="st1
+00001ee0: 2220 2f3e 0a20 2020 2020 2020 2020 203c  " />.          <
+00001ef0: 7265 6374 0a20 2020 2020 2020 2020 2020  rect.           
+00001f00: 2020 7374 796c 653d 2266 696c 6c3a 7572    style="fill:ur
+00001f10: 6c28 2372 6164 6961 6c47 7261 6469 656e  l(#radialGradien
+00001f20: 7431 3036 382d 3529 3b66 696c 6c2d 6f70  t1068-5);fill-op
+00001f30: 6163 6974 793a 313b 6669 6c6c 2d72 756c  acity:1;fill-rul
+00001f40: 653a 6e6f 6e7a 6572 6f3b 7374 726f 6b65  e:nonzero;stroke
+00001f50: 3a75 726c 2823 6c69 6e65 6172 4772 6164  :url(#linearGrad
+00001f60: 6965 6e74 3130 3634 2d33 293b 7374 726f  ient1064-3);stro
+00001f70: 6b65 2d77 6964 7468 3a33 2e31 3635 3136  ke-width:3.16516
+00001f80: 3330 3422 0a20 2020 2020 2020 2020 2020  304".           
+00001f90: 2020 6964 3d22 7265 6374 3633 2d39 2d36    id="rect63-9-6
+00001fa0: 220a 2020 2020 2020 2020 2020 2020 2068  ".             h
+00001fb0: 6569 6768 743d 2235 3022 0a20 2020 2020  eight="50".     
+00001fc0: 2020 2020 2020 2020 7769 6474 683d 2235          width="5
+00001fd0: 332e 3730 3030 3031 220a 2020 2020 2020  3.700001".      
+00001fe0: 2020 2020 2020 2063 6c61 7373 3d22 7374         class="st
+00001ff0: 3222 0a20 2020 2020 2020 2020 2020 2020  2".             
+00002000: 7472 616e 7366 6f72 6d3d 2272 6f74 6174  transform="rotat
+00002010: 6528 3137 392e 3939 3939 352c 3231 302e  e(179.99995,210.
+00002020: 3731 3231 312c 3838 2e39 3030 3133 3429  71211,88.900134)
+00002030: 220a 2020 2020 2020 2020 2020 2020 2079  ".             y
+00002040: 3d22 3633 2e39 3030 3030 3222 0a20 2020  ="63.900002".   
+00002050: 2020 2020 2020 2020 2020 783d 2231 3833            x="183
+00002060: 2e38 2220 2f3e 0a20 2020 2020 2020 203c  .8" />.        <
+00002070: 2f67 3e0a 2020 2020 2020 3c2f 673e 0a20  /g>.      </g>. 
+00002080: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
+00002090: 2020 2020 2020 7374 796c 653d 2273 7472        style="str
+000020a0: 6f6b 652d 7769 6474 683a 302e 3833 3734  oke-width:0.8374
+000020b0: 3439 3337 220a 2020 2020 2020 2020 2069  4937".         i
+000020c0: 643d 2263 6972 636c 6536 392d 3122 0a20  d="circle69-1". 
+000020d0: 2020 2020 2020 2020 723d 2234 2e31 3533          r="4.153
+000020e0: 3935 3833 220a 2020 2020 2020 2020 2063  9583".         c
+000020f0: 793d 2232 3934 2e36 3834 3636 220a 2020  y="294.68466".  
+00002100: 2020 2020 2020 2063 783d 2231 342e 3736         cx="14.76
+00002110: 3438 3938 2220 2f3e 0a20 2020 203c 2f67  4898" />.    </g
+00002120: 3e0a 2020 3c2f 673e 0a3c 2f73 7667 3e0a  >.  </g>.</svg>.
```

### Comparing `django-ddm-0.1.9/ddm/static/ddm/js/bootstrap4/bootstrap.bundle.min.js` & `django-ddm-1.0.0/ddm/static/ddm/js/bootstrap/bootstrap.bundle.min.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,2512 +1,3101 @@
 /*!
- * Bootstrap v4.5.2 (https://getbootstrap.com/)
- * Copyright 2011-2020 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
+ * Bootstrap v5.1.3 (https://getbootstrap.com/)
+ * Copyright 2011-2021 The Bootstrap Authors (https://github.com/twbs/bootstrap/graphs/contributors)
  * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE)
  */
 ! function(t, e) {
-    "object" == typeof exports && "undefined" != typeof module ? e(exports, require("jquery")) : "function" == typeof define && define.amd ? define(["exports", "jquery"], e) : e((t = "undefined" != typeof globalThis ? globalThis : t || self).bootstrap = {}, t.jQuery)
-}(this, (function(t, e) {
+    "object" == typeof exports && "undefined" != typeof module ? module.exports = e() : "function" == typeof define && define.amd ? define(e) : (t = "undefined" != typeof globalThis ? globalThis : t || self).bootstrap = e()
+}(this, (function() {
     "use strict";
-
-    function n(t, e) {
-        for (var n = 0; n < e.length; n++) {
-            var i = e[n];
-            i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
-        }
-    }
-
-    function i(t, e, i) {
-        return e && n(t.prototype, e), i && n(t, i), t
-    }
-
-    function o() {
-        return (o = Object.assign || function(t) {
-            for (var e = 1; e < arguments.length; e++) {
-                var n = arguments[e];
-                for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
-            }
-            return t
-        }).apply(this, arguments)
-    }
-    e = e && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e;
-
-    function r(t) {
-        var n = this,
-            i = !1;
-        return e(this).one(s.TRANSITION_END, (function() {
-            i = !0
-        })), setTimeout((function() {
-            i || s.triggerTransitionEnd(n)
-        }), t), this
-    }
-    var s = {
-        TRANSITION_END: "bsTransitionEnd",
-        getUID: function(t) {
-            do {
-                t += ~~(1e6 * Math.random())
-            } while (document.getElementById(t));
-            return t
-        },
-        getSelectorFromElement: function(t) {
-            var e = t.getAttribute("data-target");
+    const t = "transitionend",
+        e = t => {
+            let e = t.getAttribute("data-bs-target");
             if (!e || "#" === e) {
-                var n = t.getAttribute("href");
-                e = n && "#" !== n ? n.trim() : ""
-            }
-            try {
-                return document.querySelector(e) ? e : null
-            } catch (t) {
-                return null
-            }
-        },
-        getTransitionDurationFromElement: function(t) {
-            if (!t) return 0;
-            var n = e(t).css("transition-duration"),
-                i = e(t).css("transition-delay"),
-                o = parseFloat(n),
-                r = parseFloat(i);
-            return o || r ? (n = n.split(",")[0], i = i.split(",")[0], 1e3 * (parseFloat(n) + parseFloat(i))) : 0
-        },
-        reflow: function(t) {
-            return t.offsetHeight
-        },
-        triggerTransitionEnd: function(t) {
-            e(t).trigger("transitionend")
-        },
-        supportsTransitionEnd: function() {
-            return Boolean("transitionend")
-        },
-        isElement: function(t) {
-            return (t[0] || t).nodeType
-        },
-        typeCheckConfig: function(t, e, n) {
-            for (var i in n)
-                if (Object.prototype.hasOwnProperty.call(n, i)) {
-                    var o = n[i],
-                        r = e[i],
-                        a = r && s.isElement(r) ? "element" : null === (l = r) || "undefined" == typeof l ? "" + l : {}.toString.call(l).match(/\s([a-z]+)/i)[1].toLowerCase();
-                    if (!new RegExp(o).test(a)) throw new Error(t.toUpperCase() + ': Option "' + i + '" provided type "' + a + '" but expected type "' + o + '".')
-                } var l
+                let i = t.getAttribute("href");
+                if (!i || !i.includes("#") && !i.startsWith(".")) return null;
+                i.includes("#") && !i.startsWith("#") && (i = `#${i.split("#")[1]}`), e = i && "#" !== i ? i.trim() : null
+            }
+            return e
+        },
+        i = t => {
+            const i = e(t);
+            return i && document.querySelector(i) ? i : null
+        },
+        n = t => {
+            const i = e(t);
+            return i ? document.querySelector(i) : null
+        },
+        s = e => {
+            e.dispatchEvent(new Event(t))
+        },
+        o = t => !(!t || "object" != typeof t) && (void 0 !== t.jquery && (t = t[0]), void 0 !== t.nodeType),
+        r = t => o(t) ? t.jquery ? t[0] : t : "string" == typeof t && t.length > 0 ? document.querySelector(t) : null,
+        a = (t, e, i) => {
+            Object.keys(i).forEach((n => {
+                const s = i[n],
+                    r = e[n],
+                    a = r && o(r) ? "element" : null == (l = r) ? `${l}` : {}.toString.call(l).match(/\s([a-z]+)/i)[1].toLowerCase();
+                var l;
+                if (!new RegExp(s).test(a)) throw new TypeError(`${t.toUpperCase()}: Option "${n}" provided type "${a}" but expected type "${s}".`)
+            }))
         },
-        findShadowRoot: function(t) {
+        l = t => !(!o(t) || 0 === t.getClientRects().length) && "visible" === getComputedStyle(t).getPropertyValue("visibility"),
+        c = t => !t || t.nodeType !== Node.ELEMENT_NODE || !!t.classList.contains("disabled") || (void 0 !== t.disabled ? t.disabled : t.hasAttribute("disabled") && "false" !== t.getAttribute("disabled")),
+        h = t => {
             if (!document.documentElement.attachShadow) return null;
             if ("function" == typeof t.getRootNode) {
-                var e = t.getRootNode();
+                const e = t.getRootNode();
                 return e instanceof ShadowRoot ? e : null
             }
-            return t instanceof ShadowRoot ? t : t.parentNode ? s.findShadowRoot(t.parentNode) : null
+            return t instanceof ShadowRoot ? t : t.parentNode ? h(t.parentNode) : null
         },
-        jQueryDetection: function() {
-            if ("undefined" == typeof e) throw new TypeError("Bootstrap's JavaScript requires jQuery. jQuery must be included before Bootstrap's JavaScript.");
-            var t = e.fn.jquery.split(" ")[0].split(".");
-            if (t[0] < 2 && t[1] < 9 || 1 === t[0] && 9 === t[1] && t[2] < 1 || t[0] >= 4) throw new Error("Bootstrap's JavaScript requires at least jQuery v1.9.1 but less than v4.0.0")
+        d = () => {},
+        u = t => {
+            t.offsetHeight
+        },
+        f = () => {
+            const {
+                jQuery: t
+            } = window;
+            return t && !document.body.hasAttribute("data-bs-no-jquery") ? t : null
+        },
+        p = [],
+        m = () => "rtl" === document.documentElement.dir,
+        g = t => {
+            var e;
+            e = () => {
+                const e = f();
+                if (e) {
+                    const i = t.NAME,
+                        n = e.fn[i];
+                    e.fn[i] = t.jQueryInterface, e.fn[i].Constructor = t, e.fn[i].noConflict = () => (e.fn[i] = n, t.jQueryInterface)
+                }
+            }, "loading" === document.readyState ? (p.length || document.addEventListener("DOMContentLoaded", (() => {
+                p.forEach((t => t()))
+            })), p.push(e)) : e()
+        },
+        _ = t => {
+            "function" == typeof t && t()
+        },
+        b = (e, i, n = !0) => {
+            if (!n) return void _(e);
+            const o = (t => {
+                if (!t) return 0;
+                let {
+                    transitionDuration: e,
+                    transitionDelay: i
+                } = window.getComputedStyle(t);
+                const n = Number.parseFloat(e),
+                    s = Number.parseFloat(i);
+                return n || s ? (e = e.split(",")[0], i = i.split(",")[0], 1e3 * (Number.parseFloat(e) + Number.parseFloat(i))) : 0
+            })(i) + 5;
+            let r = !1;
+            const a = ({
+                target: n
+            }) => {
+                n === i && (r = !0, i.removeEventListener(t, a), _(e))
+            };
+            i.addEventListener(t, a), setTimeout((() => {
+                r || s(i)
+            }), o)
+        },
+        v = (t, e, i, n) => {
+            let s = t.indexOf(e);
+            if (-1 === s) return t[!i && n ? t.length - 1 : 0];
+            const o = t.length;
+            return s += i ? 1 : -1, n && (s = (s + o) % o), t[Math.max(0, Math.min(s, o - 1))]
+        },
+        y = /[^.]*(?=\..*)\.|.*/,
+        w = /\..*/,
+        E = /::\d+$/,
+        A = {};
+    let T = 1;
+    const O = {
+            mouseenter: "mouseover",
+            mouseleave: "mouseout"
+        },
+        C = /^(mouseenter|mouseleave)/i,
+        k = new Set(["click", "dblclick", "mouseup", "mousedown", "contextmenu", "mousewheel", "DOMMouseScroll", "mouseover", "mouseout", "mousemove", "selectstart", "selectend", "keydown", "keypress", "keyup", "orientationchange", "touchstart", "touchmove", "touchend", "touchcancel", "pointerdown", "pointermove", "pointerup", "pointerleave", "pointercancel", "gesturestart", "gesturechange", "gestureend", "focus", "blur", "change", "reset", "select", "submit", "focusin", "focusout", "load", "unload", "beforeunload", "resize", "move", "DOMContentLoaded", "readystatechange", "error", "abort", "scroll"]);
+
+    function L(t, e) {
+        return e && `${e}::${T++}` || t.uidEvent || T++
+    }
+
+    function x(t) {
+        const e = L(t);
+        return t.uidEvent = e, A[e] = A[e] || {}, A[e]
+    }
+
+    function D(t, e, i = null) {
+        const n = Object.keys(t);
+        for (let s = 0, o = n.length; s < o; s++) {
+            const o = t[n[s]];
+            if (o.originalHandler === e && o.delegationSelector === i) return o
         }
-    };
-    s.jQueryDetection(), e.fn.emulateTransitionEnd = r, e.event.special[s.TRANSITION_END] = {
-        bindType: "transitionend",
-        delegateType: "transitionend",
-        handle: function(t) {
-            if (e(t.target).is(this)) return t.handleObj.handler.apply(this, arguments)
+        return null
+    }
+
+    function S(t, e, i) {
+        const n = "string" == typeof e,
+            s = n ? i : e;
+        let o = P(t);
+        return k.has(o) || (o = t), [n, s, o]
+    }
+
+    function N(t, e, i, n, s) {
+        if ("string" != typeof e || !t) return;
+        if (i || (i = n, n = null), C.test(e)) {
+            const t = t => function(e) {
+                if (!e.relatedTarget || e.relatedTarget !== e.delegateTarget && !e.delegateTarget.contains(e.relatedTarget)) return t.call(this, e)
+            };
+            n ? n = t(n) : i = t(i)
         }
-    };
-    var a = "alert",
-        l = e.fn[a],
-        c = function() {
-            function t(t) {
-                this._element = t
-            }
-            var n = t.prototype;
-            return n.close = function(t) {
-                var e = this._element;
-                t && (e = this._getRootElement(t)), this._triggerCloseEvent(e).isDefaultPrevented() || this._removeElement(e)
-            }, n.dispose = function() {
-                e.removeData(this._element, "bs.alert"), this._element = null
-            }, n._getRootElement = function(t) {
-                var n = s.getSelectorFromElement(t),
-                    i = !1;
-                return n && (i = document.querySelector(n)), i || (i = e(t).closest(".alert")[0]), i
-            }, n._triggerCloseEvent = function(t) {
-                var n = e.Event("close.bs.alert");
-                return e(t).trigger(n), n
-            }, n._removeElement = function(t) {
-                var n = this;
-                if (e(t).removeClass("show"), e(t).hasClass("fade")) {
-                    var i = s.getTransitionDurationFromElement(t);
-                    e(t).one(s.TRANSITION_END, (function(e) {
-                        return n._destroyElement(t, e)
-                    })).emulateTransitionEnd(i)
-                } else this._destroyElement(t)
-            }, n._destroyElement = function(t) {
-                e(t).detach().trigger("closed.bs.alert").remove()
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this),
-                        o = i.data("bs.alert");
-                    o || (o = new t(this), i.data("bs.alert", o)), "close" === n && o[n](this)
-                }))
-            }, t._handleDismiss = function(t) {
-                return function(e) {
-                    e && e.preventDefault(), t.close(this)
-                }
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }]), t
-        }();
-    e(document).on("click.bs.alert.data-api", '[data-dismiss="alert"]', c._handleDismiss(new c)), e.fn[a] = c._jQueryInterface, e.fn[a].Constructor = c, e.fn[a].noConflict = function() {
-        return e.fn[a] = l, c._jQueryInterface
-    };
-    var h = e.fn.button,
-        u = function() {
-            function t(t) {
-                this._element = t
-            }
-            var n = t.prototype;
-            return n.toggle = function() {
-                var t = !0,
-                    n = !0,
-                    i = e(this._element).closest('[data-toggle="buttons"]')[0];
-                if (i) {
-                    var o = this._element.querySelector('input:not([type="hidden"])');
-                    if (o) {
-                        if ("radio" === o.type)
-                            if (o.checked && this._element.classList.contains("active")) t = !1;
-                            else {
-                                var r = i.querySelector(".active");
-                                r && e(r).removeClass("active")
-                            } t && ("checkbox" !== o.type && "radio" !== o.type || (o.checked = !this._element.classList.contains("active")), e(o).trigger("change")), o.focus(), n = !1
-                    }
+        const [o, r, a] = S(e, i, n), l = x(t), c = l[a] || (l[a] = {}), h = D(c, r, o ? i : null);
+        if (h) return void(h.oneOff = h.oneOff && s);
+        const d = L(r, e.replace(y, "")),
+            u = o ? function(t, e, i) {
+                return function n(s) {
+                    const o = t.querySelectorAll(e);
+                    for (let {
+                            target: r
+                        } = s; r && r !== this; r = r.parentNode)
+                        for (let a = o.length; a--;)
+                            if (o[a] === r) return s.delegateTarget = r, n.oneOff && j.off(t, s.type, e, i), i.apply(r, [s]);
+                    return null
+                }
+            }(t, i, n) : function(t, e) {
+                return function i(n) {
+                    return n.delegateTarget = t, i.oneOff && j.off(t, n.type, e), e.apply(t, [n])
                 }
-                this._element.hasAttribute("disabled") || this._element.classList.contains("disabled") || (n && this._element.setAttribute("aria-pressed", !this._element.classList.contains("active")), t && e(this._element).toggleClass("active"))
-            }, n.dispose = function() {
-                e.removeData(this._element, "bs.button"), this._element = null
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this).data("bs.button");
-                    i || (i = new t(this), e(this).data("bs.button", i)), "toggle" === n && i[n]()
+            }(t, i);
+        u.delegationSelector = o ? i : null, u.originalHandler = r, u.oneOff = s, u.uidEvent = d, c[d] = u, t.addEventListener(a, u, o)
+    }
+
+    function I(t, e, i, n, s) {
+        const o = D(e[i], n, s);
+        o && (t.removeEventListener(i, o, Boolean(s)), delete e[i][o.uidEvent])
+    }
+
+    function P(t) {
+        return t = t.replace(w, ""), O[t] || t
+    }
+    const j = {
+            on(t, e, i, n) {
+                N(t, e, i, n, !1)
+            },
+            one(t, e, i, n) {
+                N(t, e, i, n, !0)
+            },
+            off(t, e, i, n) {
+                if ("string" != typeof e || !t) return;
+                const [s, o, r] = S(e, i, n), a = r !== e, l = x(t), c = e.startsWith(".");
+                if (void 0 !== o) {
+                    if (!l || !l[r]) return;
+                    return void I(t, l, r, o, s ? i : null)
+                }
+                c && Object.keys(l).forEach((i => {
+                    ! function(t, e, i, n) {
+                        const s = e[i] || {};
+                        Object.keys(s).forEach((o => {
+                            if (o.includes(n)) {
+                                const n = s[o];
+                                I(t, e, i, n.originalHandler, n.delegationSelector)
+                            }
+                        }))
+                    }(t, l, i, e.slice(1))
+                }));
+                const h = l[r] || {};
+                Object.keys(h).forEach((i => {
+                    const n = i.replace(E, "");
+                    if (!a || e.includes(n)) {
+                        const e = h[i];
+                        I(t, l, r, e.originalHandler, e.delegationSelector)
+                    }
                 }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }]), t
-        }();
-    e(document).on("click.bs.button.data-api", '[data-toggle^="button"]', (function(t) {
-        var n = t.target,
-            i = n;
-        if (e(n).hasClass("btn") || (n = e(n).closest(".btn")[0]), !n || n.hasAttribute("disabled") || n.classList.contains("disabled")) t.preventDefault();
-        else {
-            var o = n.querySelector('input:not([type="hidden"])');
-            if (o && (o.hasAttribute("disabled") || o.classList.contains("disabled"))) return void t.preventDefault();
-            ("LABEL" !== i.tagName || o && "checkbox" !== o.type) && u._jQueryInterface.call(e(n), "toggle")
-        }
-    })).on("focus.bs.button.data-api blur.bs.button.data-api", '[data-toggle^="button"]', (function(t) {
-        var n = e(t.target).closest(".btn")[0];
-        e(n).toggleClass("focus", /^focus(in)?$/.test(t.type))
-    })), e(window).on("load.bs.button.data-api", (function() {
-        for (var t = [].slice.call(document.querySelectorAll('[data-toggle="buttons"] .btn')), e = 0, n = t.length; e < n; e++) {
-            var i = t[e],
-                o = i.querySelector('input:not([type="hidden"])');
-            o.checked || o.hasAttribute("checked") ? i.classList.add("active") : i.classList.remove("active")
-        }
-        for (var r = 0, s = (t = [].slice.call(document.querySelectorAll('[data-toggle="button"]'))).length; r < s; r++) {
-            var a = t[r];
-            "true" === a.getAttribute("aria-pressed") ? a.classList.add("active") : a.classList.remove("active")
+            },
+            trigger(t, e, i) {
+                if ("string" != typeof e || !t) return null;
+                const n = f(),
+                    s = P(e),
+                    o = e !== s,
+                    r = k.has(s);
+                let a, l = !0,
+                    c = !0,
+                    h = !1,
+                    d = null;
+                return o && n && (a = n.Event(e, i), n(t).trigger(a), l = !a.isPropagationStopped(), c = !a.isImmediatePropagationStopped(), h = a.isDefaultPrevented()), r ? (d = document.createEvent("HTMLEvents"), d.initEvent(s, l, !0)) : d = new CustomEvent(e, {
+                    bubbles: l,
+                    cancelable: !0
+                }), void 0 !== i && Object.keys(i).forEach((t => {
+                    Object.defineProperty(d, t, {
+                        get: () => i[t]
+                    })
+                })), h && d.preventDefault(), c && t.dispatchEvent(d), d.defaultPrevented && void 0 !== a && a.preventDefault(), d
+            }
+        },
+        M = new Map,
+        H = {
+            set(t, e, i) {
+                M.has(t) || M.set(t, new Map);
+                const n = M.get(t);
+                n.has(e) || 0 === n.size ? n.set(e, i) : console.error(`Bootstrap doesn't allow more than one instance per element. Bound instance: ${Array.from(n.keys())[0]}.`)
+            },
+            get: (t, e) => M.has(t) && M.get(t).get(e) || null,
+            remove(t, e) {
+                if (!M.has(t)) return;
+                const i = M.get(t);
+                i.delete(e), 0 === i.size && M.delete(t)
+            }
+        };
+    class B {
+        constructor(t) {
+            (t = r(t)) && (this._element = t, H.set(this._element, this.constructor.DATA_KEY, this))
         }
-    })), e.fn.button = u._jQueryInterface, e.fn.button.Constructor = u, e.fn.button.noConflict = function() {
-        return e.fn.button = h, u._jQueryInterface
+        dispose() {
+            H.remove(this._element, this.constructor.DATA_KEY), j.off(this._element, this.constructor.EVENT_KEY), Object.getOwnPropertyNames(this).forEach((t => {
+                this[t] = null
+            }))
+        }
+        _queueCallback(t, e, i = !0) {
+            b(t, e, i)
+        }
+        static getInstance(t) {
+            return H.get(r(t), this.DATA_KEY)
+        }
+        static getOrCreateInstance(t, e = {}) {
+            return this.getInstance(t) || new this(t, "object" == typeof e ? e : null)
+        }
+        static get VERSION() {
+            return "5.1.3"
+        }
+        static get NAME() {
+            throw new Error('You have to implement the static method "NAME", for each component!')
+        }
+        static get DATA_KEY() {
+            return `bs.${this.NAME}`
+        }
+        static get EVENT_KEY() {
+            return `.${this.DATA_KEY}`
+        }
+    }
+    const R = (t, e = "hide") => {
+        const i = `click.dismiss${t.EVENT_KEY}`,
+            s = t.NAME;
+        j.on(document, i, `[data-bs-dismiss="${s}"]`, (function(i) {
+            if (["A", "AREA"].includes(this.tagName) && i.preventDefault(), c(this)) return;
+            const o = n(this) || this.closest(`.${s}`);
+            t.getOrCreateInstance(o)[e]()
+        }))
     };
-    var f = "carousel",
-        d = ".bs.carousel",
-        p = e.fn[f],
-        m = {
+    class W extends B {
+        static get NAME() {
+            return "alert"
+        }
+        close() {
+            if (j.trigger(this._element, "close.bs.alert").defaultPrevented) return;
+            this._element.classList.remove("show");
+            const t = this._element.classList.contains("fade");
+            this._queueCallback((() => this._destroyElement()), this._element, t)
+        }
+        _destroyElement() {
+            this._element.remove(), j.trigger(this._element, "closed.bs.alert"), this.dispose()
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = W.getOrCreateInstance(this);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
+                    e[t](this)
+                }
+            }))
+        }
+    }
+    R(W, "close"), g(W);
+    const $ = '[data-bs-toggle="button"]';
+    class z extends B {
+        static get NAME() {
+            return "button"
+        }
+        toggle() {
+            this._element.setAttribute("aria-pressed", this._element.classList.toggle("active"))
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = z.getOrCreateInstance(this);
+                "toggle" === t && e[t]()
+            }))
+        }
+    }
+
+    function q(t) {
+        return "true" === t || "false" !== t && (t === Number(t).toString() ? Number(t) : "" === t || "null" === t ? null : t)
+    }
+
+    function F(t) {
+        return t.replace(/[A-Z]/g, (t => `-${t.toLowerCase()}`))
+    }
+    j.on(document, "click.bs.button.data-api", $, (t => {
+        t.preventDefault();
+        const e = t.target.closest($);
+        z.getOrCreateInstance(e).toggle()
+    })), g(z);
+    const U = {
+            setDataAttribute(t, e, i) {
+                t.setAttribute(`data-bs-${F(e)}`, i)
+            },
+            removeDataAttribute(t, e) {
+                t.removeAttribute(`data-bs-${F(e)}`)
+            },
+            getDataAttributes(t) {
+                if (!t) return {};
+                const e = {};
+                return Object.keys(t.dataset).filter((t => t.startsWith("bs"))).forEach((i => {
+                    let n = i.replace(/^bs/, "");
+                    n = n.charAt(0).toLowerCase() + n.slice(1, n.length), e[n] = q(t.dataset[i])
+                })), e
+            },
+            getDataAttribute: (t, e) => q(t.getAttribute(`data-bs-${F(e)}`)),
+            offset(t) {
+                const e = t.getBoundingClientRect();
+                return {
+                    top: e.top + window.pageYOffset,
+                    left: e.left + window.pageXOffset
+                }
+            },
+            position: t => ({
+                top: t.offsetTop,
+                left: t.offsetLeft
+            })
+        },
+        V = {
+            find: (t, e = document.documentElement) => [].concat(...Element.prototype.querySelectorAll.call(e, t)),
+            findOne: (t, e = document.documentElement) => Element.prototype.querySelector.call(e, t),
+            children: (t, e) => [].concat(...t.children).filter((t => t.matches(e))),
+            parents(t, e) {
+                const i = [];
+                let n = t.parentNode;
+                for (; n && n.nodeType === Node.ELEMENT_NODE && 3 !== n.nodeType;) n.matches(e) && i.push(n), n = n.parentNode;
+                return i
+            },
+            prev(t, e) {
+                let i = t.previousElementSibling;
+                for (; i;) {
+                    if (i.matches(e)) return [i];
+                    i = i.previousElementSibling
+                }
+                return []
+            },
+            next(t, e) {
+                let i = t.nextElementSibling;
+                for (; i;) {
+                    if (i.matches(e)) return [i];
+                    i = i.nextElementSibling
+                }
+                return []
+            },
+            focusableChildren(t) {
+                const e = ["a", "button", "input", "textarea", "select", "details", "[tabindex]", '[contenteditable="true"]'].map((t => `${t}:not([tabindex^="-"])`)).join(", ");
+                return this.find(e, t).filter((t => !c(t) && l(t)))
+            }
+        },
+        K = "carousel",
+        X = {
             interval: 5e3,
             keyboard: !0,
             slide: !1,
             pause: "hover",
             wrap: !0,
             touch: !0
         },
-        g = {
+        Y = {
             interval: "(number|boolean)",
             keyboard: "boolean",
             slide: "(boolean|string)",
             pause: "(string|boolean)",
             wrap: "boolean",
             touch: "boolean"
         },
-        _ = {
-            TOUCH: "touch",
-            PEN: "pen"
-        },
-        v = function() {
-            function t(t, e) {
-                this._items = null, this._interval = null, this._activeElement = null, this._isPaused = !1, this._isSliding = !1, this.touchTimeout = null, this.touchStartX = 0, this.touchDeltaX = 0, this._config = this._getConfig(e), this._element = t, this._indicatorsElement = this._element.querySelector(".carousel-indicators"), this._touchSupported = "ontouchstart" in document.documentElement || navigator.maxTouchPoints > 0, this._pointerEvent = Boolean(window.PointerEvent || window.MSPointerEvent), this._addEventListeners()
-            }
-            var n = t.prototype;
-            return n.next = function() {
-                this._isSliding || this._slide("next")
-            }, n.nextWhenVisible = function() {
-                !document.hidden && e(this._element).is(":visible") && "hidden" !== e(this._element).css("visibility") && this.next()
-            }, n.prev = function() {
-                this._isSliding || this._slide("prev")
-            }, n.pause = function(t) {
-                t || (this._isPaused = !0), this._element.querySelector(".carousel-item-next, .carousel-item-prev") && (s.triggerTransitionEnd(this._element), this.cycle(!0)), clearInterval(this._interval), this._interval = null
-            }, n.cycle = function(t) {
-                t || (this._isPaused = !1), this._interval && (clearInterval(this._interval), this._interval = null), this._config.interval && !this._isPaused && (this._interval = setInterval((document.visibilityState ? this.nextWhenVisible : this.next).bind(this), this._config.interval))
-            }, n.to = function(t) {
-                var n = this;
-                this._activeElement = this._element.querySelector(".active.carousel-item");
-                var i = this._getItemIndex(this._activeElement);
-                if (!(t > this._items.length - 1 || t < 0))
-                    if (this._isSliding) e(this._element).one("slid.bs.carousel", (function() {
-                        return n.to(t)
-                    }));
-                    else {
-                        if (i === t) return this.pause(), void this.cycle();
-                        var o = t > i ? "next" : "prev";
-                        this._slide(o, this._items[t])
-                    }
-            }, n.dispose = function() {
-                e(this._element).off(d), e.removeData(this._element, "bs.carousel"), this._items = null, this._config = null, this._element = null, this._interval = null, this._isPaused = null, this._isSliding = null, this._activeElement = null, this._indicatorsElement = null
-            }, n._getConfig = function(t) {
-                return t = o({}, m, t), s.typeCheckConfig(f, t, g), t
-            }, n._handleSwipe = function() {
-                var t = Math.abs(this.touchDeltaX);
-                if (!(t <= 40)) {
-                    var e = t / this.touchDeltaX;
-                    this.touchDeltaX = 0, e > 0 && this.prev(), e < 0 && this.next()
-                }
-            }, n._addEventListeners = function() {
-                var t = this;
-                this._config.keyboard && e(this._element).on("keydown.bs.carousel", (function(e) {
-                    return t._keydown(e)
-                })), "hover" === this._config.pause && e(this._element).on("mouseenter.bs.carousel", (function(e) {
-                    return t.pause(e)
-                })).on("mouseleave.bs.carousel", (function(e) {
-                    return t.cycle(e)
-                })), this._config.touch && this._addTouchEventListeners()
-            }, n._addTouchEventListeners = function() {
-                var t = this;
-                if (this._touchSupported) {
-                    var n = function(e) {
-                            t._pointerEvent && _[e.originalEvent.pointerType.toUpperCase()] ? t.touchStartX = e.originalEvent.clientX : t._pointerEvent || (t.touchStartX = e.originalEvent.touches[0].clientX)
-                        },
-                        i = function(e) {
-                            t._pointerEvent && _[e.originalEvent.pointerType.toUpperCase()] && (t.touchDeltaX = e.originalEvent.clientX - t.touchStartX), t._handleSwipe(), "hover" === t._config.pause && (t.pause(), t.touchTimeout && clearTimeout(t.touchTimeout), t.touchTimeout = setTimeout((function(e) {
-                                return t.cycle(e)
-                            }), 500 + t._config.interval))
-                        };
-                    e(this._element.querySelectorAll(".carousel-item img")).on("dragstart.bs.carousel", (function(t) {
-                        return t.preventDefault()
-                    })), this._pointerEvent ? (e(this._element).on("pointerdown.bs.carousel", (function(t) {
-                        return n(t)
-                    })), e(this._element).on("pointerup.bs.carousel", (function(t) {
-                        return i(t)
-                    })), this._element.classList.add("pointer-event")) : (e(this._element).on("touchstart.bs.carousel", (function(t) {
-                        return n(t)
-                    })), e(this._element).on("touchmove.bs.carousel", (function(e) {
-                        return function(e) {
-                            e.originalEvent.touches && e.originalEvent.touches.length > 1 ? t.touchDeltaX = 0 : t.touchDeltaX = e.originalEvent.touches[0].clientX - t.touchStartX
-                        }(e)
-                    })), e(this._element).on("touchend.bs.carousel", (function(t) {
-                        return i(t)
-                    })))
-                }
-            }, n._keydown = function(t) {
-                if (!/input|textarea/i.test(t.target.tagName)) switch (t.which) {
-                    case 37:
-                        t.preventDefault(), this.prev();
-                        break;
-                    case 39:
-                        t.preventDefault(), this.next()
-                }
-            }, n._getItemIndex = function(t) {
-                return this._items = t && t.parentNode ? [].slice.call(t.parentNode.querySelectorAll(".carousel-item")) : [], this._items.indexOf(t)
-            }, n._getItemByDirection = function(t, e) {
-                var n = "next" === t,
-                    i = "prev" === t,
-                    o = this._getItemIndex(e),
-                    r = this._items.length - 1;
-                if ((i && 0 === o || n && o === r) && !this._config.wrap) return e;
-                var s = (o + ("prev" === t ? -1 : 1)) % this._items.length;
-                return -1 === s ? this._items[this._items.length - 1] : this._items[s]
-            }, n._triggerSlideEvent = function(t, n) {
-                var i = this._getItemIndex(t),
-                    o = this._getItemIndex(this._element.querySelector(".active.carousel-item")),
-                    r = e.Event("slide.bs.carousel", {
-                        relatedTarget: t,
-                        direction: n,
-                        from: o,
-                        to: i
-                    });
-                return e(this._element).trigger(r), r
-            }, n._setActiveIndicatorElement = function(t) {
-                if (this._indicatorsElement) {
-                    var n = [].slice.call(this._indicatorsElement.querySelectorAll(".active"));
-                    e(n).removeClass("active");
-                    var i = this._indicatorsElement.children[this._getItemIndex(t)];
-                    i && e(i).addClass("active")
-                }
-            }, n._slide = function(t, n) {
-                var i, o, r, a = this,
-                    l = this._element.querySelector(".active.carousel-item"),
-                    c = this._getItemIndex(l),
-                    h = n || l && this._getItemByDirection(t, l),
-                    u = this._getItemIndex(h),
-                    f = Boolean(this._interval);
-                if ("next" === t ? (i = "carousel-item-left", o = "carousel-item-next", r = "left") : (i = "carousel-item-right", o = "carousel-item-prev", r = "right"), h && e(h).hasClass("active")) this._isSliding = !1;
-                else if (!this._triggerSlideEvent(h, r).isDefaultPrevented() && l && h) {
-                    this._isSliding = !0, f && this.pause(), this._setActiveIndicatorElement(h);
-                    var d = e.Event("slid.bs.carousel", {
-                        relatedTarget: h,
-                        direction: r,
-                        from: c,
-                        to: u
-                    });
-                    if (e(this._element).hasClass("slide")) {
-                        e(h).addClass(o), s.reflow(h), e(l).addClass(i), e(h).addClass(i);
-                        var p = parseInt(h.getAttribute("data-interval"), 10);
-                        p ? (this._config.defaultInterval = this._config.defaultInterval || this._config.interval, this._config.interval = p) : this._config.interval = this._config.defaultInterval || this._config.interval;
-                        var m = s.getTransitionDurationFromElement(l);
-                        e(l).one(s.TRANSITION_END, (function() {
-                            e(h).removeClass(i + " " + o).addClass("active"), e(l).removeClass("active " + o + " " + i), a._isSliding = !1, setTimeout((function() {
-                                return e(a._element).trigger(d)
-                            }), 0)
-                        })).emulateTransitionEnd(m)
-                    } else e(l).removeClass("active"), e(h).addClass("active"), this._isSliding = !1, e(this._element).trigger(d);
-                    f && this.cycle()
-                }
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this).data("bs.carousel"),
-                        r = o({}, m, e(this).data());
-                    "object" == typeof n && (r = o({}, r, n));
-                    var s = "string" == typeof n ? n : r.slide;
-                    if (i || (i = new t(this, r), e(this).data("bs.carousel", i)), "number" == typeof n) i.to(n);
-                    else if ("string" == typeof s) {
-                        if ("undefined" == typeof i[s]) throw new TypeError('No method named "' + s + '"');
-                        i[s]()
-                    } else r.interval && r.ride && (i.pause(), i.cycle())
-                }))
-            }, t._dataApiClickHandler = function(n) {
-                var i = s.getSelectorFromElement(this);
-                if (i) {
-                    var r = e(i)[0];
-                    if (r && e(r).hasClass("carousel")) {
-                        var a = o({}, e(r).data(), e(this).data()),
-                            l = this.getAttribute("data-slide-to");
-                        l && (a.interval = !1), t._jQueryInterface.call(e(r), a), l && e(r).data("bs.carousel").to(l), n.preventDefault()
+        Q = "next",
+        G = "prev",
+        Z = "left",
+        J = "right",
+        tt = {
+            ArrowLeft: J,
+            ArrowRight: Z
+        },
+        et = "slid.bs.carousel",
+        it = "active",
+        nt = ".active.carousel-item";
+    class st extends B {
+        constructor(t, e) {
+            super(t), this._items = null, this._interval = null, this._activeElement = null, this._isPaused = !1, this._isSliding = !1, this.touchTimeout = null, this.touchStartX = 0, this.touchDeltaX = 0, this._config = this._getConfig(e), this._indicatorsElement = V.findOne(".carousel-indicators", this._element), this._touchSupported = "ontouchstart" in document.documentElement || navigator.maxTouchPoints > 0, this._pointerEvent = Boolean(window.PointerEvent), this._addEventListeners()
+        }
+        static get Default() {
+            return X
+        }
+        static get NAME() {
+            return K
+        }
+        next() {
+            this._slide(Q)
+        }
+        nextWhenVisible() {
+            !document.hidden && l(this._element) && this.next()
+        }
+        prev() {
+            this._slide(G)
+        }
+        pause(t) {
+            t || (this._isPaused = !0), V.findOne(".carousel-item-next, .carousel-item-prev", this._element) && (s(this._element), this.cycle(!0)), clearInterval(this._interval), this._interval = null
+        }
+        cycle(t) {
+            t || (this._isPaused = !1), this._interval && (clearInterval(this._interval), this._interval = null), this._config && this._config.interval && !this._isPaused && (this._updateInterval(), this._interval = setInterval((document.visibilityState ? this.nextWhenVisible : this.next).bind(this), this._config.interval))
+        }
+        to(t) {
+            this._activeElement = V.findOne(nt, this._element);
+            const e = this._getItemIndex(this._activeElement);
+            if (t > this._items.length - 1 || t < 0) return;
+            if (this._isSliding) return void j.one(this._element, et, (() => this.to(t)));
+            if (e === t) return this.pause(), void this.cycle();
+            const i = t > e ? Q : G;
+            this._slide(i, this._items[t])
+        }
+        _getConfig(t) {
+            return t = {
+                ...X,
+                ...U.getDataAttributes(this._element),
+                ..."object" == typeof t ? t : {}
+            }, a(K, t, Y), t
+        }
+        _handleSwipe() {
+            const t = Math.abs(this.touchDeltaX);
+            if (t <= 40) return;
+            const e = t / this.touchDeltaX;
+            this.touchDeltaX = 0, e && this._slide(e > 0 ? J : Z)
+        }
+        _addEventListeners() {
+            this._config.keyboard && j.on(this._element, "keydown.bs.carousel", (t => this._keydown(t))), "hover" === this._config.pause && (j.on(this._element, "mouseenter.bs.carousel", (t => this.pause(t))), j.on(this._element, "mouseleave.bs.carousel", (t => this.cycle(t)))), this._config.touch && this._touchSupported && this._addTouchEventListeners()
+        }
+        _addTouchEventListeners() {
+            const t = t => this._pointerEvent && ("pen" === t.pointerType || "touch" === t.pointerType),
+                e = e => {
+                    t(e) ? this.touchStartX = e.clientX : this._pointerEvent || (this.touchStartX = e.touches[0].clientX)
+                },
+                i = t => {
+                    this.touchDeltaX = t.touches && t.touches.length > 1 ? 0 : t.touches[0].clientX - this.touchStartX
+                },
+                n = e => {
+                    t(e) && (this.touchDeltaX = e.clientX - this.touchStartX), this._handleSwipe(), "hover" === this._config.pause && (this.pause(), this.touchTimeout && clearTimeout(this.touchTimeout), this.touchTimeout = setTimeout((t => this.cycle(t)), 500 + this._config.interval))
+                };
+            V.find(".carousel-item img", this._element).forEach((t => {
+                j.on(t, "dragstart.bs.carousel", (t => t.preventDefault()))
+            })), this._pointerEvent ? (j.on(this._element, "pointerdown.bs.carousel", (t => e(t))), j.on(this._element, "pointerup.bs.carousel", (t => n(t))), this._element.classList.add("pointer-event")) : (j.on(this._element, "touchstart.bs.carousel", (t => e(t))), j.on(this._element, "touchmove.bs.carousel", (t => i(t))), j.on(this._element, "touchend.bs.carousel", (t => n(t))))
+        }
+        _keydown(t) {
+            if (/input|textarea/i.test(t.target.tagName)) return;
+            const e = tt[t.key];
+            e && (t.preventDefault(), this._slide(e))
+        }
+        _getItemIndex(t) {
+            return this._items = t && t.parentNode ? V.find(".carousel-item", t.parentNode) : [], this._items.indexOf(t)
+        }
+        _getItemByOrder(t, e) {
+            const i = t === Q;
+            return v(this._items, e, i, this._config.wrap)
+        }
+        _triggerSlideEvent(t, e) {
+            const i = this._getItemIndex(t),
+                n = this._getItemIndex(V.findOne(nt, this._element));
+            return j.trigger(this._element, "slide.bs.carousel", {
+                relatedTarget: t,
+                direction: e,
+                from: n,
+                to: i
+            })
+        }
+        _setActiveIndicatorElement(t) {
+            if (this._indicatorsElement) {
+                const e = V.findOne(".active", this._indicatorsElement);
+                e.classList.remove(it), e.removeAttribute("aria-current");
+                const i = V.find("[data-bs-target]", this._indicatorsElement);
+                for (let e = 0; e < i.length; e++)
+                    if (Number.parseInt(i[e].getAttribute("data-bs-slide-to"), 10) === this._getItemIndex(t)) {
+                        i[e].classList.add(it), i[e].setAttribute("aria-current", "true");
+                        break
                     }
-                }
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return m
-                }
-            }]), t
-        }();
-    e(document).on("click.bs.carousel.data-api", "[data-slide], [data-slide-to]", v._dataApiClickHandler), e(window).on("load.bs.carousel.data-api", (function() {
-        for (var t = [].slice.call(document.querySelectorAll('[data-ride="carousel"]')), n = 0, i = t.length; n < i; n++) {
-            var o = e(t[n]);
-            v._jQueryInterface.call(o, o.data())
+            }
         }
-    })), e.fn[f] = v._jQueryInterface, e.fn[f].Constructor = v, e.fn[f].noConflict = function() {
-        return e.fn[f] = p, v._jQueryInterface
-    };
-    var b = "collapse",
-        y = e.fn[b],
-        w = {
+        _updateInterval() {
+            const t = this._activeElement || V.findOne(nt, this._element);
+            if (!t) return;
+            const e = Number.parseInt(t.getAttribute("data-bs-interval"), 10);
+            e ? (this._config.defaultInterval = this._config.defaultInterval || this._config.interval, this._config.interval = e) : this._config.interval = this._config.defaultInterval || this._config.interval
+        }
+        _slide(t, e) {
+            const i = this._directionToOrder(t),
+                n = V.findOne(nt, this._element),
+                s = this._getItemIndex(n),
+                o = e || this._getItemByOrder(i, n),
+                r = this._getItemIndex(o),
+                a = Boolean(this._interval),
+                l = i === Q,
+                c = l ? "carousel-item-start" : "carousel-item-end",
+                h = l ? "carousel-item-next" : "carousel-item-prev",
+                d = this._orderToDirection(i);
+            if (o && o.classList.contains(it)) return void(this._isSliding = !1);
+            if (this._isSliding) return;
+            if (this._triggerSlideEvent(o, d).defaultPrevented) return;
+            if (!n || !o) return;
+            this._isSliding = !0, a && this.pause(), this._setActiveIndicatorElement(o), this._activeElement = o;
+            const f = () => {
+                j.trigger(this._element, et, {
+                    relatedTarget: o,
+                    direction: d,
+                    from: s,
+                    to: r
+                })
+            };
+            if (this._element.classList.contains("slide")) {
+                o.classList.add(h), u(o), n.classList.add(c), o.classList.add(c);
+                const t = () => {
+                    o.classList.remove(c, h), o.classList.add(it), n.classList.remove(it, h, c), this._isSliding = !1, setTimeout(f, 0)
+                };
+                this._queueCallback(t, n, !0)
+            } else n.classList.remove(it), o.classList.add(it), this._isSliding = !1, f();
+            a && this.cycle()
+        }
+        _directionToOrder(t) {
+            return [J, Z].includes(t) ? m() ? t === Z ? G : Q : t === Z ? Q : G : t
+        }
+        _orderToDirection(t) {
+            return [Q, G].includes(t) ? m() ? t === G ? Z : J : t === G ? J : Z : t
+        }
+        static carouselInterface(t, e) {
+            const i = st.getOrCreateInstance(t, e);
+            let {
+                _config: n
+            } = i;
+            "object" == typeof e && (n = {
+                ...n,
+                ...e
+            });
+            const s = "string" == typeof e ? e : n.slide;
+            if ("number" == typeof e) i.to(e);
+            else if ("string" == typeof s) {
+                if (void 0 === i[s]) throw new TypeError(`No method named "${s}"`);
+                i[s]()
+            } else n.interval && n.ride && (i.pause(), i.cycle())
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                st.carouselInterface(this, t)
+            }))
+        }
+        static dataApiClickHandler(t) {
+            const e = n(this);
+            if (!e || !e.classList.contains("carousel")) return;
+            const i = {
+                    ...U.getDataAttributes(e),
+                    ...U.getDataAttributes(this)
+                },
+                s = this.getAttribute("data-bs-slide-to");
+            s && (i.interval = !1), st.carouselInterface(e, i), s && st.getInstance(e).to(s), t.preventDefault()
+        }
+    }
+    j.on(document, "click.bs.carousel.data-api", "[data-bs-slide], [data-bs-slide-to]", st.dataApiClickHandler), j.on(window, "load.bs.carousel.data-api", (() => {
+        const t = V.find('[data-bs-ride="carousel"]');
+        for (let e = 0, i = t.length; e < i; e++) st.carouselInterface(t[e], st.getInstance(t[e]))
+    })), g(st);
+    const ot = "collapse",
+        rt = {
             toggle: !0,
-            parent: ""
+            parent: null
         },
-        E = {
+        at = {
             toggle: "boolean",
-            parent: "(string|element)"
+            parent: "(null|element)"
         },
-        T = function() {
-            function t(t, e) {
-                this._isTransitioning = !1, this._element = t, this._config = this._getConfig(e), this._triggerArray = [].slice.call(document.querySelectorAll('[data-toggle="collapse"][href="#' + t.id + '"],[data-toggle="collapse"][data-target="#' + t.id + '"]'));
-                for (var n = [].slice.call(document.querySelectorAll('[data-toggle="collapse"]')), i = 0, o = n.length; i < o; i++) {
-                    var r = n[i],
-                        a = s.getSelectorFromElement(r),
-                        l = [].slice.call(document.querySelectorAll(a)).filter((function(e) {
-                            return e === t
-                        }));
-                    null !== a && l.length > 0 && (this._selector = a, this._triggerArray.push(r))
-                }
-                this._parent = this._config.parent ? this._getParent() : null, this._config.parent || this._addAriaAndCollapsedClass(this._element, this._triggerArray), this._config.toggle && this.toggle()
-            }
-            var n = t.prototype;
-            return n.toggle = function() {
-                e(this._element).hasClass("show") ? this.hide() : this.show()
-            }, n.show = function() {
-                var n, i, o = this;
-                if (!this._isTransitioning && !e(this._element).hasClass("show") && (this._parent && 0 === (n = [].slice.call(this._parent.querySelectorAll(".show, .collapsing")).filter((function(t) {
-                        return "string" == typeof o._config.parent ? t.getAttribute("data-parent") === o._config.parent : t.classList.contains("collapse")
-                    }))).length && (n = null), !(n && (i = e(n).not(this._selector).data("bs.collapse")) && i._isTransitioning))) {
-                    var r = e.Event("show.bs.collapse");
-                    if (e(this._element).trigger(r), !r.isDefaultPrevented()) {
-                        n && (t._jQueryInterface.call(e(n).not(this._selector), "hide"), i || e(n).data("bs.collapse", null));
-                        var a = this._getDimension();
-                        e(this._element).removeClass("collapse").addClass("collapsing"), this._element.style[a] = 0, this._triggerArray.length && e(this._triggerArray).removeClass("collapsed").attr("aria-expanded", !0), this.setTransitioning(!0);
-                        var l = "scroll" + (a[0].toUpperCase() + a.slice(1)),
-                            c = s.getTransitionDurationFromElement(this._element);
-                        e(this._element).one(s.TRANSITION_END, (function() {
-                            e(o._element).removeClass("collapsing").addClass("collapse show"), o._element.style[a] = "", o.setTransitioning(!1), e(o._element).trigger("shown.bs.collapse")
-                        })).emulateTransitionEnd(c), this._element.style[a] = this._element[l] + "px"
-                    }
-                }
-            }, n.hide = function() {
-                var t = this;
-                if (!this._isTransitioning && e(this._element).hasClass("show")) {
-                    var n = e.Event("hide.bs.collapse");
-                    if (e(this._element).trigger(n), !n.isDefaultPrevented()) {
-                        var i = this._getDimension();
-                        this._element.style[i] = this._element.getBoundingClientRect()[i] + "px", s.reflow(this._element), e(this._element).addClass("collapsing").removeClass("collapse show");
-                        var o = this._triggerArray.length;
-                        if (o > 0)
-                            for (var r = 0; r < o; r++) {
-                                var a = this._triggerArray[r],
-                                    l = s.getSelectorFromElement(a);
-                                if (null !== l) e([].slice.call(document.querySelectorAll(l))).hasClass("show") || e(a).addClass("collapsed").attr("aria-expanded", !1)
-                            }
-                        this.setTransitioning(!0);
-                        this._element.style[i] = "";
-                        var c = s.getTransitionDurationFromElement(this._element);
-                        e(this._element).one(s.TRANSITION_END, (function() {
-                            t.setTransitioning(!1), e(t._element).removeClass("collapsing").addClass("collapse").trigger("hidden.bs.collapse")
-                        })).emulateTransitionEnd(c)
-                    }
+        lt = "show",
+        ct = "collapse",
+        ht = "collapsing",
+        dt = "collapsed",
+        ut = ":scope .collapse .collapse",
+        ft = '[data-bs-toggle="collapse"]';
+    class pt extends B {
+        constructor(t, e) {
+            super(t), this._isTransitioning = !1, this._config = this._getConfig(e), this._triggerArray = [];
+            const n = V.find(ft);
+            for (let t = 0, e = n.length; t < e; t++) {
+                const e = n[t],
+                    s = i(e),
+                    o = V.find(s).filter((t => t === this._element));
+                null !== s && o.length && (this._selector = s, this._triggerArray.push(e))
+            }
+            this._initializeChildren(), this._config.parent || this._addAriaAndCollapsedClass(this._triggerArray, this._isShown()), this._config.toggle && this.toggle()
+        }
+        static get Default() {
+            return rt
+        }
+        static get NAME() {
+            return ot
+        }
+        toggle() {
+            this._isShown() ? this.hide() : this.show()
+        }
+        show() {
+            if (this._isTransitioning || this._isShown()) return;
+            let t, e = [];
+            if (this._config.parent) {
+                const t = V.find(ut, this._config.parent);
+                e = V.find(".collapse.show, .collapse.collapsing", this._config.parent).filter((e => !t.includes(e)))
+            }
+            const i = V.findOne(this._selector);
+            if (e.length) {
+                const n = e.find((t => i !== t));
+                if (t = n ? pt.getInstance(n) : null, t && t._isTransitioning) return
+            }
+            if (j.trigger(this._element, "show.bs.collapse").defaultPrevented) return;
+            e.forEach((e => {
+                i !== e && pt.getOrCreateInstance(e, {
+                    toggle: !1
+                }).hide(), t || H.set(e, "bs.collapse", null)
+            }));
+            const n = this._getDimension();
+            this._element.classList.remove(ct), this._element.classList.add(ht), this._element.style[n] = 0, this._addAriaAndCollapsedClass(this._triggerArray, !0), this._isTransitioning = !0;
+            const s = `scroll${n[0].toUpperCase()+n.slice(1)}`;
+            this._queueCallback((() => {
+                this._isTransitioning = !1, this._element.classList.remove(ht), this._element.classList.add(ct, lt), this._element.style[n] = "", j.trigger(this._element, "shown.bs.collapse")
+            }), this._element, !0), this._element.style[n] = `${this._element[s]}px`
+        }
+        hide() {
+            if (this._isTransitioning || !this._isShown()) return;
+            if (j.trigger(this._element, "hide.bs.collapse").defaultPrevented) return;
+            const t = this._getDimension();
+            this._element.style[t] = `${this._element.getBoundingClientRect()[t]}px`, u(this._element), this._element.classList.add(ht), this._element.classList.remove(ct, lt);
+            const e = this._triggerArray.length;
+            for (let t = 0; t < e; t++) {
+                const e = this._triggerArray[t],
+                    i = n(e);
+                i && !this._isShown(i) && this._addAriaAndCollapsedClass([e], !1)
+            }
+            this._isTransitioning = !0, this._element.style[t] = "", this._queueCallback((() => {
+                this._isTransitioning = !1, this._element.classList.remove(ht), this._element.classList.add(ct), j.trigger(this._element, "hidden.bs.collapse")
+            }), this._element, !0)
+        }
+        _isShown(t = this._element) {
+            return t.classList.contains(lt)
+        }
+        _getConfig(t) {
+            return (t = {
+                ...rt,
+                ...U.getDataAttributes(this._element),
+                ...t
+            }).toggle = Boolean(t.toggle), t.parent = r(t.parent), a(ot, t, at), t
+        }
+        _getDimension() {
+            return this._element.classList.contains("collapse-horizontal") ? "width" : "height"
+        }
+        _initializeChildren() {
+            if (!this._config.parent) return;
+            const t = V.find(ut, this._config.parent);
+            V.find(ft, this._config.parent).filter((e => !t.includes(e))).forEach((t => {
+                const e = n(t);
+                e && this._addAriaAndCollapsedClass([t], this._isShown(e))
+            }))
+        }
+        _addAriaAndCollapsedClass(t, e) {
+            t.length && t.forEach((t => {
+                e ? t.classList.remove(dt) : t.classList.add(dt), t.setAttribute("aria-expanded", e)
+            }))
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = {};
+                "string" == typeof t && /show|hide/.test(t) && (e.toggle = !1);
+                const i = pt.getOrCreateInstance(this, e);
+                if ("string" == typeof t) {
+                    if (void 0 === i[t]) throw new TypeError(`No method named "${t}"`);
+                    i[t]()
                 }
-            }, n.setTransitioning = function(t) {
-                this._isTransitioning = t
-            }, n.dispose = function() {
-                e.removeData(this._element, "bs.collapse"), this._config = null, this._parent = null, this._element = null, this._triggerArray = null, this._isTransitioning = null
-            }, n._getConfig = function(t) {
-                return (t = o({}, w, t)).toggle = Boolean(t.toggle), s.typeCheckConfig(b, t, E), t
-            }, n._getDimension = function() {
-                return e(this._element).hasClass("width") ? "width" : "height"
-            }, n._getParent = function() {
-                var n, i = this;
-                s.isElement(this._config.parent) ? (n = this._config.parent, "undefined" != typeof this._config.parent.jquery && (n = this._config.parent[0])) : n = document.querySelector(this._config.parent);
-                var o = '[data-toggle="collapse"][data-parent="' + this._config.parent + '"]',
-                    r = [].slice.call(n.querySelectorAll(o));
-                return e(r).each((function(e, n) {
-                    i._addAriaAndCollapsedClass(t._getTargetFromElement(n), [n])
-                })), n
-            }, n._addAriaAndCollapsedClass = function(t, n) {
-                var i = e(t).hasClass("show");
-                n.length && e(n).toggleClass("collapsed", !i).attr("aria-expanded", i)
-            }, t._getTargetFromElement = function(t) {
-                var e = s.getSelectorFromElement(t);
-                return e ? document.querySelector(e) : null
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this),
-                        r = i.data("bs.collapse"),
-                        s = o({}, w, i.data(), "object" == typeof n && n ? n : {});
-                    if (!r && s.toggle && "string" == typeof n && /show|hide/.test(n) && (s.toggle = !1), r || (r = new t(this, s), i.data("bs.collapse", r)), "string" == typeof n) {
-                        if ("undefined" == typeof r[n]) throw new TypeError('No method named "' + n + '"');
-                        r[n]()
-                    }
-                }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return w
-                }
-            }]), t
-        }();
-    e(document).on("click.bs.collapse.data-api", '[data-toggle="collapse"]', (function(t) {
-        "A" === t.currentTarget.tagName && t.preventDefault();
-        var n = e(this),
-            i = s.getSelectorFromElement(this),
-            o = [].slice.call(document.querySelectorAll(i));
-        e(o).each((function() {
-            var t = e(this),
-                i = t.data("bs.collapse") ? "toggle" : n.data();
-            T._jQueryInterface.call(t, i)
+            }))
+        }
+    }
+    j.on(document, "click.bs.collapse.data-api", ft, (function(t) {
+        ("A" === t.target.tagName || t.delegateTarget && "A" === t.delegateTarget.tagName) && t.preventDefault();
+        const e = i(this);
+        V.find(e).forEach((t => {
+            pt.getOrCreateInstance(t, {
+                toggle: !1
+            }).toggle()
         }))
-    })), e.fn[b] = T._jQueryInterface, e.fn[b].Constructor = T, e.fn[b].noConflict = function() {
-        return e.fn[b] = y, T._jQueryInterface
-    };
-    var C = "undefined" != typeof window && "undefined" != typeof document && "undefined" != typeof navigator,
-        S = function() {
-            for (var t = ["Edge", "Trident", "Firefox"], e = 0; e < t.length; e += 1)
-                if (C && navigator.userAgent.indexOf(t[e]) >= 0) return 1;
-            return 0
-        }();
-    var D = C && window.Promise ? function(t) {
-        var e = !1;
-        return function() {
-            e || (e = !0, window.Promise.resolve().then((function() {
-                e = !1, t()
-            })))
-        }
-    } : function(t) {
-        var e = !1;
-        return function() {
-            e || (e = !0, setTimeout((function() {
-                e = !1, t()
-            }), S))
+    })), g(pt);
+    var mt = "top",
+        gt = "bottom",
+        _t = "right",
+        bt = "left",
+        vt = "auto",
+        yt = [mt, gt, _t, bt],
+        wt = "start",
+        Et = "end",
+        At = "clippingParents",
+        Tt = "viewport",
+        Ot = "popper",
+        Ct = "reference",
+        kt = yt.reduce((function(t, e) {
+            return t.concat([e + "-" + wt, e + "-" + Et])
+        }), []),
+        Lt = [].concat(yt, [vt]).reduce((function(t, e) {
+            return t.concat([e, e + "-" + wt, e + "-" + Et])
+        }), []),
+        xt = "beforeRead",
+        Dt = "read",
+        St = "afterRead",
+        Nt = "beforeMain",
+        It = "main",
+        Pt = "afterMain",
+        jt = "beforeWrite",
+        Mt = "write",
+        Ht = "afterWrite",
+        Bt = [xt, Dt, St, Nt, It, Pt, jt, Mt, Ht];
+
+    function Rt(t) {
+        return t ? (t.nodeName || "").toLowerCase() : null
+    }
+
+    function Wt(t) {
+        if (null == t) return window;
+        if ("[object Window]" !== t.toString()) {
+            var e = t.ownerDocument;
+            return e && e.defaultView || window
         }
-    };
-
-    function N(t) {
-        return t && "[object Function]" === {}.toString.call(t)
+        return t
     }
 
-    function k(t, e) {
-        if (1 !== t.nodeType) return [];
-        var n = t.ownerDocument.defaultView.getComputedStyle(t, null);
-        return e ? n[e] : n
+    function $t(t) {
+        return t instanceof Wt(t).Element || t instanceof Element
     }
 
-    function A(t) {
-        return "HTML" === t.nodeName ? t : t.parentNode || t.host
+    function zt(t) {
+        return t instanceof Wt(t).HTMLElement || t instanceof HTMLElement
+    }
+
+    function qt(t) {
+        return "undefined" != typeof ShadowRoot && (t instanceof Wt(t).ShadowRoot || t instanceof ShadowRoot)
+    }
+    const Ft = {
+        name: "applyStyles",
+        enabled: !0,
+        phase: "write",
+        fn: function(t) {
+            var e = t.state;
+            Object.keys(e.elements).forEach((function(t) {
+                var i = e.styles[t] || {},
+                    n = e.attributes[t] || {},
+                    s = e.elements[t];
+                zt(s) && Rt(s) && (Object.assign(s.style, i), Object.keys(n).forEach((function(t) {
+                    var e = n[t];
+                    !1 === e ? s.removeAttribute(t) : s.setAttribute(t, !0 === e ? "" : e)
+                })))
+            }))
+        },
+        effect: function(t) {
+            var e = t.state,
+                i = {
+                    popper: {
+                        position: e.options.strategy,
+                        left: "0",
+                        top: "0",
+                        margin: "0"
+                    },
+                    arrow: {
+                        position: "absolute"
+                    },
+                    reference: {}
+                };
+            return Object.assign(e.elements.popper.style, i.popper), e.styles = i, e.elements.arrow && Object.assign(e.elements.arrow.style, i.arrow),
+                function() {
+                    Object.keys(e.elements).forEach((function(t) {
+                        var n = e.elements[t],
+                            s = e.attributes[t] || {},
+                            o = Object.keys(e.styles.hasOwnProperty(t) ? e.styles[t] : i[t]).reduce((function(t, e) {
+                                return t[e] = "", t
+                            }), {});
+                        zt(n) && Rt(n) && (Object.assign(n.style, o), Object.keys(s).forEach((function(t) {
+                            n.removeAttribute(t)
+                        })))
+                    }))
+                }
+        },
+        requires: ["computeStyles"]
+    };
+
+    function Ut(t) {
+        return t.split("-")[0]
     }
 
-    function I(t) {
-        if (!t) return document.body;
-        switch (t.nodeName) {
-            case "HTML":
-            case "BODY":
-                return t.ownerDocument.body;
-            case "#document":
-                return t.body
+    function Vt(t, e) {
+        var i = t.getBoundingClientRect();
+        return {
+            width: i.width / 1,
+            height: i.height / 1,
+            top: i.top / 1,
+            right: i.right / 1,
+            bottom: i.bottom / 1,
+            left: i.left / 1,
+            x: i.left / 1,
+            y: i.top / 1
         }
-        var e = k(t),
-            n = e.overflow,
-            i = e.overflowX,
-            o = e.overflowY;
-        return /(auto|scroll|overlay)/.test(n + o + i) ? t : I(A(t))
     }
 
-    function O(t) {
-        return t && t.referenceNode ? t.referenceNode : t
+    function Kt(t) {
+        var e = Vt(t),
+            i = t.offsetWidth,
+            n = t.offsetHeight;
+        return Math.abs(e.width - i) <= 1 && (i = e.width), Math.abs(e.height - n) <= 1 && (n = e.height), {
+            x: t.offsetLeft,
+            y: t.offsetTop,
+            width: i,
+            height: n
+        }
     }
-    var x = C && !(!window.MSInputMethodContext || !document.documentMode),
-        j = C && /MSIE 10/.test(navigator.userAgent);
 
-    function L(t) {
-        return 11 === t ? x : 10 === t ? j : x || j
+    function Xt(t, e) {
+        var i = e.getRootNode && e.getRootNode();
+        if (t.contains(e)) return !0;
+        if (i && qt(i)) {
+            var n = e;
+            do {
+                if (n && t.isSameNode(n)) return !0;
+                n = n.parentNode || n.host
+            } while (n)
+        }
+        return !1
     }
 
-    function P(t) {
-        if (!t) return document.documentElement;
-        for (var e = L(10) ? document.body : null, n = t.offsetParent || null; n === e && t.nextElementSibling;) n = (t = t.nextElementSibling).offsetParent;
-        var i = n && n.nodeName;
-        return i && "BODY" !== i && "HTML" !== i ? -1 !== ["TH", "TD", "TABLE"].indexOf(n.nodeName) && "static" === k(n, "position") ? P(n) : n : t ? t.ownerDocument.documentElement : document.documentElement
+    function Yt(t) {
+        return Wt(t).getComputedStyle(t)
     }
 
-    function F(t) {
-        return null !== t.parentNode ? F(t.parentNode) : t
-    }
+    function Qt(t) {
+        return ["table", "td", "th"].indexOf(Rt(t)) >= 0
+    }
+
+    function Gt(t) {
+        return (($t(t) ? t.ownerDocument : t.document) || window.document).documentElement
+    }
+
+    function Zt(t) {
+        return "html" === Rt(t) ? t : t.assignedSlot || t.parentNode || (qt(t) ? t.host : null) || Gt(t)
+    }
+
+    function Jt(t) {
+        return zt(t) && "fixed" !== Yt(t).position ? t.offsetParent : null
+    }
+
+    function te(t) {
+        for (var e = Wt(t), i = Jt(t); i && Qt(i) && "static" === Yt(i).position;) i = Jt(i);
+        return i && ("html" === Rt(i) || "body" === Rt(i) && "static" === Yt(i).position) ? e : i || function(t) {
+            var e = -1 !== navigator.userAgent.toLowerCase().indexOf("firefox");
+            if (-1 !== navigator.userAgent.indexOf("Trident") && zt(t) && "fixed" === Yt(t).position) return null;
+            for (var i = Zt(t); zt(i) && ["html", "body"].indexOf(Rt(i)) < 0;) {
+                var n = Yt(i);
+                if ("none" !== n.transform || "none" !== n.perspective || "paint" === n.contain || -1 !== ["transform", "perspective"].indexOf(n.willChange) || e && "filter" === n.willChange || e && n.filter && "none" !== n.filter) return i;
+                i = i.parentNode
+            }
+            return null
+        }(t) || e
+    }
+
+    function ee(t) {
+        return ["top", "bottom"].indexOf(t) >= 0 ? "x" : "y"
+    }
+    var ie = Math.max,
+        ne = Math.min,
+        se = Math.round;
+
+    function oe(t, e, i) {
+        return ie(t, ne(e, i))
+    }
+
+    function re(t) {
+        return Object.assign({}, {
+            top: 0,
+            right: 0,
+            bottom: 0,
+            left: 0
+        }, t)
+    }
+
+    function ae(t, e) {
+        return e.reduce((function(e, i) {
+            return e[i] = t, e
+        }), {})
+    }
+    const le = {
+        name: "arrow",
+        enabled: !0,
+        phase: "main",
+        fn: function(t) {
+            var e, i = t.state,
+                n = t.name,
+                s = t.options,
+                o = i.elements.arrow,
+                r = i.modifiersData.popperOffsets,
+                a = Ut(i.placement),
+                l = ee(a),
+                c = [bt, _t].indexOf(a) >= 0 ? "height" : "width";
+            if (o && r) {
+                var h = function(t, e) {
+                        return re("number" != typeof(t = "function" == typeof t ? t(Object.assign({}, e.rects, {
+                            placement: e.placement
+                        })) : t) ? t : ae(t, yt))
+                    }(s.padding, i),
+                    d = Kt(o),
+                    u = "y" === l ? mt : bt,
+                    f = "y" === l ? gt : _t,
+                    p = i.rects.reference[c] + i.rects.reference[l] - r[l] - i.rects.popper[c],
+                    m = r[l] - i.rects.reference[l],
+                    g = te(o),
+                    _ = g ? "y" === l ? g.clientHeight || 0 : g.clientWidth || 0 : 0,
+                    b = p / 2 - m / 2,
+                    v = h[u],
+                    y = _ - d[c] - h[f],
+                    w = _ / 2 - d[c] / 2 + b,
+                    E = oe(v, w, y),
+                    A = l;
+                i.modifiersData[n] = ((e = {})[A] = E, e.centerOffset = E - w, e)
+            }
+        },
+        effect: function(t) {
+            var e = t.state,
+                i = t.options.element,
+                n = void 0 === i ? "[data-popper-arrow]" : i;
+            null != n && ("string" != typeof n || (n = e.elements.popper.querySelector(n))) && Xt(e.elements.popper, n) && (e.elements.arrow = n)
+        },
+        requires: ["popperOffsets"],
+        requiresIfExists: ["preventOverflow"]
+    };
 
-    function R(t, e) {
-        if (!(t && t.nodeType && e && e.nodeType)) return document.documentElement;
-        var n = t.compareDocumentPosition(e) & Node.DOCUMENT_POSITION_FOLLOWING,
-            i = n ? t : e,
-            o = n ? e : t,
-            r = document.createRange();
-        r.setStart(i, 0), r.setEnd(o, 0);
-        var s, a, l = r.commonAncestorContainer;
-        if (t !== l && e !== l || i.contains(o)) return "BODY" === (a = (s = l).nodeName) || "HTML" !== a && P(s.firstElementChild) !== s ? P(l) : l;
-        var c = F(t);
-        return c.host ? R(c.host, e) : R(t, F(e).host)
+    function ce(t) {
+        return t.split("-")[1]
     }
+    var he = {
+        top: "auto",
+        right: "auto",
+        bottom: "auto",
+        left: "auto"
+    };
 
-    function H(t) {
-        var e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "top",
-            n = "top" === e ? "scrollTop" : "scrollLeft",
-            i = t.nodeName;
-        if ("BODY" === i || "HTML" === i) {
-            var o = t.ownerDocument.documentElement,
-                r = t.ownerDocument.scrollingElement || o;
-            return r[n]
+    function de(t) {
+        var e, i = t.popper,
+            n = t.popperRect,
+            s = t.placement,
+            o = t.variation,
+            r = t.offsets,
+            a = t.position,
+            l = t.gpuAcceleration,
+            c = t.adaptive,
+            h = t.roundOffsets,
+            d = !0 === h ? function(t) {
+                var e = t.x,
+                    i = t.y,
+                    n = window.devicePixelRatio || 1;
+                return {
+                    x: se(se(e * n) / n) || 0,
+                    y: se(se(i * n) / n) || 0
+                }
+            }(r) : "function" == typeof h ? h(r) : r,
+            u = d.x,
+            f = void 0 === u ? 0 : u,
+            p = d.y,
+            m = void 0 === p ? 0 : p,
+            g = r.hasOwnProperty("x"),
+            _ = r.hasOwnProperty("y"),
+            b = bt,
+            v = mt,
+            y = window;
+        if (c) {
+            var w = te(i),
+                E = "clientHeight",
+                A = "clientWidth";
+            w === Wt(i) && "static" !== Yt(w = Gt(i)).position && "absolute" === a && (E = "scrollHeight", A = "scrollWidth"), w = w, s !== mt && (s !== bt && s !== _t || o !== Et) || (v = gt, m -= w[E] - n.height, m *= l ? 1 : -1), s !== bt && (s !== mt && s !== gt || o !== Et) || (b = _t, f -= w[A] - n.width, f *= l ? 1 : -1)
         }
-        return t[n]
-    }
-
-    function M(t, e) {
-        var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
-            i = H(e, "top"),
-            o = H(e, "left"),
-            r = n ? -1 : 1;
-        return t.top += i * r, t.bottom += i * r, t.left += o * r, t.right += o * r, t
-    }
+        var T, O = Object.assign({
+            position: a
+        }, c && he);
+        return l ? Object.assign({}, O, ((T = {})[v] = _ ? "0" : "", T[b] = g ? "0" : "", T.transform = (y.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + m + "px)" : "translate3d(" + f + "px, " + m + "px, 0)", T)) : Object.assign({}, O, ((e = {})[v] = _ ? m + "px" : "", e[b] = g ? f + "px" : "", e.transform = "", e))
+    }
+    const ue = {
+        name: "computeStyles",
+        enabled: !0,
+        phase: "beforeWrite",
+        fn: function(t) {
+            var e = t.state,
+                i = t.options,
+                n = i.gpuAcceleration,
+                s = void 0 === n || n,
+                o = i.adaptive,
+                r = void 0 === o || o,
+                a = i.roundOffsets,
+                l = void 0 === a || a,
+                c = {
+                    placement: Ut(e.placement),
+                    variation: ce(e.placement),
+                    popper: e.elements.popper,
+                    popperRect: e.rects.popper,
+                    gpuAcceleration: s
+                };
+            null != e.modifiersData.popperOffsets && (e.styles.popper = Object.assign({}, e.styles.popper, de(Object.assign({}, c, {
+                offsets: e.modifiersData.popperOffsets,
+                position: e.options.strategy,
+                adaptive: r,
+                roundOffsets: l
+            })))), null != e.modifiersData.arrow && (e.styles.arrow = Object.assign({}, e.styles.arrow, de(Object.assign({}, c, {
+                offsets: e.modifiersData.arrow,
+                position: "absolute",
+                adaptive: !1,
+                roundOffsets: l
+            })))), e.attributes.popper = Object.assign({}, e.attributes.popper, {
+                "data-popper-placement": e.placement
+            })
+        },
+        data: {}
+    };
+    var fe = {
+        passive: !0
+    };
+    const pe = {
+        name: "eventListeners",
+        enabled: !0,
+        phase: "write",
+        fn: function() {},
+        effect: function(t) {
+            var e = t.state,
+                i = t.instance,
+                n = t.options,
+                s = n.scroll,
+                o = void 0 === s || s,
+                r = n.resize,
+                a = void 0 === r || r,
+                l = Wt(e.elements.popper),
+                c = [].concat(e.scrollParents.reference, e.scrollParents.popper);
+            return o && c.forEach((function(t) {
+                    t.addEventListener("scroll", i.update, fe)
+                })), a && l.addEventListener("resize", i.update, fe),
+                function() {
+                    o && c.forEach((function(t) {
+                        t.removeEventListener("scroll", i.update, fe)
+                    })), a && l.removeEventListener("resize", i.update, fe)
+                }
+        },
+        data: {}
+    };
+    var me = {
+        left: "right",
+        right: "left",
+        bottom: "top",
+        top: "bottom"
+    };
 
-    function B(t, e) {
-        var n = "x" === e ? "Left" : "Top",
-            i = "Left" === n ? "Right" : "Bottom";
-        return parseFloat(t["border" + n + "Width"]) + parseFloat(t["border" + i + "Width"])
+    function ge(t) {
+        return t.replace(/left|right|bottom|top/g, (function(t) {
+            return me[t]
+        }))
     }
+    var _e = {
+        start: "end",
+        end: "start"
+    };
 
-    function q(t, e, n, i) {
-        return Math.max(e["offset" + t], e["scroll" + t], n["client" + t], n["offset" + t], n["scroll" + t], L(10) ? parseInt(n["offset" + t]) + parseInt(i["margin" + ("Height" === t ? "Top" : "Left")]) + parseInt(i["margin" + ("Height" === t ? "Bottom" : "Right")]) : 0)
+    function be(t) {
+        return t.replace(/start|end/g, (function(t) {
+            return _e[t]
+        }))
     }
 
-    function Q(t) {
-        var e = t.body,
-            n = t.documentElement,
-            i = L(10) && getComputedStyle(n);
+    function ve(t) {
+        var e = Wt(t);
         return {
-            height: q("Height", e, n, i),
-            width: q("Width", e, n, i)
+            scrollLeft: e.pageXOffset,
+            scrollTop: e.pageYOffset
         }
     }
-    var W = function(t, e) {
-            if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
-        },
-        U = function() {
-            function t(t, e) {
-                for (var n = 0; n < e.length; n++) {
-                    var i = e[n];
-                    i.enumerable = i.enumerable || !1, i.configurable = !0, "value" in i && (i.writable = !0), Object.defineProperty(t, i.key, i)
-                }
-            }
-            return function(e, n, i) {
-                return n && t(e.prototype, n), i && t(e, i), e
-            }
-        }(),
-        V = function(t, e, n) {
-            return e in t ? Object.defineProperty(t, e, {
-                value: n,
-                enumerable: !0,
-                configurable: !0,
-                writable: !0
-            }) : t[e] = n, t
-        },
-        Y = Object.assign || function(t) {
-            for (var e = 1; e < arguments.length; e++) {
-                var n = arguments[e];
-                for (var i in n) Object.prototype.hasOwnProperty.call(n, i) && (t[i] = n[i])
-            }
-            return t
-        };
 
-    function z(t) {
-        return Y({}, t, {
-            right: t.left + t.width,
-            bottom: t.top + t.height
-        })
+    function ye(t) {
+        return Vt(Gt(t)).left + ve(t).scrollLeft
     }
 
-    function X(t) {
-        var e = {};
-        try {
-            if (L(10)) {
-                e = t.getBoundingClientRect();
-                var n = H(t, "top"),
-                    i = H(t, "left");
-                e.top += n, e.left += i, e.bottom += n, e.right += i
-            } else e = t.getBoundingClientRect()
-        } catch (t) {}
-        var o = {
-                left: e.left,
-                top: e.top,
-                width: e.right - e.left,
-                height: e.bottom - e.top
-            },
-            r = "HTML" === t.nodeName ? Q(t.ownerDocument) : {},
-            s = r.width || t.clientWidth || o.width,
-            a = r.height || t.clientHeight || o.height,
-            l = t.offsetWidth - s,
-            c = t.offsetHeight - a;
-        if (l || c) {
-            var h = k(t);
-            l -= B(h, "x"), c -= B(h, "y"), o.width -= l, o.height -= c
-        }
-        return z(o)
-    }
-
-    function K(t, e) {
-        var n = arguments.length > 2 && void 0 !== arguments[2] && arguments[2],
-            i = L(10),
-            o = "HTML" === e.nodeName,
-            r = X(t),
-            s = X(e),
-            a = I(t),
-            l = k(e),
-            c = parseFloat(l.borderTopWidth),
-            h = parseFloat(l.borderLeftWidth);
-        n && o && (s.top = Math.max(s.top, 0), s.left = Math.max(s.left, 0));
-        var u = z({
-            top: r.top - s.top - c,
-            left: r.left - s.left - h,
-            width: r.width,
-            height: r.height
-        });
-        if (u.marginTop = 0, u.marginLeft = 0, !i && o) {
-            var f = parseFloat(l.marginTop),
-                d = parseFloat(l.marginLeft);
-            u.top -= c - f, u.bottom -= c - f, u.left -= h - d, u.right -= h - d, u.marginTop = f, u.marginLeft = d
-        }
-        return (i && !n ? e.contains(a) : e === a && "BODY" !== a.nodeName) && (u = M(u, e)), u
-    }
-
-    function G(t) {
-        var e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-            n = t.ownerDocument.documentElement,
-            i = K(t, n),
-            o = Math.max(n.clientWidth, window.innerWidth || 0),
-            r = Math.max(n.clientHeight, window.innerHeight || 0),
-            s = e ? 0 : H(n),
-            a = e ? 0 : H(n, "left"),
-            l = {
-                top: s - i.top + i.marginTop,
-                left: a - i.left + i.marginLeft,
-                width: o,
-                height: r
-            };
-        return z(l)
-    }
-
-    function $(t) {
-        var e = t.nodeName;
-        if ("BODY" === e || "HTML" === e) return !1;
-        if ("fixed" === k(t, "position")) return !0;
-        var n = A(t);
-        return !!n && $(n)
-    }
-
-    function J(t) {
-        if (!t || !t.parentElement || L()) return document.documentElement;
-        for (var e = t.parentElement; e && "none" === k(e, "transform");) e = e.parentElement;
-        return e || document.documentElement
+    function we(t) {
+        var e = Yt(t),
+            i = e.overflow,
+            n = e.overflowX,
+            s = e.overflowY;
+        return /auto|scroll|overlay|hidden/.test(i + s + n)
+    }
+
+    function Ee(t) {
+        return ["html", "body", "#document"].indexOf(Rt(t)) >= 0 ? t.ownerDocument.body : zt(t) && we(t) ? t : Ee(Zt(t))
+    }
+
+    function Ae(t, e) {
+        var i;
+        void 0 === e && (e = []);
+        var n = Ee(t),
+            s = n === (null == (i = t.ownerDocument) ? void 0 : i.body),
+            o = Wt(n),
+            r = s ? [o].concat(o.visualViewport || [], we(n) ? n : []) : n,
+            a = e.concat(r);
+        return s ? a : a.concat(Ae(Zt(r)))
+    }
+
+    function Te(t) {
+        return Object.assign({}, t, {
+            left: t.x,
+            top: t.y,
+            right: t.x + t.width,
+            bottom: t.y + t.height
+        })
     }
 
-    function Z(t, e, n, i) {
-        var o = arguments.length > 4 && void 0 !== arguments[4] && arguments[4],
-            r = {
-                top: 0,
-                left: 0
-            },
-            s = o ? J(t) : R(t, O(e));
-        if ("viewport" === i) r = G(s, o);
-        else {
-            var a = void 0;
-            "scrollParent" === i ? "BODY" === (a = I(A(e))).nodeName && (a = t.ownerDocument.documentElement) : a = "window" === i ? t.ownerDocument.documentElement : i;
-            var l = K(a, s, o);
-            if ("HTML" !== a.nodeName || $(s)) r = l;
-            else {
-                var c = Q(t.ownerDocument),
-                    h = c.height,
-                    u = c.width;
-                r.top += l.top - l.marginTop, r.bottom = h + l.top, r.left += l.left - l.marginLeft, r.right = u + l.left
-            }
-        }
-        var f = "number" == typeof(n = n || 0);
-        return r.left += f ? n : n.left || 0, r.top += f ? n : n.top || 0, r.right -= f ? n : n.right || 0, r.bottom -= f ? n : n.bottom || 0, r
-    }
-
-    function tt(t) {
-        return t.width * t.height
-    }
-
-    function et(t, e, n, i, o) {
-        var r = arguments.length > 5 && void 0 !== arguments[5] ? arguments[5] : 0;
-        if (-1 === t.indexOf("auto")) return t;
-        var s = Z(n, i, r, o),
-            a = {
-                top: {
-                    width: s.width,
-                    height: e.top - s.top
-                },
-                right: {
-                    width: s.right - e.right,
-                    height: s.height
-                },
-                bottom: {
-                    width: s.width,
-                    height: s.bottom - e.bottom
-                },
-                left: {
-                    width: e.left - s.left,
-                    height: s.height
+    function Oe(t, e) {
+        return e === Tt ? Te(function(t) {
+            var e = Wt(t),
+                i = Gt(t),
+                n = e.visualViewport,
+                s = i.clientWidth,
+                o = i.clientHeight,
+                r = 0,
+                a = 0;
+            return n && (s = n.width, o = n.height, /^((?!chrome|android).)*safari/i.test(navigator.userAgent) || (r = n.offsetLeft, a = n.offsetTop)), {
+                width: s,
+                height: o,
+                x: r + ye(t),
+                y: a
+            }
+        }(t)) : zt(e) ? function(t) {
+            var e = Vt(t);
+            return e.top = e.top + t.clientTop, e.left = e.left + t.clientLeft, e.bottom = e.top + t.clientHeight, e.right = e.left + t.clientWidth, e.width = t.clientWidth, e.height = t.clientHeight, e.x = e.left, e.y = e.top, e
+        }(e) : Te(function(t) {
+            var e, i = Gt(t),
+                n = ve(t),
+                s = null == (e = t.ownerDocument) ? void 0 : e.body,
+                o = ie(i.scrollWidth, i.clientWidth, s ? s.scrollWidth : 0, s ? s.clientWidth : 0),
+                r = ie(i.scrollHeight, i.clientHeight, s ? s.scrollHeight : 0, s ? s.clientHeight : 0),
+                a = -n.scrollLeft + ye(t),
+                l = -n.scrollTop;
+            return "rtl" === Yt(s || i).direction && (a += ie(i.clientWidth, s ? s.clientWidth : 0) - o), {
+                width: o,
+                height: r,
+                x: a,
+                y: l
+            }
+        }(Gt(t)))
+    }
+
+    function Ce(t) {
+        var e, i = t.reference,
+            n = t.element,
+            s = t.placement,
+            o = s ? Ut(s) : null,
+            r = s ? ce(s) : null,
+            a = i.x + i.width / 2 - n.width / 2,
+            l = i.y + i.height / 2 - n.height / 2;
+        switch (o) {
+            case mt:
+                e = {
+                    x: a,
+                    y: i.y - n.height
+                };
+                break;
+            case gt:
+                e = {
+                    x: a,
+                    y: i.y + i.height
+                };
+                break;
+            case _t:
+                e = {
+                    x: i.x + i.width,
+                    y: l
+                };
+                break;
+            case bt:
+                e = {
+                    x: i.x - n.width,
+                    y: l
+                };
+                break;
+            default:
+                e = {
+                    x: i.x,
+                    y: i.y
                 }
-            },
-            l = Object.keys(a).map((function(t) {
-                return Y({
-                    key: t
-                }, a[t], {
-                    area: tt(a[t])
-                })
-            })).sort((function(t, e) {
-                return e.area - t.area
-            })),
-            c = l.filter((function(t) {
-                var e = t.width,
-                    i = t.height;
-                return e >= n.clientWidth && i >= n.clientHeight
-            })),
-            h = c.length > 0 ? c[0].key : l[0].key,
-            u = t.split("-")[1];
-        return h + (u ? "-" + u : "")
-    }
-
-    function nt(t, e, n) {
-        var i = arguments.length > 3 && void 0 !== arguments[3] ? arguments[3] : null,
-            o = i ? J(e) : R(e, O(n));
-        return K(n, o, i)
-    }
-
-    function it(t) {
-        var e = t.ownerDocument.defaultView.getComputedStyle(t),
-            n = parseFloat(e.marginTop || 0) + parseFloat(e.marginBottom || 0),
-            i = parseFloat(e.marginLeft || 0) + parseFloat(e.marginRight || 0);
-        return {
-            width: t.offsetWidth + i,
-            height: t.offsetHeight + n
         }
+        var c = o ? ee(o) : null;
+        if (null != c) {
+            var h = "y" === c ? "height" : "width";
+            switch (r) {
+                case wt:
+                    e[c] = e[c] - (i[h] / 2 - n[h] / 2);
+                    break;
+                case Et:
+                    e[c] = e[c] + (i[h] / 2 - n[h] / 2)
+            }
+        }
+        return e
     }
 
-    function ot(t) {
-        var e = {
-            left: "right",
-            right: "left",
-            bottom: "top",
-            top: "bottom"
-        };
-        return t.replace(/left|right|bottom|top/g, (function(t) {
-            return e[t]
-        }))
-    }
-
-    function rt(t, e, n) {
-        n = n.split("-")[0];
-        var i = it(t),
-            o = {
-                width: i.width,
-                height: i.height
+    function ke(t, e) {
+        void 0 === e && (e = {});
+        var i = e,
+            n = i.placement,
+            s = void 0 === n ? t.placement : n,
+            o = i.boundary,
+            r = void 0 === o ? At : o,
+            a = i.rootBoundary,
+            l = void 0 === a ? Tt : a,
+            c = i.elementContext,
+            h = void 0 === c ? Ot : c,
+            d = i.altBoundary,
+            u = void 0 !== d && d,
+            f = i.padding,
+            p = void 0 === f ? 0 : f,
+            m = re("number" != typeof p ? p : ae(p, yt)),
+            g = h === Ot ? Ct : Ot,
+            _ = t.rects.popper,
+            b = t.elements[u ? g : h],
+            v = function(t, e, i) {
+                var n = "clippingParents" === e ? function(t) {
+                        var e = Ae(Zt(t)),
+                            i = ["absolute", "fixed"].indexOf(Yt(t).position) >= 0 && zt(t) ? te(t) : t;
+                        return $t(i) ? e.filter((function(t) {
+                            return $t(t) && Xt(t, i) && "body" !== Rt(t)
+                        })) : []
+                    }(t) : [].concat(e),
+                    s = [].concat(n, [i]),
+                    o = s[0],
+                    r = s.reduce((function(e, i) {
+                        var n = Oe(t, i);
+                        return e.top = ie(n.top, e.top), e.right = ne(n.right, e.right), e.bottom = ne(n.bottom, e.bottom), e.left = ie(n.left, e.left), e
+                    }), Oe(t, o));
+                return r.width = r.right - r.left, r.height = r.bottom - r.top, r.x = r.left, r.y = r.top, r
+            }($t(b) ? b : b.contextElement || Gt(t.elements.popper), r, l),
+            y = Vt(t.elements.reference),
+            w = Ce({
+                reference: y,
+                element: _,
+                strategy: "absolute",
+                placement: s
+            }),
+            E = Te(Object.assign({}, _, w)),
+            A = h === Ot ? E : y,
+            T = {
+                top: v.top - A.top + m.top,
+                bottom: A.bottom - v.bottom + m.bottom,
+                left: v.left - A.left + m.left,
+                right: A.right - v.right + m.right
             },
-            r = -1 !== ["right", "left"].indexOf(n),
-            s = r ? "top" : "left",
-            a = r ? "left" : "top",
-            l = r ? "height" : "width",
-            c = r ? "width" : "height";
-        return o[s] = e[s] + e[l] / 2 - i[l] / 2, o[a] = n === a ? e[a] - i[c] : e[ot(a)], o
-    }
-
-    function st(t, e) {
-        return Array.prototype.find ? t.find(e) : t.filter(e)[0]
-    }
-
-    function at(t, e, n) {
-        return (void 0 === n ? t : t.slice(0, function(t, e, n) {
-            if (Array.prototype.findIndex) return t.findIndex((function(t) {
-                return t[e] === n
-            }));
-            var i = st(t, (function(t) {
-                return t[e] === n
-            }));
-            return t.indexOf(i)
-        }(t, "name", n))).forEach((function(t) {
-            t.function && console.warn("`modifier.function` is deprecated, use `modifier.fn`!");
-            var n = t.function || t.fn;
-            t.enabled && N(n) && (e.offsets.popper = z(e.offsets.popper), e.offsets.reference = z(e.offsets.reference), e = n(e, t))
-        })), e
-    }
-
-    function lt() {
-        if (!this.state.isDestroyed) {
-            var t = {
-                instance: this,
-                styles: {},
-                arrowStyles: {},
-                attributes: {},
-                flipped: !1,
-                offsets: {}
-            };
-            t.offsets.reference = nt(this.state, this.popper, this.reference, this.options.positionFixed), t.placement = et(this.options.placement, t.offsets.reference, this.popper, this.reference, this.options.modifiers.flip.boundariesElement, this.options.modifiers.flip.padding), t.originalPlacement = t.placement, t.positionFixed = this.options.positionFixed, t.offsets.popper = rt(this.popper, t.offsets.reference, t.placement), t.offsets.popper.position = this.options.positionFixed ? "fixed" : "absolute", t = at(this.modifiers, t), this.state.isCreated ? this.options.onUpdate(t) : (this.state.isCreated = !0, this.options.onCreate(t))
+            O = t.modifiersData.offset;
+        if (h === Ot && O) {
+            var C = O[s];
+            Object.keys(T).forEach((function(t) {
+                var e = [_t, gt].indexOf(t) >= 0 ? 1 : -1,
+                    i = [mt, gt].indexOf(t) >= 0 ? "y" : "x";
+                T[t] += C[i] * e
+            }))
         }
+        return T
     }
 
-    function ct(t, e) {
-        return t.some((function(t) {
-            var n = t.name;
-            return t.enabled && n === e
+    function Le(t, e) {
+        void 0 === e && (e = {});
+        var i = e,
+            n = i.placement,
+            s = i.boundary,
+            o = i.rootBoundary,
+            r = i.padding,
+            a = i.flipVariations,
+            l = i.allowedAutoPlacements,
+            c = void 0 === l ? Lt : l,
+            h = ce(n),
+            d = h ? a ? kt : kt.filter((function(t) {
+                return ce(t) === h
+            })) : yt,
+            u = d.filter((function(t) {
+                return c.indexOf(t) >= 0
+            }));
+        0 === u.length && (u = d);
+        var f = u.reduce((function(e, i) {
+            return e[i] = ke(t, {
+                placement: i,
+                boundary: s,
+                rootBoundary: o,
+                padding: r
+            })[Ut(i)], e
+        }), {});
+        return Object.keys(f).sort((function(t, e) {
+            return f[t] - f[e]
         }))
     }
-
-    function ht(t) {
-        for (var e = [!1, "ms", "Webkit", "Moz", "O"], n = t.charAt(0).toUpperCase() + t.slice(1), i = 0; i < e.length; i++) {
-            var o = e[i],
-                r = o ? "" + o + n : t;
-            if ("undefined" != typeof document.body.style[r]) return r
+    const xe = {
+        name: "flip",
+        enabled: !0,
+        phase: "main",
+        fn: function(t) {
+            var e = t.state,
+                i = t.options,
+                n = t.name;
+            if (!e.modifiersData[n]._skip) {
+                for (var s = i.mainAxis, o = void 0 === s || s, r = i.altAxis, a = void 0 === r || r, l = i.fallbackPlacements, c = i.padding, h = i.boundary, d = i.rootBoundary, u = i.altBoundary, f = i.flipVariations, p = void 0 === f || f, m = i.allowedAutoPlacements, g = e.options.placement, _ = Ut(g), b = l || (_ !== g && p ? function(t) {
+                        if (Ut(t) === vt) return [];
+                        var e = ge(t);
+                        return [be(t), e, be(e)]
+                    }(g) : [ge(g)]), v = [g].concat(b).reduce((function(t, i) {
+                        return t.concat(Ut(i) === vt ? Le(e, {
+                            placement: i,
+                            boundary: h,
+                            rootBoundary: d,
+                            padding: c,
+                            flipVariations: p,
+                            allowedAutoPlacements: m
+                        }) : i)
+                    }), []), y = e.rects.reference, w = e.rects.popper, E = new Map, A = !0, T = v[0], O = 0; O < v.length; O++) {
+                    var C = v[O],
+                        k = Ut(C),
+                        L = ce(C) === wt,
+                        x = [mt, gt].indexOf(k) >= 0,
+                        D = x ? "width" : "height",
+                        S = ke(e, {
+                            placement: C,
+                            boundary: h,
+                            rootBoundary: d,
+                            altBoundary: u,
+                            padding: c
+                        }),
+                        N = x ? L ? _t : bt : L ? gt : mt;
+                    y[D] > w[D] && (N = ge(N));
+                    var I = ge(N),
+                        P = [];
+                    if (o && P.push(S[k] <= 0), a && P.push(S[N] <= 0, S[I] <= 0), P.every((function(t) {
+                            return t
+                        }))) {
+                        T = C, A = !1;
+                        break
+                    }
+                    E.set(C, P)
+                }
+                if (A)
+                    for (var j = function(t) {
+                            var e = v.find((function(e) {
+                                var i = E.get(e);
+                                if (i) return i.slice(0, t).every((function(t) {
+                                    return t
+                                }))
+                            }));
+                            if (e) return T = e, "break"
+                        }, M = p ? 3 : 1; M > 0 && "break" !== j(M); M--);
+                e.placement !== T && (e.modifiersData[n]._skip = !0, e.placement = T, e.reset = !0)
+            }
+        },
+        requiresIfExists: ["offset"],
+        data: {
+            _skip: !1
         }
-        return null
-    }
-
-    function ut() {
-        return this.state.isDestroyed = !0, ct(this.modifiers, "applyStyle") && (this.popper.removeAttribute("x-placement"), this.popper.style.position = "", this.popper.style.top = "", this.popper.style.left = "", this.popper.style.right = "", this.popper.style.bottom = "", this.popper.style.willChange = "", this.popper.style[ht("transform")] = ""), this.disableEventListeners(), this.options.removeOnDestroy && this.popper.parentNode.removeChild(this.popper), this
-    }
-
-    function ft(t) {
-        var e = t.ownerDocument;
-        return e ? e.defaultView : window
-    }
+    };
 
-    function dt(t, e, n, i) {
-        n.updateBound = i, ft(t).addEventListener("resize", n.updateBound, {
-            passive: !0
-        });
-        var o = I(t);
-        return function t(e, n, i, o) {
-            var r = "BODY" === e.nodeName,
-                s = r ? e.ownerDocument.defaultView : e;
-            s.addEventListener(n, i, {
-                passive: !0
-            }), r || t(I(s.parentNode), n, i, o), o.push(s)
-        }(o, "scroll", n.updateBound, n.scrollParents), n.scrollElement = o, n.eventsEnabled = !0, n
+    function De(t, e, i) {
+        return void 0 === i && (i = {
+            x: 0,
+            y: 0
+        }), {
+            top: t.top - e.height - i.y,
+            right: t.right - e.width + i.x,
+            bottom: t.bottom - e.height + i.y,
+            left: t.left - e.width - i.x
+        }
     }
 
-    function pt() {
-        this.state.eventsEnabled || (this.state = dt(this.reference, this.options, this.state, this.scheduleUpdate))
+    function Se(t) {
+        return [mt, _t, gt, bt].some((function(e) {
+            return t[e] >= 0
+        }))
     }
+    const Ne = {
+            name: "hide",
+            enabled: !0,
+            phase: "main",
+            requiresIfExists: ["preventOverflow"],
+            fn: function(t) {
+                var e = t.state,
+                    i = t.name,
+                    n = e.rects.reference,
+                    s = e.rects.popper,
+                    o = e.modifiersData.preventOverflow,
+                    r = ke(e, {
+                        elementContext: "reference"
+                    }),
+                    a = ke(e, {
+                        altBoundary: !0
+                    }),
+                    l = De(r, n),
+                    c = De(a, s, o),
+                    h = Se(l),
+                    d = Se(c);
+                e.modifiersData[i] = {
+                    referenceClippingOffsets: l,
+                    popperEscapeOffsets: c,
+                    isReferenceHidden: h,
+                    hasPopperEscaped: d
+                }, e.attributes.popper = Object.assign({}, e.attributes.popper, {
+                    "data-popper-reference-hidden": h,
+                    "data-popper-escaped": d
+                })
+            }
+        },
+        Ie = {
+            name: "offset",
+            enabled: !0,
+            phase: "main",
+            requires: ["popperOffsets"],
+            fn: function(t) {
+                var e = t.state,
+                    i = t.options,
+                    n = t.name,
+                    s = i.offset,
+                    o = void 0 === s ? [0, 0] : s,
+                    r = Lt.reduce((function(t, i) {
+                        return t[i] = function(t, e, i) {
+                            var n = Ut(t),
+                                s = [bt, mt].indexOf(n) >= 0 ? -1 : 1,
+                                o = "function" == typeof i ? i(Object.assign({}, e, {
+                                    placement: t
+                                })) : i,
+                                r = o[0],
+                                a = o[1];
+                            return r = r || 0, a = (a || 0) * s, [bt, _t].indexOf(n) >= 0 ? {
+                                x: a,
+                                y: r
+                            } : {
+                                x: r,
+                                y: a
+                            }
+                        }(i, e.rects, o), t
+                    }), {}),
+                    a = r[e.placement],
+                    l = a.x,
+                    c = a.y;
+                null != e.modifiersData.popperOffsets && (e.modifiersData.popperOffsets.x += l, e.modifiersData.popperOffsets.y += c), e.modifiersData[n] = r
+            }
+        },
+        Pe = {
+            name: "popperOffsets",
+            enabled: !0,
+            phase: "read",
+            fn: function(t) {
+                var e = t.state,
+                    i = t.name;
+                e.modifiersData[i] = Ce({
+                    reference: e.rects.reference,
+                    element: e.rects.popper,
+                    strategy: "absolute",
+                    placement: e.placement
+                })
+            },
+            data: {}
+        },
+        je = {
+            name: "preventOverflow",
+            enabled: !0,
+            phase: "main",
+            fn: function(t) {
+                var e = t.state,
+                    i = t.options,
+                    n = t.name,
+                    s = i.mainAxis,
+                    o = void 0 === s || s,
+                    r = i.altAxis,
+                    a = void 0 !== r && r,
+                    l = i.boundary,
+                    c = i.rootBoundary,
+                    h = i.altBoundary,
+                    d = i.padding,
+                    u = i.tether,
+                    f = void 0 === u || u,
+                    p = i.tetherOffset,
+                    m = void 0 === p ? 0 : p,
+                    g = ke(e, {
+                        boundary: l,
+                        rootBoundary: c,
+                        padding: d,
+                        altBoundary: h
+                    }),
+                    _ = Ut(e.placement),
+                    b = ce(e.placement),
+                    v = !b,
+                    y = ee(_),
+                    w = "x" === y ? "y" : "x",
+                    E = e.modifiersData.popperOffsets,
+                    A = e.rects.reference,
+                    T = e.rects.popper,
+                    O = "function" == typeof m ? m(Object.assign({}, e.rects, {
+                        placement: e.placement
+                    })) : m,
+                    C = {
+                        x: 0,
+                        y: 0
+                    };
+                if (E) {
+                    if (o || a) {
+                        var k = "y" === y ? mt : bt,
+                            L = "y" === y ? gt : _t,
+                            x = "y" === y ? "height" : "width",
+                            D = E[y],
+                            S = E[y] + g[k],
+                            N = E[y] - g[L],
+                            I = f ? -T[x] / 2 : 0,
+                            P = b === wt ? A[x] : T[x],
+                            j = b === wt ? -T[x] : -A[x],
+                            M = e.elements.arrow,
+                            H = f && M ? Kt(M) : {
+                                width: 0,
+                                height: 0
+                            },
+                            B = e.modifiersData["arrow#persistent"] ? e.modifiersData["arrow#persistent"].padding : {
+                                top: 0,
+                                right: 0,
+                                bottom: 0,
+                                left: 0
+                            },
+                            R = B[k],
+                            W = B[L],
+                            $ = oe(0, A[x], H[x]),
+                            z = v ? A[x] / 2 - I - $ - R - O : P - $ - R - O,
+                            q = v ? -A[x] / 2 + I + $ + W + O : j + $ + W + O,
+                            F = e.elements.arrow && te(e.elements.arrow),
+                            U = F ? "y" === y ? F.clientTop || 0 : F.clientLeft || 0 : 0,
+                            V = e.modifiersData.offset ? e.modifiersData.offset[e.placement][y] : 0,
+                            K = E[y] + z - V - U,
+                            X = E[y] + q - V;
+                        if (o) {
+                            var Y = oe(f ? ne(S, K) : S, D, f ? ie(N, X) : N);
+                            E[y] = Y, C[y] = Y - D
+                        }
+                        if (a) {
+                            var Q = "x" === y ? mt : bt,
+                                G = "x" === y ? gt : _t,
+                                Z = E[w],
+                                J = Z + g[Q],
+                                tt = Z - g[G],
+                                et = oe(f ? ne(J, K) : J, Z, f ? ie(tt, X) : tt);
+                            E[w] = et, C[w] = et - Z
+                        }
+                    }
+                    e.modifiersData[n] = C
+                }
+            },
+            requiresIfExists: ["offset"]
+        };
 
-    function mt() {
-        var t, e;
-        this.state.eventsEnabled && (cancelAnimationFrame(this.scheduleUpdate), this.state = (t = this.reference, e = this.state, ft(t).removeEventListener("resize", e.updateBound), e.scrollParents.forEach((function(t) {
-            t.removeEventListener("scroll", e.updateBound)
-        })), e.updateBound = null, e.scrollParents = [], e.scrollElement = null, e.eventsEnabled = !1, e))
+    function Me(t, e, i) {
+        void 0 === i && (i = !1);
+        var n = zt(e);
+        zt(e) && function(t) {
+            var e = t.getBoundingClientRect();
+            e.width, t.offsetWidth, e.height, t.offsetHeight
+        }(e);
+        var s, o, r = Gt(e),
+            a = Vt(t),
+            l = {
+                scrollLeft: 0,
+                scrollTop: 0
+            },
+            c = {
+                x: 0,
+                y: 0
+            };
+        return (n || !n && !i) && (("body" !== Rt(e) || we(r)) && (l = (s = e) !== Wt(s) && zt(s) ? {
+            scrollLeft: (o = s).scrollLeft,
+            scrollTop: o.scrollTop
+        } : ve(s)), zt(e) ? ((c = Vt(e)).x += e.clientLeft, c.y += e.clientTop) : r && (c.x = ye(r))), {
+            x: a.left + l.scrollLeft - c.x,
+            y: a.top + l.scrollTop - c.y,
+            width: a.width,
+            height: a.height
+        }
     }
 
-    function gt(t) {
-        return "" !== t && !isNaN(parseFloat(t)) && isFinite(t)
-    }
+    function He(t) {
+        var e = new Map,
+            i = new Set,
+            n = [];
+
+        function s(t) {
+            i.add(t.name), [].concat(t.requires || [], t.requiresIfExists || []).forEach((function(t) {
+                if (!i.has(t)) {
+                    var n = e.get(t);
+                    n && s(n)
+                }
+            })), n.push(t)
+        }
+        return t.forEach((function(t) {
+            e.set(t.name, t)
+        })), t.forEach((function(t) {
+            i.has(t.name) || s(t)
+        })), n
+    }
+    var Be = {
+        placement: "bottom",
+        modifiers: [],
+        strategy: "absolute"
+    };
 
-    function _t(t, e) {
-        Object.keys(e).forEach((function(n) {
-            var i = ""; - 1 !== ["width", "height", "top", "right", "bottom", "left"].indexOf(n) && gt(e[n]) && (i = "px"), t.style[n] = e[n] + i
+    function Re() {
+        for (var t = arguments.length, e = new Array(t), i = 0; i < t; i++) e[i] = arguments[i];
+        return !e.some((function(t) {
+            return !(t && "function" == typeof t.getBoundingClientRect)
         }))
     }
-    var vt = C && /Firefox/i.test(navigator.userAgent);
 
-    function bt(t, e, n) {
-        var i = st(t, (function(t) {
-                return t.name === e
-            })),
-            o = !!i && t.some((function(t) {
-                return t.name === n && t.enabled && t.order < i.order
-            }));
-        if (!o) {
-            var r = "`" + e + "`",
-                s = "`" + n + "`";
-            console.warn(s + " modifier is required by " + r + " modifier in order to work, be sure to include it before " + r + "!")
-        }
-        return o
-    }
-    var yt = ["auto-start", "auto", "auto-end", "top-start", "top", "top-end", "right-start", "right", "right-end", "bottom-end", "bottom", "bottom-start", "left-end", "left", "left-start"],
-        wt = yt.slice(3);
-
-    function Et(t) {
-        var e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-            n = wt.indexOf(t),
-            i = wt.slice(n + 1).concat(wt.slice(0, n));
-        return e ? i.reverse() : i
-    }
-    var Tt = "flip",
-        Ct = "clockwise",
-        St = "counterclockwise";
-
-    function Dt(t, e, n, i) {
-        var o = [0, 0],
-            r = -1 !== ["right", "left"].indexOf(i),
-            s = t.split(/(\+|\-)/).map((function(t) {
-                return t.trim()
-            })),
-            a = s.indexOf(st(s, (function(t) {
-                return -1 !== t.search(/,|\s/)
-            })));
-        s[a] && -1 === s[a].indexOf(",") && console.warn("Offsets separated by white space(s) are deprecated, use a comma (,) instead.");
-        var l = /\s*,\s*|\s+/,
-            c = -1 !== a ? [s.slice(0, a).concat([s[a].split(l)[0]]), [s[a].split(l)[1]].concat(s.slice(a + 1))] : [s];
-        return (c = c.map((function(t, i) {
-            var o = (1 === i ? !r : r) ? "height" : "width",
-                s = !1;
-            return t.reduce((function(t, e) {
-                return "" === t[t.length - 1] && -1 !== ["+", "-"].indexOf(e) ? (t[t.length - 1] = e, s = !0, t) : s ? (t[t.length - 1] += e, s = !1, t) : t.concat(e)
-            }), []).map((function(t) {
-                return function(t, e, n, i) {
-                    var o = t.match(/((?:\-|\+)?\d*\.?\d*)(.*)/),
-                        r = +o[1],
-                        s = o[2];
-                    if (!r) return t;
-                    if (0 === s.indexOf("%")) {
-                        var a = void 0;
-                        switch (s) {
-                            case "%p":
-                                a = n;
-                                break;
-                            case "%":
-                            case "%r":
-                            default:
-                                a = i
-                        }
-                        return z(a)[e] / 100 * r
-                    }
-                    if ("vh" === s || "vw" === s) {
-                        return ("vh" === s ? Math.max(document.documentElement.clientHeight, window.innerHeight || 0) : Math.max(document.documentElement.clientWidth, window.innerWidth || 0)) / 100 * r
-                    }
-                    return r
-                }(t, o, e, n)
-            }))
-        }))).forEach((function(t, e) {
-            t.forEach((function(n, i) {
-                gt(n) && (o[e] += n * ("-" === t[i - 1] ? -1 : 1))
-            }))
-        })), o
-    }
-    var Nt = {
-            placement: "bottom",
-            positionFixed: !1,
-            eventsEnabled: !0,
-            removeOnDestroy: !1,
-            onCreate: function() {},
-            onUpdate: function() {},
-            modifiers: {
-                shift: {
-                    order: 100,
-                    enabled: !0,
-                    fn: function(t) {
-                        var e = t.placement,
-                            n = e.split("-")[0],
-                            i = e.split("-")[1];
-                        if (i) {
-                            var o = t.offsets,
-                                r = o.reference,
-                                s = o.popper,
-                                a = -1 !== ["bottom", "top"].indexOf(n),
-                                l = a ? "left" : "top",
-                                c = a ? "width" : "height",
-                                h = {
-                                    start: V({}, l, r[l]),
-                                    end: V({}, l, r[l] + r[c] - s[c])
-                                };
-                            t.offsets.popper = Y({}, s, h[i])
-                        }
-                        return t
-                    }
-                },
-                offset: {
-                    order: 200,
-                    enabled: !0,
-                    fn: function(t, e) {
-                        var n = e.offset,
-                            i = t.placement,
-                            o = t.offsets,
-                            r = o.popper,
-                            s = o.reference,
-                            a = i.split("-")[0],
-                            l = void 0;
-                        return l = gt(+n) ? [+n, 0] : Dt(n, r, s, a), "left" === a ? (r.top += l[0], r.left -= l[1]) : "right" === a ? (r.top += l[0], r.left += l[1]) : "top" === a ? (r.left += l[0], r.top -= l[1]) : "bottom" === a && (r.left += l[0], r.top += l[1]), t.popper = r, t
+    function We(t) {
+        void 0 === t && (t = {});
+        var e = t,
+            i = e.defaultModifiers,
+            n = void 0 === i ? [] : i,
+            s = e.defaultOptions,
+            o = void 0 === s ? Be : s;
+        return function(t, e, i) {
+            void 0 === i && (i = o);
+            var s, r, a = {
+                    placement: "bottom",
+                    orderedModifiers: [],
+                    options: Object.assign({}, Be, o),
+                    modifiersData: {},
+                    elements: {
+                        reference: t,
+                        popper: e
                     },
-                    offset: 0
+                    attributes: {},
+                    styles: {}
                 },
-                preventOverflow: {
-                    order: 300,
-                    enabled: !0,
-                    fn: function(t, e) {
-                        var n = e.boundariesElement || P(t.instance.popper);
-                        t.instance.reference === n && (n = P(n));
-                        var i = ht("transform"),
-                            o = t.instance.popper.style,
-                            r = o.top,
-                            s = o.left,
-                            a = o[i];
-                        o.top = "", o.left = "", o[i] = "";
-                        var l = Z(t.instance.popper, t.instance.reference, e.padding, n, t.positionFixed);
-                        o.top = r, o.left = s, o[i] = a, e.boundaries = l;
-                        var c = e.priority,
-                            h = t.offsets.popper,
-                            u = {
-                                primary: function(t) {
-                                    var n = h[t];
-                                    return h[t] < l[t] && !e.escapeWithReference && (n = Math.max(h[t], l[t])), V({}, t, n)
-                                },
-                                secondary: function(t) {
-                                    var n = "right" === t ? "left" : "top",
-                                        i = h[n];
-                                    return h[t] > l[t] && !e.escapeWithReference && (i = Math.min(h[n], l[t] - ("right" === t ? h.width : h.height))), V({}, n, i)
-                                }
-                            };
-                        return c.forEach((function(t) {
-                            var e = -1 !== ["left", "top"].indexOf(t) ? "primary" : "secondary";
-                            h = Y({}, h, u[e](t))
-                        })), t.offsets.popper = h, t
-                    },
-                    priority: ["left", "right", "top", "bottom"],
-                    padding: 5,
-                    boundariesElement: "scrollParent"
-                },
-                keepTogether: {
-                    order: 400,
-                    enabled: !0,
-                    fn: function(t) {
-                        var e = t.offsets,
-                            n = e.popper,
-                            i = e.reference,
-                            o = t.placement.split("-")[0],
-                            r = Math.floor,
-                            s = -1 !== ["top", "bottom"].indexOf(o),
-                            a = s ? "right" : "bottom",
-                            l = s ? "left" : "top",
-                            c = s ? "width" : "height";
-                        return n[a] < r(i[l]) && (t.offsets.popper[l] = r(i[l]) - n[c]), n[l] > r(i[a]) && (t.offsets.popper[l] = r(i[a])), t
-                    }
-                },
-                arrow: {
-                    order: 500,
-                    enabled: !0,
-                    fn: function(t, e) {
-                        var n;
-                        if (!bt(t.instance.modifiers, "arrow", "keepTogether")) return t;
-                        var i = e.element;
-                        if ("string" == typeof i) {
-                            if (!(i = t.instance.popper.querySelector(i))) return t
-                        } else if (!t.instance.popper.contains(i)) return console.warn("WARNING: `arrow.element` must be child of its popper element!"), t;
-                        var o = t.placement.split("-")[0],
-                            r = t.offsets,
-                            s = r.popper,
-                            a = r.reference,
-                            l = -1 !== ["left", "right"].indexOf(o),
-                            c = l ? "height" : "width",
-                            h = l ? "Top" : "Left",
-                            u = h.toLowerCase(),
-                            f = l ? "left" : "top",
-                            d = l ? "bottom" : "right",
-                            p = it(i)[c];
-                        a[d] - p < s[u] && (t.offsets.popper[u] -= s[u] - (a[d] - p)), a[u] + p > s[d] && (t.offsets.popper[u] += a[u] + p - s[d]), t.offsets.popper = z(t.offsets.popper);
-                        var m = a[u] + a[c] / 2 - p / 2,
-                            g = k(t.instance.popper),
-                            _ = parseFloat(g["margin" + h]),
-                            v = parseFloat(g["border" + h + "Width"]),
-                            b = m - t.offsets.popper[u] - _ - v;
-                        return b = Math.max(Math.min(s[c] - p, b), 0), t.arrowElement = i, t.offsets.arrow = (V(n = {}, u, Math.round(b)), V(n, f, ""), n), t
+                l = [],
+                c = !1,
+                h = {
+                    state: a,
+                    setOptions: function(i) {
+                        var s = "function" == typeof i ? i(a.options) : i;
+                        d(), a.options = Object.assign({}, o, a.options, s), a.scrollParents = {
+                            reference: $t(t) ? Ae(t) : t.contextElement ? Ae(t.contextElement) : [],
+                            popper: Ae(e)
+                        };
+                        var r, c, u = function(t) {
+                            var e = He(t);
+                            return Bt.reduce((function(t, i) {
+                                return t.concat(e.filter((function(t) {
+                                    return t.phase === i
+                                })))
+                            }), [])
+                        }((r = [].concat(n, a.options.modifiers), c = r.reduce((function(t, e) {
+                            var i = t[e.name];
+                            return t[e.name] = i ? Object.assign({}, i, e, {
+                                options: Object.assign({}, i.options, e.options),
+                                data: Object.assign({}, i.data, e.data)
+                            }) : e, t
+                        }), {}), Object.keys(c).map((function(t) {
+                            return c[t]
+                        }))));
+                        return a.orderedModifiers = u.filter((function(t) {
+                            return t.enabled
+                        })), a.orderedModifiers.forEach((function(t) {
+                            var e = t.name,
+                                i = t.options,
+                                n = void 0 === i ? {} : i,
+                                s = t.effect;
+                            if ("function" == typeof s) {
+                                var o = s({
+                                    state: a,
+                                    name: e,
+                                    instance: h,
+                                    options: n
+                                });
+                                l.push(o || function() {})
+                            }
+                        })), h.update()
                     },
-                    element: "[x-arrow]"
-                },
-                flip: {
-                    order: 600,
-                    enabled: !0,
-                    fn: function(t, e) {
-                        if (ct(t.instance.modifiers, "inner")) return t;
-                        if (t.flipped && t.placement === t.originalPlacement) return t;
-                        var n = Z(t.instance.popper, t.instance.reference, e.padding, e.boundariesElement, t.positionFixed),
-                            i = t.placement.split("-")[0],
-                            o = ot(i),
-                            r = t.placement.split("-")[1] || "",
-                            s = [];
-                        switch (e.behavior) {
-                            case Tt:
-                                s = [i, o];
-                                break;
-                            case Ct:
-                                s = Et(i);
-                                break;
-                            case St:
-                                s = Et(i, !0);
-                                break;
-                            default:
-                                s = e.behavior
+                    forceUpdate: function() {
+                        if (!c) {
+                            var t = a.elements,
+                                e = t.reference,
+                                i = t.popper;
+                            if (Re(e, i)) {
+                                a.rects = {
+                                    reference: Me(e, te(i), "fixed" === a.options.strategy),
+                                    popper: Kt(i)
+                                }, a.reset = !1, a.placement = a.options.placement, a.orderedModifiers.forEach((function(t) {
+                                    return a.modifiersData[t.name] = Object.assign({}, t.data)
+                                }));
+                                for (var n = 0; n < a.orderedModifiers.length; n++)
+                                    if (!0 !== a.reset) {
+                                        var s = a.orderedModifiers[n],
+                                            o = s.fn,
+                                            r = s.options,
+                                            l = void 0 === r ? {} : r,
+                                            d = s.name;
+                                        "function" == typeof o && (a = o({
+                                            state: a,
+                                            options: l,
+                                            name: d,
+                                            instance: h
+                                        }) || a)
+                                    } else a.reset = !1, n = -1
+                            }
                         }
-                        return s.forEach((function(a, l) {
-                            if (i !== a || s.length === l + 1) return t;
-                            i = t.placement.split("-")[0], o = ot(i);
-                            var c = t.offsets.popper,
-                                h = t.offsets.reference,
-                                u = Math.floor,
-                                f = "left" === i && u(c.right) > u(h.left) || "right" === i && u(c.left) < u(h.right) || "top" === i && u(c.bottom) > u(h.top) || "bottom" === i && u(c.top) < u(h.bottom),
-                                d = u(c.left) < u(n.left),
-                                p = u(c.right) > u(n.right),
-                                m = u(c.top) < u(n.top),
-                                g = u(c.bottom) > u(n.bottom),
-                                _ = "left" === i && d || "right" === i && p || "top" === i && m || "bottom" === i && g,
-                                v = -1 !== ["top", "bottom"].indexOf(i),
-                                b = !!e.flipVariations && (v && "start" === r && d || v && "end" === r && p || !v && "start" === r && m || !v && "end" === r && g),
-                                y = !!e.flipVariationsByContent && (v && "start" === r && p || v && "end" === r && d || !v && "start" === r && g || !v && "end" === r && m),
-                                w = b || y;
-                            (f || _ || w) && (t.flipped = !0, (f || _) && (i = s[l + 1]), w && (r = function(t) {
-                                return "end" === t ? "start" : "start" === t ? "end" : t
-                            }(r)), t.placement = i + (r ? "-" + r : ""), t.offsets.popper = Y({}, t.offsets.popper, rt(t.instance.popper, t.offsets.reference, t.placement)), t = at(t.instance.modifiers, t, "flip"))
-                        })), t
                     },
-                    behavior: "flip",
-                    padding: 5,
-                    boundariesElement: "viewport",
-                    flipVariations: !1,
-                    flipVariationsByContent: !1
-                },
-                inner: {
-                    order: 700,
-                    enabled: !1,
-                    fn: function(t) {
-                        var e = t.placement,
-                            n = e.split("-")[0],
-                            i = t.offsets,
-                            o = i.popper,
-                            r = i.reference,
-                            s = -1 !== ["left", "right"].indexOf(n),
-                            a = -1 === ["top", "left"].indexOf(n);
-                        return o[s ? "left" : "top"] = r[n] - (a ? o[s ? "width" : "height"] : 0), t.placement = ot(e), t.offsets.popper = z(o), t
-                    }
-                },
-                hide: {
-                    order: 800,
-                    enabled: !0,
-                    fn: function(t) {
-                        if (!bt(t.instance.modifiers, "hide", "preventOverflow")) return t;
-                        var e = t.offsets.reference,
-                            n = st(t.instance.modifiers, (function(t) {
-                                return "preventOverflow" === t.name
-                            })).boundaries;
-                        if (e.bottom < n.top || e.left > n.right || e.top > n.bottom || e.right < n.left) {
-                            if (!0 === t.hide) return t;
-                            t.hide = !0, t.attributes["x-out-of-boundaries"] = ""
-                        } else {
-                            if (!1 === t.hide) return t;
-                            t.hide = !1, t.attributes["x-out-of-boundaries"] = !1
-                        }
-                        return t
+                    update: (s = function() {
+                        return new Promise((function(t) {
+                            h.forceUpdate(), t(a)
+                        }))
+                    }, function() {
+                        return r || (r = new Promise((function(t) {
+                            Promise.resolve().then((function() {
+                                r = void 0, t(s())
+                            }))
+                        }))), r
+                    }),
+                    destroy: function() {
+                        d(), c = !0
                     }
-                },
-                computeStyle: {
-                    order: 850,
-                    enabled: !0,
-                    fn: function(t, e) {
-                        var n = e.x,
-                            i = e.y,
-                            o = t.offsets.popper,
-                            r = st(t.instance.modifiers, (function(t) {
-                                return "applyStyle" === t.name
-                            })).gpuAcceleration;
-                        void 0 !== r && console.warn("WARNING: `gpuAcceleration` option moved to `computeStyle` modifier and will not be supported in future versions of Popper.js!");
-                        var s = void 0 !== r ? r : e.gpuAcceleration,
-                            a = P(t.instance.popper),
-                            l = X(a),
-                            c = {
-                                position: o.position
-                            },
-                            h = function(t, e) {
-                                var n = t.offsets,
-                                    i = n.popper,
-                                    o = n.reference,
-                                    r = Math.round,
-                                    s = Math.floor,
-                                    a = function(t) {
-                                        return t
-                                    },
-                                    l = r(o.width),
-                                    c = r(i.width),
-                                    h = -1 !== ["left", "right"].indexOf(t.placement),
-                                    u = -1 !== t.placement.indexOf("-"),
-                                    f = e ? h || u || l % 2 == c % 2 ? r : s : a,
-                                    d = e ? r : a;
-                                return {
-                                    left: f(l % 2 == 1 && c % 2 == 1 && !u && e ? i.left - 1 : i.left),
-                                    top: d(i.top),
-                                    bottom: d(i.bottom),
-                                    right: f(i.right)
-                                }
-                            }(t, window.devicePixelRatio < 2 || !vt),
-                            u = "bottom" === n ? "top" : "bottom",
-                            f = "right" === i ? "left" : "right",
-                            d = ht("transform"),
-                            p = void 0,
-                            m = void 0;
-                        if (m = "bottom" === u ? "HTML" === a.nodeName ? -a.clientHeight + h.bottom : -l.height + h.bottom : h.top, p = "right" === f ? "HTML" === a.nodeName ? -a.clientWidth + h.right : -l.width + h.right : h.left, s && d) c[d] = "translate3d(" + p + "px, " + m + "px, 0)", c[u] = 0, c[f] = 0, c.willChange = "transform";
-                        else {
-                            var g = "bottom" === u ? -1 : 1,
-                                _ = "right" === f ? -1 : 1;
-                            c[u] = m * g, c[f] = p * _, c.willChange = u + ", " + f
-                        }
-                        var v = {
-                            "x-placement": t.placement
-                        };
-                        return t.attributes = Y({}, v, t.attributes), t.styles = Y({}, c, t.styles), t.arrowStyles = Y({}, t.offsets.arrow, t.arrowStyles), t
-                    },
-                    gpuAcceleration: !0,
-                    x: "bottom",
-                    y: "right"
-                },
-                applyStyle: {
-                    order: 900,
-                    enabled: !0,
-                    fn: function(t) {
-                        var e, n;
-                        return _t(t.instance.popper, t.styles), e = t.instance.popper, n = t.attributes, Object.keys(n).forEach((function(t) {
-                            !1 !== n[t] ? e.setAttribute(t, n[t]) : e.removeAttribute(t)
-                        })), t.arrowElement && Object.keys(t.arrowStyles).length && _t(t.arrowElement, t.arrowStyles), t
-                    },
-                    onLoad: function(t, e, n, i, o) {
-                        var r = nt(o, e, t, n.positionFixed),
-                            s = et(n.placement, r, e, t, n.modifiers.flip.boundariesElement, n.modifiers.flip.padding);
-                        return e.setAttribute("x-placement", s), _t(e, {
-                            position: n.positionFixed ? "fixed" : "absolute"
-                        }), n
-                    },
-                    gpuAcceleration: void 0
-                }
-            }
-        },
-        kt = function() {
-            function t(e, n) {
-                var i = this,
-                    o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-                W(this, t), this.scheduleUpdate = function() {
-                    return requestAnimationFrame(i.update)
-                }, this.update = D(this.update.bind(this)), this.options = Y({}, t.Defaults, o), this.state = {
-                    isDestroyed: !1,
-                    isCreated: !1,
-                    scrollParents: []
-                }, this.reference = e && e.jquery ? e[0] : e, this.popper = n && n.jquery ? n[0] : n, this.options.modifiers = {}, Object.keys(Y({}, t.Defaults.modifiers, o.modifiers)).forEach((function(e) {
-                    i.options.modifiers[e] = Y({}, t.Defaults.modifiers[e] || {}, o.modifiers ? o.modifiers[e] : {})
-                })), this.modifiers = Object.keys(this.options.modifiers).map((function(t) {
-                    return Y({
-                        name: t
-                    }, i.options.modifiers[t])
-                })).sort((function(t, e) {
-                    return t.order - e.order
-                })), this.modifiers.forEach((function(t) {
-                    t.enabled && N(t.onLoad) && t.onLoad(i.reference, i.popper, i.options, t, i.state)
-                })), this.update();
-                var r = this.options.eventsEnabled;
-                r && this.enableEventListeners(), this.state.eventsEnabled = r
-            }
-            return U(t, [{
-                key: "update",
-                value: function() {
-                    return lt.call(this)
-                }
-            }, {
-                key: "destroy",
-                value: function() {
-                    return ut.call(this)
-                }
-            }, {
-                key: "enableEventListeners",
-                value: function() {
-                    return pt.call(this)
-                }
-            }, {
-                key: "disableEventListeners",
-                value: function() {
-                    return mt.call(this)
-                }
-            }]), t
-        }();
-    kt.Utils = ("undefined" != typeof window ? window : global).PopperUtils, kt.placements = yt, kt.Defaults = Nt;
-    var At = "dropdown",
-        It = e.fn[At],
-        Ot = new RegExp("38|40|27"),
-        xt = {
-            offset: 0,
-            flip: !0,
-            boundary: "scrollParent",
+                };
+            if (!Re(t, e)) return h;
+
+            function d() {
+                l.forEach((function(t) {
+                    return t()
+                })), l = []
+            }
+            return h.setOptions(i).then((function(t) {
+                !c && i.onFirstUpdate && i.onFirstUpdate(t)
+            })), h
+        }
+    }
+    var $e = We(),
+        ze = We({
+            defaultModifiers: [pe, Pe, ue, Ft]
+        }),
+        qe = We({
+            defaultModifiers: [pe, Pe, ue, Ft, Ie, xe, je, le, Ne]
+        });
+    const Fe = Object.freeze({
+            __proto__: null,
+            popperGenerator: We,
+            detectOverflow: ke,
+            createPopperBase: $e,
+            createPopper: qe,
+            createPopperLite: ze,
+            top: mt,
+            bottom: gt,
+            right: _t,
+            left: bt,
+            auto: vt,
+            basePlacements: yt,
+            start: wt,
+            end: Et,
+            clippingParents: At,
+            viewport: Tt,
+            popper: Ot,
+            reference: Ct,
+            variationPlacements: kt,
+            placements: Lt,
+            beforeRead: xt,
+            read: Dt,
+            afterRead: St,
+            beforeMain: Nt,
+            main: It,
+            afterMain: Pt,
+            beforeWrite: jt,
+            write: Mt,
+            afterWrite: Ht,
+            modifierPhases: Bt,
+            applyStyles: Ft,
+            arrow: le,
+            computeStyles: ue,
+            eventListeners: pe,
+            flip: xe,
+            hide: Ne,
+            offset: Ie,
+            popperOffsets: Pe,
+            preventOverflow: je
+        }),
+        Ue = "dropdown",
+        Ve = "Escape",
+        Ke = "Space",
+        Xe = "ArrowUp",
+        Ye = "ArrowDown",
+        Qe = new RegExp("ArrowUp|ArrowDown|Escape"),
+        Ge = "click.bs.dropdown.data-api",
+        Ze = "keydown.bs.dropdown.data-api",
+        Je = "show",
+        ti = '[data-bs-toggle="dropdown"]',
+        ei = ".dropdown-menu",
+        ii = m() ? "top-end" : "top-start",
+        ni = m() ? "top-start" : "top-end",
+        si = m() ? "bottom-end" : "bottom-start",
+        oi = m() ? "bottom-start" : "bottom-end",
+        ri = m() ? "left-start" : "right-start",
+        ai = m() ? "right-start" : "left-start",
+        li = {
+            offset: [0, 2],
+            boundary: "clippingParents",
             reference: "toggle",
             display: "dynamic",
-            popperConfig: null
+            popperConfig: null,
+            autoClose: !0
         },
-        jt = {
-            offset: "(number|string|function)",
-            flip: "boolean",
+        ci = {
+            offset: "(array|string|function)",
             boundary: "(string|element)",
-            reference: "(string|element)",
+            reference: "(string|element|object)",
             display: "string",
-            popperConfig: "(null|object)"
-        },
-        Lt = function() {
-            function t(t, e) {
-                this._element = t, this._popper = null, this._config = this._getConfig(e), this._menu = this._getMenuElement(), this._inNavbar = this._detectNavbar(), this._addEventListeners()
-            }
-            var n = t.prototype;
-            return n.toggle = function() {
-                if (!this._element.disabled && !e(this._element).hasClass("disabled")) {
-                    var n = e(this._menu).hasClass("show");
-                    t._clearMenus(), n || this.show(!0)
-                }
-            }, n.show = function(n) {
-                if (void 0 === n && (n = !1), !(this._element.disabled || e(this._element).hasClass("disabled") || e(this._menu).hasClass("show"))) {
-                    var i = {
-                            relatedTarget: this._element
-                        },
-                        o = e.Event("show.bs.dropdown", i),
-                        r = t._getParentFromElement(this._element);
-                    if (e(r).trigger(o), !o.isDefaultPrevented()) {
-                        if (!this._inNavbar && n) {
-                            if ("undefined" == typeof kt) throw new TypeError("Bootstrap's dropdowns require Popper.js (https://popper.js.org/)");
-                            var a = this._element;
-                            "parent" === this._config.reference ? a = r : s.isElement(this._config.reference) && (a = this._config.reference, "undefined" != typeof this._config.reference.jquery && (a = this._config.reference[0])), "scrollParent" !== this._config.boundary && e(r).addClass("position-static"), this._popper = new kt(a, this._menu, this._getPopperConfig())
-                        }
-                        "ontouchstart" in document.documentElement && 0 === e(r).closest(".navbar-nav").length && e(document.body).children().on("mouseover", null, e.noop), this._element.focus(), this._element.setAttribute("aria-expanded", !0), e(this._menu).toggleClass("show"), e(r).toggleClass("show").trigger(e.Event("shown.bs.dropdown", i))
+            popperConfig: "(null|object|function)",
+            autoClose: "(boolean|string)"
+        };
+    class hi extends B {
+        constructor(t, e) {
+            super(t), this._popper = null, this._config = this._getConfig(e), this._menu = this._getMenuElement(), this._inNavbar = this._detectNavbar()
+        }
+        static get Default() {
+            return li
+        }
+        static get DefaultType() {
+            return ci
+        }
+        static get NAME() {
+            return Ue
+        }
+        toggle() {
+            return this._isShown() ? this.hide() : this.show()
+        }
+        show() {
+            if (c(this._element) || this._isShown(this._menu)) return;
+            const t = {
+                relatedTarget: this._element
+            };
+            if (j.trigger(this._element, "show.bs.dropdown", t).defaultPrevented) return;
+            const e = hi.getParentFromElement(this._element);
+            this._inNavbar ? U.setDataAttribute(this._menu, "popper", "none") : this._createPopper(e), "ontouchstart" in document.documentElement && !e.closest(".navbar-nav") && [].concat(...document.body.children).forEach((t => j.on(t, "mouseover", d))), this._element.focus(), this._element.setAttribute("aria-expanded", !0), this._menu.classList.add(Je), this._element.classList.add(Je), j.trigger(this._element, "shown.bs.dropdown", t)
+        }
+        hide() {
+            if (c(this._element) || !this._isShown(this._menu)) return;
+            const t = {
+                relatedTarget: this._element
+            };
+            this._completeHide(t)
+        }
+        dispose() {
+            this._popper && this._popper.destroy(), super.dispose()
+        }
+        update() {
+            this._inNavbar = this._detectNavbar(), this._popper && this._popper.update()
+        }
+        _completeHide(t) {
+            j.trigger(this._element, "hide.bs.dropdown", t).defaultPrevented || ("ontouchstart" in document.documentElement && [].concat(...document.body.children).forEach((t => j.off(t, "mouseover", d))), this._popper && this._popper.destroy(), this._menu.classList.remove(Je), this._element.classList.remove(Je), this._element.setAttribute("aria-expanded", "false"), U.removeDataAttribute(this._menu, "popper"), j.trigger(this._element, "hidden.bs.dropdown", t))
+        }
+        _getConfig(t) {
+            if (t = {
+                    ...this.constructor.Default,
+                    ...U.getDataAttributes(this._element),
+                    ...t
+                }, a(Ue, t, this.constructor.DefaultType), "object" == typeof t.reference && !o(t.reference) && "function" != typeof t.reference.getBoundingClientRect) throw new TypeError(`${Ue.toUpperCase()}: Option "reference" provided type "object" without a required "getBoundingClientRect" method.`);
+            return t
+        }
+        _createPopper(t) {
+            if (void 0 === Fe) throw new TypeError("Bootstrap's dropdowns require Popper (https://popper.js.org)");
+            let e = this._element;
+            "parent" === this._config.reference ? e = t : o(this._config.reference) ? e = r(this._config.reference) : "object" == typeof this._config.reference && (e = this._config.reference);
+            const i = this._getPopperConfig(),
+                n = i.modifiers.find((t => "applyStyles" === t.name && !1 === t.enabled));
+            this._popper = qe(e, this._menu, i), n && U.setDataAttribute(this._menu, "popper", "static")
+        }
+        _isShown(t = this._element) {
+            return t.classList.contains(Je)
+        }
+        _getMenuElement() {
+            return V.next(this._element, ei)[0]
+        }
+        _getPlacement() {
+            const t = this._element.parentNode;
+            if (t.classList.contains("dropend")) return ri;
+            if (t.classList.contains("dropstart")) return ai;
+            const e = "end" === getComputedStyle(this._menu).getPropertyValue("--bs-position").trim();
+            return t.classList.contains("dropup") ? e ? ni : ii : e ? oi : si
+        }
+        _detectNavbar() {
+            return null !== this._element.closest(".navbar")
+        }
+        _getOffset() {
+            const {
+                offset: t
+            } = this._config;
+            return "string" == typeof t ? t.split(",").map((t => Number.parseInt(t, 10))) : "function" == typeof t ? e => t(e, this._element) : t
+        }
+        _getPopperConfig() {
+            const t = {
+                placement: this._getPlacement(),
+                modifiers: [{
+                    name: "preventOverflow",
+                    options: {
+                        boundary: this._config.boundary
+                    }
+                }, {
+                    name: "offset",
+                    options: {
+                        offset: this._getOffset()
                     }
+                }]
+            };
+            return "static" === this._config.display && (t.modifiers = [{
+                name: "applyStyles",
+                enabled: !1
+            }]), {
+                ...t,
+                ..."function" == typeof this._config.popperConfig ? this._config.popperConfig(t) : this._config.popperConfig
+            }
+        }
+        _selectMenuItem({
+            key: t,
+            target: e
+        }) {
+            const i = V.find(".dropdown-menu .dropdown-item:not(.disabled):not(:disabled)", this._menu).filter(l);
+            i.length && v(i, e, t === Ye, !i.includes(e)).focus()
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = hi.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    e[t]()
                 }
-            }, n.hide = function() {
-                if (!this._element.disabled && !e(this._element).hasClass("disabled") && e(this._menu).hasClass("show")) {
-                    var n = {
-                            relatedTarget: this._element
-                        },
-                        i = e.Event("hide.bs.dropdown", n),
-                        o = t._getParentFromElement(this._element);
-                    e(o).trigger(i), i.isDefaultPrevented() || (this._popper && this._popper.destroy(), e(this._menu).toggleClass("show"), e(o).toggleClass("show").trigger(e.Event("hidden.bs.dropdown", n)))
-                }
-            }, n.dispose = function() {
-                e.removeData(this._element, "bs.dropdown"), e(this._element).off(".bs.dropdown"), this._element = null, this._menu = null, null !== this._popper && (this._popper.destroy(), this._popper = null)
-            }, n.update = function() {
-                this._inNavbar = this._detectNavbar(), null !== this._popper && this._popper.scheduleUpdate()
-            }, n._addEventListeners = function() {
-                var t = this;
-                e(this._element).on("click.bs.dropdown", (function(e) {
-                    e.preventDefault(), e.stopPropagation(), t.toggle()
-                }))
-            }, n._getConfig = function(t) {
-                return t = o({}, this.constructor.Default, e(this._element).data(), t), s.typeCheckConfig(At, t, this.constructor.DefaultType), t
-            }, n._getMenuElement = function() {
-                if (!this._menu) {
-                    var e = t._getParentFromElement(this._element);
-                    e && (this._menu = e.querySelector(".dropdown-menu"))
-                }
-                return this._menu
-            }, n._getPlacement = function() {
-                var t = e(this._element.parentNode),
-                    n = "bottom-start";
-                return t.hasClass("dropup") ? n = e(this._menu).hasClass("dropdown-menu-right") ? "top-end" : "top-start" : t.hasClass("dropright") ? n = "right-start" : t.hasClass("dropleft") ? n = "left-start" : e(this._menu).hasClass("dropdown-menu-right") && (n = "bottom-end"), n
-            }, n._detectNavbar = function() {
-                return e(this._element).closest(".navbar").length > 0
-            }, n._getOffset = function() {
-                var t = this,
-                    e = {};
-                return "function" == typeof this._config.offset ? e.fn = function(e) {
-                    return e.offsets = o({}, e.offsets, t._config.offset(e.offsets, t._element) || {}), e
-                } : e.offset = this._config.offset, e
-            }, n._getPopperConfig = function() {
-                var t = {
-                    placement: this._getPlacement(),
-                    modifiers: {
-                        offset: this._getOffset(),
-                        flip: {
-                            enabled: this._config.flip
-                        },
-                        preventOverflow: {
-                            boundariesElement: this._config.boundary
-                        }
-                    }
+            }))
+        }
+        static clearMenus(t) {
+            if (t && (2 === t.button || "keyup" === t.type && "Tab" !== t.key)) return;
+            const e = V.find(ti);
+            for (let i = 0, n = e.length; i < n; i++) {
+                const n = hi.getInstance(e[i]);
+                if (!n || !1 === n._config.autoClose) continue;
+                if (!n._isShown()) continue;
+                const s = {
+                    relatedTarget: n._element
                 };
-                return "static" === this._config.display && (t.modifiers.applyStyle = {
-                    enabled: !1
-                }), o({}, t, this._config.popperConfig)
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this).data("bs.dropdown");
-                    if (i || (i = new t(this, "object" == typeof n ? n : null), e(this).data("bs.dropdown", i)), "string" == typeof n) {
-                        if ("undefined" == typeof i[n]) throw new TypeError('No method named "' + n + '"');
-                        i[n]()
-                    }
-                }))
-            }, t._clearMenus = function(n) {
-                if (!n || 3 !== n.which && ("keyup" !== n.type || 9 === n.which))
-                    for (var i = [].slice.call(document.querySelectorAll('[data-toggle="dropdown"]')), o = 0, r = i.length; o < r; o++) {
-                        var s = t._getParentFromElement(i[o]),
-                            a = e(i[o]).data("bs.dropdown"),
-                            l = {
-                                relatedTarget: i[o]
-                            };
-                        if (n && "click" === n.type && (l.clickEvent = n), a) {
-                            var c = a._menu;
-                            if (e(s).hasClass("show") && !(n && ("click" === n.type && /input|textarea/i.test(n.target.tagName) || "keyup" === n.type && 9 === n.which) && e.contains(s, n.target))) {
-                                var h = e.Event("hide.bs.dropdown", l);
-                                e(s).trigger(h), h.isDefaultPrevented() || ("ontouchstart" in document.documentElement && e(document.body).children().off("mouseover", null, e.noop), i[o].setAttribute("aria-expanded", "false"), a._popper && a._popper.destroy(), e(c).removeClass("show"), e(s).removeClass("show").trigger(e.Event("hidden.bs.dropdown", l)))
-                            }
-                        }
-                    }
-            }, t._getParentFromElement = function(t) {
-                var e, n = s.getSelectorFromElement(t);
-                return n && (e = document.querySelector(n)), e || t.parentNode
-            }, t._dataApiKeydownHandler = function(n) {
-                if (!(/input|textarea/i.test(n.target.tagName) ? 32 === n.which || 27 !== n.which && (40 !== n.which && 38 !== n.which || e(n.target).closest(".dropdown-menu").length) : !Ot.test(n.which)) && !this.disabled && !e(this).hasClass("disabled")) {
-                    var i = t._getParentFromElement(this),
-                        o = e(i).hasClass("show");
-                    if (o || 27 !== n.which) {
-                        if (n.preventDefault(), n.stopPropagation(), !o || o && (27 === n.which || 32 === n.which)) return 27 === n.which && e(i.querySelector('[data-toggle="dropdown"]')).trigger("focus"), void e(this).trigger("click");
-                        var r = [].slice.call(i.querySelectorAll(".dropdown-menu .dropdown-item:not(.disabled):not(:disabled)")).filter((function(t) {
-                            return e(t).is(":visible")
-                        }));
-                        if (0 !== r.length) {
-                            var s = r.indexOf(n.target);
-                            38 === n.which && s > 0 && s--, 40 === n.which && s < r.length - 1 && s++, s < 0 && (s = 0), r[s].focus()
-                        }
-                    }
+                if (t) {
+                    const e = t.composedPath(),
+                        i = e.includes(n._menu);
+                    if (e.includes(n._element) || "inside" === n._config.autoClose && !i || "outside" === n._config.autoClose && i) continue;
+                    if (n._menu.contains(t.target) && ("keyup" === t.type && "Tab" === t.key || /input|select|option|textarea|form/i.test(t.target.tagName))) continue;
+                    "click" === t.type && (s.clickEvent = t)
                 }
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return xt
-                }
-            }, {
-                key: "DefaultType",
-                get: function() {
-                    return jt
-                }
-            }]), t
-        }();
-    e(document).on("keydown.bs.dropdown.data-api", '[data-toggle="dropdown"]', Lt._dataApiKeydownHandler).on("keydown.bs.dropdown.data-api", ".dropdown-menu", Lt._dataApiKeydownHandler).on("click.bs.dropdown.data-api keyup.bs.dropdown.data-api", Lt._clearMenus).on("click.bs.dropdown.data-api", '[data-toggle="dropdown"]', (function(t) {
-        t.preventDefault(), t.stopPropagation(), Lt._jQueryInterface.call(e(this), "toggle")
-    })).on("click.bs.dropdown.data-api", ".dropdown form", (function(t) {
-        t.stopPropagation()
-    })), e.fn[At] = Lt._jQueryInterface, e.fn[At].Constructor = Lt, e.fn[At].noConflict = function() {
-        return e.fn[At] = It, Lt._jQueryInterface
-    };
-    var Pt = e.fn.modal,
-        Ft = {
+                n._completeHide(s)
+            }
+        }
+        static getParentFromElement(t) {
+            return n(t) || t.parentNode
+        }
+        static dataApiKeydownHandler(t) {
+            if (/input|textarea/i.test(t.target.tagName) ? t.key === Ke || t.key !== Ve && (t.key !== Ye && t.key !== Xe || t.target.closest(ei)) : !Qe.test(t.key)) return;
+            const e = this.classList.contains(Je);
+            if (!e && t.key === Ve) return;
+            if (t.preventDefault(), t.stopPropagation(), c(this)) return;
+            const i = this.matches(ti) ? this : V.prev(this, ti)[0],
+                n = hi.getOrCreateInstance(i);
+            if (t.key !== Ve) return t.key === Xe || t.key === Ye ? (e || n.show(), void n._selectMenuItem(t)) : void(e && t.key !== Ke || hi.clearMenus());
+            n.hide()
+        }
+    }
+    j.on(document, Ze, ti, hi.dataApiKeydownHandler), j.on(document, Ze, ei, hi.dataApiKeydownHandler), j.on(document, Ge, hi.clearMenus), j.on(document, "keyup.bs.dropdown.data-api", hi.clearMenus), j.on(document, Ge, ti, (function(t) {
+        t.preventDefault(), hi.getOrCreateInstance(this).toggle()
+    })), g(hi);
+    const di = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
+        ui = ".sticky-top";
+    class fi {
+        constructor() {
+            this._element = document.body
+        }
+        getWidth() {
+            const t = document.documentElement.clientWidth;
+            return Math.abs(window.innerWidth - t)
+        }
+        hide() {
+            const t = this.getWidth();
+            this._disableOverFlow(), this._setElementAttributes(this._element, "paddingRight", (e => e + t)), this._setElementAttributes(di, "paddingRight", (e => e + t)), this._setElementAttributes(ui, "marginRight", (e => e - t))
+        }
+        _disableOverFlow() {
+            this._saveInitialAttribute(this._element, "overflow"), this._element.style.overflow = "hidden"
+        }
+        _setElementAttributes(t, e, i) {
+            const n = this.getWidth();
+            this._applyManipulationCallback(t, (t => {
+                if (t !== this._element && window.innerWidth > t.clientWidth + n) return;
+                this._saveInitialAttribute(t, e);
+                const s = window.getComputedStyle(t)[e];
+                t.style[e] = `${i(Number.parseFloat(s))}px`
+            }))
+        }
+        reset() {
+            this._resetElementAttributes(this._element, "overflow"), this._resetElementAttributes(this._element, "paddingRight"), this._resetElementAttributes(di, "paddingRight"), this._resetElementAttributes(ui, "marginRight")
+        }
+        _saveInitialAttribute(t, e) {
+            const i = t.style[e];
+            i && U.setDataAttribute(t, e, i)
+        }
+        _resetElementAttributes(t, e) {
+            this._applyManipulationCallback(t, (t => {
+                const i = U.getDataAttribute(t, e);
+                void 0 === i ? t.style.removeProperty(e) : (U.removeDataAttribute(t, e), t.style[e] = i)
+            }))
+        }
+        _applyManipulationCallback(t, e) {
+            o(t) ? e(t) : V.find(t, this._element).forEach(e)
+        }
+        isOverflowing() {
+            return this.getWidth() > 0
+        }
+    }
+    const pi = {
+            className: "modal-backdrop",
+            isVisible: !0,
+            isAnimated: !1,
+            rootElement: "body",
+            clickCallback: null
+        },
+        mi = {
+            className: "string",
+            isVisible: "boolean",
+            isAnimated: "boolean",
+            rootElement: "(element|string)",
+            clickCallback: "(function|null)"
+        },
+        gi = "show",
+        _i = "mousedown.bs.backdrop";
+    class bi {
+        constructor(t) {
+            this._config = this._getConfig(t), this._isAppended = !1, this._element = null
+        }
+        show(t) {
+            this._config.isVisible ? (this._append(), this._config.isAnimated && u(this._getElement()), this._getElement().classList.add(gi), this._emulateAnimation((() => {
+                _(t)
+            }))) : _(t)
+        }
+        hide(t) {
+            this._config.isVisible ? (this._getElement().classList.remove(gi), this._emulateAnimation((() => {
+                this.dispose(), _(t)
+            }))) : _(t)
+        }
+        _getElement() {
+            if (!this._element) {
+                const t = document.createElement("div");
+                t.className = this._config.className, this._config.isAnimated && t.classList.add("fade"), this._element = t
+            }
+            return this._element
+        }
+        _getConfig(t) {
+            return (t = {
+                ...pi,
+                ..."object" == typeof t ? t : {}
+            }).rootElement = r(t.rootElement), a("backdrop", t, mi), t
+        }
+        _append() {
+            this._isAppended || (this._config.rootElement.append(this._getElement()), j.on(this._getElement(), _i, (() => {
+                _(this._config.clickCallback)
+            })), this._isAppended = !0)
+        }
+        dispose() {
+            this._isAppended && (j.off(this._element, _i), this._element.remove(), this._isAppended = !1)
+        }
+        _emulateAnimation(t) {
+            b(t, this._getElement(), this._config.isAnimated)
+        }
+    }
+    const vi = {
+            trapElement: null,
+            autofocus: !0
+        },
+        yi = {
+            trapElement: "element",
+            autofocus: "boolean"
+        },
+        wi = ".bs.focustrap",
+        Ei = "backward";
+    class Ai {
+        constructor(t) {
+            this._config = this._getConfig(t), this._isActive = !1, this._lastTabNavDirection = null
+        }
+        activate() {
+            const {
+                trapElement: t,
+                autofocus: e
+            } = this._config;
+            this._isActive || (e && t.focus(), j.off(document, wi), j.on(document, "focusin.bs.focustrap", (t => this._handleFocusin(t))), j.on(document, "keydown.tab.bs.focustrap", (t => this._handleKeydown(t))), this._isActive = !0)
+        }
+        deactivate() {
+            this._isActive && (this._isActive = !1, j.off(document, wi))
+        }
+        _handleFocusin(t) {
+            const {
+                target: e
+            } = t, {
+                trapElement: i
+            } = this._config;
+            if (e === document || e === i || i.contains(e)) return;
+            const n = V.focusableChildren(i);
+            0 === n.length ? i.focus() : this._lastTabNavDirection === Ei ? n[n.length - 1].focus() : n[0].focus()
+        }
+        _handleKeydown(t) {
+            "Tab" === t.key && (this._lastTabNavDirection = t.shiftKey ? Ei : "forward")
+        }
+        _getConfig(t) {
+            return t = {
+                ...vi,
+                ..."object" == typeof t ? t : {}
+            }, a("focustrap", t, yi), t
+        }
+    }
+    const Ti = "modal",
+        Oi = "Escape",
+        Ci = {
             backdrop: !0,
             keyboard: !0,
-            focus: !0,
-            show: !0
+            focus: !0
         },
-        Rt = {
+        ki = {
             backdrop: "(boolean|string)",
             keyboard: "boolean",
-            focus: "boolean",
-            show: "boolean"
+            focus: "boolean"
         },
-        Ht = function() {
-            function t(t, e) {
-                this._config = this._getConfig(e), this._element = t, this._dialog = t.querySelector(".modal-dialog"), this._backdrop = null, this._isShown = !1, this._isBodyOverflowing = !1, this._ignoreBackdropClick = !1, this._isTransitioning = !1, this._scrollbarWidth = 0
-            }
-            var n = t.prototype;
-            return n.toggle = function(t) {
-                return this._isShown ? this.hide() : this.show(t)
-            }, n.show = function(t) {
-                var n = this;
-                if (!this._isShown && !this._isTransitioning) {
-                    e(this._element).hasClass("fade") && (this._isTransitioning = !0);
-                    var i = e.Event("show.bs.modal", {
-                        relatedTarget: t
-                    });
-                    e(this._element).trigger(i), this._isShown || i.isDefaultPrevented() || (this._isShown = !0, this._checkScrollbar(), this._setScrollbar(), this._adjustDialog(), this._setEscapeEvent(), this._setResizeEvent(), e(this._element).on("click.dismiss.bs.modal", '[data-dismiss="modal"]', (function(t) {
-                        return n.hide(t)
-                    })), e(this._dialog).on("mousedown.dismiss.bs.modal", (function() {
-                        e(n._element).one("mouseup.dismiss.bs.modal", (function(t) {
-                            e(t.target).is(n._element) && (n._ignoreBackdropClick = !0)
-                        }))
-                    })), this._showBackdrop((function() {
-                        return n._showElement(t)
-                    })))
-                }
-            }, n.hide = function(t) {
-                var n = this;
-                if (t && t.preventDefault(), this._isShown && !this._isTransitioning) {
-                    var i = e.Event("hide.bs.modal");
-                    if (e(this._element).trigger(i), this._isShown && !i.isDefaultPrevented()) {
-                        this._isShown = !1;
-                        var o = e(this._element).hasClass("fade");
-                        if (o && (this._isTransitioning = !0), this._setEscapeEvent(), this._setResizeEvent(), e(document).off("focusin.bs.modal"), e(this._element).removeClass("show"), e(this._element).off("click.dismiss.bs.modal"), e(this._dialog).off("mousedown.dismiss.bs.modal"), o) {
-                            var r = s.getTransitionDurationFromElement(this._element);
-                            e(this._element).one(s.TRANSITION_END, (function(t) {
-                                return n._hideModal(t)
-                            })).emulateTransitionEnd(r)
-                        } else this._hideModal()
-                    }
-                }
-            }, n.dispose = function() {
-                [window, this._element, this._dialog].forEach((function(t) {
-                    return e(t).off(".bs.modal")
-                })), e(document).off("focusin.bs.modal"), e.removeData(this._element, "bs.modal"), this._config = null, this._element = null, this._dialog = null, this._backdrop = null, this._isShown = null, this._isBodyOverflowing = null, this._ignoreBackdropClick = null, this._isTransitioning = null, this._scrollbarWidth = null
-            }, n.handleUpdate = function() {
-                this._adjustDialog()
-            }, n._getConfig = function(t) {
-                return t = o({}, Ft, t), s.typeCheckConfig("modal", t, Rt), t
-            }, n._triggerBackdropTransition = function() {
-                var t = this;
-                if ("static" === this._config.backdrop) {
-                    var n = e.Event("hidePrevented.bs.modal");
-                    if (e(this._element).trigger(n), n.defaultPrevented) return;
-                    var i = this._element.scrollHeight > document.documentElement.clientHeight;
-                    i || (this._element.style.overflowY = "hidden"), this._element.classList.add("modal-static");
-                    var o = s.getTransitionDurationFromElement(this._dialog);
-                    e(this._element).off(s.TRANSITION_END), e(this._element).one(s.TRANSITION_END, (function() {
-                        t._element.classList.remove("modal-static"), i || e(t._element).one(s.TRANSITION_END, (function() {
-                            t._element.style.overflowY = ""
-                        })).emulateTransitionEnd(t._element, o)
-                    })).emulateTransitionEnd(o), this._element.focus()
-                } else this.hide()
-            }, n._showElement = function(t) {
-                var n = this,
-                    i = e(this._element).hasClass("fade"),
-                    o = this._dialog ? this._dialog.querySelector(".modal-body") : null;
-                this._element.parentNode && this._element.parentNode.nodeType === Node.ELEMENT_NODE || document.body.appendChild(this._element), this._element.style.display = "block", this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), e(this._dialog).hasClass("modal-dialog-scrollable") && o ? o.scrollTop = 0 : this._element.scrollTop = 0, i && s.reflow(this._element), e(this._element).addClass("show"), this._config.focus && this._enforceFocus();
-                var r = e.Event("shown.bs.modal", {
-                        relatedTarget: t
-                    }),
-                    a = function() {
-                        n._config.focus && n._element.focus(), n._isTransitioning = !1, e(n._element).trigger(r)
-                    };
-                if (i) {
-                    var l = s.getTransitionDurationFromElement(this._dialog);
-                    e(this._dialog).one(s.TRANSITION_END, a).emulateTransitionEnd(l)
-                } else a()
-            }, n._enforceFocus = function() {
-                var t = this;
-                e(document).off("focusin.bs.modal").on("focusin.bs.modal", (function(n) {
-                    document !== n.target && t._element !== n.target && 0 === e(t._element).has(n.target).length && t._element.focus()
-                }))
-            }, n._setEscapeEvent = function() {
-                var t = this;
-                this._isShown ? e(this._element).on("keydown.dismiss.bs.modal", (function(e) {
-                    t._config.keyboard && 27 === e.which ? (e.preventDefault(), t.hide()) : t._config.keyboard || 27 !== e.which || t._triggerBackdropTransition()
-                })) : this._isShown || e(this._element).off("keydown.dismiss.bs.modal")
-            }, n._setResizeEvent = function() {
-                var t = this;
-                this._isShown ? e(window).on("resize.bs.modal", (function(e) {
-                    return t.handleUpdate(e)
-                })) : e(window).off("resize.bs.modal")
-            }, n._hideModal = function() {
-                var t = this;
-                this._element.style.display = "none", this._element.setAttribute("aria-hidden", !0), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._isTransitioning = !1, this._showBackdrop((function() {
-                    e(document.body).removeClass("modal-open"), t._resetAdjustments(), t._resetScrollbar(), e(t._element).trigger("hidden.bs.modal")
-                }))
-            }, n._removeBackdrop = function() {
-                this._backdrop && (e(this._backdrop).remove(), this._backdrop = null)
-            }, n._showBackdrop = function(t) {
-                var n = this,
-                    i = e(this._element).hasClass("fade") ? "fade" : "";
-                if (this._isShown && this._config.backdrop) {
-                    if (this._backdrop = document.createElement("div"), this._backdrop.className = "modal-backdrop", i && this._backdrop.classList.add(i), e(this._backdrop).appendTo(document.body), e(this._element).on("click.dismiss.bs.modal", (function(t) {
-                            n._ignoreBackdropClick ? n._ignoreBackdropClick = !1 : t.target === t.currentTarget && n._triggerBackdropTransition()
-                        })), i && s.reflow(this._backdrop), e(this._backdrop).addClass("show"), !t) return;
-                    if (!i) return void t();
-                    var o = s.getTransitionDurationFromElement(this._backdrop);
-                    e(this._backdrop).one(s.TRANSITION_END, t).emulateTransitionEnd(o)
-                } else if (!this._isShown && this._backdrop) {
-                    e(this._backdrop).removeClass("show");
-                    var r = function() {
-                        n._removeBackdrop(), t && t()
-                    };
-                    if (e(this._element).hasClass("fade")) {
-                        var a = s.getTransitionDurationFromElement(this._backdrop);
-                        e(this._backdrop).one(s.TRANSITION_END, r).emulateTransitionEnd(a)
-                    } else r()
-                } else t && t()
-            }, n._adjustDialog = function() {
-                var t = this._element.scrollHeight > document.documentElement.clientHeight;
-                !this._isBodyOverflowing && t && (this._element.style.paddingLeft = this._scrollbarWidth + "px"), this._isBodyOverflowing && !t && (this._element.style.paddingRight = this._scrollbarWidth + "px")
-            }, n._resetAdjustments = function() {
-                this._element.style.paddingLeft = "", this._element.style.paddingRight = ""
-            }, n._checkScrollbar = function() {
-                var t = document.body.getBoundingClientRect();
-                this._isBodyOverflowing = Math.round(t.left + t.right) < window.innerWidth, this._scrollbarWidth = this._getScrollbarWidth()
-            }, n._setScrollbar = function() {
-                var t = this;
-                if (this._isBodyOverflowing) {
-                    var n = [].slice.call(document.querySelectorAll(".fixed-top, .fixed-bottom, .is-fixed, .sticky-top")),
-                        i = [].slice.call(document.querySelectorAll(".sticky-top"));
-                    e(n).each((function(n, i) {
-                        var o = i.style.paddingRight,
-                            r = e(i).css("padding-right");
-                        e(i).data("padding-right", o).css("padding-right", parseFloat(r) + t._scrollbarWidth + "px")
-                    })), e(i).each((function(n, i) {
-                        var o = i.style.marginRight,
-                            r = e(i).css("margin-right");
-                        e(i).data("margin-right", o).css("margin-right", parseFloat(r) - t._scrollbarWidth + "px")
-                    }));
-                    var o = document.body.style.paddingRight,
-                        r = e(document.body).css("padding-right");
-                    e(document.body).data("padding-right", o).css("padding-right", parseFloat(r) + this._scrollbarWidth + "px")
-                }
-                e(document.body).addClass("modal-open")
-            }, n._resetScrollbar = function() {
-                var t = [].slice.call(document.querySelectorAll(".fixed-top, .fixed-bottom, .is-fixed, .sticky-top"));
-                e(t).each((function(t, n) {
-                    var i = e(n).data("padding-right");
-                    e(n).removeData("padding-right"), n.style.paddingRight = i || ""
-                }));
-                var n = [].slice.call(document.querySelectorAll(".sticky-top"));
-                e(n).each((function(t, n) {
-                    var i = e(n).data("margin-right");
-                    "undefined" != typeof i && e(n).css("margin-right", i).removeData("margin-right")
-                }));
-                var i = e(document.body).data("padding-right");
-                e(document.body).removeData("padding-right"), document.body.style.paddingRight = i || ""
-            }, n._getScrollbarWidth = function() {
-                var t = document.createElement("div");
-                t.className = "modal-scrollbar-measure", document.body.appendChild(t);
-                var e = t.getBoundingClientRect().width - t.clientWidth;
-                return document.body.removeChild(t), e
-            }, t._jQueryInterface = function(n, i) {
-                return this.each((function() {
-                    var r = e(this).data("bs.modal"),
-                        s = o({}, Ft, e(this).data(), "object" == typeof n && n ? n : {});
-                    if (r || (r = new t(this, s), e(this).data("bs.modal", r)), "string" == typeof n) {
-                        if ("undefined" == typeof r[n]) throw new TypeError('No method named "' + n + '"');
-                        r[n](i)
-                    } else s.show && r.show(i)
+        Li = "hidden.bs.modal",
+        xi = "show.bs.modal",
+        Di = "resize.bs.modal",
+        Si = "click.dismiss.bs.modal",
+        Ni = "keydown.dismiss.bs.modal",
+        Ii = "mousedown.dismiss.bs.modal",
+        Pi = "modal-open",
+        ji = "show",
+        Mi = "modal-static";
+    class Hi extends B {
+        constructor(t, e) {
+            super(t), this._config = this._getConfig(e), this._dialog = V.findOne(".modal-dialog", this._element), this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._isShown = !1, this._ignoreBackdropClick = !1, this._isTransitioning = !1, this._scrollBar = new fi
+        }
+        static get Default() {
+            return Ci
+        }
+        static get NAME() {
+            return Ti
+        }
+        toggle(t) {
+            return this._isShown ? this.hide() : this.show(t)
+        }
+        show(t) {
+            this._isShown || this._isTransitioning || j.trigger(this._element, xi, {
+                relatedTarget: t
+            }).defaultPrevented || (this._isShown = !0, this._isAnimated() && (this._isTransitioning = !0), this._scrollBar.hide(), document.body.classList.add(Pi), this._adjustDialog(), this._setEscapeEvent(), this._setResizeEvent(), j.on(this._dialog, Ii, (() => {
+                j.one(this._element, "mouseup.dismiss.bs.modal", (t => {
+                    t.target === this._element && (this._ignoreBackdropClick = !0)
                 }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return Ft
-                }
-            }]), t
-        }();
-    e(document).on("click.bs.modal.data-api", '[data-toggle="modal"]', (function(t) {
-        var n, i = this,
-            r = s.getSelectorFromElement(this);
-        r && (n = document.querySelector(r));
-        var a = e(n).data("bs.modal") ? "toggle" : o({}, e(n).data(), e(this).data());
-        "A" !== this.tagName && "AREA" !== this.tagName || t.preventDefault();
-        var l = e(n).one("show.bs.modal", (function(t) {
-            t.isDefaultPrevented() || l.one("hidden.bs.modal", (function() {
-                e(i).is(":visible") && i.focus()
+            })), this._showBackdrop((() => this._showElement(t))))
+        }
+        hide() {
+            if (!this._isShown || this._isTransitioning) return;
+            if (j.trigger(this._element, "hide.bs.modal").defaultPrevented) return;
+            this._isShown = !1;
+            const t = this._isAnimated();
+            t && (this._isTransitioning = !0), this._setEscapeEvent(), this._setResizeEvent(), this._focustrap.deactivate(), this._element.classList.remove(ji), j.off(this._element, Si), j.off(this._dialog, Ii), this._queueCallback((() => this._hideModal()), this._element, t)
+        }
+        dispose() {
+            [window, this._dialog].forEach((t => j.off(t, ".bs.modal"))), this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
+        }
+        handleUpdate() {
+            this._adjustDialog()
+        }
+        _initializeBackDrop() {
+            return new bi({
+                isVisible: Boolean(this._config.backdrop),
+                isAnimated: this._isAnimated()
+            })
+        }
+        _initializeFocusTrap() {
+            return new Ai({
+                trapElement: this._element
+            })
+        }
+        _getConfig(t) {
+            return t = {
+                ...Ci,
+                ...U.getDataAttributes(this._element),
+                ..."object" == typeof t ? t : {}
+            }, a(Ti, t, ki), t
+        }
+        _showElement(t) {
+            const e = this._isAnimated(),
+                i = V.findOne(".modal-body", this._dialog);
+            this._element.parentNode && this._element.parentNode.nodeType === Node.ELEMENT_NODE || document.body.append(this._element), this._element.style.display = "block", this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.scrollTop = 0, i && (i.scrollTop = 0), e && u(this._element), this._element.classList.add(ji), this._queueCallback((() => {
+                this._config.focus && this._focustrap.activate(), this._isTransitioning = !1, j.trigger(this._element, "shown.bs.modal", {
+                    relatedTarget: t
+                })
+            }), this._dialog, e)
+        }
+        _setEscapeEvent() {
+            this._isShown ? j.on(this._element, Ni, (t => {
+                this._config.keyboard && t.key === Oi ? (t.preventDefault(), this.hide()) : this._config.keyboard || t.key !== Oi || this._triggerBackdropTransition()
+            })) : j.off(this._element, Ni)
+        }
+        _setResizeEvent() {
+            this._isShown ? j.on(window, Di, (() => this._adjustDialog())) : j.off(window, Di)
+        }
+        _hideModal() {
+            this._element.style.display = "none", this._element.setAttribute("aria-hidden", !0), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._isTransitioning = !1, this._backdrop.hide((() => {
+                document.body.classList.remove(Pi), this._resetAdjustments(), this._scrollBar.reset(), j.trigger(this._element, Li)
+            }))
+        }
+        _showBackdrop(t) {
+            j.on(this._element, Si, (t => {
+                this._ignoreBackdropClick ? this._ignoreBackdropClick = !1 : t.target === t.currentTarget && (!0 === this._config.backdrop ? this.hide() : "static" === this._config.backdrop && this._triggerBackdropTransition())
+            })), this._backdrop.show(t)
+        }
+        _isAnimated() {
+            return this._element.classList.contains("fade")
+        }
+        _triggerBackdropTransition() {
+            if (j.trigger(this._element, "hidePrevented.bs.modal").defaultPrevented) return;
+            const {
+                classList: t,
+                scrollHeight: e,
+                style: i
+            } = this._element, n = e > document.documentElement.clientHeight;
+            !n && "hidden" === i.overflowY || t.contains(Mi) || (n || (i.overflowY = "hidden"), t.add(Mi), this._queueCallback((() => {
+                t.remove(Mi), n || this._queueCallback((() => {
+                    i.overflowY = ""
+                }), this._dialog)
+            }), this._dialog), this._element.focus())
+        }
+        _adjustDialog() {
+            const t = this._element.scrollHeight > document.documentElement.clientHeight,
+                e = this._scrollBar.getWidth(),
+                i = e > 0;
+            (!i && t && !m() || i && !t && m()) && (this._element.style.paddingLeft = `${e}px`), (i && !t && !m() || !i && t && m()) && (this._element.style.paddingRight = `${e}px`)
+        }
+        _resetAdjustments() {
+            this._element.style.paddingLeft = "", this._element.style.paddingRight = ""
+        }
+        static jQueryInterface(t, e) {
+            return this.each((function() {
+                const i = Hi.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === i[t]) throw new TypeError(`No method named "${t}"`);
+                    i[t](e)
+                }
+            }))
+        }
+    }
+    j.on(document, "click.bs.modal.data-api", '[data-bs-toggle="modal"]', (function(t) {
+        const e = n(this);
+        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), j.one(e, xi, (t => {
+            t.defaultPrevented || j.one(e, Li, (() => {
+                l(this) && this.focus()
             }))
         }));
-        Ht._jQueryInterface.call(e(n), a, this)
-    })), e.fn.modal = Ht._jQueryInterface, e.fn.modal.Constructor = Ht, e.fn.modal.noConflict = function() {
-        return e.fn.modal = Pt, Ht._jQueryInterface
-    };
-    var Mt = ["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"],
-        Bt = {
-            "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
-            a: ["target", "href", "title", "rel"],
-            area: [],
-            b: [],
-            br: [],
-            col: [],
-            code: [],
-            div: [],
-            em: [],
-            hr: [],
-            h1: [],
-            h2: [],
-            h3: [],
-            h4: [],
-            h5: [],
-            h6: [],
-            i: [],
-            img: ["src", "srcset", "alt", "title", "width", "height"],
-            li: [],
-            ol: [],
-            p: [],
-            pre: [],
-            s: [],
-            small: [],
-            span: [],
-            sub: [],
-            sup: [],
-            strong: [],
-            u: [],
-            ul: []
-        },
-        qt = /^(?:(?:https?|mailto|ftp|tel|file):|[^#&/:?]*(?:[#/?]|$))/gi,
-        Qt = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[\d+/a-z]+=*$/i;
-
-    function Wt(t, e, n) {
-        if (0 === t.length) return t;
-        if (n && "function" == typeof n) return n(t);
-        for (var i = (new window.DOMParser).parseFromString(t, "text/html"), o = Object.keys(e), r = [].slice.call(i.body.querySelectorAll("*")), s = function(t, n) {
-                var i = r[t],
-                    s = i.nodeName.toLowerCase();
-                if (-1 === o.indexOf(i.nodeName.toLowerCase())) return i.parentNode.removeChild(i), "continue";
-                var a = [].slice.call(i.attributes),
-                    l = [].concat(e["*"] || [], e[s] || []);
-                a.forEach((function(t) {
-                    (function(t, e) {
-                        var n = t.nodeName.toLowerCase();
-                        if (-1 !== e.indexOf(n)) return -1 === Mt.indexOf(n) || Boolean(t.nodeValue.match(qt) || t.nodeValue.match(Qt));
-                        for (var i = e.filter((function(t) {
-                                return t instanceof RegExp
-                            })), o = 0, r = i.length; o < r; o++)
-                            if (n.match(i[o])) return !0;
-                        return !1
-                    })(t, l) || i.removeAttribute(t.nodeName)
-                }))
-            }, a = 0, l = r.length; a < l; a++) s(a);
-        return i.body.innerHTML
+        const i = V.findOne(".modal.show");
+        i && Hi.getInstance(i).hide(), Hi.getOrCreateInstance(e).toggle(this)
+    })), R(Hi), g(Hi);
+    const Bi = "offcanvas",
+        Ri = {
+            backdrop: !0,
+            keyboard: !0,
+            scroll: !1
+        },
+        Wi = {
+            backdrop: "boolean",
+            keyboard: "boolean",
+            scroll: "boolean"
+        },
+        $i = "show",
+        zi = ".offcanvas.show",
+        qi = "hidden.bs.offcanvas";
+    class Fi extends B {
+        constructor(t, e) {
+            super(t), this._config = this._getConfig(e), this._isShown = !1, this._backdrop = this._initializeBackDrop(), this._focustrap = this._initializeFocusTrap(), this._addEventListeners()
+        }
+        static get NAME() {
+            return Bi
+        }
+        static get Default() {
+            return Ri
+        }
+        toggle(t) {
+            return this._isShown ? this.hide() : this.show(t)
+        }
+        show(t) {
+            this._isShown || j.trigger(this._element, "show.bs.offcanvas", {
+                relatedTarget: t
+            }).defaultPrevented || (this._isShown = !0, this._element.style.visibility = "visible", this._backdrop.show(), this._config.scroll || (new fi).hide(), this._element.removeAttribute("aria-hidden"), this._element.setAttribute("aria-modal", !0), this._element.setAttribute("role", "dialog"), this._element.classList.add($i), this._queueCallback((() => {
+                this._config.scroll || this._focustrap.activate(), j.trigger(this._element, "shown.bs.offcanvas", {
+                    relatedTarget: t
+                })
+            }), this._element, !0))
+        }
+        hide() {
+            this._isShown && (j.trigger(this._element, "hide.bs.offcanvas").defaultPrevented || (this._focustrap.deactivate(), this._element.blur(), this._isShown = !1, this._element.classList.remove($i), this._backdrop.hide(), this._queueCallback((() => {
+                this._element.setAttribute("aria-hidden", !0), this._element.removeAttribute("aria-modal"), this._element.removeAttribute("role"), this._element.style.visibility = "hidden", this._config.scroll || (new fi).reset(), j.trigger(this._element, qi)
+            }), this._element, !0)))
+        }
+        dispose() {
+            this._backdrop.dispose(), this._focustrap.deactivate(), super.dispose()
+        }
+        _getConfig(t) {
+            return t = {
+                ...Ri,
+                ...U.getDataAttributes(this._element),
+                ..."object" == typeof t ? t : {}
+            }, a(Bi, t, Wi), t
+        }
+        _initializeBackDrop() {
+            return new bi({
+                className: "offcanvas-backdrop",
+                isVisible: this._config.backdrop,
+                isAnimated: !0,
+                rootElement: this._element.parentNode,
+                clickCallback: () => this.hide()
+            })
+        }
+        _initializeFocusTrap() {
+            return new Ai({
+                trapElement: this._element
+            })
+        }
+        _addEventListeners() {
+            j.on(this._element, "keydown.dismiss.bs.offcanvas", (t => {
+                this._config.keyboard && "Escape" === t.key && this.hide()
+            }))
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = Fi.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t] || t.startsWith("_") || "constructor" === t) throw new TypeError(`No method named "${t}"`);
+                    e[t](this)
+                }
+            }))
+        }
     }
-    var Ut = "tooltip",
-        Vt = e.fn[Ut],
-        Yt = new RegExp("(^|\\s)bs-tooltip\\S+", "g"),
-        zt = ["sanitize", "whiteList", "sanitizeFn"],
-        Xt = {
+    j.on(document, "click.bs.offcanvas.data-api", '[data-bs-toggle="offcanvas"]', (function(t) {
+        const e = n(this);
+        if (["A", "AREA"].includes(this.tagName) && t.preventDefault(), c(this)) return;
+        j.one(e, qi, (() => {
+            l(this) && this.focus()
+        }));
+        const i = V.findOne(zi);
+        i && i !== e && Fi.getInstance(i).hide(), Fi.getOrCreateInstance(e).toggle(this)
+    })), j.on(window, "load.bs.offcanvas.data-api", (() => V.find(zi).forEach((t => Fi.getOrCreateInstance(t).show())))), R(Fi), g(Fi);
+    const Ui = new Set(["background", "cite", "href", "itemtype", "longdesc", "poster", "src", "xlink:href"]),
+        Vi = /^(?:(?:https?|mailto|ftp|tel|file|sms):|[^#&/:?]*(?:[#/?]|$))/i,
+        Ki = /^data:(?:image\/(?:bmp|gif|jpeg|jpg|png|tiff|webp)|video\/(?:mpeg|mp4|ogg|webm)|audio\/(?:mp3|oga|ogg|opus));base64,[\d+/a-z]+=*$/i,
+        Xi = (t, e) => {
+            const i = t.nodeName.toLowerCase();
+            if (e.includes(i)) return !Ui.has(i) || Boolean(Vi.test(t.nodeValue) || Ki.test(t.nodeValue));
+            const n = e.filter((t => t instanceof RegExp));
+            for (let t = 0, e = n.length; t < e; t++)
+                if (n[t].test(i)) return !0;
+            return !1
+        };
+
+    function Yi(t, e, i) {
+        if (!t.length) return t;
+        if (i && "function" == typeof i) return i(t);
+        const n = (new window.DOMParser).parseFromString(t, "text/html"),
+            s = [].concat(...n.body.querySelectorAll("*"));
+        for (let t = 0, i = s.length; t < i; t++) {
+            const i = s[t],
+                n = i.nodeName.toLowerCase();
+            if (!Object.keys(e).includes(n)) {
+                i.remove();
+                continue
+            }
+            const o = [].concat(...i.attributes),
+                r = [].concat(e["*"] || [], e[n] || []);
+            o.forEach((t => {
+                Xi(t, r) || i.removeAttribute(t.nodeName)
+            }))
+        }
+        return n.body.innerHTML
+    }
+    const Qi = "tooltip",
+        Gi = new Set(["sanitize", "allowList", "sanitizeFn"]),
+        Zi = {
             animation: "boolean",
             template: "string",
             title: "(string|element|function)",
             trigger: "string",
             delay: "(number|object)",
             html: "boolean",
             selector: "(string|boolean)",
             placement: "(string|function)",
-            offset: "(number|string|function)",
+            offset: "(array|string|function)",
             container: "(string|element|boolean)",
-            fallbackPlacement: "(string|array)",
+            fallbackPlacements: "array",
             boundary: "(string|element)",
+            customClass: "(string|function)",
             sanitize: "boolean",
             sanitizeFn: "(null|function)",
-            whiteList: "object",
-            popperConfig: "(null|object)"
+            allowList: "object",
+            popperConfig: "(null|object|function)"
         },
-        Kt = {
+        Ji = {
             AUTO: "auto",
             TOP: "top",
-            RIGHT: "right",
+            RIGHT: m() ? "left" : "right",
             BOTTOM: "bottom",
-            LEFT: "left"
+            LEFT: m() ? "right" : "left"
         },
-        Gt = {
+        tn = {
             animation: !0,
-            template: '<div class="tooltip" role="tooltip"><div class="arrow"></div><div class="tooltip-inner"></div></div>',
+            template: '<div class="tooltip" role="tooltip"><div class="tooltip-arrow"></div><div class="tooltip-inner"></div></div>',
             trigger: "hover focus",
             title: "",
             delay: 0,
             html: !1,
             selector: !1,
             placement: "top",
-            offset: 0,
+            offset: [0, 0],
             container: !1,
-            fallbackPlacement: "flip",
-            boundary: "scrollParent",
+            fallbackPlacements: ["top", "right", "bottom", "left"],
+            boundary: "clippingParents",
+            customClass: "",
             sanitize: !0,
             sanitizeFn: null,
-            whiteList: Bt,
+            allowList: {
+                "*": ["class", "dir", "id", "lang", "role", /^aria-[\w-]*$/i],
+                a: ["target", "href", "title", "rel"],
+                area: [],
+                b: [],
+                br: [],
+                col: [],
+                code: [],
+                div: [],
+                em: [],
+                hr: [],
+                h1: [],
+                h2: [],
+                h3: [],
+                h4: [],
+                h5: [],
+                h6: [],
+                i: [],
+                img: ["src", "srcset", "alt", "title", "width", "height"],
+                li: [],
+                ol: [],
+                p: [],
+                pre: [],
+                s: [],
+                small: [],
+                span: [],
+                sub: [],
+                sup: [],
+                strong: [],
+                u: [],
+                ul: []
+            },
             popperConfig: null
         },
-        $t = {
+        en = {
             HIDE: "hide.bs.tooltip",
             HIDDEN: "hidden.bs.tooltip",
             SHOW: "show.bs.tooltip",
             SHOWN: "shown.bs.tooltip",
             INSERTED: "inserted.bs.tooltip",
             CLICK: "click.bs.tooltip",
             FOCUSIN: "focusin.bs.tooltip",
             FOCUSOUT: "focusout.bs.tooltip",
             MOUSEENTER: "mouseenter.bs.tooltip",
             MOUSELEAVE: "mouseleave.bs.tooltip"
         },
-        Jt = function() {
-            function t(t, e) {
-                if ("undefined" == typeof kt) throw new TypeError("Bootstrap's tooltips require Popper.js (https://popper.js.org/)");
-                this._isEnabled = !0, this._timeout = 0, this._hoverState = "", this._activeTrigger = {}, this._popper = null, this.element = t, this.config = this._getConfig(e), this.tip = null, this._setListeners()
-            }
-            var n = t.prototype;
-            return n.enable = function() {
-                this._isEnabled = !0
-            }, n.disable = function() {
-                this._isEnabled = !1
-            }, n.toggleEnabled = function() {
-                this._isEnabled = !this._isEnabled
-            }, n.toggle = function(t) {
-                if (this._isEnabled)
-                    if (t) {
-                        var n = this.constructor.DATA_KEY,
-                            i = e(t.currentTarget).data(n);
-                        i || (i = new this.constructor(t.currentTarget, this._getDelegateConfig()), e(t.currentTarget).data(n, i)), i._activeTrigger.click = !i._activeTrigger.click, i._isWithActiveTrigger() ? i._enter(null, i) : i._leave(null, i)
-                    } else {
-                        if (e(this.getTipElement()).hasClass("show")) return void this._leave(null, this);
-                        this._enter(null, this)
-                    }
-            }, n.dispose = function() {
-                clearTimeout(this._timeout), e.removeData(this.element, this.constructor.DATA_KEY), e(this.element).off(this.constructor.EVENT_KEY), e(this.element).closest(".modal").off("hide.bs.modal", this._hideModalHandler), this.tip && e(this.tip).remove(), this._isEnabled = null, this._timeout = null, this._hoverState = null, this._activeTrigger = null, this._popper && this._popper.destroy(), this._popper = null, this.element = null, this.config = null, this.tip = null
-            }, n.show = function() {
-                var t = this;
-                if ("none" === e(this.element).css("display")) throw new Error("Please use show on visible elements");
-                var n = e.Event(this.constructor.Event.SHOW);
-                if (this.isWithContent() && this._isEnabled) {
-                    e(this.element).trigger(n);
-                    var i = s.findShadowRoot(this.element),
-                        o = e.contains(null !== i ? i : this.element.ownerDocument.documentElement, this.element);
-                    if (n.isDefaultPrevented() || !o) return;
-                    var r = this.getTipElement(),
-                        a = s.getUID(this.constructor.NAME);
-                    r.setAttribute("id", a), this.element.setAttribute("aria-describedby", a), this.setContent(), this.config.animation && e(r).addClass("fade");
-                    var l = "function" == typeof this.config.placement ? this.config.placement.call(this, r, this.element) : this.config.placement,
-                        c = this._getAttachment(l);
-                    this.addAttachmentClass(c);
-                    var h = this._getContainer();
-                    e(r).data(this.constructor.DATA_KEY, this), e.contains(this.element.ownerDocument.documentElement, this.tip) || e(r).appendTo(h), e(this.element).trigger(this.constructor.Event.INSERTED), this._popper = new kt(this.element, r, this._getPopperConfig(c)), e(r).addClass("show"), "ontouchstart" in document.documentElement && e(document.body).children().on("mouseover", null, e.noop);
-                    var u = function() {
-                        t.config.animation && t._fixTransition();
-                        var n = t._hoverState;
-                        t._hoverState = null, e(t.element).trigger(t.constructor.Event.SHOWN), "out" === n && t._leave(null, t)
-                    };
-                    if (e(this.tip).hasClass("fade")) {
-                        var f = s.getTransitionDurationFromElement(this.tip);
-                        e(this.tip).one(s.TRANSITION_END, u).emulateTransitionEnd(f)
-                    } else u()
-                }
-            }, n.hide = function(t) {
-                var n = this,
-                    i = this.getTipElement(),
-                    o = e.Event(this.constructor.Event.HIDE),
-                    r = function() {
-                        "show" !== n._hoverState && i.parentNode && i.parentNode.removeChild(i), n._cleanTipClass(), n.element.removeAttribute("aria-describedby"), e(n.element).trigger(n.constructor.Event.HIDDEN), null !== n._popper && n._popper.destroy(), t && t()
-                    };
-                if (e(this.element).trigger(o), !o.isDefaultPrevented()) {
-                    if (e(i).removeClass("show"), "ontouchstart" in document.documentElement && e(document.body).children().off("mouseover", null, e.noop), this._activeTrigger.click = !1, this._activeTrigger.focus = !1, this._activeTrigger.hover = !1, e(this.tip).hasClass("fade")) {
-                        var a = s.getTransitionDurationFromElement(i);
-                        e(i).one(s.TRANSITION_END, r).emulateTransitionEnd(a)
-                    } else r();
-                    this._hoverState = ""
-                }
-            }, n.update = function() {
-                null !== this._popper && this._popper.scheduleUpdate()
-            }, n.isWithContent = function() {
-                return Boolean(this.getTitle())
-            }, n.addAttachmentClass = function(t) {
-                e(this.getTipElement()).addClass("bs-tooltip-" + t)
-            }, n.getTipElement = function() {
-                return this.tip = this.tip || e(this.config.template)[0], this.tip
-            }, n.setContent = function() {
-                var t = this.getTipElement();
-                this.setElementContent(e(t.querySelectorAll(".tooltip-inner")), this.getTitle()), e(t).removeClass("fade show")
-            }, n.setElementContent = function(t, n) {
-                "object" != typeof n || !n.nodeType && !n.jquery ? this.config.html ? (this.config.sanitize && (n = Wt(n, this.config.whiteList, this.config.sanitizeFn)), t.html(n)) : t.text(n) : this.config.html ? e(n).parent().is(t) || t.empty().append(n) : t.text(e(n).text())
-            }, n.getTitle = function() {
-                var t = this.element.getAttribute("data-original-title");
-                return t || (t = "function" == typeof this.config.title ? this.config.title.call(this.element) : this.config.title), t
-            }, n._getPopperConfig = function(t) {
-                var e = this;
-                return o({}, {
-                    placement: t,
-                    modifiers: {
-                        offset: this._getOffset(),
-                        flip: {
-                            behavior: this.config.fallbackPlacement
-                        },
-                        arrow: {
-                            element: ".arrow"
-                        },
-                        preventOverflow: {
-                            boundariesElement: this.config.boundary
-                        }
-                    },
-                    onCreate: function(t) {
-                        t.originalPlacement !== t.placement && e._handlePopperPlacementChange(t)
-                    },
-                    onUpdate: function(t) {
-                        return e._handlePopperPlacementChange(t)
-                    }
-                }, this.config.popperConfig)
-            }, n._getOffset = function() {
-                var t = this,
-                    e = {};
-                return "function" == typeof this.config.offset ? e.fn = function(e) {
-                    return e.offsets = o({}, e.offsets, t.config.offset(e.offsets, t.element) || {}), e
-                } : e.offset = this.config.offset, e
-            }, n._getContainer = function() {
-                return !1 === this.config.container ? document.body : s.isElement(this.config.container) ? e(this.config.container) : e(document).find(this.config.container)
-            }, n._getAttachment = function(t) {
-                return Kt[t.toUpperCase()]
-            }, n._setListeners = function() {
-                var t = this;
-                this.config.trigger.split(" ").forEach((function(n) {
-                    if ("click" === n) e(t.element).on(t.constructor.Event.CLICK, t.config.selector, (function(e) {
-                        return t.toggle(e)
-                    }));
-                    else if ("manual" !== n) {
-                        var i = "hover" === n ? t.constructor.Event.MOUSEENTER : t.constructor.Event.FOCUSIN,
-                            o = "hover" === n ? t.constructor.Event.MOUSELEAVE : t.constructor.Event.FOCUSOUT;
-                        e(t.element).on(i, t.config.selector, (function(e) {
-                            return t._enter(e)
-                        })).on(o, t.config.selector, (function(e) {
-                            return t._leave(e)
-                        }))
-                    }
-                })), this._hideModalHandler = function() {
-                    t.element && t.hide()
-                }, e(this.element).closest(".modal").on("hide.bs.modal", this._hideModalHandler), this.config.selector ? this.config = o({}, this.config, {
-                    trigger: "manual",
-                    selector: ""
-                }) : this._fixTitle()
-            }, n._fixTitle = function() {
-                var t = typeof this.element.getAttribute("data-original-title");
-                (this.element.getAttribute("title") || "string" !== t) && (this.element.setAttribute("data-original-title", this.element.getAttribute("title") || ""), this.element.setAttribute("title", ""))
-            }, n._enter = function(t, n) {
-                var i = this.constructor.DATA_KEY;
-                (n = n || e(t.currentTarget).data(i)) || (n = new this.constructor(t.currentTarget, this._getDelegateConfig()), e(t.currentTarget).data(i, n)), t && (n._activeTrigger["focusin" === t.type ? "focus" : "hover"] = !0), e(n.getTipElement()).hasClass("show") || "show" === n._hoverState ? n._hoverState = "show" : (clearTimeout(n._timeout), n._hoverState = "show", n.config.delay && n.config.delay.show ? n._timeout = setTimeout((function() {
-                    "show" === n._hoverState && n.show()
-                }), n.config.delay.show) : n.show())
-            }, n._leave = function(t, n) {
-                var i = this.constructor.DATA_KEY;
-                (n = n || e(t.currentTarget).data(i)) || (n = new this.constructor(t.currentTarget, this._getDelegateConfig()), e(t.currentTarget).data(i, n)), t && (n._activeTrigger["focusout" === t.type ? "focus" : "hover"] = !1), n._isWithActiveTrigger() || (clearTimeout(n._timeout), n._hoverState = "out", n.config.delay && n.config.delay.hide ? n._timeout = setTimeout((function() {
-                    "out" === n._hoverState && n.hide()
-                }), n.config.delay.hide) : n.hide())
-            }, n._isWithActiveTrigger = function() {
-                for (var t in this._activeTrigger)
-                    if (this._activeTrigger[t]) return !0;
-                return !1
-            }, n._getConfig = function(t) {
-                var n = e(this.element).data();
-                return Object.keys(n).forEach((function(t) {
-                    -1 !== zt.indexOf(t) && delete n[t]
-                })), "number" == typeof(t = o({}, this.constructor.Default, n, "object" == typeof t && t ? t : {})).delay && (t.delay = {
-                    show: t.delay,
-                    hide: t.delay
-                }), "number" == typeof t.title && (t.title = t.title.toString()), "number" == typeof t.content && (t.content = t.content.toString()), s.typeCheckConfig(Ut, t, this.constructor.DefaultType), t.sanitize && (t.template = Wt(t.template, t.whiteList, t.sanitizeFn)), t
-            }, n._getDelegateConfig = function() {
-                var t = {};
-                if (this.config)
-                    for (var e in this.config) this.constructor.Default[e] !== this.config[e] && (t[e] = this.config[e]);
-                return t
-            }, n._cleanTipClass = function() {
-                var t = e(this.getTipElement()),
-                    n = t.attr("class").match(Yt);
-                null !== n && n.length && t.removeClass(n.join(""))
-            }, n._handlePopperPlacementChange = function(t) {
-                this.tip = t.instance.popper, this._cleanTipClass(), this.addAttachmentClass(this._getAttachment(t.placement))
-            }, n._fixTransition = function() {
-                var t = this.getTipElement(),
-                    n = this.config.animation;
-                null === t.getAttribute("x-placement") && (e(t).removeClass("fade"), this.config.animation = !1, this.hide(), this.show(), this.config.animation = n)
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this).data("bs.tooltip"),
-                        o = "object" == typeof n && n;
-                    if ((i || !/dispose|hide/.test(n)) && (i || (i = new t(this, o), e(this).data("bs.tooltip", i)), "string" == typeof n)) {
-                        if ("undefined" == typeof i[n]) throw new TypeError('No method named "' + n + '"');
-                        i[n]()
+        nn = "fade",
+        sn = "show",
+        on = "show",
+        rn = "out",
+        an = ".tooltip-inner",
+        ln = ".modal",
+        cn = "hide.bs.modal",
+        hn = "hover",
+        dn = "focus";
+    class un extends B {
+        constructor(t, e) {
+            if (void 0 === Fe) throw new TypeError("Bootstrap's tooltips require Popper (https://popper.js.org)");
+            super(t), this._isEnabled = !0, this._timeout = 0, this._hoverState = "", this._activeTrigger = {}, this._popper = null, this._config = this._getConfig(e), this.tip = null, this._setListeners()
+        }
+        static get Default() {
+            return tn
+        }
+        static get NAME() {
+            return Qi
+        }
+        static get Event() {
+            return en
+        }
+        static get DefaultType() {
+            return Zi
+        }
+        enable() {
+            this._isEnabled = !0
+        }
+        disable() {
+            this._isEnabled = !1
+        }
+        toggleEnabled() {
+            this._isEnabled = !this._isEnabled
+        }
+        toggle(t) {
+            if (this._isEnabled)
+                if (t) {
+                    const e = this._initializeOnDelegatedTarget(t);
+                    e._activeTrigger.click = !e._activeTrigger.click, e._isWithActiveTrigger() ? e._enter(null, e) : e._leave(null, e)
+                } else {
+                    if (this.getTipElement().classList.contains(sn)) return void this._leave(null, this);
+                    this._enter(null, this)
+                }
+        }
+        dispose() {
+            clearTimeout(this._timeout), j.off(this._element.closest(ln), cn, this._hideModalHandler), this.tip && this.tip.remove(), this._disposePopper(), super.dispose()
+        }
+        show() {
+            if ("none" === this._element.style.display) throw new Error("Please use show on visible elements");
+            if (!this.isWithContent() || !this._isEnabled) return;
+            const t = j.trigger(this._element, this.constructor.Event.SHOW),
+                e = h(this._element),
+                i = null === e ? this._element.ownerDocument.documentElement.contains(this._element) : e.contains(this._element);
+            if (t.defaultPrevented || !i) return;
+            "tooltip" === this.constructor.NAME && this.tip && this.getTitle() !== this.tip.querySelector(an).innerHTML && (this._disposePopper(), this.tip.remove(), this.tip = null);
+            const n = this.getTipElement(),
+                s = (t => {
+                    do {
+                        t += Math.floor(1e6 * Math.random())
+                    } while (document.getElementById(t));
+                    return t
+                })(this.constructor.NAME);
+            n.setAttribute("id", s), this._element.setAttribute("aria-describedby", s), this._config.animation && n.classList.add(nn);
+            const o = "function" == typeof this._config.placement ? this._config.placement.call(this, n, this._element) : this._config.placement,
+                r = this._getAttachment(o);
+            this._addAttachmentClass(r);
+            const {
+                container: a
+            } = this._config;
+            H.set(n, this.constructor.DATA_KEY, this), this._element.ownerDocument.documentElement.contains(this.tip) || (a.append(n), j.trigger(this._element, this.constructor.Event.INSERTED)), this._popper ? this._popper.update() : this._popper = qe(this._element, n, this._getPopperConfig(r)), n.classList.add(sn);
+            const l = this._resolvePossibleFunction(this._config.customClass);
+            l && n.classList.add(...l.split(" ")), "ontouchstart" in document.documentElement && [].concat(...document.body.children).forEach((t => {
+                j.on(t, "mouseover", d)
+            }));
+            const c = this.tip.classList.contains(nn);
+            this._queueCallback((() => {
+                const t = this._hoverState;
+                this._hoverState = null, j.trigger(this._element, this.constructor.Event.SHOWN), t === rn && this._leave(null, this)
+            }), this.tip, c)
+        }
+        hide() {
+            if (!this._popper) return;
+            const t = this.getTipElement();
+            if (j.trigger(this._element, this.constructor.Event.HIDE).defaultPrevented) return;
+            t.classList.remove(sn), "ontouchstart" in document.documentElement && [].concat(...document.body.children).forEach((t => j.off(t, "mouseover", d))), this._activeTrigger.click = !1, this._activeTrigger.focus = !1, this._activeTrigger.hover = !1;
+            const e = this.tip.classList.contains(nn);
+            this._queueCallback((() => {
+                this._isWithActiveTrigger() || (this._hoverState !== on && t.remove(), this._cleanTipClass(), this._element.removeAttribute("aria-describedby"), j.trigger(this._element, this.constructor.Event.HIDDEN), this._disposePopper())
+            }), this.tip, e), this._hoverState = ""
+        }
+        update() {
+            null !== this._popper && this._popper.update()
+        }
+        isWithContent() {
+            return Boolean(this.getTitle())
+        }
+        getTipElement() {
+            if (this.tip) return this.tip;
+            const t = document.createElement("div");
+            t.innerHTML = this._config.template;
+            const e = t.children[0];
+            return this.setContent(e), e.classList.remove(nn, sn), this.tip = e, this.tip
+        }
+        setContent(t) {
+            this._sanitizeAndSetContent(t, this.getTitle(), an)
+        }
+        _sanitizeAndSetContent(t, e, i) {
+            const n = V.findOne(i, t);
+            e || !n ? this.setElementContent(n, e) : n.remove()
+        }
+        setElementContent(t, e) {
+            if (null !== t) return o(e) ? (e = r(e), void(this._config.html ? e.parentNode !== t && (t.innerHTML = "", t.append(e)) : t.textContent = e.textContent)) : void(this._config.html ? (this._config.sanitize && (e = Yi(e, this._config.allowList, this._config.sanitizeFn)), t.innerHTML = e) : t.textContent = e)
+        }
+        getTitle() {
+            const t = this._element.getAttribute("data-bs-original-title") || this._config.title;
+            return this._resolvePossibleFunction(t)
+        }
+        updateAttachment(t) {
+            return "right" === t ? "end" : "left" === t ? "start" : t
+        }
+        _initializeOnDelegatedTarget(t, e) {
+            return e || this.constructor.getOrCreateInstance(t.delegateTarget, this._getDelegateConfig())
+        }
+        _getOffset() {
+            const {
+                offset: t
+            } = this._config;
+            return "string" == typeof t ? t.split(",").map((t => Number.parseInt(t, 10))) : "function" == typeof t ? e => t(e, this._element) : t
+        }
+        _resolvePossibleFunction(t) {
+            return "function" == typeof t ? t.call(this._element) : t
+        }
+        _getPopperConfig(t) {
+            const e = {
+                placement: t,
+                modifiers: [{
+                    name: "flip",
+                    options: {
+                        fallbackPlacements: this._config.fallbackPlacements
+                    }
+                }, {
+                    name: "offset",
+                    options: {
+                        offset: this._getOffset()
+                    }
+                }, {
+                    name: "preventOverflow",
+                    options: {
+                        boundary: this._config.boundary
+                    }
+                }, {
+                    name: "arrow",
+                    options: {
+                        element: `.${this.constructor.NAME}-arrow`
                     }
-                }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return Gt
-                }
-            }, {
-                key: "NAME",
-                get: function() {
-                    return Ut
-                }
-            }, {
-                key: "DATA_KEY",
-                get: function() {
-                    return "bs.tooltip"
-                }
-            }, {
-                key: "Event",
-                get: function() {
-                    return $t
-                }
-            }, {
-                key: "EVENT_KEY",
-                get: function() {
-                    return ".bs.tooltip"
-                }
-            }, {
-                key: "DefaultType",
-                get: function() {
-                    return Xt
-                }
-            }]), t
-        }();
-    e.fn[Ut] = Jt._jQueryInterface, e.fn[Ut].Constructor = Jt, e.fn[Ut].noConflict = function() {
-        return e.fn[Ut] = Vt, Jt._jQueryInterface
-    };
-    var Zt = "popover",
-        te = e.fn[Zt],
-        ee = new RegExp("(^|\\s)bs-popover\\S+", "g"),
-        ne = o({}, Jt.Default, {
+                }, {
+                    name: "onChange",
+                    enabled: !0,
+                    phase: "afterWrite",
+                    fn: t => this._handlePopperPlacementChange(t)
+                }],
+                onFirstUpdate: t => {
+                    t.options.placement !== t.placement && this._handlePopperPlacementChange(t)
+                }
+            };
+            return {
+                ...e,
+                ..."function" == typeof this._config.popperConfig ? this._config.popperConfig(e) : this._config.popperConfig
+            }
+        }
+        _addAttachmentClass(t) {
+            this.getTipElement().classList.add(`${this._getBasicClassPrefix()}-${this.updateAttachment(t)}`)
+        }
+        _getAttachment(t) {
+            return Ji[t.toUpperCase()]
+        }
+        _setListeners() {
+            this._config.trigger.split(" ").forEach((t => {
+                if ("click" === t) j.on(this._element, this.constructor.Event.CLICK, this._config.selector, (t => this.toggle(t)));
+                else if ("manual" !== t) {
+                    const e = t === hn ? this.constructor.Event.MOUSEENTER : this.constructor.Event.FOCUSIN,
+                        i = t === hn ? this.constructor.Event.MOUSELEAVE : this.constructor.Event.FOCUSOUT;
+                    j.on(this._element, e, this._config.selector, (t => this._enter(t))), j.on(this._element, i, this._config.selector, (t => this._leave(t)))
+                }
+            })), this._hideModalHandler = () => {
+                this._element && this.hide()
+            }, j.on(this._element.closest(ln), cn, this._hideModalHandler), this._config.selector ? this._config = {
+                ...this._config,
+                trigger: "manual",
+                selector: ""
+            } : this._fixTitle()
+        }
+        _fixTitle() {
+            const t = this._element.getAttribute("title"),
+                e = typeof this._element.getAttribute("data-bs-original-title");
+            (t || "string" !== e) && (this._element.setAttribute("data-bs-original-title", t || ""), !t || this._element.getAttribute("aria-label") || this._element.textContent || this._element.setAttribute("aria-label", t), this._element.setAttribute("title", ""))
+        }
+        _enter(t, e) {
+            e = this._initializeOnDelegatedTarget(t, e), t && (e._activeTrigger["focusin" === t.type ? dn : hn] = !0), e.getTipElement().classList.contains(sn) || e._hoverState === on ? e._hoverState = on : (clearTimeout(e._timeout), e._hoverState = on, e._config.delay && e._config.delay.show ? e._timeout = setTimeout((() => {
+                e._hoverState === on && e.show()
+            }), e._config.delay.show) : e.show())
+        }
+        _leave(t, e) {
+            e = this._initializeOnDelegatedTarget(t, e), t && (e._activeTrigger["focusout" === t.type ? dn : hn] = e._element.contains(t.relatedTarget)), e._isWithActiveTrigger() || (clearTimeout(e._timeout), e._hoverState = rn, e._config.delay && e._config.delay.hide ? e._timeout = setTimeout((() => {
+                e._hoverState === rn && e.hide()
+            }), e._config.delay.hide) : e.hide())
+        }
+        _isWithActiveTrigger() {
+            for (const t in this._activeTrigger)
+                if (this._activeTrigger[t]) return !0;
+            return !1
+        }
+        _getConfig(t) {
+            const e = U.getDataAttributes(this._element);
+            return Object.keys(e).forEach((t => {
+                Gi.has(t) && delete e[t]
+            })), (t = {
+                ...this.constructor.Default,
+                ...e,
+                ..."object" == typeof t && t ? t : {}
+            }).container = !1 === t.container ? document.body : r(t.container), "number" == typeof t.delay && (t.delay = {
+                show: t.delay,
+                hide: t.delay
+            }), "number" == typeof t.title && (t.title = t.title.toString()), "number" == typeof t.content && (t.content = t.content.toString()), a(Qi, t, this.constructor.DefaultType), t.sanitize && (t.template = Yi(t.template, t.allowList, t.sanitizeFn)), t
+        }
+        _getDelegateConfig() {
+            const t = {};
+            for (const e in this._config) this.constructor.Default[e] !== this._config[e] && (t[e] = this._config[e]);
+            return t
+        }
+        _cleanTipClass() {
+            const t = this.getTipElement(),
+                e = new RegExp(`(^|\\s)${this._getBasicClassPrefix()}\\S+`, "g"),
+                i = t.getAttribute("class").match(e);
+            null !== i && i.length > 0 && i.map((t => t.trim())).forEach((e => t.classList.remove(e)))
+        }
+        _getBasicClassPrefix() {
+            return "bs-tooltip"
+        }
+        _handlePopperPlacementChange(t) {
+            const {
+                state: e
+            } = t;
+            e && (this.tip = e.elements.popper, this._cleanTipClass(), this._addAttachmentClass(this._getAttachment(e.placement)))
+        }
+        _disposePopper() {
+            this._popper && (this._popper.destroy(), this._popper = null)
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = un.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    e[t]()
+                }
+            }))
+        }
+    }
+    g(un);
+    const fn = {
+            ...un.Default,
             placement: "right",
+            offset: [0, 8],
             trigger: "click",
             content: "",
-            template: '<div class="popover" role="tooltip"><div class="arrow"></div><h3 class="popover-header"></h3><div class="popover-body"></div></div>'
-        }),
-        ie = o({}, Jt.DefaultType, {
+            template: '<div class="popover" role="tooltip"><div class="popover-arrow"></div><h3 class="popover-header"></h3><div class="popover-body"></div></div>'
+        },
+        pn = {
+            ...un.DefaultType,
             content: "(string|element|function)"
-        }),
-        oe = {
+        },
+        mn = {
             HIDE: "hide.bs.popover",
             HIDDEN: "hidden.bs.popover",
             SHOW: "show.bs.popover",
             SHOWN: "shown.bs.popover",
             INSERTED: "inserted.bs.popover",
             CLICK: "click.bs.popover",
             FOCUSIN: "focusin.bs.popover",
             FOCUSOUT: "focusout.bs.popover",
             MOUSEENTER: "mouseenter.bs.popover",
             MOUSELEAVE: "mouseleave.bs.popover"
-        },
-        re = function(t) {
-            var n, o;
-
-            function r() {
-                return t.apply(this, arguments) || this
-            }
-            o = t, (n = r).prototype = Object.create(o.prototype), n.prototype.constructor = n, n.__proto__ = o;
-            var s = r.prototype;
-            return s.isWithContent = function() {
-                return this.getTitle() || this._getContent()
-            }, s.addAttachmentClass = function(t) {
-                e(this.getTipElement()).addClass("bs-popover-" + t)
-            }, s.getTipElement = function() {
-                return this.tip = this.tip || e(this.config.template)[0], this.tip
-            }, s.setContent = function() {
-                var t = e(this.getTipElement());
-                this.setElementContent(t.find(".popover-header"), this.getTitle());
-                var n = this._getContent();
-                "function" == typeof n && (n = n.call(this.element)), this.setElementContent(t.find(".popover-body"), n), t.removeClass("fade show")
-            }, s._getContent = function() {
-                return this.element.getAttribute("data-content") || this.config.content
-            }, s._cleanTipClass = function() {
-                var t = e(this.getTipElement()),
-                    n = t.attr("class").match(ee);
-                null !== n && n.length > 0 && t.removeClass(n.join(""))
-            }, r._jQueryInterface = function(t) {
-                return this.each((function() {
-                    var n = e(this).data("bs.popover"),
-                        i = "object" == typeof t ? t : null;
-                    if ((n || !/dispose|hide/.test(t)) && (n || (n = new r(this, i), e(this).data("bs.popover", n)), "string" == typeof t)) {
-                        if ("undefined" == typeof n[t]) throw new TypeError('No method named "' + t + '"');
-                        n[t]()
-                    }
-                }))
-            }, i(r, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return ne
-                }
-            }, {
-                key: "NAME",
-                get: function() {
-                    return Zt
-                }
-            }, {
-                key: "DATA_KEY",
-                get: function() {
-                    return "bs.popover"
-                }
-            }, {
-                key: "Event",
-                get: function() {
-                    return oe
-                }
-            }, {
-                key: "EVENT_KEY",
-                get: function() {
-                    return ".bs.popover"
-                }
-            }, {
-                key: "DefaultType",
-                get: function() {
-                    return ie
-                }
-            }]), r
-        }(Jt);
-    e.fn[Zt] = re._jQueryInterface, e.fn[Zt].Constructor = re, e.fn[Zt].noConflict = function() {
-        return e.fn[Zt] = te, re._jQueryInterface
-    };
-    var se = "scrollspy",
-        ae = e.fn[se],
-        le = {
+        };
+    class gn extends un {
+        static get Default() {
+            return fn
+        }
+        static get NAME() {
+            return "popover"
+        }
+        static get Event() {
+            return mn
+        }
+        static get DefaultType() {
+            return pn
+        }
+        isWithContent() {
+            return this.getTitle() || this._getContent()
+        }
+        setContent(t) {
+            this._sanitizeAndSetContent(t, this.getTitle(), ".popover-header"), this._sanitizeAndSetContent(t, this._getContent(), ".popover-body")
+        }
+        _getContent() {
+            return this._resolvePossibleFunction(this._config.content)
+        }
+        _getBasicClassPrefix() {
+            return "bs-popover"
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = gn.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    e[t]()
+                }
+            }))
+        }
+    }
+    g(gn);
+    const _n = "scrollspy",
+        bn = {
             offset: 10,
             method: "auto",
             target: ""
         },
-        ce = {
+        vn = {
             offset: "number",
             method: "string",
             target: "(string|element)"
         },
-        he = function() {
-            function t(t, n) {
-                var i = this;
-                this._element = t, this._scrollElement = "BODY" === t.tagName ? window : t, this._config = this._getConfig(n), this._selector = this._config.target + " .nav-link," + this._config.target + " .list-group-item," + this._config.target + " .dropdown-item", this._offsets = [], this._targets = [], this._activeTarget = null, this._scrollHeight = 0, e(this._scrollElement).on("scroll.bs.scrollspy", (function(t) {
-                    return i._process(t)
-                })), this.refresh(), this._process()
-            }
-            var n = t.prototype;
-            return n.refresh = function() {
-                var t = this,
-                    n = this._scrollElement === this._scrollElement.window ? "offset" : "position",
-                    i = "auto" === this._config.method ? n : this._config.method,
-                    o = "position" === i ? this._getScrollTop() : 0;
-                this._offsets = [], this._targets = [], this._scrollHeight = this._getScrollHeight(), [].slice.call(document.querySelectorAll(this._selector)).map((function(t) {
-                    var n, r = s.getSelectorFromElement(t);
-                    if (r && (n = document.querySelector(r)), n) {
-                        var a = n.getBoundingClientRect();
-                        if (a.width || a.height) return [e(n)[i]().top + o, r]
-                    }
-                    return null
-                })).filter((function(t) {
-                    return t
-                })).sort((function(t, e) {
-                    return t[0] - e[0]
-                })).forEach((function(e) {
-                    t._offsets.push(e[0]), t._targets.push(e[1])
+        yn = "active",
+        wn = ".nav-link, .list-group-item, .dropdown-item",
+        En = "position";
+    class An extends B {
+        constructor(t, e) {
+            super(t), this._scrollElement = "BODY" === this._element.tagName ? window : this._element, this._config = this._getConfig(e), this._offsets = [], this._targets = [], this._activeTarget = null, this._scrollHeight = 0, j.on(this._scrollElement, "scroll.bs.scrollspy", (() => this._process())), this.refresh(), this._process()
+        }
+        static get Default() {
+            return bn
+        }
+        static get NAME() {
+            return _n
+        }
+        refresh() {
+            const t = this._scrollElement === this._scrollElement.window ? "offset" : En,
+                e = "auto" === this._config.method ? t : this._config.method,
+                n = e === En ? this._getScrollTop() : 0;
+            this._offsets = [], this._targets = [], this._scrollHeight = this._getScrollHeight(), V.find(wn, this._config.target).map((t => {
+                const s = i(t),
+                    o = s ? V.findOne(s) : null;
+                if (o) {
+                    const t = o.getBoundingClientRect();
+                    if (t.width || t.height) return [U[e](o).top + n, s]
+                }
+                return null
+            })).filter((t => t)).sort(((t, e) => t[0] - e[0])).forEach((t => {
+                this._offsets.push(t[0]), this._targets.push(t[1])
+            }))
+        }
+        dispose() {
+            j.off(this._scrollElement, ".bs.scrollspy"), super.dispose()
+        }
+        _getConfig(t) {
+            return (t = {
+                ...bn,
+                ...U.getDataAttributes(this._element),
+                ..."object" == typeof t && t ? t : {}
+            }).target = r(t.target) || document.documentElement, a(_n, t, vn), t
+        }
+        _getScrollTop() {
+            return this._scrollElement === window ? this._scrollElement.pageYOffset : this._scrollElement.scrollTop
+        }
+        _getScrollHeight() {
+            return this._scrollElement.scrollHeight || Math.max(document.body.scrollHeight, document.documentElement.scrollHeight)
+        }
+        _getOffsetHeight() {
+            return this._scrollElement === window ? window.innerHeight : this._scrollElement.getBoundingClientRect().height
+        }
+        _process() {
+            const t = this._getScrollTop() + this._config.offset,
+                e = this._getScrollHeight(),
+                i = this._config.offset + e - this._getOffsetHeight();
+            if (this._scrollHeight !== e && this.refresh(), t >= i) {
+                const t = this._targets[this._targets.length - 1];
+                this._activeTarget !== t && this._activate(t)
+            } else {
+                if (this._activeTarget && t < this._offsets[0] && this._offsets[0] > 0) return this._activeTarget = null, void this._clear();
+                for (let e = this._offsets.length; e--;) this._activeTarget !== this._targets[e] && t >= this._offsets[e] && (void 0 === this._offsets[e + 1] || t < this._offsets[e + 1]) && this._activate(this._targets[e])
+            }
+        }
+        _activate(t) {
+            this._activeTarget = t, this._clear();
+            const e = wn.split(",").map((e => `${e}[data-bs-target="${t}"],${e}[href="${t}"]`)),
+                i = V.findOne(e.join(","), this._config.target);
+            i.classList.add(yn), i.classList.contains("dropdown-item") ? V.findOne(".dropdown-toggle", i.closest(".dropdown")).classList.add(yn) : V.parents(i, ".nav, .list-group").forEach((t => {
+                V.prev(t, ".nav-link, .list-group-item").forEach((t => t.classList.add(yn))), V.prev(t, ".nav-item").forEach((t => {
+                    V.children(t, ".nav-link").forEach((t => t.classList.add(yn)))
                 }))
-            }, n.dispose = function() {
-                e.removeData(this._element, "bs.scrollspy"), e(this._scrollElement).off(".bs.scrollspy"), this._element = null, this._scrollElement = null, this._config = null, this._selector = null, this._offsets = null, this._targets = null, this._activeTarget = null, this._scrollHeight = null
-            }, n._getConfig = function(t) {
-                if ("string" != typeof(t = o({}, le, "object" == typeof t && t ? t : {})).target && s.isElement(t.target)) {
-                    var n = e(t.target).attr("id");
-                    n || (n = s.getUID(se), e(t.target).attr("id", n)), t.target = "#" + n
-                }
-                return s.typeCheckConfig(se, t, ce), t
-            }, n._getScrollTop = function() {
-                return this._scrollElement === window ? this._scrollElement.pageYOffset : this._scrollElement.scrollTop
-            }, n._getScrollHeight = function() {
-                return this._scrollElement.scrollHeight || Math.max(document.body.scrollHeight, document.documentElement.scrollHeight)
-            }, n._getOffsetHeight = function() {
-                return this._scrollElement === window ? window.innerHeight : this._scrollElement.getBoundingClientRect().height
-            }, n._process = function() {
-                var t = this._getScrollTop() + this._config.offset,
-                    e = this._getScrollHeight(),
-                    n = this._config.offset + e - this._getOffsetHeight();
-                if (this._scrollHeight !== e && this.refresh(), t >= n) {
-                    var i = this._targets[this._targets.length - 1];
-                    this._activeTarget !== i && this._activate(i)
-                } else {
-                    if (this._activeTarget && t < this._offsets[0] && this._offsets[0] > 0) return this._activeTarget = null, void this._clear();
-                    for (var o = this._offsets.length; o--;) {
-                        this._activeTarget !== this._targets[o] && t >= this._offsets[o] && ("undefined" == typeof this._offsets[o + 1] || t < this._offsets[o + 1]) && this._activate(this._targets[o])
-                    }
+            })), j.trigger(this._scrollElement, "activate.bs.scrollspy", {
+                relatedTarget: t
+            })
+        }
+        _clear() {
+            V.find(wn, this._config.target).filter((t => t.classList.contains(yn))).forEach((t => t.classList.remove(yn)))
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = An.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    e[t]()
                 }
-            }, n._activate = function(t) {
-                this._activeTarget = t, this._clear();
-                var n = this._selector.split(",").map((function(e) {
-                        return e + '[data-target="' + t + '"],' + e + '[href="' + t + '"]'
-                    })),
-                    i = e([].slice.call(document.querySelectorAll(n.join(","))));
-                i.hasClass("dropdown-item") ? (i.closest(".dropdown").find(".dropdown-toggle").addClass("active"), i.addClass("active")) : (i.addClass("active"), i.parents(".nav, .list-group").prev(".nav-link, .list-group-item").addClass("active"), i.parents(".nav, .list-group").prev(".nav-item").children(".nav-link").addClass("active")), e(this._scrollElement).trigger("activate.bs.scrollspy", {
+            }))
+        }
+    }
+    j.on(window, "load.bs.scrollspy.data-api", (() => {
+        V.find('[data-bs-spy="scroll"]').forEach((t => new An(t)))
+    })), g(An);
+    const Tn = "active",
+        On = "fade",
+        Cn = "show",
+        kn = ".active",
+        Ln = ":scope > li > .active";
+    class xn extends B {
+        static get NAME() {
+            return "tab"
+        }
+        show() {
+            if (this._element.parentNode && this._element.parentNode.nodeType === Node.ELEMENT_NODE && this._element.classList.contains(Tn)) return;
+            let t;
+            const e = n(this._element),
+                i = this._element.closest(".nav, .list-group");
+            if (i) {
+                const e = "UL" === i.nodeName || "OL" === i.nodeName ? Ln : kn;
+                t = V.find(e, i), t = t[t.length - 1]
+            }
+            const s = t ? j.trigger(t, "hide.bs.tab", {
+                relatedTarget: this._element
+            }) : null;
+            if (j.trigger(this._element, "show.bs.tab", {
+                    relatedTarget: t
+                }).defaultPrevented || null !== s && s.defaultPrevented) return;
+            this._activate(this._element, i);
+            const o = () => {
+                j.trigger(t, "hidden.bs.tab", {
+                    relatedTarget: this._element
+                }), j.trigger(this._element, "shown.bs.tab", {
                     relatedTarget: t
                 })
-            }, n._clear = function() {
-                [].slice.call(document.querySelectorAll(this._selector)).filter((function(t) {
-                    return t.classList.contains("active")
-                })).forEach((function(t) {
-                    return t.classList.remove("active")
-                }))
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this).data("bs.scrollspy");
-                    if (i || (i = new t(this, "object" == typeof n && n), e(this).data("bs.scrollspy", i)), "string" == typeof n) {
-                        if ("undefined" == typeof i[n]) throw new TypeError('No method named "' + n + '"');
-                        i[n]()
-                    }
-                }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return le
-                }
-            }]), t
-        }();
-    e(window).on("load.bs.scrollspy.data-api", (function() {
-        for (var t = [].slice.call(document.querySelectorAll('[data-spy="scroll"]')), n = t.length; n--;) {
-            var i = e(t[n]);
-            he._jQueryInterface.call(i, i.data())
+            };
+            e ? this._activate(e, e.parentNode, o) : o()
         }
-    })), e.fn[se] = he._jQueryInterface, e.fn[se].Constructor = he, e.fn[se].noConflict = function() {
-        return e.fn[se] = ae, he._jQueryInterface
-    };
-    var ue = e.fn.tab,
-        fe = function() {
-            function t(t) {
-                this._element = t
-            }
-            var n = t.prototype;
-            return n.show = function() {
-                var t = this;
-                if (!(this._element.parentNode && this._element.parentNode.nodeType === Node.ELEMENT_NODE && e(this._element).hasClass("active") || e(this._element).hasClass("disabled"))) {
-                    var n, i, o = e(this._element).closest(".nav, .list-group")[0],
-                        r = s.getSelectorFromElement(this._element);
-                    if (o) {
-                        var a = "UL" === o.nodeName || "OL" === o.nodeName ? "> li > .active" : ".active";
-                        i = (i = e.makeArray(e(o).find(a)))[i.length - 1]
-                    }
-                    var l = e.Event("hide.bs.tab", {
-                            relatedTarget: this._element
-                        }),
-                        c = e.Event("show.bs.tab", {
-                            relatedTarget: i
-                        });
-                    if (i && e(i).trigger(l), e(this._element).trigger(c), !c.isDefaultPrevented() && !l.isDefaultPrevented()) {
-                        r && (n = document.querySelector(r)), this._activate(this._element, o);
-                        var h = function() {
-                            var n = e.Event("hidden.bs.tab", {
-                                    relatedTarget: t._element
-                                }),
-                                o = e.Event("shown.bs.tab", {
-                                    relatedTarget: i
-                                });
-                            e(i).trigger(n), e(t._element).trigger(o)
-                        };
-                        n ? this._activate(n, n.parentNode, h) : h()
-                    }
-                }
-            }, n.dispose = function() {
-                e.removeData(this._element, "bs.tab"), this._element = null
-            }, n._activate = function(t, n, i) {
-                var o = this,
-                    r = (!n || "UL" !== n.nodeName && "OL" !== n.nodeName ? e(n).children(".active") : e(n).find("> li > .active"))[0],
-                    a = i && r && e(r).hasClass("fade"),
-                    l = function() {
-                        return o._transitionComplete(t, r, i)
-                    };
-                if (r && a) {
-                    var c = s.getTransitionDurationFromElement(r);
-                    e(r).removeClass("show").one(s.TRANSITION_END, l).emulateTransitionEnd(c)
-                } else l()
-            }, n._transitionComplete = function(t, n, i) {
-                if (n) {
-                    e(n).removeClass("active");
-                    var o = e(n.parentNode).find("> .dropdown-menu .active")[0];
-                    o && e(o).removeClass("active"), "tab" === n.getAttribute("role") && n.setAttribute("aria-selected", !1)
-                }
-                if (e(t).addClass("active"), "tab" === t.getAttribute("role") && t.setAttribute("aria-selected", !0), s.reflow(t), t.classList.contains("fade") && t.classList.add("show"), t.parentNode && e(t.parentNode).hasClass("dropdown-menu")) {
-                    var r = e(t).closest(".dropdown")[0];
-                    if (r) {
-                        var a = [].slice.call(r.querySelectorAll(".dropdown-toggle"));
-                        e(a).addClass("active")
-                    }
-                    t.setAttribute("aria-expanded", !0)
+        _activate(t, e, i) {
+            const n = (!e || "UL" !== e.nodeName && "OL" !== e.nodeName ? V.children(e, kn) : V.find(Ln, e))[0],
+                s = i && n && n.classList.contains(On),
+                o = () => this._transitionComplete(t, n, i);
+            n && s ? (n.classList.remove(Cn), this._queueCallback(o, t, !0)) : o()
+        }
+        _transitionComplete(t, e, i) {
+            if (e) {
+                e.classList.remove(Tn);
+                const t = V.findOne(":scope > .dropdown-menu .active", e.parentNode);
+                t && t.classList.remove(Tn), "tab" === e.getAttribute("role") && e.setAttribute("aria-selected", !1)
+            }
+            t.classList.add(Tn), "tab" === t.getAttribute("role") && t.setAttribute("aria-selected", !0), u(t), t.classList.contains(On) && t.classList.add(Cn);
+            let n = t.parentNode;
+            if (n && "LI" === n.nodeName && (n = n.parentNode), n && n.classList.contains("dropdown-menu")) {
+                const e = t.closest(".dropdown");
+                e && V.find(".dropdown-toggle", e).forEach((t => t.classList.add(Tn))), t.setAttribute("aria-expanded", !0)
+            }
+            i && i()
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = xn.getOrCreateInstance(this);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    e[t]()
                 }
-                i && i()
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this),
-                        o = i.data("bs.tab");
-                    if (o || (o = new t(this), i.data("bs.tab", o)), "string" == typeof n) {
-                        if ("undefined" == typeof o[n]) throw new TypeError('No method named "' + n + '"');
-                        o[n]()
-                    }
-                }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }]), t
-        }();
-    e(document).on("click.bs.tab.data-api", '[data-toggle="tab"], [data-toggle="pill"], [data-toggle="list"]', (function(t) {
-        t.preventDefault(), fe._jQueryInterface.call(e(this), "show")
-    })), e.fn.tab = fe._jQueryInterface, e.fn.tab.Constructor = fe, e.fn.tab.noConflict = function() {
-        return e.fn.tab = ue, fe._jQueryInterface
-    };
-    var de = e.fn.toast,
-        pe = {
+            }))
+        }
+    }
+    j.on(document, "click.bs.tab.data-api", '[data-bs-toggle="tab"], [data-bs-toggle="pill"], [data-bs-toggle="list"]', (function(t) {
+        ["A", "AREA"].includes(this.tagName) && t.preventDefault(), c(this) || xn.getOrCreateInstance(this).show()
+    })), g(xn);
+    const Dn = "toast",
+        Sn = "hide",
+        Nn = "show",
+        In = "showing",
+        Pn = {
             animation: "boolean",
             autohide: "boolean",
             delay: "number"
         },
-        me = {
+        jn = {
             animation: !0,
             autohide: !0,
-            delay: 500
-        },
-        ge = function() {
-            function t(t, e) {
-                this._element = t, this._config = this._getConfig(e), this._timeout = null, this._setListeners()
-            }
-            var n = t.prototype;
-            return n.show = function() {
-                var t = this,
-                    n = e.Event("show.bs.toast");
-                if (e(this._element).trigger(n), !n.isDefaultPrevented()) {
-                    this._clearTimeout(), this._config.animation && this._element.classList.add("fade");
-                    var i = function() {
-                        t._element.classList.remove("showing"), t._element.classList.add("show"), e(t._element).trigger("shown.bs.toast"), t._config.autohide && (t._timeout = setTimeout((function() {
-                            t.hide()
-                        }), t._config.delay))
-                    };
-                    if (this._element.classList.remove("hide"), s.reflow(this._element), this._element.classList.add("showing"), this._config.animation) {
-                        var o = s.getTransitionDurationFromElement(this._element);
-                        e(this._element).one(s.TRANSITION_END, i).emulateTransitionEnd(o)
-                    } else i()
-                }
-            }, n.hide = function() {
-                if (this._element.classList.contains("show")) {
-                    var t = e.Event("hide.bs.toast");
-                    e(this._element).trigger(t), t.isDefaultPrevented() || this._close()
-                }
-            }, n.dispose = function() {
-                this._clearTimeout(), this._element.classList.contains("show") && this._element.classList.remove("show"), e(this._element).off("click.dismiss.bs.toast"), e.removeData(this._element, "bs.toast"), this._element = null, this._config = null
-            }, n._getConfig = function(t) {
-                return t = o({}, me, e(this._element).data(), "object" == typeof t && t ? t : {}), s.typeCheckConfig("toast", t, this.constructor.DefaultType), t
-            }, n._setListeners = function() {
-                var t = this;
-                e(this._element).on("click.dismiss.bs.toast", '[data-dismiss="toast"]', (function() {
-                    return t.hide()
-                }))
-            }, n._close = function() {
-                var t = this,
-                    n = function() {
-                        t._element.classList.add("hide"), e(t._element).trigger("hidden.bs.toast")
-                    };
-                if (this._element.classList.remove("show"), this._config.animation) {
-                    var i = s.getTransitionDurationFromElement(this._element);
-                    e(this._element).one(s.TRANSITION_END, n).emulateTransitionEnd(i)
-                } else n()
-            }, n._clearTimeout = function() {
-                clearTimeout(this._timeout), this._timeout = null
-            }, t._jQueryInterface = function(n) {
-                return this.each((function() {
-                    var i = e(this),
-                        o = i.data("bs.toast");
-                    if (o || (o = new t(this, "object" == typeof n && n), i.data("bs.toast", o)), "string" == typeof n) {
-                        if ("undefined" == typeof o[n]) throw new TypeError('No method named "' + n + '"');
-                        o[n](this)
-                    }
-                }))
-            }, i(t, null, [{
-                key: "VERSION",
-                get: function() {
-                    return "4.5.2"
-                }
-            }, {
-                key: "DefaultType",
-                get: function() {
-                    return pe
-                }
-            }, {
-                key: "Default",
-                get: function() {
-                    return me
-                }
-            }]), t
-        }();
-    e.fn.toast = ge._jQueryInterface, e.fn.toast.Constructor = ge, e.fn.toast.noConflict = function() {
-        return e.fn.toast = de, ge._jQueryInterface
-    }, t.Alert = c, t.Button = u, t.Carousel = v, t.Collapse = T, t.Dropdown = Lt, t.Modal = Ht, t.Popover = re, t.Scrollspy = he, t.Tab = fe, t.Toast = ge, t.Tooltip = Jt, t.Util = s, Object.defineProperty(t, "__esModule", {
-        value: !0
-    })
+            delay: 5e3
+        };
+    class Mn extends B {
+        constructor(t, e) {
+            super(t), this._config = this._getConfig(e), this._timeout = null, this._hasMouseInteraction = !1, this._hasKeyboardInteraction = !1, this._setListeners()
+        }
+        static get DefaultType() {
+            return Pn
+        }
+        static get Default() {
+            return jn
+        }
+        static get NAME() {
+            return Dn
+        }
+        show() {
+            j.trigger(this._element, "show.bs.toast").defaultPrevented || (this._clearTimeout(), this._config.animation && this._element.classList.add("fade"), this._element.classList.remove(Sn), u(this._element), this._element.classList.add(Nn), this._element.classList.add(In), this._queueCallback((() => {
+                this._element.classList.remove(In), j.trigger(this._element, "shown.bs.toast"), this._maybeScheduleHide()
+            }), this._element, this._config.animation))
+        }
+        hide() {
+            this._element.classList.contains(Nn) && (j.trigger(this._element, "hide.bs.toast").defaultPrevented || (this._element.classList.add(In), this._queueCallback((() => {
+                this._element.classList.add(Sn), this._element.classList.remove(In), this._element.classList.remove(Nn), j.trigger(this._element, "hidden.bs.toast")
+            }), this._element, this._config.animation)))
+        }
+        dispose() {
+            this._clearTimeout(), this._element.classList.contains(Nn) && this._element.classList.remove(Nn), super.dispose()
+        }
+        _getConfig(t) {
+            return t = {
+                ...jn,
+                ...U.getDataAttributes(this._element),
+                ..."object" == typeof t && t ? t : {}
+            }, a(Dn, t, this.constructor.DefaultType), t
+        }
+        _maybeScheduleHide() {
+            this._config.autohide && (this._hasMouseInteraction || this._hasKeyboardInteraction || (this._timeout = setTimeout((() => {
+                this.hide()
+            }), this._config.delay)))
+        }
+        _onInteraction(t, e) {
+            switch (t.type) {
+                case "mouseover":
+                case "mouseout":
+                    this._hasMouseInteraction = e;
+                    break;
+                case "focusin":
+                case "focusout":
+                    this._hasKeyboardInteraction = e
+            }
+            if (e) return void this._clearTimeout();
+            const i = t.relatedTarget;
+            this._element === i || this._element.contains(i) || this._maybeScheduleHide()
+        }
+        _setListeners() {
+            j.on(this._element, "mouseover.bs.toast", (t => this._onInteraction(t, !0))), j.on(this._element, "mouseout.bs.toast", (t => this._onInteraction(t, !1))), j.on(this._element, "focusin.bs.toast", (t => this._onInteraction(t, !0))), j.on(this._element, "focusout.bs.toast", (t => this._onInteraction(t, !1)))
+        }
+        _clearTimeout() {
+            clearTimeout(this._timeout), this._timeout = null
+        }
+        static jQueryInterface(t) {
+            return this.each((function() {
+                const e = Mn.getOrCreateInstance(this, t);
+                if ("string" == typeof t) {
+                    if (void 0 === e[t]) throw new TypeError(`No method named "${t}"`);
+                    e[t](this)
+                }
+            }))
+        }
+    }
+    return R(Mn), g(Mn), {
+        Alert: W,
+        Button: z,
+        Carousel: st,
+        Collapse: pt,
+        Dropdown: hi,
+        Modal: Hi,
+        Offcanvas: Fi,
+        Popover: gn,
+        ScrollSpy: An,
+        Tab: xn,
+        Toast: Mn,
+        Tooltip: un
+    }
 }));
 //# sourceMappingURL=bootstrap.bundle.min.js.map
```

### Comparing `django-ddm-0.1.9/ddm/static/ddm/vue/favicon.ico` & `django-ddm-1.0.0/ddm/static/ddm/vue/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-ddm-0.1.9/ddm/templates/ddm/project_admin/blueprint/delete.html` & `django-ddm-1.0.0/ddm/templates/ddm/admin/data_donation/donation_blueprint/delete.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,64 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %}
+{% extends 'ddm/admin/generic/page_with_form.html' %}
 
-{% block page_title %}Delete Blueprint{% endblock %}
+{% block page_title %}Delete File Blueprint{% endblock %}
 
-{% block main_heading %}Delete Blueprint "{{ object.name }}"{% endblock %}
+{% block main_heading %}Delete File Blueprint "{{ object.name }}"{% endblock %}
 
 {% block main_top %}
 <p>You are about to delete the following blueprint:</p>
-<div>
-  <table class="table">
-    <tr>
-      <td style="width: 16%">Name:</td>
-      <td>{{ object.name }}</td>
-    </tr>
-    <tr>
-      <td>File Format:</td>
-      <td>{{ object.exp_file_format }}</td>
-    </tr>
-    <tr>
-      <td>Expected Fields:</td>
-      <td>{{ object.expected_fields }}</td>
-    </tr>
-    <tr>
-      <td>Extracted Fields:</td>
-      <td>{{ object.extracted_fields }}</td>
-    </tr>
-  </table>
+
+<div class="ddm-admin-form">
+  <p>
+    <label>Name:</label>
+    {{ object.name }}
+  </p>
+
+  <p>
+    <label>File Format:</label>
+    {{ object.exp_file_format }}
+  </p>
 </div>
-<div>
-  <div>All collected data associated with this blueprint will also be deleted.</div>
+
+<div class="mt-4">
   <div>
     <p>The following questions and instructions associated with this blueprint will also be deleted:</p>
-    <div>
+    <div class="ddm-admin-form">
       <p><b>Instructions:</b></p>
       <ul>
         {% for instruction in object.instruction_set.all %}
         <li>{{ instruction }}</li>
         {% empty %}
-        No instructions associated to this blueprint were found.
+        No instructions associated with this blueprint were found.
         {% endfor %}
       </ul>
-    </div>
-    <div>
       <p><b>Questions:</b></p>
       <ul>
         {% for question in object.questionbase_set.all %}
         <li>{{ question }}</li>
         {% empty %}
-        No questions associated to this blueprint were found.
+        No questions associated with this blueprint were found.
         {% endfor %}
       </ul>
     </div>
   </div>
 </div>
-{% endblock %}
 
-{% block main_form %}
 <form method='post'>
   {% csrf_token %}
-  <p>Are you sure you want to delete this blueprint along with all associated data, questions, and instructions? <b>This action cannot be reversed.</b></p>
-  <input class="btn-a btn-danger" type="submit" value="Delete blueprint">
+  <p><b>Are you sure you want to delete this blueprint along with all associated data donations, and questions? This action cannot be reversed.</b></p>
+  <input class="ddm-btn ddm-btn-red" type="submit" value="Delete Donation Blueprint">
+  <p class="mt-3">
+    <a href="{% url 'data-donation-overview' project.pk %}">&#129040; Cancel</a>
+  </p>
 </form>
 {% endblock %}
 
+{% block main_form %}{% endblock %}
+
+
 {% block breadcrumbs %}
-Back to:
 <a href="{% url 'project-list' %}">Projects</a> /
-<a href="{% url 'project-detail' project_pk %}">Project Cockpit</a> /
-<a href="{% url 'blueprint-list' project_pk %}">Donation Blueprints</a>
+<a href="{% url 'project-detail' project.pk %}">"{{ project.name|truncatechars:15 }}" Project</a> /
+<a href="{% url 'data-donation-overview' project.pk %}">Data Donation</a> /
+Delete Blueprint
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,28 +1,26 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %} {% block
-page_title %}Delete Blueprint{% endblock %} {% block main_heading %}Delete
+{% extends 'ddm/admin/generic/page_with_form.html' %} {% block page_title
+%}Delete File Blueprint{% endblock %} {% block main_heading %}Delete File
 Blueprint "{{ object.name }}"{% endblock %} {% block main_top %}
 You are about to delete the following blueprint:
-Name:             {{ object.name }}
-File Format:      {{ object.exp_file_format }}
-Expected Fields:  {{ object.expected_fields }}
-Extracted Fields: {{ object.extracted_fields }}
-All collected data associated with this blueprint will also be deleted.
+Name: {{ object.name }}
+File Format: {{ object.exp_file_format }}
 The following questions and instructions associated with this blueprint will
 also be deleted:
 Instructions:
     * {% for instruction in object.instruction_set.all %}
     * {{ instruction }}
-    * {% empty %} No instructions associated to this blueprint were found. {%
+    * {% empty %} No instructions associated with this blueprint were found. {%
       endfor %}
 Questions:
     * {% for question in object.questionbase_set.all %}
     * {{ question }}
-    * {% empty %} No questions associated to this blueprint were found. {%
+    * {% empty %} No questions associated with this blueprint were found. {%
       endfor %}
-{% endblock %} {% block main_form %}
 {% csrf_token %}
-Are you sure you want to delete this blueprint along with all associated data,
-questions, and instructions? This action cannot be reversed.
-[Delete blueprint]
-{% endblock %} {% block breadcrumbs %} Back to: Projects / Project_Cockpit /
-Donation_Blueprints {% endblock %}
+Are you sure you want to delete this blueprint along with all associated data
+donations, and questions? This action cannot be reversed.
+[Delete Donation Blueprint]
+_Cancel
+{% endblock %} {% block main_form %}{% endblock %} {% block breadcrumbs %}
+Projects / "{{_project.name|truncatechars:15_}}"_Project / Data_Donation /
+Delete Blueprint {% endblock %}
```

### Comparing `django-ddm-0.1.9/ddm/templates/ddm/project_admin/instructions/delete.html` & `django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/delete.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,41 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %}
+{% extends 'ddm/admin/generic/page_with_form.html' %}
 
-{% block page_title %}Delete Instruction{% endblock %}
+{% block page_title %}Delete Question{% endblock %}
 
-{% block main_heading %}Delete Instruction Page{% endblock %}
+{% block main_heading %}Delete Question "{{ object.name }}"{% endblock %}
 
-{% block main_top %}
-<p>You are about to delete the following instruction page:</p>
-<div>
-  <table class="table">
-    <tr>
-      {% if object.blueprint %}
-      <td style="width: 16%">Related blueprint:</td>
-      <td>{{ object.blueprint }}</td>
-      {% elif object.zip_blueprint.name %}
-      <td>Zipped Blueprint:</td>
-      <td>{{ object.zip_blueprint.name }}</td>
-      {% endif %}
-    </tr>
-    <tr>
-      <td>Index:</td>
-      <td>{{ object.index }}</td>
-    </tr>
-    <tr>
-      <td>Text:</td>
-      <td>{{ object.text | safe }}</td>
-    </tr>
-  </table>
-</div>
-{% endblock %}
-
-
-{% block main_form%}
+{% block main_form %}
 <form method='post'>
   {% csrf_token %}
-  <p>Are you sure you want to delete this instruction page? <b>This action cannot be reversed.</b></p>
-  <input class="btn-a btn-danger" type="submit" value="Delete instruction page">
+  <p>You are about to delete the following question:</p>
+  <div>
+    <table>
+      <tr>
+        <td>Name:</td>
+        <td>{{ object.name }}</td>
+      </tr>
+      <tr>
+        <td>Blueprint:</td>
+        <td>{{ object.blueprint }}</td>
+      </tr>
+      <tr>
+        <td>Question Type:</td>
+        <td>{{ object.question_type.label }}</td>
+      </tr>
+    </table>
+  </div>
+  <p>All collected data associated with this question will also be deleted. <b>This action cannot be reversed.</b></p>
+  <p>Are you sure you want to delete this question?</p>
+  <input class="ddm-btn ddm-btn-red" type="submit" value="Delete Question">
+  <p class="mt-3">
+    <a href="{% url 'questionnaire-overview' project_pk %}">&#129040; Cancel</a>
+  </p>
 </form>
 {% endblock %}
 
-
 {% block breadcrumbs %}
-Back to:
 <a href="{% url 'project-list' %}">Projects</a> /
-<a href="{% url 'project-detail' project_pk %}">Project Cockpit</a> /
-<a href="{% url 'blueprint-list' project_pk %}">Donation Blueprints</a> /
-<a href="{% url 'instruction-overview' project_pk blueprint.get_slug blueprint.pk %}">Instruction Overview</a>
+<a href="{% url 'project-detail' project_pk %}">"{{ project.name|truncatechars:15 }}" Project</a> /
+<a href="{% url 'questionnaire-overview' project_pk %}">Questionnaire</a> /
+Delete Question
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,16 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %} {% block
-page_title %}Delete Instruction{% endblock %} {% block main_heading %}Delete
-Instruction Page{% endblock %} {% block main_top %}
-You are about to delete the following instruction page:
-           {                                    {
-Related    { object.blueprint Zipped Blueprint: {
-blueprint: }}                                   object.zip_blueprint.name
-                                                }}
-Index:     {{ object.index }}
-Text:      {{ object.text |
-           safe }}
-{% endblock %} {% block main_form%}
+{% extends 'ddm/admin/generic/page_with_form.html' %} {% block page_title
+%}Delete Question{% endblock %} {% block main_heading %}Delete Question "{
+{ object.name }}"{% endblock %} {% block main_form %}
 {% csrf_token %}
-Are you sure you want to delete this instruction page? This action cannot be
-reversed.
-[Delete instruction page]
-{% endblock %} {% block breadcrumbs %} Back to: Projects / Project_Cockpit /
-Donation_Blueprints / Instruction_Overview {% endblock %}
+You are about to delete the following question:
+Name:          {{ object.name }}
+Blueprint:     {{ object.blueprint }}
+Question Type: {{ object.question_type.label }}
+All collected data associated with this question will also be deleted. This
+action cannot be reversed.
+Are you sure you want to delete this question?
+[Delete Question]
+_Cancel
+{% endblock %} {% block breadcrumbs %} Projects / "{
+{_project.name|truncatechars:15_}}"_Project / Questionnaire / Delete Question
+{% endblock %}
```

### Comparing `django-ddm-0.1.9/ddm/templates/ddm/project_admin/project/list.html` & `django-ddm-1.0.0/ddm/templates/ddm/admin/project/list.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'ddm/project_admin/base.html' %}
+{% extends 'ddm/admin/base.html' %}
 
 {% block page_title %}Donation Projects{% endblock %}
 
 {% block main_heading %}Donation Projects{% endblock %}
 
 {% block main_body %}
 <div>
@@ -12,22 +12,26 @@
       <th>Slug</th>
       <th></th>
     </tr>
     {% for project in object_list %}
     <tr>
       <td>{{ project.name }}</td>
       <td>{{ project.slug }}</td>
-      <td><a href="{{ project.get_absolute_url }}">Show Project</a></td>
+      <td><a href="{{ project.get_absolute_url }}">Go to Project Hub</a></td>
     </tr>
     {% empty %}
     <tr>
       <td>No projects found.</td>
     </tr>
     {% endfor %}
   </table>
 </div>
 
 <div>
-  <a class="btn btn-secondary" href="{% url 'project-create' %}"><b>+</b>&nbsp;&nbsp;Create New Project</a>
+  <a class="ddm-btn" href="{% url 'project-create' %}"><b>+</b>&nbsp;&nbsp;Create New Project</a>
 </div>
 
 {% endblock %}
+
+{% block breadcrumbs %}
+Projects
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends 'ddm/project_admin/base.html' %} {% block page_title %}Donation
-Projects{% endblock %} {% block main_heading %}Donation Projects{% endblock %}
-{% block main_body %}
+{% extends 'ddm/admin/base.html' %} {% block page_title %}Donation Projects{%
+endblock %} {% block main_heading %}Donation Projects{% endblock %} {% block
+main_body %}
 Name               Slug
-{{ project.name }} {{ project.slug }} Show_Project
+{{ project.name }} {{ project.slug }} Go_to_Project_Hub
 No projects found.
 +  Create_New_Project
-{% endblock %}
+{% endblock %} {% block breadcrumbs %} Projects {% endblock %}
```

### Comparing `django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/delete.html` & `django-ddm-1.0.0/ddm/templates/ddm/admin/project/delete.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %}
+{% extends 'ddm/admin/generic/page_with_form.html' %}
 
-{% block page_title %}Delete Question{% endblock %}
+{% block page_title %}Delete Project{% endblock %}
 
-{% block main_heading %}Delete Question "{{ object.name }}"{% endblock %}
+{% block main_heading %}Delete the Project "{{ object.name }}"{% endblock %}
 
 {% block main_form %}
 <form method='post'>
   {% csrf_token %}
-  <p>You are about to delete the following question:</p>
-  <div>
-    <table>
-      <tr>
-        <td>Name:</td>
-        <td>{{ object.name }}</td>
-      </tr>
-      <tr>
-        <td>Blueprint:</td>
-        <td>{{ object.blueprint }}</td>
-      </tr>
-      <tr>
-        <td>Question Type:</td>
-        <td>{{ object.question_type.label }}</td>
-      </tr>
-    </table>
+  <p>You are about to delete the following project:</p>
+  <div class="ddm-admin-form">
+    <p>
+      <label>Name:</label>
+      {{ object.name }}
+    </p>
+    <p>
+      <label>Slug:</label>
+      {{ object.slug }}
+    </p>
   </div>
-  <p>All collected data associated with this question will also be deleted. <b>This action cannot be reversed.</b></p>
-  <p>Are you sure you want to delete this question?</p>
-  <input class="btn-a btn-danger" type="submit" value="Delete question">
+  <div class="mt-4">
+    <p>All collected data associated with this project will also be deleted. <b>This action cannot be reversed.</b></p>
+    <p>Are you sure you want to delete this project?</p>
+  </div>
+  <input class="ddm-btn ddm-btn-red" type="submit" value="Delete project">
+  <p class="mt-3">
+    <a href="{% url 'project-detail' object.pk %}">&#129040; Cancel</a>
+  </p>
 </form>
 {% endblock %}
 
 {% block breadcrumbs %}
-Back to:
 <a href="{% url 'project-list' %}">Projects</a> /
-<a href="{% url 'project-detail' project_pk %}">Project Cockpit</a> /
-<a href="{% url 'questionnaire-overview' project_pk %}">Questionnaire</a>
+<a href="{% url 'project-detail' object.pk %}">"{{ object.name|truncatechars:15 }}" Project</a> /
+Delete
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %} {% block
-page_title %}Delete Question{% endblock %} {% block main_heading %}Delete
-Question "{{ object.name }}"{% endblock %} {% block main_form %}
+{% extends 'ddm/admin/generic/page_with_form.html' %} {% block page_title
+%}Delete Project{% endblock %} {% block main_heading %}Delete the Project "{
+{ object.name }}"{% endblock %} {% block main_form %}
 {% csrf_token %}
-You are about to delete the following question:
-Name:          {{ object.name }}
-Blueprint:     {{ object.blueprint }}
-Question Type: {{ object.question_type.label }}
-All collected data associated with this question will also be deleted. This
+You are about to delete the following project:
+Name: {{ object.name }}
+Slug: {{ object.slug }}
+All collected data associated with this project will also be deleted. This
 action cannot be reversed.
-Are you sure you want to delete this question?
-[Delete question]
-{% endblock %} {% block breadcrumbs %} Back to: Projects / Project_Cockpit /
-Questionnaire {% endblock %}
+Are you sure you want to delete this project?
+[Delete project]
+_Cancel
+{% endblock %} {% block breadcrumbs %} Projects / "{
+{_object.name|truncatechars:15_}}"_Project / Delete {% endblock %}
```

### Comparing `django-ddm-0.1.9/ddm/templates/ddm/project_admin/questionnaire/edit_set.html` & `django-ddm-1.0.0/ddm/templates/ddm/admin/questionnaire/edit_set.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,57 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %}
+{% extends 'ddm/admin/generic/page_with_form.html' %}
 
 {% block page_title %}Edit {{ context_title }}{% endblock %}
 
 {% block main_heading %}Edit {{ context_title }} for "{{ question.name }}"{% endblock %}
 
 {% block main_form %}
 <form method="post">
   {% csrf_token %}
+  {{ formset.management_form }}
   <table class="table mt-4">
-    {{ formset.management_form }}
 
     {% for form in formset.forms %}
 
     {% if forloop.first %}
     <thead>
     <tr>
       {% for field in form.visible_fields %}<th>{{ field.label }}</th>{% endfor %}
     </tr>
     </thead>
     {% endif %}
 
-    <tbody>
+    {% if form.non_field_errors %}
+      <tr><td class="border-bottom-0">{{ form.non_field_errors }}</td></tr>
+    {% endif %}
+
     <tr>
       {% for field in form.visible_fields %}
       <td>
         {% if forloop.first %}
         {% for hidden in form.hidden_fields %}
         {{ hidden }}
         {% endfor %}
         {% endif %}
         {{ field.errors.as_ul }}
         {{ field }}
       </td>
       {% endfor %}
     </tr>
-    </tbody>
 
     {% endfor %}
   </table>
-  <input class="btn btn-secondary" type="submit" value="Update {{ context_title }}">
+  <input class="ddm-btn" type="submit" value="Update {{ context_title }}">
+  <p class="mt-3">
+    <a href="{% url 'question-edit' project_pk question.question_type question.pk %}">&#129040; Back</a>
+  </p>
 </form>
 {% endblock %}
 
 {% block breadcrumbs %}
-Back to:
 <a href="{% url 'project-list' %}">Projects</a> /
-<a href="{% url 'project-detail' project_pk %}">Project Cockpit</a> /
+<a href="{% url 'project-detail' project_pk %}">"{{ project.name|truncatechars:15 }}" Project</a> /
 <a href="{% url 'questionnaire-overview' project_pk %}">Questionnaire</a> /
-<a href="{% url 'question-edit' project_pk question.question_type question.pk %}">Question</a>
+<a href="{% url 'question-edit' project_pk question.question_type question.pk %}">Question</a> /
+Items
 {% endblock %}
+
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
-{% extends 'ddm/project_admin/generic/page_with_form.html' %} {% block
-page_title %}Edit {{ context_title }}{% endblock %} {% block main_heading
-%}Edit {{ context_title }} for "{{ question.name }}"{% endblock %} {% block
-main_form %}
-{% csrf_token %}
+{% extends 'ddm/admin/generic/page_with_form.html' %} {% block page_title
+%}Edit {{ context_title }}{% endblock %} {% block main_heading %}Edit {
+{ context_title }} for "{{ question.name }}"{% endblock %} {% block main_form
+%}
+{% csrf_token %} {{ formset.management_form }}
 {{ field.label }}
+{{ form.non_field_errors }}
 {% if forloop.first %} {% for hidden in form.hidden_fields %} {{ hidden }} {%
 endfor %} {% endif %} {{ field.errors.as_ul }} {{ field }}
 [Update {{ context_title }}]
-{% endblock %} {% block breadcrumbs %} Back to: Projects / Project_Cockpit /
-Questionnaire / Question {% endblock %}
+_Back
+{% endblock %} {% block breadcrumbs %} Projects / "{
+{_project.name|truncatechars:15_}}"_Project / Questionnaire / Question / Items
+{% endblock %}
```

### Comparing `django-ddm-0.1.9/ddm/templates/ddm/public/questionnaire.html` & `django-ddm-1.0.0/ddm/templates/ddm/public/data_donation.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 {% extends "ddm/public/base.html" %}
-{% load static %}
+{% load i18n %}
 {% load render_bundle from webpack_loader %}
-
-{% block extrahead %}
-<link href="{% static 'ddm/css/questionnaire.css' %}" rel="stylesheet">
-{% endblock extrahead %}
+{% get_current_language as LANGUAGE_CODE %}
 
 {% block content %}
-<div>
-  <form method="POST">
+<div class="container">
+  <form id="uploader-form" method="POST" enctype="multipart/form-data">
     {% csrf_token %}
-    <div id="qapp"
-         data-qconfig='{{ q_config }}'
-         data-actionurl='{{ request.build_absolute_uri }}'
-         class="text-black"
+    <div id="uapp"
+         class="container text-black"
+         data-upload-config='{{ uploader_configs }}'
+         data-action-url='{{ request.build_absolute_uri }}'
+         data-exception-url='{% if request.is_secure %}https://{% else %}http://{% endif %}{{ request.get_host }}{% url "ddm-exceptions-api" project_id %}'
+         data-language='{{ LANGUAGE_CODE|slice:"0:2"}}'
     >
-      <qapp></qapp>
+      <uapp></uapp>
     </div>
+    {% render_bundle 'vue_uploader' %}
   </form>
-  {% render_bundle 'vue_questionnaire' %}
 </div>
 {% endblock content %}
```

### Comparing `django-ddm-0.1.9/ddm/views/project_admin/questionnaire.py` & `django-ddm-1.0.0/ddm/views/admin/questionnaire.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,72 @@
-from django.contrib.auth.mixins import LoginRequiredMixin
+from django.contrib import messages
+from django.contrib.messages.views import SuccessMessageMixin
 from django.forms import inlineformset_factory
 from django.urls import reverse
+from django.views.generic import ListView
 from django.views.generic.edit import CreateView, UpdateView, DeleteView
 
-from ddm.models import (
+from ddm.models.core import DonationBlueprint, DonationProject
+from ddm.models.questions import (
     QuestionBase, QuestionType, SingleChoiceQuestion, MultiChoiceQuestion,
     OpenQuestion, MatrixQuestion, SemanticDifferential, Transition, QuestionItem,
     ScalePoint
 )
-from . import ProjectBlueprintList
+from . import DdmAuthMixin
 
 
 class ProjectMixin:
     """ Mixin for all blueprint related views. """
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context.update({'project_pk': self.kwargs['project_pk']})
+        context.update({'project': self.get_project()})
         return context
 
+    def get_project(self):
+        return DonationProject.objects.get(pk=self.kwargs['project_pk'])
 
-class QuestionnaireOverview(ProjectBlueprintList):
+
+class QuestionnaireOverview(ProjectMixin, DdmAuthMixin, ListView):
     """ View to list all donation blueprints associated with a project. """
-    template_name = 'ddm/project_admin/questionnaire/list.html'
+    model = DonationBlueprint
+    context_object_name = 'donation_blueprints'
+    template_name = 'ddm/admin/questionnaire/list.html'
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         question_types = QuestionType.choices
-        context.update({'question_types': question_types})
+        context.update({
+            'question_types': question_types,
+            'general_questions': self.get_general_questions()
+        })
         return context
 
+    def get_general_questions(self):
+        project = self.get_project()
+        return project.questionbase_set.filter(blueprint=None)
+
+    def get_queryset(self):
+        return super().get_queryset().filter(project_id=self.kwargs['project_pk'])
+
 
 class QuestionFormMixin(ProjectMixin):
     model = None
     fields = '__all__'
 
     QUESTION_CLASSES = {
         'single_choice': SingleChoiceQuestion,
         'multi_choice': MultiChoiceQuestion,
         'open': OpenQuestion,
         'matrix': MatrixQuestion,
         'semantic_diff': SemanticDifferential,
         'transition': Transition
     }
 
-    SHARED_FIELDS = ['name', 'blueprint', 'index', 'variable_name', 'text', 'required']
+    SHARED_FIELDS = ['name', 'blueprint', 'page', 'index', 'variable_name', 'text', 'required']
     QUESTION_FIELDS = {
         'single_choice': SHARED_FIELDS + ['randomize_items'],
         'multi_choice': SHARED_FIELDS + ['randomize_items'],
         'matrix': SHARED_FIELDS + ['randomize_items'],
         'semantic_diff': SHARED_FIELDS + ['randomize_items'],
         'open': SHARED_FIELDS,
         'transition': SHARED_FIELDS
@@ -58,52 +77,80 @@
         self.fields = self.QUESTION_FIELDS[self.kwargs['question_type']]
         return super().get_queryset()
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         question_type_label = QuestionType(self.kwargs['question_type']).label
         context.update({'question_type': question_type_label})
+        context['form'].fields['blueprint'].queryset = DonationBlueprint.objects.filter(
+            project_id=self.kwargs['project_pk'])
+        context['form'].fields['blueprint'].empty_label = 'General Question – no Blueprint assigned'
         return context
 
 
-class QuestionCreate(LoginRequiredMixin, QuestionFormMixin, CreateView):
+class QuestionCreate(SuccessMessageMixin, DdmAuthMixin, QuestionFormMixin, CreateView):
     """ View to create question. """
-    template_name = 'ddm/project_admin/questionnaire/create.html'
+    template_name = 'ddm/admin/questionnaire/create.html'
+    success_message = 'New %(question_type)s was created.'
 
     def get_initial(self):
         initial = super().get_initial()
         initial['question_type'] = self.kwargs['question_type']
         return initial
 
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
         kwargs['instance'] = self.QUESTION_CLASSES[self.kwargs['question_type']](
             project_id=self.kwargs['project_pk'],
         )
         return kwargs
 
     def get_success_url(self):
-        return reverse('questionnaire-overview', kwargs={'project_pk': self.kwargs['project_pk']})
+        kwargs = {
+            'project_pk': self.kwargs['project_pk'],
+            'question_type': self.kwargs['question_type'],
+            'pk': self.object.pk
+        }
+        return reverse('question-edit', kwargs=kwargs)
+
+    def get_success_message(self, cleaned_data):
+        return self.success_message % dict(
+            cleaned_data,
+            question_type=self.QUESTION_CLASSES[self.kwargs['question_type']].DEFAULT_QUESTION_TYPE.label
+        )
 
 
-class QuestionEdit(LoginRequiredMixin, QuestionFormMixin, UpdateView):
+class QuestionEdit(SuccessMessageMixin, DdmAuthMixin, QuestionFormMixin, UpdateView):
     """ View to edit question. """
     model = QuestionBase
-    template_name = 'ddm/project_admin/questionnaire/edit.html'
-    fields = '__all__'
+    template_name = 'ddm/admin/questionnaire/edit.html'
+    success_message = 'Question "%(name)s" was successfully updated.'
+
+    def get_success_url(self):
+        success_kwargs = {
+            'project_pk': self.kwargs['project_pk'],
+            'question_type': self.kwargs['question_type'],
+            'pk': self.kwargs['pk']
+        }
+        return reverse('question-edit', kwargs=success_kwargs)
 
 
-class QuestionDelete(LoginRequiredMixin, ProjectMixin, DeleteView):
+class QuestionDelete(DdmAuthMixin, ProjectMixin, DeleteView):
     """ View to delete question. """
     model = QuestionBase
-    template_name = 'ddm/project_admin/questionnaire/delete.html'
+    template_name = 'ddm/admin/questionnaire/delete.html'
+    success_message = 'Question "%s" was deleted.'
 
     def get_success_url(self):
         return reverse('questionnaire-overview', kwargs={'project_pk': self.kwargs['project_pk']})
 
+    def delete(self, request, *args, **kwargs):
+        messages.success(self.request, self.success_message % self.get_object().name)
+        return super().delete(request, *args, **kwargs)
+
 
 class InlineFormsetMixin(ProjectMixin):
     model = QuestionBase
     fields = '__all__'
     formset_model = None
     context_title = None
     fields_to_exclude = ()
@@ -135,31 +182,42 @@
     def get_excluded_fields(self):
         if not isinstance(self.object, SemanticDifferential):
             excluded_fields = ('label_alt',)
         else:
             excluded_fields = ()
         return excluded_fields
 
+
+class ItemEdit(SuccessMessageMixin, DdmAuthMixin, InlineFormsetMixin, UpdateView):
+    """ View to edit the items associated with a question. """
+    model = QuestionBase
+    formset_model = QuestionItem
+    template_name = 'ddm/admin/questionnaire/edit_set.html'
+    context_title = 'Items'
+    success_message = 'Question items updated.'
+
     def get_success_url(self):
         question = self.get_object()
         success_kwargs = {
             'project_pk': self.kwargs['project_pk'],
             'question_type': question.question_type,
             'pk': question.pk
         }
-        return reverse('question-edit', kwargs=success_kwargs)
-
-
-class ItemEdit(LoginRequiredMixin, InlineFormsetMixin, UpdateView):
-    """ View to edit the items associated with a question. """
-    model = QuestionBase
-    formset_model = QuestionItem
-    template_name = 'ddm/project_admin/questionnaire/edit_set.html'
-    context_title = 'Items'
+        return reverse('question-items', kwargs=success_kwargs)
 
 
-class ScaleEdit(LoginRequiredMixin, InlineFormsetMixin, UpdateView):
+class ScaleEdit(SuccessMessageMixin, DdmAuthMixin, InlineFormsetMixin, UpdateView):
     """ View to edit the scale associated with a question. """
     model = QuestionBase
     formset_model = ScalePoint
-    template_name = 'ddm/project_admin/questionnaire/edit_set.html'
+    template_name = 'ddm/admin/questionnaire/edit_set.html'
     context_title = 'Scale Points'
+    success_message = 'Question scale updated.'
+
+    def get_success_url(self):
+        question = self.get_object()
+        success_kwargs = {
+            'project_pk': self.kwargs['project_pk'],
+            'question_type': question.question_type,
+            'pk': question.pk
+        }
+        return reverse('question-scale', kwargs=success_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-ddm-0.1.9/django_ddm.egg-info/PKG-INFO` & `django-ddm-1.0.0/django_ddm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 Metadata-Version: 2.1
 Name: django-ddm
-Version: 0.1.9
+Version: 1.0.0
 Summary: A Django app to setup data donation projects.
 Home-page: https://github.com/uzh/ddm
 Author: Nico Pfiffner
 Author-email: n.pfiffner@ikmz.uzh.ch
-License: MIT
-Project-URL: Documentation, https://data-donation-module.readthedocs.io/
+License: GPLv3
+Project-URL: Documentation, https://uzh.github.io/ddm/
 Project-URL: Website, https://datadonation.uzh.ch
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 
 # Data Donation Module (ddm)
 
 > **_NOTE:_**  This package is currently under active development.
 
 **DDM** (Data Donation Module) is a Django application that helps researchers to
 setup data donation projects and to collect data donations for academic research.
 
 This is part of a larger initiative from the University of Zurich and the Digital
 Society Initiative to strengthen the exchange about the topic of data donations and
 promote this data collection approach. For more information, visit https://datadonation.uzh.ch.
 
-Documentation: https://data-donation-module.readthedocs.io/en/latest/ \
+Documentation: https://uzh.github.io/ddm/ddm/main/index.html \
 PyPi: https://pypi.org/project/django-ddm/
-
-
```

### Comparing `django-ddm-0.1.9/docs/source/for_developers.rst` & `django-ddm-1.0.0/docs/modules/ROOT/pages/for_developers.adoc`

 * *Files 23% similar despite different names*

```diff
@@ -1,151 +1,187 @@
-##############
-For Developers
-##############
+= Documentation for Developers
+:!toc:
+:icons: font
+:stem: latexmath
+:last-update-label!:
+:favicon: static/img/ddl_favicon_black.svg
 
-This pages is addressed at developers contributing to the ddm package.
 
-Development Guidelines
-**********************
+== Development Guidelines
+
+=== Local Project for Development and Testing
 
-Local Project for Development and Testing
-=========================================
 The repository includes a django test project that can be used for local development and testing.
 
-Setup
------
-| **1. Install required packages**
-Activate your local virtual environment and install the following requirements (the requirements still need to be defined - files are currently empty)::
+==== Setup
 
-    (venv) SomePath/ddm> pip install -r requirements.txt
-    (venv) SomePath/ddm> pip install -r test_project/requirements.txt
+===== Install required packages
+Once you have cloned or forked the GitHub repository, activate your local virtual environment and install the following requirements:
 
-| **2. Test Project Configuration**
+[source]
+----
+(venv) SomePath/ddm> pip install -r requirements.txt
+----
 
+===== Adjust Test Configuration
 A basic standard configuration for the test project is specified in
-*test_project/test_config.json*. Adjust the information in this file if you
-want to use a custom setup or use another database. By default, the test project
+`test_project/test_config.json`. Adjust the information in this file if you
+want to use a custom setup, or use another database. By default, the test project
 uses SQLite as a database backend.
 
 If you do make changes to this file, please do NOT commit these changes to the
 shared repository.
 
-Now you should be good to go.
 
+==== Commands
 
-Commands
---------
 Through the setup described above, the regular django commands are now available:
 
-**Run Development Server**
-
-To start the development server use the following commands::
-
-    (venv) SomePath/ddm> cd test_project
-    (venv) SomePath/ddm/test_project> manage.py runserver
-
-**Create Database Migrations**
+===== Run Development Server
 
-To create new migrations based on the changes made to the models, run::
+To start the development server use the following commands:
 
-    (venv) SomePath/ddm/test_project> manage.py makemigrations
+[source]
+----
+(venv) SomePath/ddm/test_project> python manage.py runserver
+----
 
-.. note:: this is only necessary, if you are actively developing, NOT if you are just checking out the project)
+===== Create Database Migrations
 
+To create new migrations based on the changes made to the models, run:
 
-**Apply migrations**
+[source]
+----
+(venv) SomePath/ddm/test_project> python manage.py makemigrations
+----
 
-To apply existing migrations to your local database, run:[1]_ ::
+===== Apply migrations
 
-    (venv) SomePath/ddm/test_project> manage.py migrate
+To apply existing migrations to your local database, run: footnote:[If you are running a version of Python < 3.9, you might have to manually enable the JSON1 extension on SQLite for the migration to work properly. For an explanation on how to do this visit https://code.djangoproject.com/wiki/JSON1Extension.]
 
-**Run Unit Tests**
+[source]
+----
+(venv) SomePath/ddm/test_project> python manage.py migrate
+----
 
-To run unit tests, use::
+===== Run Unit Tests
 
-    (venv) SomePath/ddm/test_project> manage.py test ddm
+To run unit tests, use:
 
-Vue Integration
-===============
+[source]
+----
+(venv) SomePath/ddm/test_project> python manage.py test ddm
+----
 
-Development
------------
+=== Vue Integration
 
-To run the app in development mode, you will need to serve both Django’s dev server and the webpack development server. From the vue_frontend directory, run::
+==== Development
 
-    npm run serve
+To run the app in development mode, you will need to serve both Django’s dev server and the webpack development server. From the frontend directory, run:
+[source]
+----
+(venv) SomePath/ddm/frontend> npm run serve
+----
 
-And, in a separate terminal in the Django root directory, run the Django development server, e.g.::
+And, in a separate terminal in the Django root directory, run the Django development server:
+[source]
+----
+(venv) SomePath/ddm/test_project> python manage.py runserver
+----
 
-    ./manage.py runserver
+Open your locally hosted Django app in a browser (e.g. http://localhost:8000).
 
-Point your browser to your Django app (e.g. http://localhost:8000) and check out the defined vue pages.
-
-Production Deployment
----------------------
+==== Production Deployment
 
 When it is time to deploy, or when you simply want to omit running the Vue dev server,
 you can build the Vue project in production mode.
-Cancel the ``npm run serve`` process if it is running and instead run ``npm run build``.
+Cancel the `npm run serve` process if it is running and instead run `npm run build`.
 The optimized bundles will be built in and placed into the Django static file location,
 and webpack-stats.json will be updated to reflect this new configuration.
 The vue builds should end up in the static folder of the django module (ddm/static).
 
 
-CI/CD
-=====
+=== CI/CD
 
-This project uses github actions for automated testing and CI tasks.
+This project uses _GitHub actions_ for automated testing and CI tasks.
 
 
-Actions
--------
+==== GitHub Actions
 
 A **push to develop** triggers build tests for the following configurations:
 
-- Python: [3.6, 3.7, 3.8]
-- Database: [sqlite, postgres, mysql]
+- Python: [3.8, 3.10.4]
+- Database: [sqlite, mysql]
 
 A **tag (vX.X.X) push to develop** triggers build tests (see above). If the tests are successful
 develop is automatically merged into main.
 
+[IMPORTANT]
+====
+Please make sure that pushed tags are in sync with package versions on PyPi.
+
+If the build-tests of a pushed tag fail, delete the tagfootnote:[To delete a tag, first run `git tag -d tagname` then
+`git push --delete origin tagname`.] and push the fixed version again with the same tag until the tests run through.
+====
+
 A **push to main** triggers build tests and if the tests are successful, automatically
 bumps the version number (patch number) and builds a new PyPi package.
 The tests have the same configurations as on develop.
 
 A **pull request to main created by dependabot** will automatically update the
 affected dependencies and merge into main.
 
 
-Pipeline
---------
+==== Pipeline
+
+A regular **push to develop** triggers the following pipeline:
+
+1. Run tests on develop.
+2. Create new documentation for GitHub pages.
 
 A **tag ("vX.X.X") push to develop** triggers the following pipeline:
 
 1. Run tests on develop.
-2. Merge develop into main.
-3. Run tests on main.
-4. Create PyPi package.
+2. Create new documentation for GitHub pages.
+3. Merge develop into main.
+4. Run tests on main.
+5. Create PyPi package.
 
 A **pull request to main created by dependabot** triggers the following pipeline:
 
 1. Update dependencies.
 2. Merge into main.
 3. Run tests on main.
 4. Create PyPi package.
 
 
-Release
--------
+==== Release
 
 A new **release** is created manually and includes:
 
 - Bumping the minor or major part of the version.
 - Updating setup.cfg.
+- Ideally, add a changelog.
+
+
+=== Documentation
 
+This documentation is written in
+https://docs.asciidoctor.org/asciidoc/latest/syntax-quick-reference/[AsciiDoc]
+and compiled using https://docs.antora.org/antora/latest/[Antora].
 
+The documentation UI uses the https://github.com/Nico-AP/antora-ddm-ui[Antora DDM UI]
+which is based on the https://gitlab.com/antora/antora-ui-default[default Antora UI].
 
+To compile the documentation locally, you first need to install Antora following
+https://docs.antora.org/antora/latest/install-and-run-quickstart/[these instructions].
 
-.. rubric:: Notes
+Next, you can compile the documentation locally using the `antora-playbook-local.yml` file:
+[source]
+----
+(venv) .../ddm/docs> npx antora antora-playbook-local.yml
+----
+Inspect the compiled documentation by opening `.../ddm/docs/build/index.html` in
+your preferred browser.
 
-.. [1] If you are running a version of Python < 3.9, you might have to manually enable the JSON1 extension on SQLite for the migration to work properly. For an explanation on how to do this visit https://code.djangoproject.com/wiki/JSON1Extension.
 
+include::components/scripts.adoc[]
```

### Comparing `django-ddm-0.1.9/setup.cfg` & `django-ddm-1.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [metadata]
 name = django-ddm
-version = 0.1.9
+version = 1.0.0
 description = A Django app to setup data donation projects.
 long_description = file: README.md
 url = https://github.com/uzh/ddm
 project_urls = 
-	Documentation = https://data-donation-module.readthedocs.io/
+	Documentation = https://uzh.github.io/ddm/
 	Website = https://datadonation.uzh.ch
 author = Nico Pfiffner
 author_email = n.pfiffner@ikmz.uzh.ch
-license = MIT
+license = GPLv3
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
+	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 
 [options]
 include_package_data = true
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.8
 setup_requires = 
 	setuptools >= 59.4.0
 install_requires = 
 	Django>=3.2
 	pycryptodome
 	django-ckeditor
 	django-polymorphic
+	django-webpack-loader
+	djangorestframework
+	bokeh
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

