# Comparing `tmp/bodhi_server-7.1.1.tar.gz` & `tmp/bodhi_server-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodhi_server-7.1.1.tar", max compression
+gzip compressed data, was "bodhi_server-7.2.0.tar", max compression
```

## Comparing `bodhi_server-7.1.1.tar` & `bodhi_server-7.2.0.tar`

### file list

```diff
@@ -1,333 +1,340 @@
--rw-r--r--   0        0        0    18018 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/COPYING
--rw-r--r--   0        0        0     1655 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/README.rst
--rw-r--r--   0        0        0     1258 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/alembic.ini
--rw-r--r--   0        0        0      580 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/apache/bodhi.conf
--rw-r--r--   0        0        0      260 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/apache/bodhi.wsgi
--rw-r--r--   0        0        0    13265 2023-03-12 13:20:07.000000 bodhi_server-7.1.1/bodhi/server/__init__.py
--rw-r--r--   0        0        0     1552 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/__init__.py
--rw-r--r--   0        0        0      220 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/constants.py
--rw-r--r--   0        0        0     5960 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/fedora.py
--rw-r--r--   0        0        0     2604 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/oauth.py
--rw-r--r--   0        0        0     2794 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/oauth_015.py
--rw-r--r--   0        0        0     3597 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/oauth_1.py
--rw-r--r--   0        0        0     5965 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/utils.py
--rw-r--r--   0        0        0     3960 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/auth/views.py
--rw-r--r--   0        0        0    12401 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/bugs.py
--rw-r--r--   0        0        0    30159 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/buildsys.py
--rw-r--r--   0        0        0    25877 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/config.py
--rw-r--r--   0        0        0     3616 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/consumers/__init__.py
--rw-r--r--   0        0        0     8807 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/consumers/automatic_updates.py
--rw-r--r--   0        0        0     4009 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/consumers/ci.py
--rw-r--r--   0        0        0     2809 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/consumers/resultsdb.py
--rw-r--r--   0        0        0     5651 2023-03-11 14:08:26.000000 bodhi_server-7.1.1/bodhi/server/consumers/signed.py
--rw-r--r--   0        0        0     2728 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/consumers/util.py
--rw-r--r--   0        0        0     2405 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/consumers/waiverdb.py
--rw-r--r--   0        0        0     1040 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/email/templates/fedora_epel_errata_template.tpl
--rw-r--r--   0        0        0     1070 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl
--rw-r--r--   0        0        0     1051 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/email/templates/fedora_errata_template.tpl
--rw-r--r--   0        0        0     1059 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/email/templates/fedora_modular_errata_template.tpl
--rw-r--r--   0        0        0      261 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/email/templates/maillist_template.tpl
--rw-r--r--   0        0        0     1249 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/exceptions.py
--rw-r--r--   0        0        0     7154 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/ffmarkdown.py
--rw-r--r--   0        0        0        0 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/locale/.placeholder
--rw-r--r--   0        0        0     3641 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/logging.py
--rw-r--r--   0        0        0    14666 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/mail.py
--rw-r--r--   0        0        0    12964 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/metadata.py
--rw-r--r--   0        0        0      706 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/README.rst
--rw-r--r--   0        0        0      845 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/__init__.py
--rw-r--r--   0        0        0     3808 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/env.py
--rw-r--r--   0        0        0     1181 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/script.py.mako
--rw-r--r--   0        0        0     2918 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py
--rw-r--r--   0        0        0     1333 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py
--rw-r--r--   0        0        0     1380 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py
--rw-r--r--   0        0        0     1443 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py
--rw-r--r--   0        0        0     3846 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py
--rw-r--r--   0        0        0     2732 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py
--rw-r--r--   0        0        0     3041 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py
--rw-r--r--   0        0        0     1822 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py
--rw-r--r--   0        0        0     2279 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py
--rw-r--r--   0        0        0     2187 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py
--rw-r--r--   0        0        0     2586 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py
--rw-r--r--   0        0        0     2708 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py
--rw-r--r--   0        0        0     1741 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py
--rw-r--r--   0        0        0     2812 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py
--rw-r--r--   0        0        0     1503 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py
--rw-r--r--   0        0        0     1368 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py
--rw-r--r--   0        0        0     1501 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py
--rw-r--r--   0        0        0      843 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/__init__.py
--rw-r--r--   0        0        0     1321 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py
--rw-r--r--   0        0        0     2991 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py
--rw-r--r--   0        0        0     1346 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py
--rw-r--r--   0        0        0     1808 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py
--rw-r--r--   0        0        0     2341 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py
--rw-r--r--   0        0        0     2593 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py
--rw-r--r--   0        0        0     2316 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py
--rw-r--r--   0        0        0     1296 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py
--rw-r--r--   0        0        0     1329 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py
--rw-r--r--   0        0        0     1403 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py
--rw-r--r--   0        0        0     1670 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py
--rw-r--r--   0        0        0     1421 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py
--rw-r--r--   0        0        0     1403 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py
--rw-r--r--   0        0        0     1312 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py
--rw-r--r--   0        0        0     1345 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py
--rw-r--r--   0        0        0     1469 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py
--rw-r--r--   0        0        0     1353 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py
--rw-r--r--   0        0        0     1347 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py
--rw-r--r--   0        0        0   198827 2023-03-18 09:12:55.000000 bodhi_server-7.1.1/bodhi/server/models.py
--rw-r--r--   0        0        0     3016 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/notifications.py
--rw-r--r--   0        0        0    11993 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/push.py
--rw-r--r--   0        0        0     7143 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/renderers.py
--rw-r--r--   0        0        0    22232 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/schemas.py
--rw-r--r--   0        0        0      849 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/__init__.py
--rw-r--r--   0        0        0     1397 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/bshell.py
--rw-r--r--   0        0        0     3871 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/compat.py
--rw-r--r--   0        0        0     1847 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/initializedb.py
--rw-r--r--   0        0        0     4238 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/sar.py
--rw-r--r--   0        0        0    29485 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/skopeo_lite.py
--rw-r--r--   0        0        0     3839 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/scripts/untag_branched.py
--rw-r--r--   0        0        0     6158 2023-03-05 08:54:15.000000 bodhi_server-7.1.1/bodhi/server/security.py
--rw-r--r--   0        0        0      815 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/__init__.py
--rw-r--r--   0        0        0     5182 2023-02-28 06:55:11.000000 bodhi_server-7.1.1/bodhi/server/services/builds.py
--rw-r--r--   0        0        0     8633 2023-02-28 06:55:11.000000 bodhi_server-7.1.1/bodhi/server/services/comments.py
--rw-r--r--   0        0        0     3936 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/composes.py
--rw-r--r--   0        0        0     2058 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/csrf.py
--rw-r--r--   0        0        0     3793 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/errors.py
--rw-r--r--   0        0        0     1969 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/markdown.py
--rw-r--r--   0        0        0     1916 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/metrics_tween.py
--rw-r--r--   0        0        0    12983 2023-02-28 17:10:19.000000 bodhi_server-7.1.1/bodhi/server/services/overrides.py
--rw-r--r--   0        0        0     3724 2023-02-28 06:55:11.000000 bodhi_server-7.1.1/bodhi/server/services/packages.py
--rw-r--r--   0        0        0    16277 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/services/releases.py
--rw-r--r--   0        0        0     3481 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/services/schemas.py
--rw-r--r--   0        0        0    28875 2023-02-28 06:55:11.000000 bodhi_server-7.1.1/bodhi/server/services/updates.py
--rw-r--r--   0        0        0     6612 2023-02-28 06:55:11.000000 bodhi_server-7.1.1/bodhi/server/services/user.py
--rw-r--r--   0        0        0      832 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/__init__.py
--rw-r--r--   0        0        0    10425 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/bodhi-logo.svg
--rw-r--r--   0        0        0     6423 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/css/site.css
--rw-r--r--   0        0        0   124988 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/FontAwesome.otf
--rw-r--r--   0        0        0    76518 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot
--rw-r--r--   0        0        0   391622 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg
--rw-r--r--   0        0        0   152796 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    90412 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff
--rw-r--r--   0        0        0    71896 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2
--rw-r--r--   0        0        0    35152 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome.css
--rwxr-xr-x   0        0        0   139140 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot
--rwxr-xr-x   0        0        0   146800 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot
--rwxr-xr-x   0        0        0   143488 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot
--rwxr-xr-x   0        0        0   137266 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot
--rwxr-xr-x   0        0        0    28782 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot
--rwxr-xr-x   0        0        0    31454 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot
--rwxr-xr-x   0        0        0    30512 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot
--rwxr-xr-x   0        0        0    28527 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot
--rwxr-xr-x   0        0        0   389828 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf
--rwxr-xr-x   0        0        0   398888 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf
--rwxr-xr-x   0        0        0   393880 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf
--rwxr-xr-x   0        0        0   387660 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf
--rwxr-xr-x   0        0        0    73056 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf
--rwxr-xr-x   0        0        0    77808 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf
--rwxr-xr-x   0        0        0    76444 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf
--rwxr-xr-x   0        0        0    73256 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf
--rwxr-xr-x   0        0        0   171820 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff
--rwxr-xr-x   0        0        0   180204 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff
--rwxr-xr-x   0        0        0   176864 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff
--rwxr-xr-x   0        0        0   168376 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff
--rwxr-xr-x   0        0        0    31964 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff
--rwxr-xr-x   0        0        0    34720 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff
--rwxr-xr-x   0        0        0    33556 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff
--rwxr-xr-x   0        0        0    31584 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff
--rwxr-xr-x   0        0        0   124552 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2
--rwxr-xr-x   0        0        0   131588 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2
--rwxr-xr-x   0        0        0   128624 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2
--rwxr-xr-x   0        0        0   122888 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2
--rwxr-xr-x   0        0        0    25884 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2
--rwxr-xr-x   0        0        0    28232 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2
--rwxr-xr-x   0        0        0    27576 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2
--rwxr-xr-x   0        0        0    25696 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2
--rw-r--r--   0        0        0     1947 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/hack.css
--rw-r--r--   0        0        0    31896 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot
--rw-r--r--   0        0        0   254253 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg
--rw-r--r--   0        0        0    68444 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf
--rw-r--r--   0        0        0    33704 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff
--rw-r--r--   0        0        0    23816 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2
--rw-r--r--   0        0        0    30763 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot
--rw-r--r--   0        0        0   258568 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg
--rw-r--r--   0        0        0    64668 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf
--rw-r--r--   0        0        0    32300 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff
--rw-r--r--   0        0        0    22220 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2
--rw-r--r--   0        0        0    32088 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot
--rw-r--r--   0        0        0   254724 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg
--rw-r--r--   0        0        0    68776 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf
--rw-r--r--   0        0        0    33876 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff
--rw-r--r--   0        0        0    23652 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2
--rw-r--r--   0        0        0    30546 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot
--rw-r--r--   0        0        0   257617 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg
--rw-r--r--   0        0        0    65236 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf
--rw-r--r--   0        0        0    32180 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff
--rw-r--r--   0        0        0    22176 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2
--rw-r--r--   0        0        0    30880 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot
--rw-r--r--   0        0        0   258434 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg
--rw-r--r--   0        0        0    65072 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf
--rw-r--r--   0        0        0    32212 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff
--rw-r--r--   0        0        0    22196 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2
--rw-r--r--   0        0        0    31491 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot
--rw-r--r--   0        0        0   255338 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg
--rw-r--r--   0        0        0    66740 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf
--rw-r--r--   0        0        0    33060 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff
--rw-r--r--   0        0        0    23048 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2
--rw-r--r--   0        0        0     4956 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans.css
--rw-r--r--   0        0        0     4255 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/ico/favicon.ico
--rw-r--r--   0        0        0    13117 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/img/bodhi-logo.png
--rw-r--r--   0        0        0    17444 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/img/bodhi-logo.svg
--rw-r--r--   0        0        0    30769 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/img/logo-large.png
--rw-r--r--   0        0        0     4388 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/img/logo.png
--rw-r--r--   0        0        0     1775 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/js/comment_form.js
--rw-r--r--   0        0        0     4723 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/static/js/forms.js
--rw-r--r--   0        0        0     3238 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/js/override_form.js
--rw-r--r--   0        0        0     3485 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/js/search.js
--rw-r--r--   0        0        0     1475 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/js/site.js
--rw-r--r--   0        0        0    14397 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/static/js/update_form.js
--rw-r--r--   0        0        0   197005 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/chartjs/chart.min.js
--rw-r--r--   0        0        0   199088 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css
--rw-r--r--   0        0        0    75244 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map
--rw-r--r--   0        0        0    79790 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js
--rw-r--r--   0        0        0   330849 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map
--rw-r--r--   0        0        0    89501 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js
--rw-r--r--   0        0        0   137972 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map
--rw-r--r--   0        0        0    12438 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css
--rw-r--r--   0        0        0    48148 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js
--rw-r--r--   0        0        0     5855 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-spinner.css
--rw-r--r--   0        0        0    12969 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css
--rw-r--r--   0        0        0     3908 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css
--rw-r--r--   0        0        0    13273 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css
--rw-r--r--   0        0        0    16828 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css
--rw-r--r--   0        0        0     4399 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css
--rw-r--r--   0        0        0     3086 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger.css
--rw-r--r--   0        0        0     1281 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js
--rw-r--r--   0        0        0     1301 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js
--rw-r--r--   0        0        0    40813 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger.js
--rw-r--r--   0        0        0    19068 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger.min.js
--rw-r--r--   0        0        0    32364 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/moment/moment.min.js
--rw-r--r--   0        0        0   126299 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.js
--rw-r--r--   0        0        0    55382 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js
--rw-r--r--   0        0        0    14594 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css
--rw-r--r--   0        0        0   104302 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/static/vendor/typeahead/typeahead.bundle.js
--rw-r--r--   0        0        0     6095 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/__init__.py
--rw-r--r--   0        0        0     7848 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/approve_testing.py
--rw-r--r--   0        0        0     2158 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/check_policies.py
--rw-r--r--   0        0        0     4591 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/check_signed_builds.py
--rw-r--r--   0        0        0     2397 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/clean_old_composes.py
--rw-r--r--   0        0        0    62192 2023-03-18 09:12:55.000000 bodhi_server-7.1.1/bodhi/server/tasks/composer.py
--rw-r--r--   0        0        0     2035 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/expire_overrides.py
--rw-r--r--   0        0        0     1785 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/fetch_test_cases.py
--rw-r--r--   0        0        0     2833 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/handle_side_and_related_tags.py
--rw-r--r--   0        0        0     1469 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/tasks/tag_update_builds.py
--rw-r--r--   0        0        0     3706 2022-12-31 15:13:57.000000 bodhi_server-7.1.1/bodhi/server/tasks/work_on_bugs.py
--rw-r--r--   0        0        0      105 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/comment.html
--rw-r--r--   0        0        0     1331 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/comments.html
--rw-r--r--   0        0        0     3575 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/compose.html
--rw-r--r--   0        0        0     1270 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/composes.html
--rw-r--r--   0        0        0      352 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/errors.html
--rw-r--r--   0        0        0    15751 2023-03-11 14:08:26.000000 bodhi_server-7.1.1/bodhi/server/templates/fragments.html
--rw-r--r--   0        0        0     5525 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/home.html
--rw-r--r--   0        0        0    10635 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/master.html
--rw-r--r--   0        0        0    20775 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/templates/new_update.html
--rw-r--r--   0        0        0     9352 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/override.html
--rw-r--r--   0        0        0     9731 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/bodhi/server/templates/overrides.html
--rw-r--r--   0        0        0      882 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/pager.html
--rw-r--r--   0        0        0    12532 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/release.html
--rw-r--r--   0        0        0     2386 2023-03-05 09:29:39.000000 bodhi_server-7.1.1/bodhi/server/templates/releases.html
--rw-r--r--   0        0        0    56086 2023-03-18 09:12:55.000000 bodhi_server-7.1.1/bodhi/server/templates/update.html
--rw-r--r--   0        0        0    15964 2023-03-11 14:08:26.000000 bodhi_server-7.1.1/bodhi/server/templates/updates.html
--rw-r--r--   0        0        0     4796 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/templates/user.html
--rw-r--r--   0        0        0    50365 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/util.py
--rw-r--r--   0        0        0    51627 2023-03-11 14:08:26.000000 bodhi_server-7.1.1/bodhi/server/validators.py
--rw-r--r--   0        0        0      812 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/views/__init__.py
--rw-r--r--   0        0        0    22716 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/bodhi/server/views/generic.py
--rw-r--r--   0        0        0     3545 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/bodhi/server/webapp.py
--rw-r--r--   0        0        0     1592 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/celeryconfig.py
--rw-r--r--   0        0        0      776 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/Makefile
--rw-r--r--   0        0        0     1757 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/conf.py
--rw-r--r--   0        0        0        0 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/index.rst
--rw-r--r--   0        0        0     1244 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/man_pages/bodhi-push.rst
--rw-r--r--   0        0        0      797 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/man_pages/bodhi-sar.rst
--rw-r--r--   0        0        0      523 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/man_pages/bodhi-shell.rst
--rw-r--r--   0        0        0     1866 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/man_pages/bodhi-skopeo-lite.rst
--rw-r--r--   0        0        0      718 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/man_pages/bodhi-untag-branched.rst
--rw-r--r--   0        0        0      623 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/docs/man_pages/initialize_bodhi_db.rst
--rw-r--r--   0        0        0    24410 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/production.ini
--rw-r--r--   0        0        0     4911 2023-03-18 09:16:35.000000 bodhi_server-7.1.1/pyproject.toml
--rw-r--r--   0        0        0      418 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/setup.cfg
--rw-r--r--   0        0        0      816 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/__init__.py
--rw-r--r--   0        0        0       39 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/auth/__init__.py
--rw-r--r--   0        0        0     4790 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/auth/test_fedora.py
--rw-r--r--   0        0        0    16947 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/auth/test_oauth.py
--rw-r--r--   0        0        0     5487 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/auth/test_utils.py
--rw-r--r--   0        0        0     5442 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/auth/test_views.py
--rw-r--r--   0        0        0     2293 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/auth/utils.py
--rw-r--r--   0        0        0    19027 2023-02-28 06:55:11.000000 bodhi_server-7.1.1/tests/base.py
--rw-r--r--   0        0        0     2214 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/conftest.py
--rw-r--r--   0        0        0      821 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/__init__.py
--rwxr-xr-x   0        0        0      335 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/pungi.basepath/fake-pungi.sh
--rw-r--r--   0        0        0       76 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/pungi.basepath/pungi.module.conf
--rw-r--r--   0        0        0       76 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/pungi.basepath/pungi.rpm.conf
--rw-r--r--   0        0        0      210 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/pungi.basepath/variants.module.xml.j2
--rw-r--r--   0        0        0       76 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/pungi.basepath/variants.rpm.xml.j2
--rw-r--r--   0        0        0    20022 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/tests/consumers/test_automatic_updates.py
--rw-r--r--   0        0        0    11457 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/test_ci.py
--rw-r--r--   0        0        0     4779 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/test_consumers.py
--rw-r--r--   0        0        0    13766 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/test_resultsdb.py
--rw-r--r--   0        0        0    13241 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/consumers/test_signed.py
--rw-r--r--   0        0        0     9849 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/consumers/test_waiverdb.py
--rw-r--r--   0        0        0      913 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/functional/__init__.py
--rw-r--r--   0        0        0     2571 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/functional/test_packages.py
--rw-r--r--   0        0        0     8272 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/functional/test_users.py
--rw-r--r--   0        0        0      819 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/__init__.py
--rw-r--r--   0        0        0     2072 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/test_bshell.py
--rw-r--r--   0        0        0     5128 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/test_compat.py
--rw-r--r--   0        0        0     3597 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/test_initializedb.py
--rw-r--r--   0        0        0     5341 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/test_sar.py
--rw-r--r--   0        0        0    26242 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/test_skopeo_lite.py
--rw-r--r--   0        0        0    15411 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/scripts/test_untag_branched.py
--rw-r--r--   0        0        0      820 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/__init__.py
--rw-r--r--   0        0        0     4067 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_builds.py
--rw-r--r--   0        0        0    27002 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_comments.py
--rw-r--r--   0        0        0     6469 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_composes.py
--rw-r--r--   0        0        0     1512 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_csrf.py
--rw-r--r--   0        0        0     1827 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_errors.py
--rw-r--r--   0        0        0    31133 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_overrides.py
--rw-r--r--   0        0        0    28879 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/services/test_releases.py
--rw-r--r--   0        0        0     3801 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/services/test_schemas.py
--rw-r--r--   0        0        0   299956 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/tests/services/test_updates.py
--rw-r--r--   0        0        0      817 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1531 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/base.py
--rw-r--r--   0        0        0    42724 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/tasks/test_approve_testing.py
--rw-r--r--   0        0        0    29342 2023-03-18 09:12:55.000000 bodhi_server-7.1.1/tests/tasks/test_check_policies.py
--rw-r--r--   0        0        0     8649 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/tasks/test_check_signed_builds.py
--rw-r--r--   0        0        0     5949 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/test_clean_old_composes.py
--rw-r--r--   0        0        0   175769 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/tasks/test_composer.py
--rw-r--r--   0        0        0     3792 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/test_expire_overrides.py
--rw-r--r--   0        0        0     3677 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/tasks/test_fetch_test_cases.py
--rw-r--r--   0        0        0     2799 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/test_handle_side_and_related_tags.py
--rw-r--r--   0        0        0     2321 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/test_tag_update_builds.py
--rw-r--r--   0        0        0     5085 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/tasks/test_work_on_bugs.py
--rw-r--r--   0        0        0    11553 2023-03-12 13:20:07.000000 bodhi_server-7.1.1/tests/test___init__.py
--rw-r--r--   0        0        0     2185 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_alembic.py
--rw-r--r--   0        0        0    28061 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_bugs.py
--rw-r--r--   0        0        0    17610 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_buildsys.py
--rw-r--r--   0        0        0    16269 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_config.py
--rw-r--r--   0        0        0     4319 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_logging.py
--rw-r--r--   0        0        0    15586 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_mail.py
--rw-r--r--   0        0        0    25674 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_metadata.py
--rw-r--r--   0        0        0   217618 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/tests/test_models.py
--rw-r--r--   0        0        0     3897 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_notifications.py
--rw-r--r--   0        0        0    72085 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/test_push.py
--rw-r--r--   0        0        0     2238 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_renderers.py
--rw-r--r--   0        0        0     1642 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_schemas.py
--rw-r--r--   0        0        0     7195 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_security.py
--rw-r--r--   0        0        0    69803 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/tests/test_util.py
--rw-r--r--   0        0        0    44272 2023-03-05 14:50:21.000000 bodhi_server-7.1.1/tests/test_validators.py
--rw-r--r--   0        0        0     2614 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/test_webapp.py
--rw-r--r--   0        0        0     4217 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/testing.ini
--rw-r--r--   0        0        0      992 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/utils.py
--rw-r--r--   0        0        0      817 2022-12-23 15:08:00.000000 bodhi_server-7.1.1/tests/views/__init__.py
--rw-r--r--   0        0        0    23763 2023-03-11 13:42:51.000000 bodhi_server-7.1.1/tests/views/test_generic.py
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 bodhi_server-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18018 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/COPYING
+-rw-r--r--   0        0        0     1655 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/README.rst
+-rw-r--r--   0        0        0     1258 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/alembic.ini
+-rw-r--r--   0        0        0      580 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/apache/bodhi.conf
+-rw-r--r--   0        0        0      260 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/apache/bodhi.wsgi
+-rw-r--r--   0        0        0    13319 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/__init__.py
+-rw-r--r--   0        0        0      220 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/constants.py
+-rw-r--r--   0        0        0     5960 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/fedora.py
+-rw-r--r--   0        0        0     2604 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/oauth.py
+-rw-r--r--   0        0        0     2794 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/oauth_015.py
+-rw-r--r--   0        0        0     3597 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/oauth_1.py
+-rw-r--r--   0        0        0     5965 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/utils.py
+-rw-r--r--   0        0        0     3960 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/auth/views.py
+-rw-r--r--   0        0        0    12401 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/bugs.py
+-rw-r--r--   0        0        0    30159 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/buildsys.py
+-rw-r--r--   0        0        0    25877 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/config.py
+-rw-r--r--   0        0        0     3616 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/consumers/__init__.py
+-rw-r--r--   0        0        0     8807 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/consumers/automatic_updates.py
+-rw-r--r--   0        0        0     4009 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/consumers/ci.py
+-rw-r--r--   0        0        0     2863 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/consumers/resultsdb.py
+-rw-r--r--   0        0        0     5651 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/consumers/signed.py
+-rw-r--r--   0        0        0     2728 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/consumers/util.py
+-rw-r--r--   0        0        0     2569 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/consumers/waiverdb.py
+-rw-r--r--   0        0        0     1040 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_errata_template.tpl
+-rw-r--r--   0        0        0     1070 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl
+-rw-r--r--   0        0        0     1051 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_errata_template.tpl
+-rw-r--r--   0        0        0     1059 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/fedora_modular_errata_template.tpl
+-rw-r--r--   0        0        0      261 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/email/templates/maillist_template.tpl
+-rw-r--r--   0        0        0     1249 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/exceptions.py
+-rw-r--r--   0        0        0     7154 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/ffmarkdown.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/locale/.placeholder
+-rw-r--r--   0        0        0     3641 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/logging.py
+-rw-r--r--   0        0        0    14666 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/mail.py
+-rw-r--r--   0        0        0    12964 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/metadata.py
+-rw-r--r--   0        0        0      706 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/README.rst
+-rw-r--r--   0        0        0      845 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/__init__.py
+-rw-r--r--   0        0        0     3808 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/env.py
+-rw-r--r--   0        0        0     1181 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/script.py.mako
+-rw-r--r--   0        0        0     2918 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py
+-rw-r--r--   0        0        0     1333 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py
+-rw-r--r--   0        0        0     1380 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py
+-rw-r--r--   0        0        0     1443 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py
+-rw-r--r--   0        0        0     3846 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py
+-rw-r--r--   0        0        0     2732 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py
+-rw-r--r--   0        0        0     3041 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py
+-rw-r--r--   0        0        0     1822 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py
+-rw-r--r--   0        0        0     2279 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py
+-rw-r--r--   0        0        0     2187 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py
+-rw-r--r--   0        0        0     2586 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py
+-rw-r--r--   0        0        0     2708 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py
+-rw-r--r--   0        0        0     1741 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py
+-rw-r--r--   0        0        0     2812 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py
+-rw-r--r--   0        0        0     1503 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py
+-rw-r--r--   0        0        0     1368 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py
+-rw-r--r--   0        0        0     1501 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py
+-rw-r--r--   0        0        0      843 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     1321 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py
+-rw-r--r--   0        0        0     2991 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py
+-rw-r--r--   0        0        0     1346 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py
+-rw-r--r--   0        0        0     1808 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py
+-rw-r--r--   0        0        0     2341 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py
+-rw-r--r--   0        0        0     2593 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py
+-rw-r--r--   0        0        0     2316 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py
+-rw-r--r--   0        0        0     1296 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py
+-rw-r--r--   0        0        0     1329 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py
+-rw-r--r--   0        0        0     1403 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py
+-rw-r--r--   0        0        0     1670 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py
+-rw-r--r--   0        0        0     1421 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py
+-rw-r--r--   0        0        0     1403 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py
+-rw-r--r--   0        0        0     1312 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py
+-rw-r--r--   0        0        0     1345 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py
+-rw-r--r--   0        0        0     1469 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py
+-rw-r--r--   0        0        0     1353 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py
+-rw-r--r--   0        0        0     1347 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py
+-rw-r--r--   0        0        0   198699 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/models.py
+-rw-r--r--   0        0        0     3016 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/notifications.py
+-rw-r--r--   0        0        0    11988 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/push.py
+-rw-r--r--   0        0        0     7143 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/renderers.py
+-rw-r--r--   0        0        0    22381 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/schemas.py
+-rw-r--r--   0        0        0      849 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/__init__.py
+-rw-r--r--   0        0        0     1397 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/bshell.py
+-rw-r--r--   0        0        0     3871 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/compat.py
+-rw-r--r--   0        0        0     1847 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/initializedb.py
+-rw-r--r--   0        0        0     4238 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/sar.py
+-rw-r--r--   0        0        0    29485 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/skopeo_lite.py
+-rw-r--r--   0        0        0     3839 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/scripts/untag_branched.py
+-rw-r--r--   0        0        0     6158 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/security.py
+-rw-r--r--   0        0        0      815 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/__init__.py
+-rw-r--r--   0        0        0     5182 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/builds.py
+-rw-r--r--   0        0        0     8633 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/comments.py
+-rw-r--r--   0        0        0     3936 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/composes.py
+-rw-r--r--   0        0        0     2058 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/csrf.py
+-rw-r--r--   0        0        0     3793 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/errors.py
+-rw-r--r--   0        0        0     1969 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/markdown.py
+-rw-r--r--   0        0        0     1916 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/metrics_tween.py
+-rw-r--r--   0        0        0    12983 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/overrides.py
+-rw-r--r--   0        0        0     3724 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/packages.py
+-rw-r--r--   0        0        0    16707 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/services/releases.py
+-rw-r--r--   0        0        0     3481 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/schemas.py
+-rw-r--r--   0        0        0    28875 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/updates.py
+-rw-r--r--   0        0        0     6612 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/services/user.py
+-rw-r--r--   0        0        0      832 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/__init__.py
+-rw-r--r--   0        0        0    10425 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/bodhi-logo.svg
+-rw-r--r--   0        0        0     6423 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/css/site.css
+-rw-r--r--   0        0        0   124988 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/FontAwesome.otf
+-rw-r--r--   0        0        0    76518 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   391622 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   152796 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    90412 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    71896 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0    35152 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome.css
+-rwxr-xr-x   0        0        0   139140 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot
+-rwxr-xr-x   0        0        0   146800 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot
+-rwxr-xr-x   0        0        0   143488 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot
+-rwxr-xr-x   0        0        0   137266 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot
+-rwxr-xr-x   0        0        0    28782 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot
+-rwxr-xr-x   0        0        0    31454 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot
+-rwxr-xr-x   0        0        0    30512 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot
+-rwxr-xr-x   0        0        0    28527 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot
+-rwxr-xr-x   0        0        0   389828 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf
+-rwxr-xr-x   0        0        0   398888 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf
+-rwxr-xr-x   0        0        0   393880 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf
+-rwxr-xr-x   0        0        0   387660 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf
+-rwxr-xr-x   0        0        0    73056 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    77808 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    76444 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf
+-rwxr-xr-x   0        0        0    73256 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf
+-rwxr-xr-x   0        0        0   171820 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff
+-rwxr-xr-x   0        0        0   180204 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff
+-rwxr-xr-x   0        0        0   176864 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff
+-rwxr-xr-x   0        0        0   168376 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff
+-rwxr-xr-x   0        0        0    31964 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff
+-rwxr-xr-x   0        0        0    34720 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff
+-rwxr-xr-x   0        0        0    33556 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff
+-rwxr-xr-x   0        0        0    31584 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff
+-rwxr-xr-x   0        0        0   124552 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2
+-rwxr-xr-x   0        0        0   131588 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2
+-rwxr-xr-x   0        0        0   128624 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2
+-rwxr-xr-x   0        0        0   122888 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2
+-rwxr-xr-x   0        0        0    25884 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    28232 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    27576 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2
+-rwxr-xr-x   0        0        0    25696 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2
+-rw-r--r--   0        0        0     1947 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/hack.css
+-rw-r--r--   0        0        0    31896 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot
+-rw-r--r--   0        0        0   254253 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg
+-rw-r--r--   0        0        0    68444 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf
+-rw-r--r--   0        0        0    33704 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff
+-rw-r--r--   0        0        0    23816 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2
+-rw-r--r--   0        0        0    30763 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot
+-rw-r--r--   0        0        0   258568 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg
+-rw-r--r--   0        0        0    64668 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf
+-rw-r--r--   0        0        0    32300 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff
+-rw-r--r--   0        0        0    22220 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2
+-rw-r--r--   0        0        0    32088 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot
+-rw-r--r--   0        0        0   254724 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg
+-rw-r--r--   0        0        0    68776 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf
+-rw-r--r--   0        0        0    33876 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff
+-rw-r--r--   0        0        0    23652 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2
+-rw-r--r--   0        0        0    30546 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot
+-rw-r--r--   0        0        0   257617 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg
+-rw-r--r--   0        0        0    65236 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf
+-rw-r--r--   0        0        0    32180 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff
+-rw-r--r--   0        0        0    22176 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2
+-rw-r--r--   0        0        0    30880 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot
+-rw-r--r--   0        0        0   258434 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg
+-rw-r--r--   0        0        0    65072 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf
+-rw-r--r--   0        0        0    32212 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff
+-rw-r--r--   0        0        0    22196 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2
+-rw-r--r--   0        0        0    31491 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot
+-rw-r--r--   0        0        0   255338 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg
+-rw-r--r--   0        0        0    66740 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf
+-rw-r--r--   0        0        0    33060 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff
+-rw-r--r--   0        0        0    23048 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2
+-rw-r--r--   0        0        0     4956 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans.css
+-rw-r--r--   0        0        0     4255 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/ico/favicon.ico
+-rw-r--r--   0        0        0    13117 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.png
+-rw-r--r--   0        0        0    17444 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.svg
+-rw-r--r--   0        0        0    30769 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/logo-large.png
+-rw-r--r--   0        0        0     4388 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/img/logo.png
+-rw-r--r--   0        0        0     1775 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/comment_form.js
+-rw-r--r--   0        0        0     4723 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/js/forms.js
+-rw-r--r--   0        0        0     3238 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/override_form.js
+-rw-r--r--   0        0        0     3485 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/search.js
+-rw-r--r--   0        0        0     1475 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/js/site.js
+-rw-r--r--   0        0        0    14397 2023-04-29 08:26:58.000000 bodhi_server-7.2.0/bodhi/server/static/js/update_form.js
+-rw-r--r--   0        0        0   197005 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/chartjs/chart.min.js
+-rw-r--r--   0        0        0   199088 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css
+-rw-r--r--   0        0        0    75244 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map
+-rw-r--r--   0        0        0    79790 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js
+-rw-r--r--   0        0        0   330849 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map
+-rw-r--r--   0        0        0    89501 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0   137972 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map
+-rw-r--r--   0        0        0    12438 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css
+-rw-r--r--   0        0        0    48148 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js
+-rw-r--r--   0        0        0     5855 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-spinner.css
+-rw-r--r--   0        0        0    12969 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css
+-rw-r--r--   0        0        0     3908 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css
+-rw-r--r--   0        0        0    13273 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css
+-rw-r--r--   0        0        0    16828 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css
+-rw-r--r--   0        0        0     4399 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css
+-rw-r--r--   0        0        0     3086 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger.css
+-rw-r--r--   0        0        0     1281 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js
+-rw-r--r--   0        0        0     1301 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js
+-rw-r--r--   0        0        0    40813 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.js
+-rw-r--r--   0        0        0    19068 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.min.js
+-rw-r--r--   0        0        0    32364 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0    66344 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.14.0.min.js
+-rw-r--r--   0        0        0   335718 2022-11-14 19:44:00.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.0.min.js
+-rw-r--r--   0        0        0   126299 2022-11-17 17:24:15.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.1.js
+-rw-r--r--   0        0        0   336699 2022-11-17 17:24:15.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.1.min.js
+-rw-r--r--   0        0        0   126299 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.js
+-rw-r--r--   0        0        0    55382 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js
+-rw-r--r--   0        0        0     9368 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.14.0.css
+-rw-r--r--   0        0        0    36947 2022-11-14 19:44:00.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.0.css
+-rw-r--r--   0        0        0    37022 2022-11-17 17:24:15.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.1.css
+-rw-r--r--   0        0        0    14594 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css
+-rw-r--r--   0        0        0   104302 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/static/vendor/typeahead/typeahead.bundle.js
+-rw-r--r--   0        0        0     6095 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/__init__.py
+-rw-r--r--   0        0        0     7848 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/approve_testing.py
+-rw-r--r--   0        0        0     2158 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/check_policies.py
+-rw-r--r--   0        0        0     4591 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/check_signed_builds.py
+-rw-r--r--   0        0        0     2397 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/clean_old_composes.py
+-rw-r--r--   0        0        0    62185 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/tasks/composer.py
+-rw-r--r--   0        0        0     2035 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/expire_overrides.py
+-rw-r--r--   0        0        0     1785 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/fetch_test_cases.py
+-rw-r--r--   0        0        0     2833 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/handle_side_and_related_tags.py
+-rw-r--r--   0        0        0     1469 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/tag_update_builds.py
+-rw-r--r--   0        0        0     3706 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/tasks/work_on_bugs.py
+-rw-r--r--   0        0        0      105 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/comment.html
+-rw-r--r--   0        0        0     1331 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/comments.html
+-rw-r--r--   0        0        0     3575 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/compose.html
+-rw-r--r--   0        0        0     1270 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/composes.html
+-rw-r--r--   0        0        0      352 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/errors.html
+-rw-r--r--   0        0        0    15764 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/templates/fragments.html
+-rw-r--r--   0        0        0     5525 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/home.html
+-rw-r--r--   0        0        0    10635 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/master.html
+-rw-r--r--   0        0        0    20775 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/templates/new_update.html
+-rw-r--r--   0        0        0     9352 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/override.html
+-rw-r--r--   0        0        0     9731 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/templates/overrides.html
+-rw-r--r--   0        0        0      882 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/pager.html
+-rw-r--r--   0        0        0    12532 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/release.html
+-rw-r--r--   0        0        0     2938 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/templates/releases.html
+-rw-r--r--   0        0        0    55990 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/bodhi/server/templates/update.html
+-rw-r--r--   0        0        0    15964 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/templates/updates.html
+-rw-r--r--   0        0        0     4796 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/templates/user.html
+-rw-r--r--   0        0        0    50365 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/bodhi/server/util.py
+-rw-r--r--   0        0        0    51587 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/validators.py
+-rw-r--r--   0        0        0      812 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/views/__init__.py
+-rw-r--r--   0        0        0    22706 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/bodhi/server/views/generic.py
+-rw-r--r--   0        0        0     3545 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/bodhi/server/webapp.py
+-rw-r--r--   0        0        0     1592 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/celeryconfig.py
+-rw-r--r--   0        0        0      776 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1757 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/conf.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/index.rst
+-rw-r--r--   0        0        0     1244 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-push.rst
+-rw-r--r--   0        0        0      797 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-sar.rst
+-rw-r--r--   0        0        0      523 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-shell.rst
+-rw-r--r--   0        0        0     1866 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-skopeo-lite.rst
+-rw-r--r--   0        0        0      718 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/bodhi-untag-branched.rst
+-rw-r--r--   0        0        0      623 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/docs/man_pages/initialize_bodhi_db.rst
+-rw-r--r--   0        0        0    24410 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/production.ini
+-rw-r--r--   0        0        0     4911 2023-04-30 06:59:12.000000 bodhi_server-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0      418 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/setup.cfg
+-rw-r--r--   0        0        0      816 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       39 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/__init__.py
+-rw-r--r--   0        0        0     4790 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/test_fedora.py
+-rw-r--r--   0        0        0    16947 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/test_oauth.py
+-rw-r--r--   0        0        0     5487 2023-04-29 08:07:12.000000 bodhi_server-7.2.0/tests/auth/test_utils.py
+-rw-r--r--   0        0        0     5442 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/auth/test_views.py
+-rw-r--r--   0        0        0     2293 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/auth/utils.py
+-rw-r--r--   0        0        0    19037 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/base.py
+-rw-r--r--   0        0        0     2214 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      821 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/__init__.py
+-rwxr-xr-x   0        0        0      335 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/fake-pungi.sh
+-rw-r--r--   0        0        0       76 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/pungi.module.conf
+-rw-r--r--   0        0        0       76 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/pungi.rpm.conf
+-rw-r--r--   0        0        0      210 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/variants.module.xml.j2
+-rw-r--r--   0        0        0       76 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/pungi.basepath/variants.rpm.xml.j2
+-rw-r--r--   0        0        0    20022 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/consumers/test_automatic_updates.py
+-rw-r--r--   0        0        0    11457 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/test_ci.py
+-rw-r--r--   0        0        0     4779 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/consumers/test_consumers.py
+-rw-r--r--   0        0        0    14326 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/consumers/test_resultsdb.py
+-rw-r--r--   0        0        0    13241 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/consumers/test_signed.py
+-rw-r--r--   0        0        0    10129 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/consumers/test_waiverdb.py
+-rw-r--r--   0        0        0      913 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/functional/__init__.py
+-rw-r--r--   0        0        0     2571 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/functional/test_packages.py
+-rw-r--r--   0        0        0     8272 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/functional/test_users.py
+-rw-r--r--   0        0        0      819 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/__init__.py
+-rw-r--r--   0        0        0     2072 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_bshell.py
+-rw-r--r--   0        0        0     5128 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_compat.py
+-rw-r--r--   0        0        0     3597 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_initializedb.py
+-rw-r--r--   0        0        0     5341 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_sar.py
+-rw-r--r--   0        0        0    26242 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_skopeo_lite.py
+-rw-r--r--   0        0        0    15411 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/scripts/test_untag_branched.py
+-rw-r--r--   0        0        0      820 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/__init__.py
+-rw-r--r--   0        0        0     4067 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_builds.py
+-rw-r--r--   0        0        0    27002 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_comments.py
+-rw-r--r--   0        0        0     6469 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_composes.py
+-rw-r--r--   0        0        0     1512 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_csrf.py
+-rw-r--r--   0        0        0     1827 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_errors.py
+-rw-r--r--   0        0        0    31133 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_overrides.py
+-rw-r--r--   0        0        0    30447 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/services/test_releases.py
+-rw-r--r--   0        0        0     3801 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/services/test_schemas.py
+-rw-r--r--   0        0        0   299158 2023-04-29 13:41:50.000000 bodhi_server-7.2.0/tests/services/test_updates.py
+-rw-r--r--   0        0        0      817 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1531 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/base.py
+-rw-r--r--   0        0        0    42724 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/tasks/test_approve_testing.py
+-rw-r--r--   0        0        0    29342 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/tasks/test_check_policies.py
+-rw-r--r--   0        0        0     8649 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/tasks/test_check_signed_builds.py
+-rw-r--r--   0        0        0     5949 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_clean_old_composes.py
+-rw-r--r--   0        0        0   175797 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/tasks/test_composer.py
+-rw-r--r--   0        0        0     3792 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_expire_overrides.py
+-rw-r--r--   0        0        0     3677 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/tasks/test_fetch_test_cases.py
+-rw-r--r--   0        0        0     2799 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_handle_side_and_related_tags.py
+-rw-r--r--   0        0        0     2321 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_tag_update_builds.py
+-rw-r--r--   0        0        0     5085 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/tasks/test_work_on_bugs.py
+-rw-r--r--   0        0        0    11553 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/test___init__.py
+-rw-r--r--   0        0        0     2185 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_alembic.py
+-rw-r--r--   0        0        0    28061 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_bugs.py
+-rw-r--r--   0        0        0    17610 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_buildsys.py
+-rw-r--r--   0        0        0    16269 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_config.py
+-rw-r--r--   0        0        0     4319 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_logging.py
+-rw-r--r--   0        0        0    15586 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_mail.py
+-rw-r--r--   0        0        0    25674 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_metadata.py
+-rw-r--r--   0        0        0   216666 2023-04-29 13:40:09.000000 bodhi_server-7.2.0/tests/test_models.py
+-rw-r--r--   0        0        0     3897 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_notifications.py
+-rw-r--r--   0        0        0    72085 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/test_push.py
+-rw-r--r--   0        0        0     2238 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_renderers.py
+-rw-r--r--   0        0        0     1642 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     7195 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_security.py
+-rw-r--r--   0        0        0    69803 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/test_util.py
+-rw-r--r--   0        0        0    44272 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/test_validators.py
+-rw-r--r--   0        0        0     2614 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/test_webapp.py
+-rw-r--r--   0        0        0     4217 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/testing.ini
+-rw-r--r--   0        0        0      992 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/utils.py
+-rw-r--r--   0        0        0      817 2023-04-29 08:07:13.000000 bodhi_server-7.2.0/tests/views/__init__.py
+-rw-r--r--   0        0        0    23763 2023-04-29 08:18:48.000000 bodhi_server-7.2.0/tests/views/test_generic.py
+-rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 bodhi_server-7.2.0/PKG-INFO
```

### Comparing `bodhi_server-7.1.1/COPYING` & `bodhi_server-7.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/README.rst` & `bodhi_server-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/alembic.ini` & `bodhi_server-7.2.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/apache/bodhi.conf` & `bodhi_server-7.2.0/apache/bodhi.conf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/__init__.py` & `bodhi_server-7.2.0/bodhi/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,17 +357,18 @@
     if not hasattr(generic._generate_home_page_stats, 'invalidate'):
         generic._generate_home_page_stats = get_cacheregion(None).cache_on_arguments()(
             generic._generate_home_page_stats)
 
     if bodhi_config['warm_cache_on_start']:
         log.info('Warming up caches…')
 
-        # Let's warm up the Releases._all_releases cache. We can just call the function - we don't
-        # need to capture the return value.
+        # Let's warm up the Release.all_releases and Release_get_tags caches.
+        # We can just call the function - we don't need to capture the return value.
         models.Release.all_releases()
+        models.Release.get_tags()
 
         # Let's warm up the home page cache by calling _generate_home_page_stats(). We can ignore
         # the return value.
         generic._generate_home_page_stats()
 
     # Let's close out the db session we used to warm the caches.
     Session.remove()
```

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/__init__.py` & `bodhi_server-7.2.0/bodhi/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/fedora.py` & `bodhi_server-7.2.0/bodhi/server/auth/fedora.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/oauth.py` & `bodhi_server-7.2.0/bodhi/server/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/oauth_015.py` & `bodhi_server-7.2.0/bodhi/server/auth/oauth_015.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/oauth_1.py` & `bodhi_server-7.2.0/bodhi/server/auth/oauth_1.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/utils.py` & `bodhi_server-7.2.0/bodhi/server/auth/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/auth/views.py` & `bodhi_server-7.2.0/bodhi/server/auth/views.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/bugs.py` & `bodhi_server-7.2.0/bodhi/server/bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/buildsys.py` & `bodhi_server-7.2.0/bodhi/server/buildsys.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/config.py` & `bodhi_server-7.2.0/bodhi/server/config.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/__init__.py` & `bodhi_server-7.2.0/bodhi/server/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/automatic_updates.py` & `bodhi_server-7.2.0/bodhi/server/consumers/automatic_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/ci.py` & `bodhi_server-7.2.0/bodhi/server/consumers/ci.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/resultsdb.py` & `bodhi_server-7.2.0/bodhi/server/consumers/resultsdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,12 +67,13 @@
                 # update_from_db_message will already have logged why
                 return
             # update the gating status if there's a chance it changed
             status = update.test_gating_status
             if (
                 (passed and status == TestGatingStatus.passed)
                 or (not passed and status == TestGatingStatus.failed)
+                or status == TestGatingStatus.ignored
             ):
                 log.debug("Not updating test_gating_status as no chance of a change")
                 return
             log.info(f"Updating the test_gating_status for: {update.alias}")
             update.update_test_gating_status()
```

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/signed.py` & `bodhi_server-7.2.0/bodhi/server/consumers/signed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/util.py` & `bodhi_server-7.2.0/bodhi/server/consumers/util.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/consumers/waiverdb.py` & `bodhi_server-7.2.0/bodhi/server/consumers/waiverdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,12 +56,15 @@
         if subject is None:
             log.error(f"Couldn't find subject in WaiverDB message {message.id}")
             return
 
         with self.db_factory():
             # find the update
             update = update_from_db_message(message.id, subject)
-            # update the gating status unless it's already "passed", a
-            # waiver can't change it from passed to anything else
-            if update and update.test_gating_status != TestGatingStatus.passed:
-                log.info(f"Updating the test_gating_status for: {update.alias}")
-                update.update_test_gating_status()
+            if update:
+                # update the gating status unless it's already "passed" (a
+                # waiver can't change it from passed to anything else) or
+                # "ignored" (that's not going to change either)
+                updtgs = update.test_gating_status
+                if updtgs not in (TestGatingStatus.passed, TestGatingStatus.ignored):
+                    log.info(f"Updating the test_gating_status for: {update.alias}")
+                    update.update_test_gating_status()
```

### Comparing `bodhi_server-7.1.1/bodhi/server/email/templates/fedora_epel_errata_template.tpl` & `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl` & `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_epel_legacy_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/email/templates/fedora_errata_template.tpl` & `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/email/templates/fedora_modular_errata_template.tpl` & `bodhi_server-7.2.0/bodhi/server/email/templates/fedora_modular_errata_template.tpl`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/exceptions.py` & `bodhi_server-7.2.0/bodhi/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/ffmarkdown.py` & `bodhi_server-7.2.0/bodhi/server/ffmarkdown.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/logging.py` & `bodhi_server-7.2.0/bodhi/server/logging.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/mail.py` & `bodhi_server-7.2.0/bodhi/server/mail.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/metadata.py` & `bodhi_server-7.2.0/bodhi/server/metadata.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/README.rst` & `bodhi_server-7.2.0/bodhi/server/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/__init__.py` & `bodhi_server-7.2.0/bodhi/server/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/env.py` & `bodhi_server-7.2.0/bodhi/server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/script.py.mako` & `bodhi_server-7.2.0/bodhi/server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/190ba571c7d2_remove_the_batching_request_state.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/19e28e9851a2_index_comment_update_id.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/1c97477e38ee_convert_br_override_notes_to_unicodetext.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/2fc96aa44a74_drop_the_user_show_popup_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/325954bac9f7_link_testcases_to_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/3a2e248d1757_add_the_unspecified_enum_to_updatetype.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/499ac8bbe09a_remove_unused_update_sidetag_statuses.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/559acf7e2c16_make_comments_update_not_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/5703ddfe855d_add_package_manager_and_testing_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/58b7919b942c_remove_the_updates_title_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/5c86a3f9dc03_drop_support_for_cve_tracking.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/6b3eb9ae2b87_remove_unused_updatestatus_processing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/7ba286412ad4_drop_the_relationship_between_packages_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/8c4d6aad9b78_add_the_greenwave_failed_enum_to_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/8e9dc57e082d_obsolete_updates_for_archived_release.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/9991cf10ec50_mark_the_bugs_private_field_as_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/9c0a34961768_remove_the_greenwave_unsatisfied_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/__init__.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/a3580bdf5129_remove_the_ci_url_field_from_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/a418acf470f8_drop_the_stacks_table.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/aae0d29d49b7_remove_the_private_field_on_the_bug_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/b1fd856efcf6_add_autopush_boolean_and_stable_days_to_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/bdf0e37ab793_disallow_null_values_in_stable_karma_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/c60d95eef4f1_add_frozen_release_state.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/c98beb4940b5_remove_the_comments_anonymous_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/d399493275b6_add_the_eol_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/d3f8bd499ecd_add_from_tag_column_to_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/d986618207bc_add_composed_by_bodhi_flag_to_releases_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/e3988e00b338_drop_date_pushed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/e5b3ddb35df3_remove_the_greenwave_summary_string_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/e8a059156d38_add_the_create_automatic_updates_bool_.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/eec610d7ab3a_index_the_builds_update_id_column.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/f393d006559b_add_critpath_groups_to_update.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/f50dc199039c_make_comments_user_id_not_nullable.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/f8a44498c806_remove_legacy_old_updateid.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py` & `bodhi_server-7.2.0/bodhi/server/migrations/versions/ff834fa4f23e_increase_the_update_alias_size.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/models.py` & `bodhi_server-7.2.0/bodhi/server/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Bodhi's database models."""
 
 from collections import defaultdict
 from datetime import date, datetime, timedelta
+from functools import lru_cache
 from textwrap import wrap
 import hashlib
 import json
 import os
 import re
 import time
 import typing
@@ -949,76 +950,64 @@
 
         Returns:
             str: The collection name of this release.
         """
         return ' '.join(self.long_name.split()[:-1])
 
     @classmethod
+    @lru_cache(maxsize=1)
     def all_releases(cls):
         """
         Return a mapping of release states to a list of dictionaries describing the releases.
 
         Returns:
             defaultdict: Mapping strings of :class:`ReleaseState` names to lists of dictionaries
             that describe the releases in those states.
         """
-        if cls._all_releases:
-            return cls._all_releases
         releases = defaultdict(list)
         for release in cls.query.order_by(cls.name.desc()).all():
             releases[release.state.value].append(release.__json__())
-        cls._all_releases = releases
-        return cls._all_releases
-    _all_releases = None
+        return releases
 
     @classmethod
-    def clear_all_releases_cache(cls):
-        """Clear up Release cache."""
-        cls._all_releases = None
-
-    @classmethod
-    def get_tags(cls, session):
+    @lru_cache(maxsize=1)
+    def get_tags(cls):
         """
         Return a 2-tuple mapping tags to releases.
 
-        Args:
-            session (sqlalchemy.orm.session.Session): A database session.
         Returns:
             tuple: A 2-tuple. The first element maps the keys 'candidate', 'testing', 'stable',
             'override', 'pending_testing', and 'pending_stable' each to a list of tags for various
             releases that correspond to those tag semantics. The second element maps each koji tag
             to the release's name that uses it.
         """
-        if cls._tag_cache:
-            return cls._tag_cache
         data = {'candidate': [], 'testing': [], 'stable': [], 'override': [],
                 'pending_testing': [], 'pending_stable': []}
         tags = {}  # tag -> release lookup
-        for release in session.query(cls).all():
+        for release in cls.query.filter(cls.state.notin_([ReleaseState.archived,
+                                                          ReleaseState.disabled])).all():
             for key in data:
-                tag = getattr(release, '%s_tag' % key)
+                tag = getattr(release, f'{key}_tag')
                 data[key].append(tag)
                 tags[tag] = release.name
-        cls._tag_cache = (data, tags)
-        return cls._tag_cache
-    _tag_cache = None
+        return (data, tags)
 
     @classmethod
     def from_tags(cls, tags, session):
         """
         Find a release associated with one of the given koji tags.
 
         Args:
             tags (list): A list of koji tags for which an associated release is desired.
             session (sqlalchemy.orm.session.Session): A database session.
         Returns:
             Release or None: The first release found that matches the first tag. If no release is
                 found, ``None`` is returned.
         """
-        tag_types, tag_rels = cls.get_tags(session)
+        tag_types, tag_rels = cls.get_tags()
         for tag in tags:
             if tag not in tag_rels:
                 continue
             release = session.query(cls).filter_by(name=tag_rels[tag]).first()
             if release:
                 return release
 
@@ -2703,16 +2692,23 @@
             up.set_request(db, req, request.user.name)
 
         for key, value in data.items():
             setattr(up, key, value)
 
         up.date_modified = datetime.utcnow()
 
-        notifications.publish(update_schemas.UpdateEditV1.from_dict(
-            message={'update': up, 'agent': request.user.name, 'new_bugs': new_bugs}))
+        notifications.publish(update_schemas.UpdateEditV2.from_dict(
+            message={
+                'update': up,
+                'agent': request.user.name,
+                'new_bugs': new_bugs,
+                'new_builds': new_builds,
+                'removed_builds': removed_builds
+            }
+        ))
 
         # If editing a Pending update, all of whose builds are signed, for a release
         # which isn't composed by Bodhi (i.e. Rawhide), move it directly to Testing.
         if not up.release.composed_by_bodhi and up.status == UpdateStatus.pending \
                 and up.signed:
             log.info("Every build in the update is signed, set status to testing")
             up.status = UpdateStatus.testing
@@ -3705,15 +3701,15 @@
 
         Args:
             db (sqlalchemy.orm.session.Session): A database session.
             preserve_override: whether to preserve the override tag or not
         """
         log.info("Untagging %s", self.alias)
         koji = buildsys.get_session()
-        tag_types, tag_rels = Release.get_tags(db)
+        tag_types, tag_rels = Release.get_tags()
         koji.multicall = True
         for build in self.builds:
             for tag in build.get_tags():
                 # Only remove tags that we know about
                 if tag in tag_rels:
                     if preserve_override and tag == self.release.override_tag:
                         log.info("Skipping override tag")
```

### Comparing `bodhi_server-7.1.1/bodhi/server/notifications.py` & `bodhi_server-7.2.0/bodhi/server/notifications.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/push.py` & `bodhi_server-7.2.0/bodhi/server/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # We don't want to authenticate to the buildsystem, because this script is often mistakenly
         # run as root and this can cause the ticket cache to become root owned with 0600 perms,
         # which will cause the compose to fail when it tries to use it to authenticate to Koji.
         buildsys.setup_buildsystem(config, authenticate=False)
         _koji = get_koji(None)
     for build in update.builds:
         if not build.signed:
-            build_tags = build.get_tags(_koji)
+            build_tags = build.get_tags()
             if update.release.pending_signing_tag not in build_tags:
                 click.echo('Build %s was refreshed as signed' % build.nvr)
                 build.signed = True
             else:
                 click.echo('Build %s still unsigned' % build.nvr)
```

### Comparing `bodhi_server-7.1.1/bodhi/server/renderers.py` & `bodhi_server-7.2.0/bodhi/server/renderers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/schemas.py` & `bodhi_server-7.2.0/bodhi/server/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,20 @@
 
     exclude_archived = colander.SchemaNode(
         colander.Boolean(true_choices=('true', '1')),
         location="querystring",
         missing=None,
     )
 
+    active = colander.SchemaNode(
+        colander.Boolean(true_choices=('true', '1')),
+        location="querystring",
+        missing=True,
+    )
+
 
 class SaveReleaseSchema(CSRFProtectedSchema, colander.MappingSchema):
     """An API schema for bodhi.server.services.releases.save_release()."""
 
     name = colander.SchemaNode(
         colander.String(),
     )
```

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/__init__.py` & `bodhi_server-7.2.0/bodhi/server/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/bshell.py` & `bodhi_server-7.2.0/bodhi/server/scripts/bshell.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/compat.py` & `bodhi_server-7.2.0/bodhi/server/scripts/compat.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/initializedb.py` & `bodhi_server-7.2.0/bodhi/server/scripts/initializedb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/sar.py` & `bodhi_server-7.2.0/bodhi/server/scripts/sar.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/skopeo_lite.py` & `bodhi_server-7.2.0/bodhi/server/scripts/skopeo_lite.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/scripts/untag_branched.py` & `bodhi_server-7.2.0/bodhi/server/scripts/untag_branched.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/security.py` & `bodhi_server-7.2.0/bodhi/server/security.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/__init__.py` & `bodhi_server-7.2.0/bodhi/server/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/builds.py` & `bodhi_server-7.2.0/bodhi/server/services/builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/comments.py` & `bodhi_server-7.2.0/bodhi/server/services/comments.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/composes.py` & `bodhi_server-7.2.0/bodhi/server/services/composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/csrf.py` & `bodhi_server-7.2.0/bodhi/server/services/csrf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/errors.py` & `bodhi_server-7.2.0/bodhi/server/services/errors.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/markdown.py` & `bodhi_server-7.2.0/bodhi/server/services/markdown.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/metrics_tween.py` & `bodhi_server-7.2.0/bodhi/server/services/metrics_tween.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/overrides.py` & `bodhi_server-7.2.0/bodhi/server/services/overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/packages.py` & `bodhi_server-7.2.0/bodhi/server/services/packages.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/releases.py` & `bodhi_server-7.2.0/bodhi/server/services/releases.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,15 +233,15 @@
             dict: A dictionary describing the counts of the updates, as described above.
         """
         basequery = basequery.filter(Update.status == status)
         return {
             '{}_updates_total'.format(status.description): basequery.count(),
         }
 
-    def get_update_counts(releaseid):
+    def get_update_counts(releaseid, stable_only: bool = False):
         """
         Return counts for the various states and types of updates in the given release.
 
         This function returns a dictionary that tabulates the counts of the various
         types of Bodhi updates at the various states they can appear in. The
         dictionary has the following keys, with pretty self-explanatory names:
 
@@ -253,27 +253,36 @@
             releaseid (str): The id of the Release object you would like the counts performed on
         Returns:
             dict: A dictionary expressing the counts, as described above.
         """
         release = Release.get(releaseid)
         basequery = Update.query.filter(Update.release == release)
         counts = {}
-        counts.update(_get_status_counts(basequery, UpdateStatus.pending))
-        counts.update(_get_status_counts(basequery, UpdateStatus.testing))
+        if not stable_only:
+            counts.update(_get_status_counts(basequery, UpdateStatus.pending))
+            counts.update(_get_status_counts(basequery, UpdateStatus.testing))
         counts.update(_get_status_counts(basequery, UpdateStatus.stable))
 
         return counts
 
+    data = request.validated
+
     release_updates_counts = {}
     releases = Release.all_releases()
-    for release in (releases['current'] + releases['pending'] + releases['archived']
-                    + releases['frozen']):
-        release_updates_counts[release["name"]] = get_update_counts(release["name"])
+    active = data.get('active')
+    if active is False:
+        for release in (releases['archived'] + releases['disabled']):
+            release_updates_counts[release["name"]] = get_update_counts(release["name"],
+                                                                        stable_only=True)
+    else:
+        for release in (releases['current'] + releases['pending'] + releases['frozen']):
+            release_updates_counts[release["name"]] = get_update_counts(release["name"])
 
-    return {"release_updates_counts": release_updates_counts}
+    return {"release_updates_counts": release_updates_counts,
+            "active": active}
 
 
 @releases.get(accept=('application/json', 'text/json'),
               schema=bodhi.server.schemas.ListReleaseSchema(), renderer='json',
               error_handler=bodhi.server.services.errors.json_handler,
               validators=releases_get_validators)
 def query_releases_json(request):
@@ -370,15 +379,14 @@
     # it since the models don't care about a csrf argument.
     data.pop('csrf_token', None)
 
     try:
         if edited is None:
             log.info("Creating a new release: %s" % data['name'])
             r = Release(**data)
-
         else:
             log.info("Editing release: %s" % edited)
             r = request.db.query(Release).filter(Release.name == edited).one()
             for k, v in data.items():
                 # We have to change updates status to obsolete
                 # if state of release changes to archived
                 if k == "state" and v == ReleaseState.archived and \
@@ -410,21 +418,21 @@
                         u.comment(
                             request.db,
                             'There is an ongoing freeze; this will be pushed to'
                             ' stable after the freeze is over.',
                             author='bodhi',
                         )
                 setattr(r, k, v)
-
-        # We have to invalidate the release cache after change
-        Release.clear_all_releases_cache()
-
     except Exception as e:
         log.exception(e)
         request.errors.add('body', 'release',
                            'Unable to create/edit release: %s' % e)
         return
 
     request.db.add(r)
-    request.db.flush()
+    request.db.commit()
+
+    # We have to invalidate the release caches after change
+    Release.all_releases.cache_clear()
+    Release.get_tags.cache_clear()
 
     return r
```

### Comparing `bodhi_server-7.1.1/bodhi/server/services/schemas.py` & `bodhi_server-7.2.0/bodhi/server/services/schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/updates.py` & `bodhi_server-7.2.0/bodhi/server/services/updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/services/user.py` & `bodhi_server-7.2.0/bodhi/server/services/user.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/__init__.py` & `bodhi_server-7.2.0/bodhi/server/static/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/bodhi-logo.svg` & `bodhi_server-7.2.0/bodhi/server/static/bodhi-logo.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/css/site.css` & `bodhi_server-7.2.0/bodhi/server/static/css/site.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/FontAwesome.otf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/font-awesome.css` & `bodhi_server-7.2.0/bodhi/server/static/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-bolditalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/hack-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bold-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-bolditalic-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-italic-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/eot/latin/hack-regular-latin-webfont.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-bolditalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/hack-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bold-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-bolditalic-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-italic-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/web-ttf/latin/hack-regular-latin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-bolditalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/hack-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bold-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-bolditalic-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-italic-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff/latin/hack-regular-latin-webfont.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-bolditalic-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-italic-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/hack-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bold-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-bolditalic-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-italic-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack/woff2/latin/hack-regular-latin-webfont.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/hack.css` & `bodhi_server-7.2.0/bodhi/server/static/fonts/hack.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.eot`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.ttf`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans/open-sans-v13-latin_latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/fonts/open-sans.css` & `bodhi_server-7.2.0/bodhi/server/static/fonts/open-sans.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/ico/favicon.ico` & `bodhi_server-7.2.0/bodhi/server/static/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/img/bodhi-logo.png` & `bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/img/bodhi-logo.svg` & `bodhi_server-7.2.0/bodhi/server/static/img/bodhi-logo.svg`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/img/logo-large.png` & `bodhi_server-7.2.0/bodhi/server/static/img/logo-large.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/img/logo.png` & `bodhi_server-7.2.0/bodhi/server/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/js/comment_form.js` & `bodhi_server-7.2.0/bodhi/server/static/js/comment_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/js/forms.js` & `bodhi_server-7.2.0/bodhi/server/static/js/forms.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/js/override_form.js` & `bodhi_server-7.2.0/bodhi/server/static/js/override_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/js/search.js` & `bodhi_server-7.2.0/bodhi/server/static/js/search.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/js/site.js` & `bodhi_server-7.2.0/bodhi/server/static/js/site.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/js/update_form.js` & `bodhi_server-7.2.0/bodhi/server/static/js/update_form.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/chartjs/chart.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/chartjs/chart.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map` & `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map` & `bodhi_server-7.2.0/bodhi/server/static/vendor/fedora-bootstrap/fedora-bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map` & `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery/jquery-3.6.0.min.map`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/jquery-typeahead/jquery.typeahead.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-spinner.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-spinner.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-air.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-block.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-flat.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-future.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger-theme-ice.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/css/messenger.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/css/messenger.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-flat.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger-theme-future.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/messenger/js/messenger.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/messenger/js/messenger.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/moment/moment.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize-0.15.2.min.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css` & `bodhi_server-7.2.0/bodhi/server/static/vendor/selectize/selectize.bootstrap5-0.15.2.css`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/static/vendor/typeahead/typeahead.bundle.js` & `bodhi_server-7.2.0/bodhi/server/static/vendor/typeahead/typeahead.bundle.js`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/__init__.py` & `bodhi_server-7.2.0/bodhi/server/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/approve_testing.py` & `bodhi_server-7.2.0/bodhi/server/tasks/approve_testing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/check_policies.py` & `bodhi_server-7.2.0/bodhi/server/tasks/check_policies.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/check_signed_builds.py` & `bodhi_server-7.2.0/bodhi/server/tasks/check_signed_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/clean_old_composes.py` & `bodhi_server-7.2.0/bodhi/server/tasks/clean_old_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/composer.py` & `bodhi_server-7.2.0/bodhi/server/tasks/composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -560,15 +560,15 @@
     @checkpoint
     def determine_and_perform_tag_actions(self):
         """Call _determine_tag_actions() and _perform_tag_actions()."""
         self._determine_tag_actions()
         self._perform_tag_actions()
 
     def _determine_tag_actions(self):
-        tag_types, tag_rels = Release.get_tags(self.db)
+        tag_types, tag_rels = Release.get_tags()
         # sync & async tagging batches
         for i, batch in enumerate(sorted_updates(self.compose.updates)):
             for update in batch:
                 add_tags = []
                 move_tags = []
 
                 if update.status is UpdateStatus.testing:
```

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/expire_overrides.py` & `bodhi_server-7.2.0/bodhi/server/tasks/expire_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/fetch_test_cases.py` & `bodhi_server-7.2.0/bodhi/server/tasks/fetch_test_cases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/handle_side_and_related_tags.py` & `bodhi_server-7.2.0/bodhi/server/tasks/handle_side_and_related_tags.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/tag_update_builds.py` & `bodhi_server-7.2.0/bodhi/server/tasks/tag_update_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/tasks/work_on_bugs.py` & `bodhi_server-7.2.0/bodhi/server/tasks/work_on_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/comments.html` & `bodhi_server-7.2.0/bodhi/server/templates/comments.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/compose.html` & `bodhi_server-7.2.0/bodhi/server/templates/compose.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/composes.html` & `bodhi_server-7.2.0/bodhi/server/templates/composes.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/fragments.html` & `bodhi_server-7.2.0/bodhi/server/templates/fragments.html`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
       <div class="modal-content">
         <div class="modal-header">
           <button type="button" class="close" data-bs-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
           <h4 class="modal-title" id="markdown-help-label">Fedora-Flavored Markdown</h4>
         </div>
         <div class="modal-body">
           <p> Text fields in Bodhi2 support an
-          <a href="https://github.com/fedora-infra/bodhi/blob/develop/bodhi/server/ffmarkdown.py">enhanced</a>
+          <a href="https://github.com/fedora-infra/bodhi/blob/develop/bodhi-server/bodhi/server/ffmarkdown.py">enhanced</a>
           version of <a href="http://daringfireball.net/projects/markdown/syntax" target="_blank">markdown</a>.
           This is a cheat sheet for your reference.
           </p>
           <hr/>
           <div class="row">
             <div class="col-md-4">
               <p>You can do <strong>headers</strong> by underlining or by prefixing with the <code>&#35;</code> character:</p>
```

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/home.html` & `bodhi_server-7.2.0/bodhi/server/templates/home.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/master.html` & `bodhi_server-7.2.0/bodhi/server/templates/master.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/new_update.html` & `bodhi_server-7.2.0/bodhi/server/templates/new_update.html`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   eol_list = eol_releases()
 %>
 
 <%block name="css">
 ${parent.css()}
 <link href="${request.static_url('bodhi.server:static/vendor/messenger/css/messenger.css') }" rel="stylesheet" />
 <link href="${request.static_url('bodhi.server:static/vendor/messenger/css/messenger-theme-flat.css') }" rel="stylesheet" />
-<link href="${request.static_url('bodhi.server:static/vendor/selectize/selectize.bootstrap5-0.15.2.css') }" rel="stylesheet" />
+<link href="${request.static_url('bodhi.server:static/vendor/selectize/selectize.bootstrap5-0.14.0.css') }" rel="stylesheet" />
 </%block>
 
 <div class="subheader">
     <div class="container py-4">
       <div class="row">
         <div class="col">
             <h3 class="fw-bold m-0"><a href="${request.route_url('updates')}">Updates</a>
@@ -409,15 +409,15 @@
               </button>
             </div>
 
   </div>
 </div></div></div>
 <%block name="javascript">
 ${parent.javascript()}
-<script src="${request.static_url('bodhi.server:static/vendor/selectize/selectize-0.15.2.min.js')}"></script>
+<script src="${request.static_url('bodhi.server:static/vendor/selectize/selectize-0.14.0.min.js')}"></script>
 % if update and update.from_tag:
   <script>var existing_sidetag_update = true;</script>
 % else:
   <script>var existing_sidetag_update = false;</script>
 % endif
 <script src="${request.static_url('bodhi.server:static/vendor/messenger/js/messenger.min.js')}"></script>
 <script src="${request.static_url('bodhi.server:static/vendor/messenger/js/messenger-theme-flat.js')}"></script>
```

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/override.html` & `bodhi_server-7.2.0/bodhi/server/templates/override.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/overrides.html` & `bodhi_server-7.2.0/bodhi/server/templates/overrides.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/pager.html` & `bodhi_server-7.2.0/bodhi/server/templates/pager.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/release.html` & `bodhi_server-7.2.0/bodhi/server/templates/release.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/releases.html` & `bodhi_server-7.2.0/bodhi/server/templates/releases.html`

 * *Files 10% similar despite different names*

```diff
@@ -48,23 +48,35 @@
   </ul>
 </%def>
 
 <div class="subheader py-4">
     <div class="container">
       <div class="row">
           <div class="col-md-6 col-md-offset-3">
-              <h3 class="fw-bold m-0">Releases</h3>
+              % if active:
+              <h3 class="fw-bold m-0 mb-2">Active Releases</h3>
+              <span>See here for <a href="${request.route_url('releases')}?active=false">Archived and disabled Releases</a></span>
+              % else:
+              <h3 class="fw-bold m-0 mb-2">Archived and disabled Releases</h3>
+              <span>See here for <a href="${request.route_url('releases')}">Active Releases</a></span>
+              % endif
           </div>
       </div>
     </div>
   </div>
 <div class="container pt-2">
-    ${release_list('current', stable_only=False)}
-    ${release_list('pending', stable_only=False)}
-    ${release_list('archived', stable_only=True)}
+    % if active:
+      ${release_list('current', stable_only=False)}
+      ${release_list('pending', stable_only=False)}
+    % else:
+      ${release_list('archived', stable_only=True)}
+      % if request.releases['disabled']:
+        ${release_list('disabled', stable_only=True)}
+      % endif
+    % endif
 </div>
 
 <%block name="javascript">
 ${parent.javascript()}
 <script>
   $(document).ready(function() {
     // Initialize tooltips
```

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/update.html` & `bodhi_server-7.2.0/bodhi/server/templates/update.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <%inherit file="master.html"/>
 <%namespace name="json" module="json"/>
 <%
-  from urllib.parse import urljoin
+  from urllib.parse import quote, urljoin
 
   from bodhi.server import models
 
   from bodhi.server.config import config
 
   install_command = update.install_command
 %>
@@ -93,17 +93,15 @@
                 <br/><span data-bs-toggle="tooltip" title="This update is in critical path groups ${update.critpath_groups}" class="ms-n2 text-muted"><small> <i class="fa fa-fw fa-fire"></i></small></span>
                 % elif update.critpath:
                 <br/><span data-bs-toggle="tooltip" title="This update is in the critical path" class="ms-n2 text-muted"><small> <i class="fa fa-fw fa-fire"></i></small></span>
                 % endif
               </div>
               <div class="flex-grow-1 ms-0">
                     <h3 class="fw-bold">
-                      <a href="${request.route_url('update', id=update['alias'])}">
                       ${update.get_title(amp=True,nvr=True,beautify=True) | h}
-                      </a>
                     </h3>
                     ${update.alias} created by <a href="${request.route_url('user', name=update['user']['name'])}"> ${update['user']['name']}</a>
                     <span title="${update['date_submitted']} UTC"> ${self.util.age(update['date_submitted'])} </span>
                     for <a href="${request.route_url('release', name=update['release']['name'])}">${update['release']['long_name']}
                     </a>
               </div>
             </div>
@@ -601,15 +599,15 @@
               % if build.signed:
               <span class="fa fa-key text-muted me-2" aria-hidden="true" data-bs-toggle="tooltip" data-placement="top" title="Build signed"></span>
               % endif
             </div>
             <div class="flex-grow-1">
               <%
                 koji_web_url = request.registry.settings.get('koji_web_url').strip('/') + '/'
-                build_url = urljoin(koji_web_url, 'search?terms='+build.nvr+'&type=build&match=exact')
+                build_url = urljoin(koji_web_url, 'search?terms='+quote(build.nvr)+'&type=build&match=exact')
               %>
               <a href="${build_url}" target="_blank">${build.nvr}</a>
             </div>
             <div class="flex-shrink-0">
               <a href='${request.route_url("updates_rss") + "?packages="}${build.package.name | u}'>
                 <span class="fa fa-rss ms-1" data-bs-toggle="tooltip" data-placement="top" title="RSS feed for new Bodhi updates containing ${build.package.name}"></span>
               </a>
@@ -764,16 +762,16 @@
       PASSED: 'check-circle',
       INFO: 'info-circle',
       FAILED: 'minus-circle',
       NEEDS_INSPECTION: 'exclamation-circle',
       ABORTED: 'trash',
       CRASHED: 'fire', // no joke.
       ABSENT: 'question-circle',
-      QUEUED: 'hourglass-top',
-      RUNNING: 'hourglass-split'
+      QUEUED: 'hourglass-start',
+      RUNNING: 'hourglass-half'
     }
 
     var update = '${update.alias}';
     var builds = ${update.builds_json | n};
 
     // These are the required taskotron tests
     var requirements = ${update.requirements_json | h};
```

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/updates.html` & `bodhi_server-7.2.0/bodhi/server/templates/updates.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/templates/user.html` & `bodhi_server-7.2.0/bodhi/server/templates/user.html`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/util.py` & `bodhi_server-7.2.0/bodhi/server/util.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/validators.py` & `bodhi_server-7.2.0/bodhi/server/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
     """
     Ensure that all of the referenced builds are tagged as candidates.
 
     Args:
         request (pyramid.request.Request): The current request.
         kwargs (dict): The kwargs of the related service definition. Unused.
     """
-    tag_types, tag_rels = Release.get_tags(request.db)
+    tag_types, tag_rels = Release.get_tags()
     edited = request.validated.get('edited')
     release = None
     if edited:
         valid_tags = tag_types['candidate'] + tag_types['testing']
         update = request.db.query(Update).filter_by(alias=edited).first()
         if not update:
             # No need to tack on any more errors here, since they should have
@@ -361,15 +361,15 @@
     """
     Ensure that the referenced tags are valid Koji tags.
 
     Args:
         request (pyramid.request.Request): The current request.
         kwargs (dict): The kwargs of the related service definition. Unused.
     """
-    tag_types, tag_rels = Release.get_tags(request.db)
+    tag_types, tag_rels = Release.get_tags()
 
     for tag_type in tag_types:
         tag_name = request.validated.get("%s_tag" % tag_type)
 
         if not tag_name:
             continue
 
@@ -1146,15 +1146,15 @@
             request.errors.add("body", "nvr", "Cannot create a buildroot override"
                                " if build's test gating status is failed.")
             return
 
         if not build.release:
             # Oddly, the build has no associated release.  Let's try to figure
             # that out and apply it.
-            tag_types, tag_rels = Release.get_tags(request.db)
+            tag_types, tag_rels = Release.get_tags()
             valid_tags = tag_types['candidate'] + tag_types['testing']
 
             tags = [tag['name'] for tag in request.koji.listTags(nvr)
                     if tag['name'] in valid_tags]
 
             release = Release.from_tags(tags, db)
 
@@ -1179,15 +1179,15 @@
             # The build is tagged neither as a candidate or testing, it can't
             # be in a buildroot override
             request.errors.add('body', 'nvr', 'Invalid build.  It must be '
                                'tagged as either candidate or testing.')
             return
 
     else:
-        tag_types, tag_rels = Release.get_tags(request.db)
+        tag_types, tag_rels = Release.get_tags()
         valid_tags = tag_types['candidate'] + tag_types['testing']
 
         try:
             tags = [tag['name'] for tag in request.koji.listTags(nvr)
                     if tag['name'] in valid_tags]
         except Exception as e:
             request.errors.add('body', 'nvr', "Couldn't determine koji tags "
```

### Comparing `bodhi_server-7.1.1/bodhi/server/views/__init__.py` & `bodhi_server-7.2.0/bodhi/server/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/bodhi/server/views/generic.py` & `bodhi_server-7.2.0/bodhi/server/views/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
             used to pass the package name being queried.
     Returns:
         dict: A dictionary of the release dist tag to the latest build.
     """
     builds = {}
     koji = request.koji
     package = request.params.get('package')
-    for tag_type, tags in models.Release.get_tags(request.db)[0].items():
+    for tag_type, tags in models.Release.get_tags()[0].items():
         for tag in tags:
             try:
                 for build in koji.getLatestBuilds(tag, package=package):
                     builds[tag] = build['nvr']
             except Exception:  # Things like EPEL don't have pending tags
                 pass
     return builds
```

### Comparing `bodhi_server-7.1.1/bodhi/server/webapp.py` & `bodhi_server-7.2.0/bodhi/server/webapp.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/celeryconfig.py` & `bodhi_server-7.2.0/celeryconfig.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/Makefile` & `bodhi_server-7.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/conf.py` & `bodhi_server-7.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/man_pages/bodhi-push.rst` & `bodhi_server-7.2.0/docs/man_pages/bodhi-push.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/man_pages/bodhi-sar.rst` & `bodhi_server-7.2.0/docs/man_pages/bodhi-sar.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/man_pages/bodhi-shell.rst` & `bodhi_server-7.2.0/docs/man_pages/bodhi-shell.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/man_pages/bodhi-skopeo-lite.rst` & `bodhi_server-7.2.0/docs/man_pages/bodhi-skopeo-lite.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/man_pages/bodhi-untag-branched.rst` & `bodhi_server-7.2.0/docs/man_pages/bodhi-untag-branched.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/docs/man_pages/initialize_bodhi_db.rst` & `bodhi_server-7.2.0/docs/man_pages/initialize_bodhi_db.rst`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/production.ini` & `bodhi_server-7.2.0/production.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/pyproject.toml` & `bodhi_server-7.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bodhi-server"
-version = "7.1.1"
+version = "7.2.0"
 description = "Bodhi server"
 readme = "README.rst"
 authors = ["Fedora Infrastructure Team"]
 maintainers = ["Fedora Infrastructure Team <infrastructure@lists.fedoraproject.org>"]
 repository = "https://github.com/fedora-infra/bodhi"
 homepage = "https://bodhi.fedoraproject.rog"
 keywords = ["web", "fedora", "pyramid"]
```

### Comparing `bodhi_server-7.1.1/tests/__init__.py` & `bodhi_server-7.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/auth/test_fedora.py` & `bodhi_server-7.2.0/tests/auth/test_fedora.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/auth/test_oauth.py` & `bodhi_server-7.2.0/tests/auth/test_oauth.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/auth/test_utils.py` & `bodhi_server-7.2.0/tests/auth/test_utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/auth/test_views.py` & `bodhi_server-7.2.0/tests/auth/test_views.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/auth/utils.py` & `bodhi_server-7.2.0/tests/auth/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/base.py` & `bodhi_server-7.2.0/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,16 +228,16 @@
         """Set up Bodhi for testing."""
         self.config = testing.setUp()
         self.app_settings = get_appsettings(os.environ["BODHI_CONFIG"])
         config.config.clear()
         config.config.load_config(self.app_settings)
 
         # Ensure "cached" objects are cleared before each test.
-        models.Release.clear_all_releases_cache()
-        models.Release._tag_cache = None
+        models.Release.all_releases.cache_clear()
+        models.Release.get_tags.cache_clear()
 
         if engine is None:
             self.engine = _configure_test_db(config.config["sqlalchemy.url"])
         else:
             self.engine = engine
 
         self.connection = self.engine.connect()
@@ -382,16 +382,16 @@
             pending_stable_tag='f{}-updates-pending'.format(version),
             override_tag='f{}-override'.format(version),
             branch='f{}'.format(version), state=models.ReleaseState.current,
             create_automatic_updates=create_automatic_updates,
             package_manager=models.PackageManager.unspecified,
             testing_repository=None)
         self.db.add(release)
-        models.Release.clear_all_releases_cache()
-        models.Release._tag_cache = None
+        models.Release.all_releases.cache_clear()
+        models.Release.get_tags.cache_clear()
         self.db.flush()
         return release
 
 
 class BasePyTestCase(BaseTestCaseMixin):
     """Wraps BaseTestCaseMixin for pytest users.
```

### Comparing `bodhi_server-7.1.1/tests/conftest.py` & `bodhi_server-7.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/consumers/__init__.py` & `bodhi_server-7.2.0/tests/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/consumers/test_automatic_updates.py` & `bodhi_server-7.2.0/tests/consumers/test_automatic_updates.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/consumers/test_ci.py` & `bodhi_server-7.2.0/tests/consumers/test_ci.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/consumers/test_consumers.py` & `bodhi_server-7.2.0/tests/consumers/test_consumers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/consumers/test_resultsdb.py` & `bodhi_server-7.2.0/tests/consumers/test_resultsdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,18 +97,23 @@
             update.test_gating_status = models.TestGatingStatus.failed
             self.handler(testmsg)
             assert update.test_gating_status == models.TestGatingStatus.passed
             # and waiting
             update.test_gating_status = models.TestGatingStatus.waiting
             self.handler(testmsg)
             assert update.test_gating_status == models.TestGatingStatus.passed
-            # now check we don't update if already passed
+            # now check we don't update if already passed...
             with mock.patch("bodhi.server.models.Update.update_test_gating_status") as updmock:
                 self.handler(testmsg)
                 assert updmock.call_count == 0
+                # ...or ignored
+                update.test_gating_status = models.TestGatingStatus.ignored
+                self.handler(testmsg)
+                assert updmock.call_count == 0
+                assert update.test_gating_status == models.TestGatingStatus.ignored
 
     def test_resultsdb_failed_koji_test(self):
         """
         Assert that a failed test ResultsDB message for a Koji build
         from an update updates the gating status of the update if in
         passed or waiting status, or with no status.
         """
@@ -148,18 +153,23 @@
             update.test_gating_status = models.TestGatingStatus.failed
             self.handler(testmsg)
             assert update.test_gating_status == models.TestGatingStatus.failed
             # and waiting
             update.test_gating_status = models.TestGatingStatus.waiting
             self.handler(testmsg)
             assert update.test_gating_status == models.TestGatingStatus.failed
-            # now check we don't update if already failed
+            # now check we don't update if already failed...
             with mock.patch("bodhi.server.models.Update.update_test_gating_status") as updmock:
                 self.handler(testmsg)
                 assert updmock.call_count == 0
+                # ...or ignored
+                update.test_gating_status = models.TestGatingStatus.ignored
+                self.handler(testmsg)
+                assert updmock.call_count == 0
+                assert update.test_gating_status == models.TestGatingStatus.ignored
 
     def test_resultsdb_bodhi_tests(self):
         """
         Assert that ResultsDB messages for tests on an update result in
         the gating status of that update being updated.
         """
         update = self.single_build_update
```

### Comparing `bodhi_server-7.1.1/tests/consumers/test_signed.py` & `bodhi_server-7.2.0/tests/consumers/test_signed.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/consumers/test_waiverdb.py` & `bodhi_server-7.2.0/tests/consumers/test_waiverdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,18 +92,23 @@
             update.test_gating_status = models.TestGatingStatus.failed
             self.handler(testmsg)
             assert update.test_gating_status == models.TestGatingStatus.passed
             # and waiting
             update.test_gating_status = models.TestGatingStatus.waiting
             self.handler(testmsg)
             assert update.test_gating_status == models.TestGatingStatus.passed
-            # now check we don't update if already passed
+            # now check we don't update if already passed...
             with mock.patch("bodhi.server.models.Update.update_test_gating_status") as updmock:
                 self.handler(testmsg)
                 assert updmock.call_count == 0
+                # ...or ignored
+                update.test_gating_status = models.TestGatingStatus.ignored
+                self.handler(testmsg)
+                assert updmock.call_count == 0
+                assert update.test_gating_status == models.TestGatingStatus.ignored
 
     def test_waiverdb_bodhi_waiver(self):
         """
         Assert that a Bodhi update waiver message updates the gating
         status of the update.
         """
         update = self.single_build_update
```

### Comparing `bodhi_server-7.1.1/tests/functional/__init__.py` & `bodhi_server-7.2.0/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/functional/test_packages.py` & `bodhi_server-7.2.0/tests/functional/test_packages.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/functional/test_users.py` & `bodhi_server-7.2.0/tests/functional/test_users.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/__init__.py` & `bodhi_server-7.2.0/tests/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/test_bshell.py` & `bodhi_server-7.2.0/tests/scripts/test_bshell.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/test_compat.py` & `bodhi_server-7.2.0/tests/scripts/test_compat.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/test_initializedb.py` & `bodhi_server-7.2.0/tests/scripts/test_initializedb.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/test_sar.py` & `bodhi_server-7.2.0/tests/scripts/test_sar.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/test_skopeo_lite.py` & `bodhi_server-7.2.0/tests/scripts/test_skopeo_lite.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/scripts/test_untag_branched.py` & `bodhi_server-7.2.0/tests/scripts/test_untag_branched.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/__init__.py` & `bodhi_server-7.2.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_builds.py` & `bodhi_server-7.2.0/tests/services/test_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_comments.py` & `bodhi_server-7.2.0/tests/services/test_comments.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_composes.py` & `bodhi_server-7.2.0/tests/services/test_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_csrf.py` & `bodhi_server-7.2.0/tests/services/test_csrf.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_errors.py` & `bodhi_server-7.2.0/tests/services/test_errors.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_overrides.py` & `bodhi_server-7.2.0/tests/services/test_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_releases.py` & `bodhi_server-7.2.0/tests/services/test_releases.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,14 +584,27 @@
             pending_signing_tag='f37-updates-testing-signing',
             pending_testing_tag='f37-updates-testing-pending',
             pending_stable_tag='f37-updates-pending',
             override_tag='f37-override',
             branch='f37', state=ReleaseState.frozen)
         self.db.add(release)
 
+        release = Release(
+            name='F25', long_name='Fedora 25',
+            id_prefix='FEDORA', version='25',
+            dist_tag='f25', stable_tag='f25-updates',
+            testing_tag='f25-updates-testing',
+            candidate_tag='f25-updates-candidate',
+            pending_signing_tag='f25-updates-testing-signing',
+            pending_testing_tag='f25-updates-testing-pending',
+            pending_stable_tag='f25-updates-pending',
+            override_tag='f25-override',
+            branch='f25', state=ReleaseState.archived)
+        self.db.add(release)
+
         currentrelease = self.db.query(Release).filter_by(name='F17').one()
         addedupdates = [[UpdateStatus.pending,
                          [[UpdateType.security, 5],
                           [UpdateType.bugfix, 4],
                           [UpdateType.enhancement, 3],
                           [UpdateType.newpackage, 2]]],
                         [UpdateStatus.testing,
@@ -642,17 +655,26 @@
                           [[UpdateType.security, 7],
                            [UpdateType.bugfix, 14],
                            [UpdateType.enhancement, 31],
                            [UpdateType.newpackage, 45]]]]
         with fml_testing.mock_sends():
             _add_updates(addedupdates3, user2, frozenrelease, "fc37")
 
+        archivedrelease = self.db.query(Release).filter_by(name='F25').one()
+        addedupdates4 = [[UpdateStatus.stable,
+                          [[UpdateType.security, 19],
+                           [UpdateType.bugfix, 18],
+                           [UpdateType.enhancement, 17],
+                           [UpdateType.newpackage, 16]]]]
+        with fml_testing.mock_sends():
+            _add_updates(addedupdates4, user2, archivedrelease, "fc25")
+
         self.db.flush()
         # Clear the caches
-        Release._tag_cache = None
+        Release.get_tags.cache_clear()
         generic._generate_home_page_stats.invalidate()
 
     def test_release_counts(self):
         """Test the release page update counts"""
         res = self.app.get('/releases/', headers={'Accept': 'text/html'}, status=200)
         # Assert that pending updates counts in a current release are displayed properly
         # Note the bug update count here is one more than what we generate above
@@ -675,7 +697,19 @@
                 'until freeze is lifted">frozen</span>') in res
 
         # Assert that testing updates counts in a frozen release are displayed properly
         assert '?releases=F37&amp;status=testing">80' in res
 
         # Assert that stable updates counts in a frozen release are displayed properly
         assert '?releases=F37&amp;status=stable">97' in res
+
+        # Assert that archived release is not showed
+        assert '?releases=F25&amp;status=stable' not in res
+
+    def test_archived_release_page(self):
+        """Test the release page update counts"""
+        res = self.app.get('/releases/?active=false', headers={'Accept': 'text/html'}, status=200)
+        # Assert that archived release is showed
+        assert '?releases=F25&amp;status=stable">70' in res
+
+        # Assert that current release is not showed
+        assert '?releases=F17&amp;status=stable' not in res
```

### Comparing `bodhi_server-7.1.1/tests/services/test_schemas.py` & `bodhi_server-7.2.0/tests/services/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/services/test_updates.py` & `bodhi_server-7.2.0/tests/services/test_updates.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 from bodhi.server.exceptions import BodhiException, LockedUpdateException
 from bodhi.server.models import (
     Build,
     BuildrootOverride,
     Compose,
     Group,
     ModulePackage,
-    PackageManager,
     Release,
     ReleaseState,
     RpmBuild,
     RpmPackage,
     TestGatingStatus,
     Update,
     UpdateRequest,
@@ -860,15 +859,15 @@
         assert up['critpath_groups'] == "core"
 
         args['edited'] = up['alias']
         # just edit anything, it doesn't matter, the point here is to
         # hit the critpath re-discovery code in the edit codepath
         args['stable_days'] = '50'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             ed = self.app.post_json('/updates/', args).json_body
 
         assert ed['critpath']
         assert ed['critpath_groups'] == "core"
 
     @mock.patch(**mock_valid_requirements)
     def test_obsoletion(self, *args):
@@ -1602,15 +1601,15 @@
         with mock.patch('bodhi.server.Session.remove'):
             app = TestApp(main({}, testing='lloyd', session=self.db, **self.app_settings))
         update = self.get_update(nvr)
         update['csrf_token'] = app.get('/csrf').json_body['csrf_token']
         update['notes'] = 'testing!!!'
         update['edited'] = res.json['alias']
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             res = app.post_json('/updates/', update)
 
         assert 'bodhi does not have commit access to bodhi' not in res
         build = self.db.query(RpmBuild).filter_by(nvr=nvr).one()
         assert build.update is not None
         assert build.update.notes == 'testing!!!'
 
@@ -3238,15 +3237,15 @@
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1):
             r = self.app.post_json('/updates/', args)
 
         args['edited'] = r.json['alias']
         args['builds'] = 'bodhi-2.0.0-3.fc17'
         args['requirements'] = 'upgradepath'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['title'] == 'bodhi-2.0.0-3.fc17'
         assert up['status'] == 'pending'
         assert up['request'] == 'testing'
         assert up['user']['name'] == 'guest'
@@ -3304,15 +3303,15 @@
             r = self.app.post_json('/updates/', update)
 
         update['edited'] = r.json['alias']
         update['builds'] = 'bodhi-2.0.0-3.fc17'
         update['requirements'] = 'upgradepath'
 
         with mock.patch('bodhi.server.buildsys.DevBuildsys.getTag', self.mock_getTag):
-            with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+            with fml_testing.mock_sends(update_schemas.UpdateEditV2):
                 r = self.app.post_json('/updates/', update)
 
         up = r.json_body
         assert up['title'] == 'bodhi-2.0.0-3.fc17'
         assert up['status'] == 'pending'
         assert up['request'] is None
         assert up['user']['name'] == 'guest'
@@ -3370,15 +3369,15 @@
 
         get_tags.return_value = ['f17-updates-candidate',
                                  'f17-updates-testing-pending']
 
         args['edited'] = upd.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         info.assert_any_call('Unpushing bodhi-2.0.0-2.fc17')
         info.assert_any_call('Removing f17-updates-testing-pending tag from bodhi-2.0.0-2.fc17')
         assert mock.call(
             'Removing f17-updates-candidate tag from bodhi-2.0.0-2.fc17'
         ) not in info.call_args_list
@@ -3429,15 +3428,15 @@
 
         get_tags.return_value = ['f17-updates-testing']
 
         args['edited'] = upd.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
 
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1,
-                                    update_schemas.UpdateEditV1):
+                                    update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         info.assert_any_call('Unpushing bodhi-2.0.0-2.fc17')
         info.assert_any_call(
             'Moving bodhi-2.0.0-2.fc17 from f17-updates-testing to f17-updates-candidate')
         tag_task.delay.assert_called_once_with(tag='f17-updates-signing-pending',
                                                builds=['bodhi-2.0.0-3.fc17'])
@@ -3489,15 +3488,15 @@
         get_tags.return_value = ['f17-updates-testing',
                                  'f17-updates-pending']
 
         args['edited'] = upd.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
 
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1,
-                                    update_schemas.UpdateEditV1):
+                                    update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         info.assert_any_call('Unpushing bodhi-2.0.0-2.fc17')
         info.assert_any_call('Removing f17-updates-pending tag from bodhi-2.0.0-2.fc17')
         info.assert_any_call(
             'Moving bodhi-2.0.0-2.fc17 from f17-updates-testing to f17-updates-candidate')
         tag_task.delay.assert_called_once_with(tag='f17-updates-signing-pending',
@@ -3545,15 +3544,15 @@
         # Clear pending messages
         self.db.info['messages'] = []
         self.db.commit()
 
         args['edited'] = upd.alias
         args['notes'] = 'A nifty description.'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['title'] == 'bodhi-2.0.0-2.fc17'
         assert up['status'] == 'testing'
         assert up['request'] == 'stable'
         assert up['notes'] == 'A nifty description.'
@@ -3586,15 +3585,15 @@
         get_tags.return_value = ['f17-updates-candidate',
                                  'f17-updates-testing-pending',
                                  'f17-build-side-12345']
 
         args['edited'] = upd.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         info.assert_any_call('Unpushing bodhi-2.0.0-2.fc17')
         info.assert_any_call('Removing f17-updates-testing-pending tag from bodhi-2.0.0-2.fc17')
         info.assert_any_call('Removing f17-updates-candidate tag from bodhi-2.0.0-2.fc17')
         tag_task.delay.assert_any_call(tag='f17-updates-signing-pending',
                                        builds=['bodhi-2.0.0-3.fc17'])
@@ -3647,15 +3646,15 @@
         get_tags.return_value = ['f17-updates-testing',
                                  'f17-build-side-12345']
 
         args['edited'] = upd.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
 
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1,
-                                    update_schemas.UpdateEditV1):
+                                    update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         info.assert_any_call('Unpushing bodhi-2.0.0-2.fc17')
         info.assert_any_call('Removing f17-updates-testing tag from bodhi-2.0.0-2.fc17')
         tag_task.delay.assert_any_call(tag='f17-updates-signing-pending',
                                        builds=['bodhi-2.0.0-3.fc17'])
         up = r.json_body
@@ -3689,29 +3688,15 @@
         """Test editing an update for one release with builds from another."""
         args = self.get_update('bodhi-2.0.0-2.fc17')
 
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1):
             r = self.app.post_json('/updates/', args)
 
         # Add another release and package
-        Release._tag_cache = None
-        release = Release(
-            name='F18', long_name='Fedora 18',
-            id_prefix='FEDORA', version='18',
-            dist_tag='f18', stable_tag='f18-updates',
-            testing_tag='f18-updates-testing',
-            candidate_tag='f18-updates-candidate',
-            pending_signing_tag='f18-updates-testing-signing',
-            pending_testing_tag='f18-updates-testing-pending',
-            pending_stable_tag='f18-updates-pending',
-            override_tag='f18-override',
-            branch='f18',
-            package_manager=PackageManager.unspecified,
-            testing_repository=None)
-        self.db.add(release)
+        self.create_release('18')
         pkg = RpmPackage(name='nethack')
         self.db.add(pkg)
         self.db.commit()
 
         args = self.get_update('bodhi-2.0.0-2.fc17,nethack-4.0.0-1.fc18')
         args['edited'] = r.json['alias']
         r = self.app.post_json('/updates/', args, status=400)
@@ -3759,15 +3744,15 @@
         # Clear pending messages
         self.db.info['messages'] = []
 
         # Changing the notes should work
         args['edited'] = up.alias
         args['notes'] = 'Some new notes'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             up = self.app.post_json('/updates/', args, status=200).json_body
 
         assert up['notes'] == 'Some new notes'
 
         # Changing the builds should fail
         args['notes'] = 'And yet some other notes'
         args['builds'] = 'bodhi-2.0.0-3.fc17'
@@ -4638,29 +4623,15 @@
         body = res.json_body
         assert not body['updates']
 
     @mock.patch(**mock_valid_requirements)
     def test_submitting_multi_release_updates(self, *args):
         """ https://github.com/fedora-infra/bodhi/issues/219 """
         # Add another release and package
-        Release._tag_cache = None
-        release = Release(
-            name='F18', long_name='Fedora 18',
-            id_prefix='FEDORA', version='18',
-            dist_tag='f18', stable_tag='f18-updates',
-            testing_tag='f18-updates-testing',
-            candidate_tag='f18-updates-candidate',
-            pending_signing_tag='f18-updates-testing-signing',
-            pending_testing_tag='f18-updates-testing-pending',
-            pending_stable_tag='f18-updates-pending',
-            override_tag='f18-override',
-            branch='f18',
-            package_manager=PackageManager.unspecified,
-            testing_repository=None)
-        self.db.add(release)
+        self.create_release('18')
         pkg = RpmPackage(name='nethack')
         self.db.add(pkg)
         self.db.commit()
 
         # A multi-release submission!!!  This should create *two* updates
         args = self.get_update('bodhi-2.0.0-2.fc17,bodhi-2.0.0-2.fc18')
 
@@ -4712,15 +4683,15 @@
 
         # Mark it as testing
         args['edited'] = update.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
         args['bugs'] = '56789,98765'
 
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1,
-                                    update_schemas.UpdateEditV1):
+                                    update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
 
         assert len(up['bugs']) == 2
         bug_ids = [bug['bug_id'] for bug in up['bugs']]
         assert 56789 in bug_ids
@@ -4728,15 +4699,15 @@
         assert up['status'] == 'pending'
         assert up['request'] == 'testing'
 
         # now remove a bug
         args['edited'] = update.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
         args['bugs'] = '98765'
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert len(up['bugs']) == 1
         bug_ids = [bug['bug_id'] for bug in up['bugs']]
         assert 98765 in bug_ids
         assert up['status'] == 'pending'
@@ -4780,15 +4751,15 @@
         args['edited'] = update.alias
 
         # Toggle a bunch of the booleans
         args['autokarma'] = False
         args['require_testcases'] = False
         args['require_bugs'] = True
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['status'] == 'testing'
         assert up['request'] is None
 
         assert up['require_bugs'] is True
@@ -4817,15 +4788,15 @@
         self.db.info['messages'] = []
         self.db.commit()
 
         # Mark it as testing
         args['edited'] = update.alias
         args['type'] = 'bugfix'
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['status'] == 'testing'
         assert up['request'] is None
         assert up['type'] == 'bugfix'
 
@@ -5114,15 +5085,15 @@
         # Mark it as testing
         args['edited'] = update.alias
 
         # Change Karma Thresholds
         args['stable_karma'] = 4
         args['unstable_karma'] = -4
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['status'] == 'testing'
         assert up['request'] is None
         assert up['autokarma'] is False
         assert up['stable_karma'] == 4
@@ -5901,25 +5872,25 @@
         self.db.commit()
 
         # Edit it and change the builds
         new_nvr = 'bodhi-2.0.0-3.fc17'
         args['edited'] = upd.alias
         args['builds'] = new_nvr
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['title'] == new_nvr
 
         # Change it back to ensure we can still reference the older build
         args['edited'] = upd.alias
         args['builds'] = nvr
 
-        with fml_testing.mock_sends(update_schemas.UpdateEditV1):
+        with fml_testing.mock_sends(update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
         assert up['title'] == nvr
 
     @mock.patch(**mock_taskotron_results)
     @mock.patch(**mock_valid_requirements)
@@ -6054,15 +6025,15 @@
 
         assert update.meets_testing_requirements is False
 
         args['edited'] = update.alias
         args['builds'] = 'bodhi-2.0.0-3.fc17'
 
         with fml_testing.mock_sends(update_schemas.UpdateRequestTestingV1,
-                                    update_schemas.UpdateEditV1):
+                                    update_schemas.UpdateEditV2):
             r = self.app.post_json('/updates/', args)
 
         up = r.json_body
 
         assert up['title'] == 'bodhi-2.0.0-3.fc17'
         assert up['karma'] == 0
         assert up['date_testing'] is None
@@ -6109,14 +6080,25 @@
         if update_status != UpdateStatus.stable and release_state == ReleaseState.frozen:
             assert ('This update will not be pushed to stable until freeze is lifted '
                     f'from {release.long_name}.') in resp
         else:
             assert ('This update will not be pushed to stable until freeze is lifted '
                     f'from {release.long_name}.') not in resp
 
+    def test_koji_build_url_encoding(self):
+        """Test HTML URL to koji build is correctly encoded."""
+        update = self.create_update(['hylafax+-7.0.3-1.fc17'])
+        self.db.commit()
+
+        resp = self.app.get(f'/updates/{update.alias}', headers={'Accept': 'text/html'})
+
+        assert 'text/html' in resp.headers['Content-Type']
+        assert ('search?terms=hylafax%2B-7.0.3-1.fc17&amp;type=build&amp;match=exact" '
+                'target="_blank">hylafax+-7.0.3-1.fc17</a>') in resp
+
 
 class TestWaiveTestResults(BasePyTestCase):
     """
     This class contains tests for the waive_test_results() function.
     """
     def test_cannot_waive_test_results_on_locked_update(self, *args):
         """Ensure that we get an error if trying to waive test results of a locked update"""
```

### Comparing `bodhi_server-7.1.1/tests/tasks/__init__.py` & `bodhi_server-7.2.0/tests/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/base.py` & `bodhi_server-7.2.0/tests/tasks/base.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_approve_testing.py` & `bodhi_server-7.2.0/tests/tasks/test_approve_testing.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_check_policies.py` & `bodhi_server-7.2.0/tests/tasks/test_check_policies.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_check_signed_builds.py` & `bodhi_server-7.2.0/tests/tasks/test_check_signed_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_clean_old_composes.py` & `bodhi_server-7.2.0/tests/tasks/test_clean_old_composes.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_composer.py` & `bodhi_server-7.2.0/tests/tasks/test_composer.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,16 @@
         self.koji = buildsys.get_session()
 
         self.tempdir = tempfile.mkdtemp('bodhi')
         self.db_factory = base.TransactionalSessionMaker(self.Session)
         self.handler = ComposerHandler(db_factory=self.db_factory, compose_dir=self.tempdir)
 
         # Reset "cached" objects before each test.
-        Release.clear_all_releases_cache()
-        Release._tag_cache = None
+        Release.all_releases.cache_clear()
+        Release.get_tags.cache_clear()
 
         self.expected_sems = 0
         self.semmock = mock.MagicMock()
         self.handler.max_composes_sem = self.semmock
 
     def teardown_method(self, method):
         """Call assert_sems and remove temporary files."""
@@ -989,15 +989,15 @@
                 type=UpdateType.security)
 
             update.test_gating_status = TestGatingStatus.passed
 
             db.add(update)
 
             # Wipe out the tag cache so it picks up our new release
-            Release._tag_cache = None
+            Release.get_tags.cache_clear()
 
             # Clear pending messages
             self.db.info['messages'] = []
 
         with mock_sends(*expected_messages):
             task = self._make_task()
             api_version = task.pop("api_version")
@@ -1073,15 +1073,15 @@
                 type=UpdateType.enhancement)
 
             update.test_gating_status = TestGatingStatus.passed
 
             db.add(update)
 
             # Wipe out the tag cache so it picks up our new release
-            Release._tag_cache = None
+            Release.get_tags.cache_clear()
 
             # Clear pending messages
             self.db.info['messages'] = []
 
         with mock_sends(*expected_messages):
             task = self._make_task()
             api_version = task.pop("api_version")
@@ -1147,15 +1147,15 @@
                 type=UpdateType.security)
 
             update.test_gating_status = TestGatingStatus.passed
 
             db.add(update)
 
             # Wipe out the tag cache so it picks up our new release
-            Release._tag_cache = None
+            Release.get_tags.cache_clear()
 
             # Clear pending messages
             self.db.info['messages'] = []
 
         with mock_sends(*expected_messages):
             task = self._make_task()
             api_version = task.pop("api_version")
@@ -1527,15 +1527,15 @@
                 type=UpdateType.security)
 
             update.test_gating_status = TestGatingStatus.passed
 
             db.add(update)
 
             # Wipe out the tag cache so it picks up our new release
-            Release._tag_cache = None
+            Release.get_tags.cache_clear()
 
             # Clear pending messages
             self.db.info['messages'] = []
 
         task = self._make_task(['--releases', 'F27M'])
         t = ModuleComposerThread(self.semmock, task['composes'][0],
                                  'puiterwijk', self.db_factory, self.tempdir)
@@ -2341,15 +2341,15 @@
             release=release,
             type=UpdateType.bugfix)
 
         update.test_gating_status = TestGatingStatus.passed
 
         self.db.add(update)
         # Wipe out the tag cache so it picks up our new release
-        Release._tag_cache = None
+        Release.get_tags.cache_clear()
         self.db.flush()
 
     @mock.patch('bodhi.server.tasks.composer.subprocess.Popen')
     def test_request_not_stable(self, Popen):
         """Ensure that the correct destination tag is used for non-stable updates."""
         Popen.return_value.communicate.return_value = ('out', 'err')
         Popen.return_value.returncode = 0
@@ -2510,15 +2510,15 @@
             release=release,
             type=UpdateType.bugfix)
 
         update.test_gating_status = TestGatingStatus.passed
 
         self.db.add(update)
         # Wipe out the tag cache so it picks up our new release
-        Release._tag_cache = None
+        Release.get_tags.cache_clear()
         self.db.flush()
 
     @mock.patch('bodhi.server.tasks.composer.subprocess.Popen')
     def test_flatpak_compose(self, Popen):
         """
         Basic test that FlatpakComposerThread does the expected thing.
 
@@ -2817,15 +2817,15 @@
         t.db = self.db
         t.id = getattr(self.db.query(Release).one(), '{}_tag'.format('stable'))
         t.skip_compose = True
         expected_messages = (
             update_schemas.UpdateEjectV1.from_dict({
                 'repo': 'f17-updates', 'update': self.db.query(Update).one().__json__(),
                 'reason': f"Cannot find relevant tag for bodhi-2.0-1.fc17.  None of {tags} are in "
-                          f"{Release.get_tags(self.db)[0]['candidate']}.",
+                          f"{Release.get_tags()[0]['candidate']}.",
                 'request': UpdateRequest.testing,
                 'release': t.compose.release, 'agent': 'bowlofeggs'}),)
 
         with mock_sends(*expected_messages):
             t._determine_tag_actions()
             expected_messages[0].body['update'] = self.db.query(Update).one().__json__()
```

### Comparing `bodhi_server-7.1.1/tests/tasks/test_expire_overrides.py` & `bodhi_server-7.2.0/tests/tasks/test_expire_overrides.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_fetch_test_cases.py` & `bodhi_server-7.2.0/tests/tasks/test_fetch_test_cases.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_handle_side_and_related_tags.py` & `bodhi_server-7.2.0/tests/tasks/test_handle_side_and_related_tags.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_tag_update_builds.py` & `bodhi_server-7.2.0/tests/tasks/test_tag_update_builds.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/tasks/test_work_on_bugs.py` & `bodhi_server-7.2.0/tests/tasks/test_work_on_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test___init__.py` & `bodhi_server-7.2.0/tests/test___init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,23 +259,23 @@
         _generate_home_page_stats.return_value = 7
         assert generic._generate_home_page_stats() == 5
         # If we invalidate the cache, we should see the new return value.
         generic._generate_home_page_stats.invalidate()
         assert generic._generate_home_page_stats() == 7
 
     def test_warms_up_releases_cache(self):
-        """main() should warm up the _all_releases cache."""
+        """main() should warm up the all_releases cache."""
         # Let's clear the release cache
         config["warm_cache_on_start"] = True
-        models.Release.clear_all_releases_cache()
+        models.Release.all_releases.cache_clear()
 
         server.main({}, testing='guest', session=self.db)
 
         # The cache should have a release in it now - let's just spot check it
-        assert models.Release._all_releases['current'][0]['name'] == 'F17'
+        assert models.Release.all_releases()['current'][0]['name'] == 'F17'
 
     def test_calls_initialize_db(self):
         """main() should call initialize_db() when called without a session arg."""
         with mock.patch('bodhi.server.initialize_db') as init_db:
             server.main({}, **self.app_settings)
 
         init_db.assert_called_once()
```

### Comparing `bodhi_server-7.1.1/tests/test_alembic.py` & `bodhi_server-7.2.0/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_bugs.py` & `bodhi_server-7.2.0/tests/test_bugs.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_buildsys.py` & `bodhi_server-7.2.0/tests/test_buildsys.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_config.py` & `bodhi_server-7.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_logging.py` & `bodhi_server-7.2.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_mail.py` & `bodhi_server-7.2.0/tests/test_mail.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_metadata.py` & `bodhi_server-7.2.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_models.py` & `bodhi_server-7.2.0/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -820,20 +820,14 @@
         releases = model.Release.all_releases()
 
         state = ReleaseState.from_string(list(releases.keys())[0])
         assert 'long_name' in releases[state.value][0], releases
         # Make sure it's the same cached object
         assert releases is model.Release.all_releases()
 
-    def test_clear_all_releases_cache(self):
-        model.Release.all_releases()
-        assert model.Release._all_releases is not None
-        model.Release.clear_all_releases_cache()
-        assert model.Release._all_releases is None
-
     def test_get_pending_signing_side_tag_found(self):
         """
         Assert that correct side tag is returned.
         """
         config.update({
             'f11.koji-signing-pending-side-tag': '-signing-pending-test'
         })
@@ -918,20 +912,14 @@
         releases = model.Release.all_releases()
 
         state = ReleaseState.from_string(list(releases.keys())[0])
         assert 'long_name' in releases[state.value][0], releases
         # Make sure it's the same cached object
         assert releases is model.Release.all_releases()
 
-    def test_clear_all_releases_cache(self):
-        model.Release.all_releases()
-        assert model.Release._all_releases is not None
-        model.Release.clear_all_releases_cache()
-        assert model.Release._all_releases is None
-
 
 class TestReleaseContainer(ModelTest):
     """Unit test case for the ``Release`` model for container releases."""
     klass = model.Release
     attrs = dict(
         name="F11C",
         long_name="Fedora 11 Container",
@@ -958,20 +946,14 @@
         releases = model.Release.all_releases()
 
         state = ReleaseState.from_string(list(releases.keys())[0])
         assert 'long_name' in releases[state.value][0], releases
         # Make sure it's the same cached object
         assert releases is model.Release.all_releases()
 
-    def test_clear_all_releases_cache(self):
-        model.Release.all_releases()
-        assert model.Release._all_releases is not None
-        model.Release.clear_all_releases_cache()
-        assert model.Release._all_releases is None
-
 
 class TestReleaseFlatpak(ModelTest):
     """Unit test case for the ``Release`` model for flatpak releases."""
     klass = model.Release
     attrs = dict(
         name="F29F",
         long_name="Fedora 29 Flatpaks",
@@ -998,20 +980,14 @@
         releases = model.Release.all_releases()
 
         state = ReleaseState.from_string(list(releases.keys())[0])
         assert 'long_name' in releases[state.value][0], releases
         # Make sure it's the same cached object
         assert releases is model.Release.all_releases()
 
-    def test_clear_all_releases_cache(self):
-        model.Release.all_releases()
-        assert model.Release._all_releases is not None
-        model.Release.clear_all_releases_cache()
-        assert model.Release._all_releases is None
-
 
 class TestPackageModel(BasePyTestCase):
     """Tests for the Package model."""
 
     def test_two_package_different_types(self):
         """Assert two different package types with the same name is fine."""
         package1 = model.Package(name='python-requests')
@@ -2044,15 +2020,15 @@
         update.test_gating_status = None
         data = {
             'edited': update.alias, 'builds': [update.builds[0].nvr],
             'bugs': [], 'display_name': '  '}
         request = mock.MagicMock()
         request.db = self.db
         request.user.name = 'tester'
-        with mock_sends(update_schemas.UpdateEditV1):
+        with mock_sends(update_schemas.UpdateEditV2):
             with mock.patch('bodhi.server.models.util.greenwave_api_post') as mock_greenwave:
                 greenwave_response = {
                     'policies_satisfied': False,
                     'summary': 'what have you done‽',
                     'applicable_policies': ['taskotron_release_critical_tasks'],
                     'unsatisfied_requirements': [
                         {'testcase': 'dist.rpmdeplint',
@@ -2074,15 +2050,15 @@
         update.test_gating_status = None
         data = {
             'edited': update.alias, 'builds': [update.builds[0].nvr],
             'bugs': [], 'display_name': '  '}
         request = mock.MagicMock()
         request.db = self.db
         request.user.name = 'tester'
-        with mock_sends(update_schemas.UpdateEditV1):
+        with mock_sends(update_schemas.UpdateEditV2):
             with mock.patch('bodhi.server.models.util.greenwave_api_post') as mock_greenwave:
                 greenwave_response = {
                     'policies_satisfied': False,
                     'summary': 'what have you done‽',
                     'applicable_policies': ['taskotron_release_critical_tasks'],
                     'unsatisfied_requirements': [
                         {'testcase': 'dist.rpmdeplint',
@@ -2110,15 +2086,15 @@
         data = {
             'edited': update.alias, 'builds': [update.builds[0].nvr],
             'bugs': [], 'display_name': '  '}
         request = mock.MagicMock()
         request.db = self.db
         request.user.name = 'tester'
 
-        with mock_sends(update_schemas.UpdateEditV1, update_schemas.UpdateReadyForTestingV2):
+        with mock_sends(update_schemas.UpdateEditV2, update_schemas.UpdateReadyForTestingV2):
             with mock.patch('bodhi.server.models.util.greenwave_api_post') as mock_greenwave:
                 greenwave_response = {
                     'policies_satisfied': False,
                     'summary': 'what have you done‽',
                     'applicable_policies': ['taskotron_release_critical_tasks'],
                     'unsatisfied_requirements': [
                         {'testcase': 'dist.rpmdeplint',
@@ -2146,15 +2122,15 @@
         data = {
             'edited': update.alias, 'builds': [update.builds[0].nvr],
             'bugs': [], 'display_name': '  '}
         request = mock.MagicMock()
         request.db = self.db
         request.user.name = 'tester'
 
-        with mock_sends(update_schemas.UpdateEditV1):
+        with mock_sends(update_schemas.UpdateEditV2):
             with mock.patch('bodhi.server.models.util.greenwave_api_post') as mock_greenwave:
                 greenwave_response = {
                     'policies_satisfied': False,
                     'summary': 'what have you done‽',
                     'applicable_policies': ['taskotron_release_critical_tasks'],
                     'unsatisfied_requirements': [
                         {'testcase': 'dist.rpmdeplint',
@@ -2182,15 +2158,15 @@
         data = {
             'edited': update.alias, 'builds': [update.builds[0].nvr],
             'bugs': [], 'display_name': '  '}
         request = mock.MagicMock()
         request.db = self.db
         request.user.name = 'tester'
 
-        with mock_sends(update_schemas.UpdateEditV1):
+        with mock_sends(update_schemas.UpdateEditV2):
             with mock.patch('bodhi.server.models.util.greenwave_api_post') as mock_greenwave:
                 greenwave_response = {
                     'policies_satisfied': False,
                     'summary': 'what have you done‽',
                     'applicable_policies': ['taskotron_release_critical_tasks'],
                     'unsatisfied_requirements': [
                         {'testcase': 'dist.rpmdeplint',
```

### Comparing `bodhi_server-7.1.1/tests/test_notifications.py` & `bodhi_server-7.2.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_push.py` & `bodhi_server-7.2.0/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_renderers.py` & `bodhi_server-7.2.0/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_schemas.py` & `bodhi_server-7.2.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_security.py` & `bodhi_server-7.2.0/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_util.py` & `bodhi_server-7.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_validators.py` & `bodhi_server-7.2.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/test_webapp.py` & `bodhi_server-7.2.0/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/testing.ini` & `bodhi_server-7.2.0/tests/testing.ini`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/utils.py` & `bodhi_server-7.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/views/__init__.py` & `bodhi_server-7.2.0/tests/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/tests/views/test_generic.py` & `bodhi_server-7.2.0/tests/views/test_generic.py`

 * *Files identical despite different names*

### Comparing `bodhi_server-7.1.1/PKG-INFO` & `bodhi_server-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodhi-server
-Version: 7.1.1
+Version: 7.2.0
 Summary: Bodhi server
 Home-page: https://bodhi.fedoraproject.rog
 License: GPL-2.0-or-later
 Keywords: web,fedora,pyramid
 Author: Fedora Infrastructure Team
 Maintainer: Fedora Infrastructure Team
 Maintainer-email: infrastructure@lists.fedoraproject.org
```

