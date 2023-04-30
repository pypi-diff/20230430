# Comparing `tmp/django-cast-0.2.8.tar.gz` & `tmp/django-cast-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cast-0.2.8.tar", last modified: Sun Mar 12 22:53:37 2023, max compression
+gzip compressed data, was "django-cast-0.2.9.tar", last modified: Mon Mar 20 06:09:57 2023, max compression
```

## Comparing `django-cast-0.2.8.tar` & `django-cast-0.2.9.tar`

### file list

```diff
@@ -1,374 +1,387 @@
--rw-r--r--   0        0        0      331 2020-12-14 06:01:37.748978 django-cast-0.2.8/.editorconfig
--rw-r--r--   0        0        0      340 2020-12-14 06:01:37.749087 django-cast-0.2.8/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      945 2023-02-20 06:17:57.899206 django-cast-0.2.8/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      932 2022-12-18 08:57:34.948078 django-cast-0.2.8/.gitignore
--rw-r--r--   0        0        0     2054 2023-02-26 07:05:53.133395 django-cast-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0       50 2020-12-14 06:01:37.749209 django-cast-0.2.8/.readthedocs.yml
--rw-r--r--   0        0        0      500 2022-12-18 08:57:34.949060 django-cast-0.2.8/.travis.yml
--rw-r--r--   0        0        0      185 2022-11-09 16:01:36.193748 django-cast-0.2.8/AUTHORS.rst
--rw-r--r--   0        0        0     3210 2022-11-09 16:01:36.193901 django-cast-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1501 2022-11-09 16:01:36.193999 django-cast-0.2.8/LICENSE
--rw-r--r--   0        0        0      160 2022-12-18 08:57:34.949346 django-cast-0.2.8/Procfile
--rw-r--r--   0        0        0     2282 2023-03-12 22:53:21.138181 django-cast-0.2.8/README.md
--rw-r--r--   0        0        0     5271 2022-12-18 08:57:34.949979 django-cast-0.2.8/README_OLD.rst
--rw-r--r--   0        0        0      671 2022-12-18 09:06:19.412296 django-cast-0.2.8/bootstrap.md
--rw-r--r--   0        0        0       85 2023-03-12 22:53:21.138569 django-cast-0.2.8/cast/__init__.py
--rw-r--r--   0        0        0     3973 2023-02-12 09:06:05.609865 django-cast-0.2.8/cast/admin.py
--rw-r--r--   0        0        0      560 2023-02-12 09:06:05.610163 django-cast-0.2.8/cast/admin_urls/audio.py
--rw-r--r--   0        0        0      560 2023-02-12 09:06:05.610406 django-cast-0.2.8/cast/admin_urls/video.py
--rw-r--r--   0        0        0        0 2020-12-14 06:01:37.750115 django-cast-0.2.8/cast/api/__init__.py
--rw-r--r--   0        0        0     1280 2023-01-15 12:33:49.372425 django-cast-0.2.8/cast/api/serializers.py
--rw-r--r--   0        0        0     1188 2023-02-26 07:05:53.133893 django-cast-0.2.8/cast/api/urls.py
--rw-r--r--   0        0        0      744 2023-02-12 09:06:05.610869 django-cast-0.2.8/cast/api/viewmixins.py
--rw-r--r--   0        0        0     4429 2023-03-05 14:24:40.476089 django-cast-0.2.8/cast/api/views.py
--rw-r--r--   0        0        0      773 2023-02-12 09:06:05.611650 django-cast-0.2.8/cast/apps.py
--rw-r--r--   0        0        0      410 2023-01-30 05:52:09.387409 django-cast-0.2.8/cast/appsettings.py
--rw-r--r--   0        0        0     3288 2023-02-12 09:06:05.611976 django-cast-0.2.8/cast/blocks.py
--rw-r--r--   0        0        0     8237 2023-02-23 17:07:51.458204 django-cast-0.2.8/cast/feeds.py
--rw-r--r--   0        0        0     8052 2023-02-23 05:58:47.091761 django-cast-0.2.8/cast/filters.py
--rw-r--r--   0        0        0     6261 2023-02-12 09:06:05.613123 django-cast-0.2.8/cast/forms.py
--rw-r--r--   0        0        0     4094 2020-12-14 06:01:37.751186 django-cast-0.2.8/cast/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6148 2020-12-14 06:01:37.751304 django-cast-0.2.8/cast/management/.DS_Store
--rw-r--r--   0        0        0    12288 2020-12-14 06:01:37.751493 django-cast-0.2.8/cast/management/commands/.s3_stale.py.swp
--rw-r--r--   0        0        0        0 2020-12-14 06:01:37.751553 django-cast-0.2.8/cast/management/commands/__init__.py
--rw-r--r--   0        0        0      443 2023-01-21 14:08:59.166854 django-cast-0.2.8/cast/management/commands/add_missing_media_objects.py
--rw-r--r--   0        0        0      552 2023-01-21 14:08:59.167148 django-cast-0.2.8/cast/management/commands/get_api_token.py
--rw-r--r--   0        0        0      386 2020-12-14 06:01:37.751844 django-cast-0.2.8/cast/management/commands/recalc_video_posters.py
--rw-r--r--   0        0        0      598 2022-11-09 16:01:36.202046 django-cast-0.2.8/cast/management/commands/s3_backup.py
--rw-r--r--   0        0        0     1194 2022-11-09 16:01:36.202772 django-cast-0.2.8/cast/management/commands/s3_media_sizes.py
--rw-r--r--   0        0        0      726 2022-11-09 16:01:36.202874 django-cast-0.2.8/cast/management/commands/s3_replace.py
--rw-r--r--   0        0        0      601 2023-01-21 14:08:59.167393 django-cast-0.2.8/cast/management/commands/s3_restore.py
--rw-r--r--   0        0        0     2382 2023-01-30 05:52:09.388926 django-cast-0.2.8/cast/management/commands/s3_stale.py
--rw-r--r--   0        0        0    19623 2022-11-09 16:01:36.203740 django-cast-0.2.8/cast/migrations/0001_initial.py
--rw-r--r--   0        0        0      317 2022-11-09 16:01:36.203922 django-cast-0.2.8/cast/migrations/0002_remove_blog_description.py
--rw-r--r--   0        0        0      333 2022-11-09 16:01:36.203981 django-cast-0.2.8/cast/migrations/0003_remove_post_parent_blog.py
--rw-r--r--   0        0        0      702 2022-11-09 16:01:36.204039 django-cast-0.2.8/cast/migrations/0004_homepage_alias_for_page.py
--rw-r--r--   0        0        0      881 2022-11-09 16:01:36.204113 django-cast-0.2.8/cast/migrations/0005_auto_20201024_0613.py
--rw-r--r--   0        0        0     3342 2022-11-09 16:01:36.204169 django-cast-0.2.8/cast/migrations/0006_auto_20210628_1628.py
--rw-r--r--   0        0        0      994 2022-11-09 16:01:36.204528 django-cast-0.2.8/cast/migrations/0007_alter_post_body.py
--rw-r--r--   0        0        0     2138 2022-11-09 16:01:36.204765 django-cast-0.2.8/cast/migrations/0008_auto_20210712_0919.py
--rw-r--r--   0        0        0     1104 2022-11-09 16:01:36.205160 django-cast-0.2.8/cast/migrations/0009_alter_post_body.py
--rw-r--r--   0        0        0      359 2022-11-09 16:01:36.205213 django-cast-0.2.8/cast/migrations/0010_rename_intro_blog_description.py
--rw-r--r--   0        0        0     2459 2022-11-09 16:01:36.205340 django-cast-0.2.8/cast/migrations/0011_alter_post_body.py
--rw-r--r--   0        0        0      465 2022-11-09 16:01:36.205400 django-cast-0.2.8/cast/migrations/0012_alter_post_images.py
--rw-r--r--   0        0        0      458 2022-11-09 16:01:36.205457 django-cast-0.2.8/cast/migrations/0013_alter_gallery_images.py
--rw-r--r--   0        0        0      326 2022-11-09 16:01:36.205515 django-cast-0.2.8/cast/migrations/0014_remove_gallery_user.py
--rw-r--r--   0        0        0      494 2022-11-09 16:01:36.205576 django-cast-0.2.8/cast/migrations/0015_delete_blogindexpage.py
--rw-r--r--   0        0        0     1143 2022-11-09 16:01:36.205635 django-cast-0.2.8/cast/migrations/0016_auto_20210830_0422.py
--rw-r--r--   0        0        0     2906 2022-11-09 16:01:36.205753 django-cast-0.2.8/cast/migrations/0017_alter_post_body.py
--rw-r--r--   0        0        0      424 2022-11-09 16:01:36.206068 django-cast-0.2.8/cast/migrations/0018_alter_chaptermark_start.py
--rw-r--r--   0        0        0      419 2022-11-09 16:01:36.206270 django-cast-0.2.8/cast/migrations/0019_alter_chaptermark_start.py
--rw-r--r--   0        0        0     2991 2022-11-09 16:01:36.206623 django-cast-0.2.8/cast/migrations/0020_auto_20210926_1556.py
--rw-r--r--   0        0        0     1249 2022-11-09 16:01:36.206773 django-cast-0.2.8/cast/migrations/0021_spamfilter.py
--rw-r--r--   0        0        0      515 2022-11-09 16:01:36.207208 django-cast-0.2.8/cast/migrations/0022_alter_spamfilter_model.py
--rw-r--r--   0        0        0      621 2022-11-09 16:01:36.207872 django-cast-0.2.8/cast/migrations/0023_alter_spamfilter_model.py
--rw-r--r--   0        0        0     3514 2022-12-18 08:57:34.951279 django-cast-0.2.8/cast/migrations/0024_alter_homepage_body_alter_post_body.py
--rw-r--r--   0        0        0      456 2023-01-06 13:26:12.969194 django-cast-0.2.8/cast/migrations/0025_add_performance_indicators.py
--rw-r--r--   0        0        0     4993 2023-01-30 05:52:09.389439 django-cast-0.2.8/cast/migrations/0026_delete_request_alter_post_body.py
--rw-r--r--   0        0        0     2496 2023-01-30 05:52:09.389746 django-cast-0.2.8/cast/migrations/0027_episode.py
--rw-r--r--   0        0        0     1217 2023-01-30 05:52:09.389945 django-cast-0.2.8/cast/migrations/0028_rename_and_drop_itune_fields.py
--rw-r--r--   0        0        0      424 2023-01-30 05:52:09.390078 django-cast-0.2.8/cast/migrations/0029_add_metadata_field_to_audio.py
--rw-r--r--   0        0        0      334 2023-02-06 06:19:29.734552 django-cast-0.2.8/cast/migrations/0030_remove_pub_date_is_handled_by_wagtail.py
--rw-r--r--   0        0        0      446 2023-02-06 06:19:29.735460 django-cast-0.2.8/cast/migrations/0031_remove_timestampedmodel_because_wagtail.py
--rw-r--r--   0        0        0      448 2023-02-06 06:19:29.735828 django-cast-0.2.8/cast/migrations/0032_remove_timestampedmodel_because_wagtail.py
--rw-r--r--   0        0        0     2516 2023-02-06 06:19:29.736266 django-cast-0.2.8/cast/migrations/0033_add_new_podcast_model.py
--rw-r--r--   0        0        0      652 2023-02-06 06:19:29.736523 django-cast-0.2.8/cast/migrations/0034_remove_old_podcast_fields_from_blog.py
--rw-r--r--   0        0        0      857 2023-02-06 06:19:29.736759 django-cast-0.2.8/cast/migrations/0035_remove_new_prefix_podcast_fields.py
--rw-r--r--   0        0        0      586 2023-02-06 06:19:29.737273 django-cast-0.2.8/cast/migrations/0036_alter_blog_author.py
--rw-r--r--   0        0        0     1957 2023-02-06 06:19:29.737589 django-cast-0.2.8/cast/migrations/0037_alter_episode_block_alter_episode_explicit_and_more.py
--rw-r--r--   0        0        0      653 2023-02-12 09:06:05.613416 django-cast-0.2.8/cast/migrations/0038_alter_episode_keywords.py
--rw-r--r--   0        0        0      551 2023-03-05 14:24:40.476688 django-cast-0.2.8/cast/migrations/0039_blog_noindex.py
--rw-r--r--   0        0        0      578 2023-03-12 22:53:21.138717 django-cast-0.2.8/cast/migrations/0040_alter_blog_noindex.py
--rw-r--r--   0        0        0     1163 2023-03-12 22:53:21.138820 django-cast-0.2.8/cast/migrations/0041_templatebasedirectory.py
--rw-r--r--   0        0        0      509 2023-03-12 22:53:21.139225 django-cast-0.2.8/cast/migrations/0042_blog_template_base_dir.py
--rw-r--r--   0        0        0      592 2023-03-12 22:53:21.139465 django-cast-0.2.8/cast/migrations/0043_alter_blog_template_base_dir.py
--rw-r--r--   0        0        0     1252 2023-03-12 22:53:21.139821 django-cast-0.2.8/cast/migrations/0044_alter_blog_template_base_dir_and_more.py
--rw-r--r--   0        0        0        0 2020-12-14 06:01:37.752618 django-cast-0.2.8/cast/migrations/__init__.py
--rw-r--r--   0        0        0      718 2023-03-12 22:53:21.140303 django-cast-0.2.8/cast/models/__init__.py
--rw-r--r--   0        0        0    12196 2023-03-05 14:24:40.477317 django-cast-0.2.8/cast/models/audio.py
--rw-r--r--   0        0        0      409 2023-02-12 09:06:05.614188 django-cast-0.2.8/cast/models/file.py
--rw-r--r--   0        0        0     1253 2023-02-12 09:06:05.614492 django-cast-0.2.8/cast/models/gallery.py
--rw-r--r--   0        0        0     8341 2023-03-12 22:53:21.140695 django-cast-0.2.8/cast/models/index_pages.py
--rw-r--r--   0        0        0      430 2023-01-21 14:08:59.168853 django-cast-0.2.8/cast/models/itunes.py
--rw-r--r--   0        0        0    11561 2023-02-12 09:06:05.615073 django-cast-0.2.8/cast/models/moderation.py
--rw-r--r--   0        0        0    13447 2023-03-12 22:53:21.141084 django-cast-0.2.8/cast/models/pages.py
--rw-r--r--   0        0        0     4522 2023-03-12 22:53:21.141361 django-cast-0.2.8/cast/models/theme.py
--rw-r--r--   0        0        0     6067 2023-02-12 09:06:05.615815 django-cast-0.2.8/cast/models/video.py
--rw-r--r--   0        0        0     1388 2023-02-12 09:06:05.616127 django-cast-0.2.8/cast/moderation.py
--rw-r--r--   0        0        0      895 2023-02-12 09:06:05.616396 django-cast-0.2.8/cast/runner.py
--rw-r--r--   0        0        0     5606 2023-03-12 22:53:21.141569 django-cast-0.2.8/cast/settings.py
--rw-r--r--   0        0        0     6554 2023-02-20 06:17:57.901130 django-cast-0.2.8/cast/static/css/cast.css
--rw-r--r--   0        0        0       93 2020-12-14 06:01:37.753112 django-cast-0.2.8/cast/static/css/my_div.css
--rw-r--r--   0        0        0       33 2023-03-12 22:53:21.141721 django-cast-0.2.8/cast/static/css/plain/cast.css
--rw-r--r--   0        0        0        0 2020-12-14 06:01:37.753178 django-cast-0.2.8/cast/static/img/.gitignore
--rw-r--r--   0        0        0     1357 2022-11-09 16:01:36.213103 django-cast-0.2.8/cast/static/img/cast/Audio-icon.svg
--rw-r--r--   0        0        0     1125 2022-11-09 16:01:36.213224 django-cast-0.2.8/cast/static/img/cast/Feed-icon.svg
--rw-r--r--   0        0        0    10504 2020-12-14 06:01:37.753463 django-cast-0.2.8/cast/static/img/cast/Video-icon.svg
--rw-r--r--   0        0        0        0 2020-12-14 06:01:37.753524 django-cast-0.2.8/cast/static/js/cast.js
--rw-r--r--   0        0        0      251 2020-12-14 06:01:37.753880 django-cast-0.2.8/cast/static/js/cast/dashboard.js
--rw-r--r--   0        0        0     1396 2022-11-29 05:40:21.313099 django-cast-0.2.8/cast/static/js/cast/gallery.js
--rw-r--r--   0        0        0     5321 2022-11-09 16:01:36.213750 django-cast-0.2.8/cast/static/js/cast/wagtail/audio-chooser-modal.js
--rw-r--r--   0        0        0      643 2022-11-09 16:01:36.214150 django-cast-0.2.8/cast/static/js/cast/wagtail/audio-chooser-telepath.js
--rw-r--r--   0        0        0     1969 2022-11-20 05:23:10.428455 django-cast-0.2.8/cast/static/js/cast/wagtail/audio-chooser.js
--rw-r--r--   0        0        0     5321 2022-11-09 16:01:36.214977 django-cast-0.2.8/cast/static/js/cast/wagtail/video-chooser-modal.js
--rw-r--r--   0        0        0      643 2022-11-09 16:01:36.215855 django-cast-0.2.8/cast/static/js/cast/wagtail/video-chooser-telepath.js
--rw-r--r--   0        0        0     1969 2022-11-09 16:01:36.216336 django-cast-0.2.8/cast/static/js/cast/wagtail/video-chooser.js
--rw-r--r--   0        0        0   145311 2023-01-30 05:19:56.108250 django-cast-0.2.8/cast/static/js/cast/web-player/embed.4.js
--rw-r--r--   0        0        0   134043 2023-01-30 05:19:56.109270 django-cast-0.2.8/cast/static/js/cast/web-player/embed.5.js
--rw-r--r--   0        0        0     6148 2022-11-09 16:01:36.217492 django-cast-0.2.8/cast/templates/.DS_Store
--rw-r--r--   0        0        0      995 2023-03-05 22:31:39.355713 django-cast-0.2.8/cast/templates/base.html
--rw-r--r--   0        0        0     1409 2023-01-21 14:08:59.169893 django-cast-0.2.8/cast/templates/cast/audio/add.html
--rw-r--r--   0        0        0       39 2022-11-20 08:32:17.698952 django-cast-0.2.8/cast/templates/cast/audio/audio.html
--rw-r--r--   0        0        0      254 2023-01-21 14:08:59.170356 django-cast-0.2.8/cast/templates/cast/audio/chooser.html
--rw-r--r--   0        0        0     2319 2023-01-21 14:08:59.170771 django-cast-0.2.8/cast/templates/cast/audio/chooser_chooser.html
--rw-r--r--   0        0        0      599 2023-01-21 14:08:59.171161 django-cast-0.2.8/cast/templates/cast/audio/chooser_results.html
--rw-r--r--   0        0        0      675 2022-11-09 16:01:36.220766 django-cast-0.2.8/cast/templates/cast/audio/confirm_delete.html
--rw-r--r--   0        0        0     2227 2022-11-09 16:01:36.221033 django-cast-0.2.8/cast/templates/cast/audio/edit.html
--rw-r--r--   0        0        0     2481 2023-01-21 14:08:59.171802 django-cast-0.2.8/cast/templates/cast/audio/index.html
--rw-r--r--   0        0        0     2105 2023-01-21 14:08:59.172246 django-cast-0.2.8/cast/templates/cast/audio/list.html
--rw-r--r--   0        0        0     1192 2023-01-21 14:08:59.172537 django-cast-0.2.8/cast/templates/cast/audio/results.html
--rw-r--r--   0        0        0      661 2022-11-09 16:01:36.222449 django-cast-0.2.8/cast/templates/cast/base.html
--rw-r--r--   0        0        0     2827 2023-03-12 22:53:21.141907 django-cast-0.2.8/cast/templates/cast/bootstrap4/blog_list_of_posts.html
--rw-r--r--   0        0        0      162 2023-03-12 22:53:21.142001 django-cast-0.2.8/cast/templates/cast/bootstrap4/cast_base.html
--rw-r--r--   0        0        0      213 2023-03-12 22:53:21.142096 django-cast-0.2.8/cast/templates/cast/bootstrap4/episode.html
--rw-r--r--   0        0        0     1705 2023-03-12 22:53:21.142193 django-cast-0.2.8/cast/templates/cast/bootstrap4/pagination.html
--rw-r--r--   0        0        0     2097 2023-03-12 22:53:21.142302 django-cast-0.2.8/cast/templates/cast/bootstrap4/post.html
--rw-r--r--   0        0        0      573 2023-03-12 22:53:21.142396 django-cast-0.2.8/cast/templates/cast/bootstrap4/post_body.html
--rw-r--r--   0        0        0      160 2023-01-21 14:08:59.173195 django-cast-0.2.8/cast/templates/cast/cast_base.html
--rw-r--r--   0        0        0     1467 2022-11-29 12:34:11.419174 django-cast-0.2.8/cast/templates/cast/gallery.html
--rw-r--r--   0        0        0      430 2022-11-09 16:01:36.223242 django-cast-0.2.8/cast/templates/cast/home_page.html
--rw-r--r--   0        0        0      164 2022-11-29 12:40:41.302441 django-cast-0.2.8/cast/templates/cast/image/image.html
--rw-r--r--   0        0        0      284 2020-12-14 06:01:37.755401 django-cast-0.2.8/cast/templates/cast/image_form.html
--rw-r--r--   0        0        0     1133 2023-03-12 22:53:21.142536 django-cast-0.2.8/cast/templates/cast/plain/base.html
--rw-r--r--   0        0        0     1216 2023-03-12 22:53:21.142626 django-cast-0.2.8/cast/templates/cast/plain/blog_list_of_posts.html
--rw-r--r--   0        0        0      213 2023-03-12 22:53:21.142699 django-cast-0.2.8/cast/templates/cast/plain/episode.html
--rw-r--r--   0        0        0      968 2023-03-12 22:53:21.142794 django-cast-0.2.8/cast/templates/cast/plain/post.html
--rw-r--r--   0        0        0      573 2023-03-12 22:53:21.142873 django-cast-0.2.8/cast/templates/cast/plain/post_body.html
--rw-r--r--   0        0        0     1133 2023-01-30 05:52:09.393268 django-cast-0.2.8/cast/templates/cast/twitter/card_player.html
--rw-r--r--   0        0        0     1409 2023-01-21 14:08:59.173820 django-cast-0.2.8/cast/templates/cast/video/add.html
--rw-r--r--   0        0        0      254 2023-01-21 14:08:59.174168 django-cast-0.2.8/cast/templates/cast/video/chooser.html
--rw-r--r--   0        0        0     2319 2023-01-21 14:08:59.174466 django-cast-0.2.8/cast/templates/cast/video/chooser_chooser.html
--rw-r--r--   0        0        0      598 2023-01-21 14:08:59.174682 django-cast-0.2.8/cast/templates/cast/video/chooser_results.html
--rw-r--r--   0        0        0      675 2022-11-09 16:01:36.226562 django-cast-0.2.8/cast/templates/cast/video/confirm_delete.html
--rw-r--r--   0        0        0     2229 2022-11-09 16:01:36.226736 django-cast-0.2.8/cast/templates/cast/video/edit.html
--rw-r--r--   0        0        0     2481 2023-01-21 14:08:59.175076 django-cast-0.2.8/cast/templates/cast/video/index.html
--rw-r--r--   0        0        0     2105 2023-01-21 14:08:59.175361 django-cast-0.2.8/cast/templates/cast/video/list.html
--rw-r--r--   0        0        0     1192 2023-01-21 14:08:59.175697 django-cast-0.2.8/cast/templates/cast/video/results.html
--rw-r--r--   0        0        0      454 2022-11-26 17:44:15.868652 django-cast-0.2.8/cast/templates/cast/video/video.html
--rw-r--r--   0        0        0      279 2020-12-14 06:01:37.755773 django-cast-0.2.8/cast/templates/cast/video_form.html
--rw-r--r--   0        0        0      245 2023-01-21 14:08:59.176089 django-cast-0.2.8/cast/templates/cast/wagtail/_file_field.html
--rw-r--r--   0        0        0      224 2023-01-21 14:08:59.176485 django-cast-0.2.8/cast/templates/cast/wagtail/_file_field_as_li.html
--rw-r--r--   0        0        0      320 2023-01-21 14:08:59.176752 django-cast-0.2.8/cast/templates/cast/wagtail/_thumbnail_field.html
--rw-r--r--   0        0        0      229 2023-01-21 14:08:59.177009 django-cast-0.2.8/cast/templates/cast/wagtail/_thumbnail_field_as_li.html
--rw-r--r--   0        0        0     1084 2023-01-21 14:08:59.177366 django-cast-0.2.8/cast/templates/comments/comment.html
--rw-r--r--   0        0        0     1705 2023-02-12 09:48:16.819321 django-cast-0.2.8/cast/templates/pagination.html
--rw-r--r--   0        0        0      937 2023-02-25 06:06:16.491075 django-cast-0.2.8/cast/urls.py
--rw-r--r--   0        0        0      499 2023-02-12 09:06:05.618267 django-cast-0.2.8/cast/utils.py
--rw-r--r--   0        0        0      142 2023-02-12 09:06:05.618726 django-cast-0.2.8/cast/views/__init__.py
--rw-r--r--   0        0        0    10246 2023-02-12 09:06:05.619080 django-cast-0.2.8/cast/views/audio.py
--rw-r--r--   0        0        0      795 2023-01-30 05:52:09.393804 django-cast-0.2.8/cast/views/meta.py
--rw-r--r--   0        0        0     9741 2023-02-12 09:06:05.619686 django-cast-0.2.8/cast/views/video.py
--rw-r--r--   0        0        0     2274 2023-02-12 09:06:05.620015 django-cast-0.2.8/cast/wagtail_hooks.py
--rw-r--r--   0        0        0     4661 2023-02-12 09:06:05.620306 django-cast-0.2.8/cast/widgets.py
--rw-r--r--   0        0        0      228 2022-11-19 08:32:39.905422 django-cast-0.2.8/command_lines.txt
--rw-r--r--   0        0        0     3478 2023-01-30 05:52:09.394405 django-cast-0.2.8/commands.py
--rw-r--r--   0        0        0      158 2022-11-09 16:01:36.233324 django-cast-0.2.8/django-cast-example.ps1
--rw-r--r--   0        0        0      634 2022-12-18 08:57:34.953400 django-cast-0.2.8/docs/Makefile
--rw-r--r--   0        0        0      971 2023-03-12 22:53:21.143285 django-cast-0.2.8/docs/conf.py
--rw-r--r--   0        0        0       45 2022-12-18 08:57:34.954013 django-cast-0.2.8/docs/contributing.rst
--rw-r--r--   0        0        0     3057 2023-03-12 22:53:21.143724 django-cast-0.2.8/docs/features.rst
--rw-r--r--   0        0        0     3910 2023-02-06 06:19:29.739700 django-cast-0.2.8/docs/howto/index.rst
--rw-r--r--   0        0        0    46438 2023-03-12 22:53:21.145005 django-cast-0.2.8/docs/images/blog_template_base_dir_setting.png
--rw-r--r--   0        0        0   143585 2023-01-30 05:52:09.396034 django-cast-0.2.8/docs/images/cache_file_sizes_admin_action.png
--rw-r--r--   0        0        0    50259 2023-01-06 13:26:12.972329 django-cast-0.2.8/docs/images/spam_filter_performance.png
--rw-r--r--   0        0        0    82268 2023-03-12 22:53:21.146414 django-cast-0.2.8/docs/images/template_base_dir_setting.png
--rw-r--r--   0        0        0   167962 2023-01-30 05:52:09.397690 django-cast-0.2.8/docs/images/twitter_card.png
--rw-r--r--   0        0        0      509 2023-03-12 22:53:21.146641 django-cast-0.2.8/docs/index.rst
--rw-r--r--   0        0        0       70 2023-02-06 06:19:29.740150 django-cast-0.2.8/docs/installation.rst
--rw-r--r--   0        0        0      800 2022-12-18 08:57:34.954986 django-cast-0.2.8/docs/make.bat
--rw-r--r--   0        0        0      806 2023-03-12 22:53:21.146731 django-cast-0.2.8/docs/models.rst
--rw-r--r--   0        0        0      866 2023-02-06 06:19:29.740351 django-cast-0.2.8/docs/release.rst
--rw-r--r--   0        0        0       64 2023-02-06 06:19:29.740882 django-cast-0.2.8/docs/releases/0.1/0.1.0.rst
--rw-r--r--   0        0        0       61 2023-02-06 06:19:29.741149 django-cast-0.2.8/docs/releases/0.1/0.1.1.rst
--rw-r--r--   0        0        0      202 2023-02-06 06:19:29.741403 django-cast-0.2.8/docs/releases/0.1/0.1.10.rst
--rw-r--r--   0        0        0       74 2023-02-06 06:19:29.741623 django-cast-0.2.8/docs/releases/0.1/0.1.11.rst
--rw-r--r--   0        0        0       79 2023-02-06 06:19:29.741850 django-cast-0.2.8/docs/releases/0.1/0.1.12.rst
--rw-r--r--   0        0        0       75 2023-02-06 06:19:29.742065 django-cast-0.2.8/docs/releases/0.1/0.1.13.rst
--rw-r--r--   0        0        0      103 2023-02-06 06:19:29.742317 django-cast-0.2.8/docs/releases/0.1/0.1.14.rst
--rw-r--r--   0        0        0       78 2023-02-06 06:19:29.742535 django-cast-0.2.8/docs/releases/0.1/0.1.15.rst
--rw-r--r--   0        0        0       96 2023-02-06 06:19:29.742757 django-cast-0.2.8/docs/releases/0.1/0.1.16.rst
--rw-r--r--   0        0        0      212 2023-02-06 06:19:29.743020 django-cast-0.2.8/docs/releases/0.1/0.1.17.rst
--rw-r--r--   0        0        0      141 2023-02-06 06:19:29.743407 django-cast-0.2.8/docs/releases/0.1/0.1.18.rst
--rw-r--r--   0        0        0      222 2023-02-06 06:19:29.743625 django-cast-0.2.8/docs/releases/0.1/0.1.19.rst
--rw-r--r--   0        0        0       89 2023-02-06 06:19:29.743829 django-cast-0.2.8/docs/releases/0.1/0.1.2.rst
--rw-r--r--   0        0        0       87 2023-02-06 06:19:29.744021 django-cast-0.2.8/docs/releases/0.1/0.1.20.rst
--rw-r--r--   0        0        0       92 2023-02-06 06:19:29.744238 django-cast-0.2.8/docs/releases/0.1/0.1.21.rst
--rw-r--r--   0        0        0      204 2023-02-06 06:19:29.744442 django-cast-0.2.8/docs/releases/0.1/0.1.22.rst
--rw-r--r--   0        0        0      200 2023-02-06 06:19:29.744669 django-cast-0.2.8/docs/releases/0.1/0.1.23.rst
--rw-r--r--   0        0        0      356 2023-02-06 06:19:29.744877 django-cast-0.2.8/docs/releases/0.1/0.1.24.rst
--rw-r--r--   0        0        0      134 2023-02-06 06:19:29.745085 django-cast-0.2.8/docs/releases/0.1/0.1.25.rst
--rw-r--r--   0        0        0       88 2023-02-06 06:19:29.745283 django-cast-0.2.8/docs/releases/0.1/0.1.26.rst
--rw-r--r--   0        0        0      221 2023-02-06 06:19:29.745489 django-cast-0.2.8/docs/releases/0.1/0.1.27.rst
--rw-r--r--   0        0        0      516 2023-02-06 06:19:29.745705 django-cast-0.2.8/docs/releases/0.1/0.1.28.rst
--rw-r--r--   0        0        0       95 2023-02-06 06:19:29.745924 django-cast-0.2.8/docs/releases/0.1/0.1.29.rst
--rw-r--r--   0        0        0      159 2023-02-06 06:19:29.746139 django-cast-0.2.8/docs/releases/0.1/0.1.3.rst
--rw-r--r--   0        0        0      118 2023-02-06 06:19:29.746357 django-cast-0.2.8/docs/releases/0.1/0.1.30.rst
--rw-r--r--   0        0        0       92 2023-02-06 06:19:29.746563 django-cast-0.2.8/docs/releases/0.1/0.1.31.rst
--rw-r--r--   0        0        0       61 2023-02-06 06:19:29.746754 django-cast-0.2.8/docs/releases/0.1/0.1.32.rst
--rw-r--r--   0        0        0       69 2023-02-06 06:19:29.746952 django-cast-0.2.8/docs/releases/0.1/0.1.33.rst
--rw-r--r--   0        0        0       69 2023-02-06 06:19:29.747146 django-cast-0.2.8/docs/releases/0.1/0.1.34.rst
--rw-r--r--   0        0        0       98 2023-02-06 06:19:29.747346 django-cast-0.2.8/docs/releases/0.1/0.1.35.rst
--rw-r--r--   0        0        0       86 2023-02-06 06:19:29.747543 django-cast-0.2.8/docs/releases/0.1/0.1.4.rst
--rw-r--r--   0        0        0      184 2023-02-06 06:19:29.747910 django-cast-0.2.8/docs/releases/0.1/0.1.5.rst
--rw-r--r--   0        0        0      543 2023-02-06 06:19:29.748202 django-cast-0.2.8/docs/releases/0.1/0.1.6.rst
--rw-r--r--   0        0        0       56 2023-02-06 06:19:29.748476 django-cast-0.2.8/docs/releases/0.1/0.1.7.rst
--rw-r--r--   0        0        0      158 2023-02-06 06:19:29.748680 django-cast-0.2.8/docs/releases/0.1/0.1.8.rst
--rw-r--r--   0        0        0      266 2023-02-06 06:19:29.748885 django-cast-0.2.8/docs/releases/0.1/0.1.9.rst
--rw-r--r--   0        0        0      311 2023-02-06 06:19:29.749093 django-cast-0.2.8/docs/releases/0.2.0.rst
--rw-r--r--   0        0        0      242 2023-02-06 06:19:29.749292 django-cast-0.2.8/docs/releases/0.2.1.rst
--rw-r--r--   0        0        0      371 2023-02-06 06:19:29.749592 django-cast-0.2.8/docs/releases/0.2.2.rst
--rw-r--r--   0        0        0      751 2023-02-06 06:19:29.749897 django-cast-0.2.8/docs/releases/0.2.3.rst
--rw-r--r--   0        0        0      344 2023-02-06 06:19:29.750156 django-cast-0.2.8/docs/releases/0.2.4.rst
--rw-r--r--   0        0        0      280 2023-02-12 09:48:16.819700 django-cast-0.2.8/docs/releases/0.2.5.rst
--rw-r--r--   0        0        0      262 2023-02-20 06:17:57.902102 django-cast-0.2.8/docs/releases/0.2.6.rst
--rw-r--r--   0        0        0      443 2023-03-05 14:24:40.480207 django-cast-0.2.8/docs/releases/0.2.7.rst
--rw-r--r--   0        0        0      215 2023-03-12 22:53:21.147149 django-cast-0.2.8/docs/releases/0.2.8.rst
--rw-r--r--   0        0        0      710 2023-03-12 22:53:21.147376 django-cast-0.2.8/docs/releases/index.rst
--rw-r--r--   0        0        0        5 2022-12-18 08:57:34.962538 django-cast-0.2.8/docs/requirements.txt
--rw-r--r--   0        0        0      559 2023-03-12 22:53:21.147515 django-cast-0.2.8/docs/social-media.rst
--rw-r--r--   0        0        0      852 2023-02-06 06:19:29.750723 django-cast-0.2.8/docs/spamfilter.rst
--rw-r--r--   0        0        0      628 2023-03-12 22:53:21.147593 django-cast-0.2.8/docs/tests.rst
--rw-r--r--   0        0        0     6778 2022-12-18 08:57:34.962979 django-cast-0.2.8/docs_old/Makefile
--rw-r--r--   0        0        0     3011 2022-12-18 08:57:34.963238 django-cast-0.2.8/docs_old/analytics.rst
--rw-r--r--   0        0        0       28 2022-12-18 08:57:34.963321 django-cast-0.2.8/docs_old/authors.rst
--rw-r--r--   0        0        0      725 2022-12-18 08:57:34.963418 django-cast-0.2.8/docs_old/cast.api.rst
--rw-r--r--   0        0        0     5825 2022-12-18 08:57:34.963493 django-cast-0.2.8/docs_old/cast.migrations.rst
--rw-r--r--   0        0        0     2130 2022-12-18 08:57:34.963587 django-cast-0.2.8/docs_old/cast.rst
--rw-r--r--   0        0        0      376 2022-12-18 08:57:34.963662 django-cast-0.2.8/docs_old/cast.templatetags.rst
--rw-r--r--   0        0        0      601 2022-12-18 08:57:34.963752 django-cast-0.2.8/docs_old/cdn.rst
--rw-r--r--   0        0        0      871 2022-12-18 08:57:34.963843 django-cast-0.2.8/docs_old/comments.rst
--rw-r--r--   0        0        0     8272 2022-12-18 08:57:34.964144 django-cast-0.2.8/docs_old/conf.py
--rw-r--r--   0        0        0     2335 2022-12-18 08:57:34.964250 django-cast-0.2.8/docs_old/content.rst
--rw-r--r--   0        0        0       33 2022-12-18 08:57:34.964324 django-cast-0.2.8/docs_old/contributing.rst
--rw-r--r--   0        0        0      405 2022-12-18 08:57:34.964440 django-cast-0.2.8/docs_old/deployment.rst
--rw-r--r--   0        0        0     2683 2022-12-18 08:57:34.964531 django-cast-0.2.8/docs_old/ec2_install.rst
--rw-r--r--   0        0        0      106 2022-12-18 08:57:34.964601 django-cast-0.2.8/docs_old/features.rst
--rw-r--r--   0        0        0     8198 2022-12-18 08:57:34.964750 django-cast-0.2.8/docs_old/heroku.rst
--rw-r--r--   0        0        0       28 2022-12-18 08:57:34.964818 django-cast-0.2.8/docs_old/history.rst
--rw-r--r--   0        0        0      463 2022-12-18 08:57:34.965040 django-cast-0.2.8/docs_old/index.rst
--rw-r--r--   0        0        0     3327 2022-12-18 08:57:34.965129 django-cast-0.2.8/docs_old/local_install.rst
--rw-r--r--   0        0        0     6467 2022-12-18 08:57:34.965228 django-cast-0.2.8/docs_old/make.bat
--rw-r--r--   0        0        0       49 2022-12-18 08:57:34.965298 django-cast-0.2.8/docs_old/modules.rst
--rw-r--r--   0        0        0      926 2022-12-18 08:57:34.965380 django-cast-0.2.8/docs_old/production_services.rst
--rw-r--r--   0        0        0       27 2022-12-18 08:57:34.965444 django-cast-0.2.8/docs_old/readme.rst
--rw-r--r--   0        0        0     2833 2022-12-18 08:57:34.965529 django-cast-0.2.8/docs_old/templates.rst
--rw-r--r--   0        0        0     2184 2022-12-18 08:57:34.965614 django-cast-0.2.8/docs_old/windows_install.rst
--rw-r--r--   0        0        0        0 2022-11-09 16:01:36.234151 django-cast-0.2.8/example/example_site/__init__.py
--rw-r--r--   0        0        0        0 2022-11-09 16:01:36.235705 django-cast-0.2.8/example/example_site/settings/__init__.py
--rw-r--r--   0        0        0     6931 2023-03-12 22:53:21.147806 django-cast-0.2.8/example/example_site/settings/base.py
--rw-r--r--   0        0        0      536 2023-01-21 14:08:59.179674 django-cast-0.2.8/example/example_site/settings/dev.py
--rw-r--r--   0        0        0      142 2023-01-21 14:08:59.179913 django-cast-0.2.8/example/example_site/settings/production.py
--rw-r--r--   0        0        0      191 2023-01-21 14:08:59.180245 django-cast-0.2.8/example/example_site/templates/404.html
--rw-r--r--   0        0        0      363 2023-01-21 14:08:59.180425 django-cast-0.2.8/example/example_site/templates/500.html
--rw-r--r--   0        0        0     3440 2023-01-30 05:52:09.403254 django-cast-0.2.8/example/example_site/templates/base.html
--rw-r--r--   0        0        0      103 2023-01-21 14:08:59.180774 django-cast-0.2.8/example/example_site/templates/pages/about.html
--rw-r--r--   0        0        0     1820 2023-02-26 07:05:53.137212 django-cast-0.2.8/example/example_site/urls.py
--rw-r--r--   0        0        0      406 2023-01-21 14:08:59.180960 django-cast-0.2.8/example/example_site/wsgi.py
--rw-r--r--   0        0        0      849 2022-11-09 16:01:36.237384 django-cast-0.2.8/example/manage.py
--rw-r--r--   0        0        0      228 2022-11-09 16:01:36.237511 django-cast-0.2.8/example/staticfiles/css/project.css
--rw-r--r--   0        0        0      100 2022-11-09 16:01:36.237596 django-cast-0.2.8/example/staticfiles/js/project.js
--rw-r--r--   0        0        0      249 2023-01-21 14:08:59.181336 django-cast-0.2.8/manage.py
--rw-r--r--   0        0        0    10032 2023-03-05 21:13:19.598511 django-cast-0.2.8/notebooks/api/get_pages_from_production.ipynb
--rw-r--r--   0        0        0    17098 2022-11-09 16:01:36.238186 django-cast-0.2.8/notebooks/audio/audio_handling.ipynb
--rw-r--r--   0        0        0    40442 2022-11-09 16:01:36.238884 django-cast-0.2.8/notebooks/audio/chaptermarks_form.ipynb
--rw-r--r--   0        0        0     3891 2023-01-30 05:54:18.371146 django-cast-0.2.8/notebooks/audio/file_sizes_debug.ipynb
--rw-r--r--   0        0        0    57507 2022-11-09 16:01:36.239768 django-cast-0.2.8/notebooks/audio/read_chaptermarks_from_audio_file.ipynb
--rw-r--r--   0        0        0   103147 2022-11-09 16:01:36.240384 django-cast-0.2.8/notebooks/debug/debug.ipynb
--rw-r--r--   0        0        0    14276 2022-11-09 16:01:36.240722 django-cast-0.2.8/notebooks/debug/debug_add_new_post.ipynb
--rw-r--r--   0        0        0    49103 2022-11-09 16:01:36.241164 django-cast-0.2.8/notebooks/debug/debug_blog_post_list.ipynb
--rw-r--r--   0        0        0     4441 2022-11-09 16:01:36.241470 django-cast-0.2.8/notebooks/debug/debug_comments_templates.ipynb
--rw-r--r--   0        0        0    12251 2022-11-09 16:01:36.241538 django-cast-0.2.8/notebooks/debug/django_upgrade_debug.ipynb
--rw-r--r--   0        0        0     7022 2022-11-09 16:01:36.241838 django-cast-0.2.8/notebooks/debug/pagination.ipynb
--rw-r--r--   0        0        0    20426 2022-11-09 16:01:36.242740 django-cast-0.2.8/notebooks/debug/post_get_absolute_url.ipynb
--rw-r--r--   0        0        0     2767 2022-11-09 16:01:36.243045 django-cast-0.2.8/notebooks/debug/python_3.10_debug.ipynb
--rw-r--r--   0        0        0    20471 2022-11-09 16:01:36.243288 django-cast-0.2.8/notebooks/debug/remove_obsolete_symlinks.ipynb
--rw-r--r--   0        0        0     8648 2022-11-09 16:01:36.244543 django-cast-0.2.8/notebooks/debug/render_ajax.ipynb
--rw-r--r--   0        0        0    40294 2022-11-09 16:01:36.244791 django-cast-0.2.8/notebooks/debug/sync_media_ids.ipynb
--rw-r--r--   0        0        0    24437 2022-11-09 16:01:36.245204 django-cast-0.2.8/notebooks/debug/test_file_handling.ipynb
--rw-r--r--   0        0        0    69718 2022-11-09 16:01:36.245680 django-cast-0.2.8/notebooks/debug/video_exploration_foo.ipynb
--rw-r--r--   0        0        0    23357 2022-11-09 16:01:36.246283 django-cast-0.2.8/notebooks/feed/feed_structure.ipynb
--rw-r--r--   0        0        0     1192 2023-02-06 06:19:32.679909 django-cast-0.2.8/notebooks/feed/remove_timestamped_model.ipynb
--rw-r--r--   0        0        0     7199 2023-02-12 09:06:08.029824 django-cast-0.2.8/notebooks/image/from_pillow_to_willow.ipynb
--rw-r--r--   0        0        0    25495 2022-11-09 16:01:36.246807 django-cast-0.2.8/notebooks/image/gallery_tests.ipynb
--rw-r--r--   0        0        0    18572 2022-11-09 16:01:36.247244 django-cast-0.2.8/notebooks/logs/broken_access_log.ipynb
--rw-r--r--   0        0        0    16031 2023-01-06 13:26:12.974612 django-cast-0.2.8/notebooks/moderation/2023-01-04_improve_spamfilter.ipynb
--rw-r--r--   0        0        0  2650841 2022-12-18 09:06:19.427323 django-cast-0.2.8/notebooks/moderation/comments.json
--rw-r--r--   0        0        0    82589 2023-01-06 13:26:12.975656 django-cast-0.2.8/notebooks/moderation/comments_api_endpoint_debug.ipynb
-lrwxr-xr-x   0        0        0        0 2022-11-09 16:01:36.248969 django-cast-0.2.8/notebooks/moderation/example_site -> ../../example/example_site
--rw-r--r--   0        0        0    12907 2022-12-18 09:06:19.427938 django-cast-0.2.8/notebooks/moderation/get_comments_from_production.ipynb
--rw-r--r--   0        0        0    26385 2022-12-18 09:06:19.428278 django-cast-0.2.8/notebooks/moderation/moderation_debug.ipynb
--rw-r--r--   0        0        0    53189 2023-01-06 13:26:12.976288 django-cast-0.2.8/notebooks/moderation/naive_bayes.ipynb
--rw-r--r--   0        0        0    50435 2022-11-09 16:01:36.250271 django-cast-0.2.8/notebooks/moderation/naive_bayes_class.ipynb
--rw-r--r--   0        0        0    44598 2022-11-09 16:01:36.250570 django-cast-0.2.8/notebooks/moderation/naive_bayes_from_scratch.ipynb
--rw-r--r--   0        0        0     7256 2022-11-09 16:01:36.250816 django-cast-0.2.8/notebooks/moderation/sms_dataset_to_messages.ipynb
--rw-r--r--   0        0        0   112037 2022-11-09 16:01:36.251491 django-cast-0.2.8/notebooks/moderation/spamfilter.ipynb
--rw-r--r--   0        0        0     9070 2022-12-18 09:06:19.428532 django-cast-0.2.8/notebooks/moderation/spamfilter_on_comments_from_db.ipynb
--rw-r--r--   0        0        0    58099 2022-11-09 16:01:36.252159 django-cast-0.2.8/notebooks/offtopic/dice.ipynb
--rw-r--r--   0        0        0    45371 2022-11-09 16:01:36.252482 django-cast-0.2.8/notebooks/search/faceted_navigation_debug.ipynb
--rw-r--r--   0        0        0     1116 2023-01-30 05:54:18.374803 django-cast-0.2.8/notebooks/twitter/player_card.ipynb
--rw-r--r--   0        0        0    35881 2023-02-06 06:19:32.677260 django-cast-0.2.8/notebooks/twitter/twitter_player_card.ipynb
--rw-r--r--   0        0        0     4186 2022-11-09 16:01:36.252915 django-cast-0.2.8/notebooks/wagtail/add_child_debug.ipynb
--rw-r--r--   0        0        0     1981 2023-02-26 08:29:28.223287 django-cast-0.2.8/notebooks/wagtail/api.ipynb
--rw-r--r--   0        0        0     3420 2023-01-15 12:33:49.375233 django-cast-0.2.8/notebooks/wagtail/code_block.ipynb
--rw-r--r--   0        0        0    16573 2023-03-05 21:13:19.594358 django-cast-0.2.8/notebooks/wagtail/create_content_wagtail.ipynb
--rw-r--r--   0        0        0    24960 2022-11-20 05:04:31.320939 django-cast-0.2.8/notebooks/wagtail/missing_audio.ipynb
--rw-r--r--   0        0        0    17008 2023-03-05 21:13:19.606083 django-cast-0.2.8/notebooks/wagtail/split_post_into_post_and_episode.ipynb
--rw-r--r--   0        0        0    22262 2023-03-12 22:53:21.148142 django-cast-0.2.8/notebooks/wagtail/template_settings.ipynb
--rw-r--r--   0        0        0   165131 2022-11-09 16:01:36.253921 django-cast-0.2.8/notebooks/wagtail/test_wagtail_views.ipynb
--rw-r--r--   0        0        0     9095 2023-01-30 05:20:09.492195 django-cast-0.2.8/notebooks/wagtail/wagtail_get_descendants_of_page_statements.ipynb
--rw-r--r--   0        0        0    25477 2023-01-06 13:26:12.976885 django-cast-0.2.8/notebooks/wagtail/wagtail_render_post.ipynb
--rw-r--r--   0        0        0    53276 2022-11-09 16:01:36.255073 django-cast-0.2.8/notebooks/wagtail/wagtail_video_views.ipynb
--rw-r--r--   0        0        0     3103 2023-02-26 07:05:53.137801 django-cast-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      286 2020-12-14 06:01:37.766654 django-cast-0.2.8/release.txt
--rw-r--r--   0        0        0      699 2023-01-21 14:08:59.181997 django-cast-0.2.8/runtests.py
--rw-r--r--   0        0        0      717 2022-12-18 08:57:34.967158 django-cast-0.2.8/setup.cfg
--rw-r--r--   0        0        0        0 2020-12-14 06:01:37.766864 django-cast-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-02-12 09:06:05.621645 django-cast-0.2.8/tests/admin_test.py
--rw-r--r--   0        0        0     6841 2023-02-12 09:06:05.621967 django-cast-0.2.8/tests/api_test.py
--rw-r--r--   0        0        0      692 2023-02-12 09:06:05.622219 django-cast-0.2.8/tests/apps_test.py
--rw-r--r--   0        0        0    10881 2023-02-12 09:06:05.622532 django-cast-0.2.8/tests/audio_models_test.py
--rw-r--r--   0        0        0    14880 2023-02-12 09:06:05.622857 django-cast-0.2.8/tests/audio_views_test.py
--rw-r--r--   0        0        0      984 2023-01-30 05:52:09.405779 django-cast-0.2.8/tests/blocks_test.py
--rw-r--r--   0        0        0     7065 2023-03-12 22:53:21.148443 django-cast-0.2.8/tests/blog_index_test.py
--rw-r--r--   0        0        0        0 2023-01-30 05:52:09.406006 django-cast-0.2.8/tests/cast/static/.gitkeep
--rw-r--r--   0        0        0     4871 2023-02-14 21:21:43.460183 django-cast-0.2.8/tests/comments_test.py
--rw-r--r--   0        0        0    14597 2023-02-12 09:06:05.623164 django-cast-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0      832 2023-01-30 05:52:09.406659 django-cast-0.2.8/tests/episode_detail_test.py
--rw-r--r--   0        0        0     1954 2023-02-12 09:06:05.623460 django-cast-0.2.8/tests/factories.py
--rw-r--r--   0        0        0     6609 2023-02-23 17:07:56.455208 django-cast-0.2.8/tests/feed_test.py
--rw-r--r--   0        0        0      873 2023-02-12 09:06:05.623974 django-cast-0.2.8/tests/filter_test.py
--rw-r--r--   0        0        0      526 2020-12-14 06:01:37.767120 django-cast-0.2.8/tests/fixtures/access.log
--rw-r--r--   0        0        0     6824 2020-12-14 06:01:37.767199 django-cast-0.2.8/tests/fixtures/test.m4a
--rw-r--r--   0        0        0      262 2020-12-14 06:01:37.767245 django-cast-0.2.8/tests/fixtures/test.mp4
--rw-r--r--   0        0        0     4476 2023-02-12 09:06:05.624347 django-cast-0.2.8/tests/forms_test.py
--rw-r--r--   0        0        0      331 2023-02-12 09:06:05.624566 django-cast-0.2.8/tests/meta_test.py
--rw-r--r--   0        0        0      435 2023-01-30 05:52:09.407251 django-cast-0.2.8/tests/meta_views_test.py
--rw-r--r--   0        0        0     7773 2023-03-12 22:53:21.148600 django-cast-0.2.8/tests/models_test.py
--rw-r--r--   0        0        0     5971 2023-02-12 09:06:05.625193 django-cast-0.2.8/tests/moderation_test.py
--rw-r--r--   0        0        0     1590 2023-02-12 09:48:16.820124 django-cast-0.2.8/tests/pagination_test.py
--rw-r--r--   0        0        0     6363 2023-01-30 05:52:09.407682 django-cast-0.2.8/tests/post_add_test.py
--rw-r--r--   0        0        0      935 2023-01-30 05:52:09.407773 django-cast-0.2.8/tests/post_detail_test.py
--rw-r--r--   0        0        0     2467 2023-01-30 05:52:09.407881 django-cast-0.2.8/tests/post_media_sync_test.py
--rw-r--r--   0        0        0      796 2023-02-06 06:19:29.752992 django-cast-0.2.8/tests/post_published_test.py
--rw-r--r--   0        0        0     5714 2023-03-12 22:53:21.148717 django-cast-0.2.8/tests/settings.py
--rw-r--r--   0        0        0     2223 2023-03-12 22:53:21.149039 django-cast-0.2.8/tests/theme_test.py
--rw-r--r--   0        0        0     1792 2023-01-30 05:52:09.408523 django-cast-0.2.8/tests/upload_handler_test.py
--rw-r--r--   0        0        0      748 2023-02-26 07:05:53.138104 django-cast-0.2.8/tests/urls.py
--rw-r--r--   0        0        0      447 2023-01-30 05:52:09.408676 django-cast-0.2.8/tests/utils_test.py
--rw-r--r--   0        0        0    25531 2023-01-30 05:52:09.408915 django-cast-0.2.8/tests/video_dimensions_test.py
--rw-r--r--   0        0        0     1343 2023-01-30 05:52:09.409123 django-cast-0.2.8/tests/video_upload_test.py
--rw-r--r--   0        0        0    14012 2023-02-12 09:06:05.625996 django-cast-0.2.8/tests/video_views_test.py
--rw-r--r--   0        0        0      483 2023-02-07 18:43:34.635097 django-cast-0.2.8/tests/wagtail_image_views_test.py
--rw-r--r--   0        0        0     1117 2023-02-12 09:06:05.626238 django-cast-0.2.8/tests/widget_test.py
--rw-r--r--   0        0        0      256 2023-01-30 05:52:09.409560 django-cast-0.2.8/tox.ini
--rw-r--r--   0        0        0     2679 1970-01-01 00:00:00.000000 django-cast-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      331 2020-12-14 06:01:37.748978 django-cast-0.2.9/.editorconfig
+-rw-r--r--   0        0        0      340 2020-12-14 06:01:37.749087 django-cast-0.2.9/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      945 2023-02-20 06:17:57.899206 django-cast-0.2.9/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      932 2022-12-18 08:57:34.948078 django-cast-0.2.9/.gitignore
+-rw-r--r--   0        0        0     2053 2023-03-20 06:09:43.187308 django-cast-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       50 2020-12-14 06:01:37.749209 django-cast-0.2.9/.readthedocs.yml
+-rw-r--r--   0        0        0      500 2022-12-18 08:57:34.949060 django-cast-0.2.9/.travis.yml
+-rw-r--r--   0        0        0      185 2022-11-09 16:01:36.193748 django-cast-0.2.9/AUTHORS.rst
+-rw-r--r--   0        0        0     3210 2022-11-09 16:01:36.193901 django-cast-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1501 2022-11-09 16:01:36.193999 django-cast-0.2.9/LICENSE
+-rw-r--r--   0        0        0      160 2022-12-18 08:57:34.949346 django-cast-0.2.9/Procfile
+-rw-r--r--   0        0        0     2282 2023-03-20 06:09:43.187695 django-cast-0.2.9/README.md
+-rw-r--r--   0        0        0     5271 2022-12-18 08:57:34.949979 django-cast-0.2.9/README_OLD.rst
+-rw-r--r--   0        0        0      671 2022-12-18 09:06:19.412296 django-cast-0.2.9/bootstrap.md
+-rw-r--r--   0        0        0       85 2023-03-20 06:09:43.188073 django-cast-0.2.9/cast/__init__.py
+-rw-r--r--   0        0        0     3973 2023-02-12 09:06:05.609865 django-cast-0.2.9/cast/admin.py
+-rw-r--r--   0        0        0      560 2023-02-12 09:06:05.610163 django-cast-0.2.9/cast/admin_urls/audio.py
+-rw-r--r--   0        0        0      560 2023-02-12 09:06:05.610406 django-cast-0.2.9/cast/admin_urls/video.py
+-rw-r--r--   0        0        0        0 2020-12-14 06:01:37.750115 django-cast-0.2.9/cast/api/__init__.py
+-rw-r--r--   0        0        0     1280 2023-01-15 12:33:49.372425 django-cast-0.2.9/cast/api/serializers.py
+-rw-r--r--   0        0        0     1188 2023-02-26 07:05:53.133893 django-cast-0.2.9/cast/api/urls.py
+-rw-r--r--   0        0        0      744 2023-02-12 09:06:05.610869 django-cast-0.2.9/cast/api/viewmixins.py
+-rw-r--r--   0        0        0     4429 2023-03-05 14:24:40.476089 django-cast-0.2.9/cast/api/views.py
+-rw-r--r--   0        0        0      773 2023-02-12 09:06:05.611650 django-cast-0.2.9/cast/apps.py
+-rw-r--r--   0        0        0      457 2023-03-20 06:09:43.188491 django-cast-0.2.9/cast/appsettings.py
+-rw-r--r--   0        0        0     3288 2023-02-12 09:06:05.611976 django-cast-0.2.9/cast/blocks.py
+-rw-r--r--   0        0        0      549 2023-03-20 06:09:43.188817 django-cast-0.2.9/cast/context_processors.py
+-rw-r--r--   0        0        0     8237 2023-02-23 17:07:51.458204 django-cast-0.2.9/cast/feeds.py
+-rw-r--r--   0        0        0     8190 2023-03-20 06:09:43.189266 django-cast-0.2.9/cast/filters.py
+-rw-r--r--   0        0        0     6261 2023-02-12 09:06:05.613123 django-cast-0.2.9/cast/forms.py
+-rw-r--r--   0        0        0     4094 2020-12-14 06:01:37.751186 django-cast-0.2.9/cast/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6148 2020-12-14 06:01:37.751304 django-cast-0.2.9/cast/management/.DS_Store
+-rw-r--r--   0        0        0    12288 2020-12-14 06:01:37.751493 django-cast-0.2.9/cast/management/commands/.s3_stale.py.swp
+-rw-r--r--   0        0        0        0 2020-12-14 06:01:37.751553 django-cast-0.2.9/cast/management/commands/__init__.py
+-rw-r--r--   0        0        0      443 2023-01-21 14:08:59.166854 django-cast-0.2.9/cast/management/commands/add_missing_media_objects.py
+-rw-r--r--   0        0        0      552 2023-01-21 14:08:59.167148 django-cast-0.2.9/cast/management/commands/get_api_token.py
+-rw-r--r--   0        0        0      386 2020-12-14 06:01:37.751844 django-cast-0.2.9/cast/management/commands/recalc_video_posters.py
+-rw-r--r--   0        0        0      598 2022-11-09 16:01:36.202046 django-cast-0.2.9/cast/management/commands/s3_backup.py
+-rw-r--r--   0        0        0     1194 2022-11-09 16:01:36.202772 django-cast-0.2.9/cast/management/commands/s3_media_sizes.py
+-rw-r--r--   0        0        0      726 2022-11-09 16:01:36.202874 django-cast-0.2.9/cast/management/commands/s3_replace.py
+-rw-r--r--   0        0        0      601 2023-01-21 14:08:59.167393 django-cast-0.2.9/cast/management/commands/s3_restore.py
+-rw-r--r--   0        0        0     2382 2023-01-30 05:52:09.388926 django-cast-0.2.9/cast/management/commands/s3_stale.py
+-rw-r--r--   0        0        0    19623 2022-11-09 16:01:36.203740 django-cast-0.2.9/cast/migrations/0001_initial.py
+-rw-r--r--   0        0        0      317 2022-11-09 16:01:36.203922 django-cast-0.2.9/cast/migrations/0002_remove_blog_description.py
+-rw-r--r--   0        0        0      333 2022-11-09 16:01:36.203981 django-cast-0.2.9/cast/migrations/0003_remove_post_parent_blog.py
+-rw-r--r--   0        0        0      702 2022-11-09 16:01:36.204039 django-cast-0.2.9/cast/migrations/0004_homepage_alias_for_page.py
+-rw-r--r--   0        0        0      881 2022-11-09 16:01:36.204113 django-cast-0.2.9/cast/migrations/0005_auto_20201024_0613.py
+-rw-r--r--   0        0        0     3342 2022-11-09 16:01:36.204169 django-cast-0.2.9/cast/migrations/0006_auto_20210628_1628.py
+-rw-r--r--   0        0        0      994 2022-11-09 16:01:36.204528 django-cast-0.2.9/cast/migrations/0007_alter_post_body.py
+-rw-r--r--   0        0        0     2138 2022-11-09 16:01:36.204765 django-cast-0.2.9/cast/migrations/0008_auto_20210712_0919.py
+-rw-r--r--   0        0        0     1104 2022-11-09 16:01:36.205160 django-cast-0.2.9/cast/migrations/0009_alter_post_body.py
+-rw-r--r--   0        0        0      359 2022-11-09 16:01:36.205213 django-cast-0.2.9/cast/migrations/0010_rename_intro_blog_description.py
+-rw-r--r--   0        0        0     2459 2022-11-09 16:01:36.205340 django-cast-0.2.9/cast/migrations/0011_alter_post_body.py
+-rw-r--r--   0        0        0      465 2022-11-09 16:01:36.205400 django-cast-0.2.9/cast/migrations/0012_alter_post_images.py
+-rw-r--r--   0        0        0      458 2022-11-09 16:01:36.205457 django-cast-0.2.9/cast/migrations/0013_alter_gallery_images.py
+-rw-r--r--   0        0        0      326 2022-11-09 16:01:36.205515 django-cast-0.2.9/cast/migrations/0014_remove_gallery_user.py
+-rw-r--r--   0        0        0      494 2022-11-09 16:01:36.205576 django-cast-0.2.9/cast/migrations/0015_delete_blogindexpage.py
+-rw-r--r--   0        0        0     1143 2022-11-09 16:01:36.205635 django-cast-0.2.9/cast/migrations/0016_auto_20210830_0422.py
+-rw-r--r--   0        0        0     2906 2022-11-09 16:01:36.205753 django-cast-0.2.9/cast/migrations/0017_alter_post_body.py
+-rw-r--r--   0        0        0      424 2022-11-09 16:01:36.206068 django-cast-0.2.9/cast/migrations/0018_alter_chaptermark_start.py
+-rw-r--r--   0        0        0      419 2022-11-09 16:01:36.206270 django-cast-0.2.9/cast/migrations/0019_alter_chaptermark_start.py
+-rw-r--r--   0        0        0     2991 2022-11-09 16:01:36.206623 django-cast-0.2.9/cast/migrations/0020_auto_20210926_1556.py
+-rw-r--r--   0        0        0     1249 2022-11-09 16:01:36.206773 django-cast-0.2.9/cast/migrations/0021_spamfilter.py
+-rw-r--r--   0        0        0      515 2022-11-09 16:01:36.207208 django-cast-0.2.9/cast/migrations/0022_alter_spamfilter_model.py
+-rw-r--r--   0        0        0      621 2022-11-09 16:01:36.207872 django-cast-0.2.9/cast/migrations/0023_alter_spamfilter_model.py
+-rw-r--r--   0        0        0     3514 2022-12-18 08:57:34.951279 django-cast-0.2.9/cast/migrations/0024_alter_homepage_body_alter_post_body.py
+-rw-r--r--   0        0        0      456 2023-01-06 13:26:12.969194 django-cast-0.2.9/cast/migrations/0025_add_performance_indicators.py
+-rw-r--r--   0        0        0     4993 2023-01-30 05:52:09.389439 django-cast-0.2.9/cast/migrations/0026_delete_request_alter_post_body.py
+-rw-r--r--   0        0        0     2496 2023-01-30 05:52:09.389746 django-cast-0.2.9/cast/migrations/0027_episode.py
+-rw-r--r--   0        0        0     1217 2023-01-30 05:52:09.389945 django-cast-0.2.9/cast/migrations/0028_rename_and_drop_itune_fields.py
+-rw-r--r--   0        0        0      424 2023-01-30 05:52:09.390078 django-cast-0.2.9/cast/migrations/0029_add_metadata_field_to_audio.py
+-rw-r--r--   0        0        0      334 2023-02-06 06:19:29.734552 django-cast-0.2.9/cast/migrations/0030_remove_pub_date_is_handled_by_wagtail.py
+-rw-r--r--   0        0        0      446 2023-02-06 06:19:29.735460 django-cast-0.2.9/cast/migrations/0031_remove_timestampedmodel_because_wagtail.py
+-rw-r--r--   0        0        0      448 2023-02-06 06:19:29.735828 django-cast-0.2.9/cast/migrations/0032_remove_timestampedmodel_because_wagtail.py
+-rw-r--r--   0        0        0     2516 2023-02-06 06:19:29.736266 django-cast-0.2.9/cast/migrations/0033_add_new_podcast_model.py
+-rw-r--r--   0        0        0      652 2023-02-06 06:19:29.736523 django-cast-0.2.9/cast/migrations/0034_remove_old_podcast_fields_from_blog.py
+-rw-r--r--   0        0        0      857 2023-02-06 06:19:29.736759 django-cast-0.2.9/cast/migrations/0035_remove_new_prefix_podcast_fields.py
+-rw-r--r--   0        0        0      586 2023-02-06 06:19:29.737273 django-cast-0.2.9/cast/migrations/0036_alter_blog_author.py
+-rw-r--r--   0        0        0     1957 2023-02-06 06:19:29.737589 django-cast-0.2.9/cast/migrations/0037_alter_episode_block_alter_episode_explicit_and_more.py
+-rw-r--r--   0        0        0      653 2023-02-12 09:06:05.613416 django-cast-0.2.9/cast/migrations/0038_alter_episode_keywords.py
+-rw-r--r--   0        0        0      551 2023-03-05 14:24:40.476688 django-cast-0.2.9/cast/migrations/0039_blog_noindex.py
+-rw-r--r--   0        0        0      578 2023-03-12 22:53:21.138717 django-cast-0.2.9/cast/migrations/0040_alter_blog_noindex.py
+-rw-r--r--   0        0        0     1163 2023-03-12 22:53:21.138820 django-cast-0.2.9/cast/migrations/0041_templatebasedirectory.py
+-rw-r--r--   0        0        0      509 2023-03-12 22:53:21.139225 django-cast-0.2.9/cast/migrations/0042_blog_template_base_dir.py
+-rw-r--r--   0        0        0      592 2023-03-12 22:53:21.139465 django-cast-0.2.9/cast/migrations/0043_alter_blog_template_base_dir.py
+-rw-r--r--   0        0        0     1252 2023-03-12 22:53:21.139821 django-cast-0.2.9/cast/migrations/0044_alter_blog_template_base_dir_and_more.py
+-rw-r--r--   0        0        0     1429 2023-03-20 06:09:43.189664 django-cast-0.2.9/cast/migrations/0045_alter_blog_template_base_dir_and_more.py
+-rw-r--r--   0        0        0        0 2020-12-14 06:01:37.752618 django-cast-0.2.9/cast/migrations/__init__.py
+-rw-r--r--   0        0        0      718 2023-03-12 22:53:21.140303 django-cast-0.2.9/cast/models/__init__.py
+-rw-r--r--   0        0        0    12196 2023-03-05 14:24:40.477317 django-cast-0.2.9/cast/models/audio.py
+-rw-r--r--   0        0        0      409 2023-02-12 09:06:05.614188 django-cast-0.2.9/cast/models/file.py
+-rw-r--r--   0        0        0     1253 2023-02-12 09:06:05.614492 django-cast-0.2.9/cast/models/gallery.py
+-rw-r--r--   0        0        0     7703 2023-03-20 06:09:43.190467 django-cast-0.2.9/cast/models/index_pages.py
+-rw-r--r--   0        0        0      430 2023-01-21 14:08:59.168853 django-cast-0.2.9/cast/models/itunes.py
+-rw-r--r--   0        0        0    11561 2023-02-12 09:06:05.615073 django-cast-0.2.9/cast/models/moderation.py
+-rw-r--r--   0        0        0    13447 2023-03-12 22:53:21.141084 django-cast-0.2.9/cast/models/pages.py
+-rw-r--r--   0        0        0     4795 2023-03-20 06:09:43.190843 django-cast-0.2.9/cast/models/theme.py
+-rw-r--r--   0        0        0     6067 2023-02-12 09:06:05.615815 django-cast-0.2.9/cast/models/video.py
+-rw-r--r--   0        0        0     1388 2023-02-12 09:06:05.616127 django-cast-0.2.9/cast/moderation.py
+-rw-r--r--   0        0        0      895 2023-02-12 09:06:05.616396 django-cast-0.2.9/cast/runner.py
+-rw-r--r--   0        0        0     5606 2023-03-12 22:53:21.141569 django-cast-0.2.9/cast/settings.py
+-rw-r--r--   0        0        0   162219 2023-03-20 06:09:43.192071 django-cast-0.2.9/cast/static/css/bootstrap4/bootstrap.min.css
+-rw-r--r--   0        0        0     6554 2023-02-20 06:17:57.901130 django-cast-0.2.9/cast/static/css/cast.css
+-rw-r--r--   0        0        0       93 2020-12-14 06:01:37.753112 django-cast-0.2.9/cast/static/css/my_div.css
+-rw-r--r--   0        0        0       33 2023-03-12 22:53:21.141721 django-cast-0.2.9/cast/static/css/plain/cast.css
+-rw-r--r--   0        0        0        0 2020-12-14 06:01:37.753178 django-cast-0.2.9/cast/static/img/.gitignore
+-rw-r--r--   0        0        0     1357 2022-11-09 16:01:36.213103 django-cast-0.2.9/cast/static/img/cast/Audio-icon.svg
+-rw-r--r--   0        0        0     1125 2022-11-09 16:01:36.213224 django-cast-0.2.9/cast/static/img/cast/Feed-icon.svg
+-rw-r--r--   0        0        0    10504 2020-12-14 06:01:37.753463 django-cast-0.2.9/cast/static/img/cast/Video-icon.svg
+-rw-r--r--   0        0        0    62564 2023-03-20 06:09:43.193102 django-cast-0.2.9/cast/static/js/bootstrap4/bootstrap.min.js
+-rw-r--r--   0        0        0   185258 2023-03-20 06:09:43.194604 django-cast-0.2.9/cast/static/js/bootstrap4/bootstrap.min.js.map
+-rw-r--r--   0        0        0        0 2020-12-14 06:01:37.753524 django-cast-0.2.9/cast/static/js/cast.js
+-rw-r--r--   0        0        0      251 2020-12-14 06:01:37.753880 django-cast-0.2.9/cast/static/js/cast/dashboard.js
+-rw-r--r--   0        0        0     1396 2022-11-29 05:40:21.313099 django-cast-0.2.9/cast/static/js/cast/gallery.js
+-rw-r--r--   0        0        0     5321 2022-11-09 16:01:36.213750 django-cast-0.2.9/cast/static/js/cast/wagtail/audio-chooser-modal.js
+-rw-r--r--   0        0        0      643 2022-11-09 16:01:36.214150 django-cast-0.2.9/cast/static/js/cast/wagtail/audio-chooser-telepath.js
+-rw-r--r--   0        0        0     1969 2022-11-20 05:23:10.428455 django-cast-0.2.9/cast/static/js/cast/wagtail/audio-chooser.js
+-rw-r--r--   0        0        0     5321 2022-11-09 16:01:36.214977 django-cast-0.2.9/cast/static/js/cast/wagtail/video-chooser-modal.js
+-rw-r--r--   0        0        0      643 2022-11-09 16:01:36.215855 django-cast-0.2.9/cast/static/js/cast/wagtail/video-chooser-telepath.js
+-rw-r--r--   0        0        0     1969 2022-11-09 16:01:36.216336 django-cast-0.2.9/cast/static/js/cast/wagtail/video-chooser.js
+-rw-r--r--   0        0        0   145311 2023-01-30 05:19:56.108250 django-cast-0.2.9/cast/static/js/cast/web-player/embed.4.js
+-rw-r--r--   0        0        0   134043 2023-01-30 05:19:56.109270 django-cast-0.2.9/cast/static/js/cast/web-player/embed.5.js
+-rw-r--r--   0        0        0    40884 2023-03-20 06:09:43.195148 django-cast-0.2.9/cast/static/js/htmx.min.js
+-rw-r--r--   0        0        0    89795 2023-03-20 06:09:43.196503 django-cast-0.2.9/cast/static/js/jquery/jquery-3.6.4.min.js
+-rw-r--r--   0        0        0     6148 2022-11-09 16:01:36.217492 django-cast-0.2.9/cast/templates/.DS_Store
+-rw-r--r--   0        0        0      995 2023-03-05 22:31:39.355713 django-cast-0.2.9/cast/templates/base.html
+-rw-r--r--   0        0        0     1409 2023-01-21 14:08:59.169893 django-cast-0.2.9/cast/templates/cast/audio/add.html
+-rw-r--r--   0        0        0       39 2022-11-20 08:32:17.698952 django-cast-0.2.9/cast/templates/cast/audio/audio.html
+-rw-r--r--   0        0        0      254 2023-01-21 14:08:59.170356 django-cast-0.2.9/cast/templates/cast/audio/chooser.html
+-rw-r--r--   0        0        0     2319 2023-01-21 14:08:59.170771 django-cast-0.2.9/cast/templates/cast/audio/chooser_chooser.html
+-rw-r--r--   0        0        0      599 2023-01-21 14:08:59.171161 django-cast-0.2.9/cast/templates/cast/audio/chooser_results.html
+-rw-r--r--   0        0        0      675 2022-11-09 16:01:36.220766 django-cast-0.2.9/cast/templates/cast/audio/confirm_delete.html
+-rw-r--r--   0        0        0     2227 2022-11-09 16:01:36.221033 django-cast-0.2.9/cast/templates/cast/audio/edit.html
+-rw-r--r--   0        0        0     2481 2023-01-21 14:08:59.171802 django-cast-0.2.9/cast/templates/cast/audio/index.html
+-rw-r--r--   0        0        0     2105 2023-01-21 14:08:59.172246 django-cast-0.2.9/cast/templates/cast/audio/list.html
+-rw-r--r--   0        0        0     1192 2023-01-21 14:08:59.172537 django-cast-0.2.9/cast/templates/cast/audio/results.html
+-rw-r--r--   0        0        0      661 2022-11-09 16:01:36.222449 django-cast-0.2.9/cast/templates/cast/base.html
+-rw-r--r--   0        0        0     2687 2023-03-20 06:09:43.197064 django-cast-0.2.9/cast/templates/cast/bootstrap4/base.html
+-rw-r--r--   0        0        0     2822 2023-03-20 06:09:43.197518 django-cast-0.2.9/cast/templates/cast/bootstrap4/blog_list_of_posts.html
+-rw-r--r--   0        0        0      213 2023-03-12 22:53:21.142096 django-cast-0.2.9/cast/templates/cast/bootstrap4/episode.html
+-rw-r--r--   0        0        0     1705 2023-03-20 05:29:05.438469 django-cast-0.2.9/cast/templates/cast/bootstrap4/pagination.html
+-rw-r--r--   0        0        0     2092 2023-03-20 06:09:43.197843 django-cast-0.2.9/cast/templates/cast/bootstrap4/post.html
+-rw-r--r--   0        0        0      573 2023-03-12 22:53:21.142396 django-cast-0.2.9/cast/templates/cast/bootstrap4/post_body.html
+-rw-r--r--   0        0        0      160 2023-01-21 14:08:59.173195 django-cast-0.2.9/cast/templates/cast/cast_base.html
+-rw-r--r--   0        0        0     1467 2022-11-29 12:34:11.419174 django-cast-0.2.9/cast/templates/cast/gallery.html
+-rw-r--r--   0        0        0      430 2022-11-09 16:01:36.223242 django-cast-0.2.9/cast/templates/cast/home_page.html
+-rw-r--r--   0        0        0      164 2022-11-29 12:40:41.302441 django-cast-0.2.9/cast/templates/cast/image/image.html
+-rw-r--r--   0        0        0      284 2020-12-14 06:01:37.755401 django-cast-0.2.9/cast/templates/cast/image_form.html
+-rw-r--r--   0        0        0     1133 2023-03-12 22:53:21.142536 django-cast-0.2.9/cast/templates/cast/plain/base.html
+-rw-r--r--   0        0        0     1216 2023-03-12 22:53:21.142626 django-cast-0.2.9/cast/templates/cast/plain/blog_list_of_posts.html
+-rw-r--r--   0        0        0      213 2023-03-12 22:53:21.142699 django-cast-0.2.9/cast/templates/cast/plain/episode.html
+-rw-r--r--   0        0        0      968 2023-03-12 22:53:21.142794 django-cast-0.2.9/cast/templates/cast/plain/post.html
+-rw-r--r--   0        0        0      573 2023-03-12 22:53:21.142873 django-cast-0.2.9/cast/templates/cast/plain/post_body.html
+-rw-r--r--   0        0        0     1133 2023-01-30 05:52:09.393268 django-cast-0.2.9/cast/templates/cast/twitter/card_player.html
+-rw-r--r--   0        0        0     1409 2023-01-21 14:08:59.173820 django-cast-0.2.9/cast/templates/cast/video/add.html
+-rw-r--r--   0        0        0      254 2023-01-21 14:08:59.174168 django-cast-0.2.9/cast/templates/cast/video/chooser.html
+-rw-r--r--   0        0        0     2319 2023-01-21 14:08:59.174466 django-cast-0.2.9/cast/templates/cast/video/chooser_chooser.html
+-rw-r--r--   0        0        0      598 2023-01-21 14:08:59.174682 django-cast-0.2.9/cast/templates/cast/video/chooser_results.html
+-rw-r--r--   0        0        0      675 2022-11-09 16:01:36.226562 django-cast-0.2.9/cast/templates/cast/video/confirm_delete.html
+-rw-r--r--   0        0        0     2229 2022-11-09 16:01:36.226736 django-cast-0.2.9/cast/templates/cast/video/edit.html
+-rw-r--r--   0        0        0     2481 2023-01-21 14:08:59.175076 django-cast-0.2.9/cast/templates/cast/video/index.html
+-rw-r--r--   0        0        0     2105 2023-01-21 14:08:59.175361 django-cast-0.2.9/cast/templates/cast/video/list.html
+-rw-r--r--   0        0        0     1192 2023-01-21 14:08:59.175697 django-cast-0.2.9/cast/templates/cast/video/results.html
+-rw-r--r--   0        0        0      454 2022-11-26 17:44:15.868652 django-cast-0.2.9/cast/templates/cast/video/video.html
+-rw-r--r--   0        0        0      279 2020-12-14 06:01:37.755773 django-cast-0.2.9/cast/templates/cast/video_form.html
+-rw-r--r--   0        0        0      245 2023-01-21 14:08:59.176089 django-cast-0.2.9/cast/templates/cast/wagtail/_file_field.html
+-rw-r--r--   0        0        0      224 2023-01-21 14:08:59.176485 django-cast-0.2.9/cast/templates/cast/wagtail/_file_field_as_li.html
+-rw-r--r--   0        0        0      320 2023-01-21 14:08:59.176752 django-cast-0.2.9/cast/templates/cast/wagtail/_thumbnail_field.html
+-rw-r--r--   0        0        0      229 2023-01-21 14:08:59.177009 django-cast-0.2.9/cast/templates/cast/wagtail/_thumbnail_field_as_li.html
+-rw-r--r--   0        0        0     1084 2023-01-21 14:08:59.177366 django-cast-0.2.9/cast/templates/comments/comment.html
+-rw-r--r--   0        0        0     1705 2023-03-19 14:57:20.233080 django-cast-0.2.9/cast/templates/pagination.html
+-rw-r--r--   0        0        0      937 2023-02-25 06:06:16.491075 django-cast-0.2.9/cast/urls.py
+-rw-r--r--   0        0        0      499 2023-02-12 09:06:05.618267 django-cast-0.2.9/cast/utils.py
+-rw-r--r--   0        0        0      142 2023-02-12 09:06:05.618726 django-cast-0.2.9/cast/views/__init__.py
+-rw-r--r--   0        0        0    10246 2023-02-12 09:06:05.619080 django-cast-0.2.9/cast/views/audio.py
+-rw-r--r--   0        0        0      795 2023-01-30 05:52:09.393804 django-cast-0.2.9/cast/views/meta.py
+-rw-r--r--   0        0        0     9741 2023-02-12 09:06:05.619686 django-cast-0.2.9/cast/views/video.py
+-rw-r--r--   0        0        0     2274 2023-02-12 09:06:05.620015 django-cast-0.2.9/cast/wagtail_hooks.py
+-rw-r--r--   0        0        0     4661 2023-02-12 09:06:05.620306 django-cast-0.2.9/cast/widgets.py
+-rw-r--r--   0        0        0      228 2022-11-19 08:32:39.905422 django-cast-0.2.9/command_lines.txt
+-rw-r--r--   0        0        0     3478 2023-01-30 05:52:09.394405 django-cast-0.2.9/commands.py
+-rw-r--r--   0        0        0      158 2022-11-09 16:01:36.233324 django-cast-0.2.9/django-cast-example.ps1
+-rw-r--r--   0        0        0      634 2022-12-18 08:57:34.953400 django-cast-0.2.9/docs/Makefile
+-rw-r--r--   0        0        0      971 2023-03-20 06:09:43.198340 django-cast-0.2.9/docs/conf.py
+-rw-r--r--   0        0        0     1513 2023-03-20 06:09:43.198595 django-cast-0.2.9/docs/context-processors.rst
+-rw-r--r--   0        0        0       45 2022-12-18 08:57:34.954013 django-cast-0.2.9/docs/contributing.rst
+-rw-r--r--   0        0        0     1441 2023-03-20 06:09:43.198894 django-cast-0.2.9/docs/features.rst
+-rw-r--r--   0        0        0      126 2023-03-20 06:09:43.199152 django-cast-0.2.9/docs/howto/first-cast.rst
+-rw-r--r--   0        0        0     3910 2023-02-06 06:19:29.739700 django-cast-0.2.9/docs/howto/index.rst
+-rw-r--r--   0        0        0      135 2023-03-20 06:09:43.199374 django-cast-0.2.9/docs/howto/integrate-cast.rst
+-rw-r--r--   0        0        0    46438 2023-03-12 22:53:21.145005 django-cast-0.2.9/docs/images/blog_template_base_dir_setting.png
+-rw-r--r--   0        0        0   143585 2023-01-30 05:52:09.396034 django-cast-0.2.9/docs/images/cache_file_sizes_admin_action.png
+-rw-r--r--   0        0        0    50259 2023-01-06 13:26:12.972329 django-cast-0.2.9/docs/images/spam_filter_performance.png
+-rw-r--r--   0        0        0    82268 2023-03-12 22:53:21.146414 django-cast-0.2.9/docs/images/template_base_dir_setting.png
+-rw-r--r--   0        0        0   167962 2023-01-30 05:52:09.397690 django-cast-0.2.9/docs/images/twitter_card.png
+-rw-r--r--   0        0        0      543 2023-03-20 06:09:43.199657 django-cast-0.2.9/docs/index.rst
+-rw-r--r--   0        0        0     2763 2023-03-20 06:09:43.199958 django-cast-0.2.9/docs/installation.rst
+-rw-r--r--   0        0        0      800 2022-12-18 08:57:34.954986 django-cast-0.2.9/docs/make.bat
+-rw-r--r--   0        0        0      806 2023-03-12 22:53:21.146731 django-cast-0.2.9/docs/models.rst
+-rw-r--r--   0        0        0      866 2023-02-06 06:19:29.740351 django-cast-0.2.9/docs/release.rst
+-rw-r--r--   0        0        0       64 2023-02-06 06:19:29.740882 django-cast-0.2.9/docs/releases/0.1/0.1.0.rst
+-rw-r--r--   0        0        0       61 2023-02-06 06:19:29.741149 django-cast-0.2.9/docs/releases/0.1/0.1.1.rst
+-rw-r--r--   0        0        0      202 2023-02-06 06:19:29.741403 django-cast-0.2.9/docs/releases/0.1/0.1.10.rst
+-rw-r--r--   0        0        0       74 2023-02-06 06:19:29.741623 django-cast-0.2.9/docs/releases/0.1/0.1.11.rst
+-rw-r--r--   0        0        0       79 2023-02-06 06:19:29.741850 django-cast-0.2.9/docs/releases/0.1/0.1.12.rst
+-rw-r--r--   0        0        0       75 2023-02-06 06:19:29.742065 django-cast-0.2.9/docs/releases/0.1/0.1.13.rst
+-rw-r--r--   0        0        0      103 2023-02-06 06:19:29.742317 django-cast-0.2.9/docs/releases/0.1/0.1.14.rst
+-rw-r--r--   0        0        0       78 2023-02-06 06:19:29.742535 django-cast-0.2.9/docs/releases/0.1/0.1.15.rst
+-rw-r--r--   0        0        0       96 2023-02-06 06:19:29.742757 django-cast-0.2.9/docs/releases/0.1/0.1.16.rst
+-rw-r--r--   0        0        0      212 2023-02-06 06:19:29.743020 django-cast-0.2.9/docs/releases/0.1/0.1.17.rst
+-rw-r--r--   0        0        0      141 2023-02-06 06:19:29.743407 django-cast-0.2.9/docs/releases/0.1/0.1.18.rst
+-rw-r--r--   0        0        0      222 2023-02-06 06:19:29.743625 django-cast-0.2.9/docs/releases/0.1/0.1.19.rst
+-rw-r--r--   0        0        0       89 2023-02-06 06:19:29.743829 django-cast-0.2.9/docs/releases/0.1/0.1.2.rst
+-rw-r--r--   0        0        0       87 2023-02-06 06:19:29.744021 django-cast-0.2.9/docs/releases/0.1/0.1.20.rst
+-rw-r--r--   0        0        0       92 2023-02-06 06:19:29.744238 django-cast-0.2.9/docs/releases/0.1/0.1.21.rst
+-rw-r--r--   0        0        0      204 2023-02-06 06:19:29.744442 django-cast-0.2.9/docs/releases/0.1/0.1.22.rst
+-rw-r--r--   0        0        0      200 2023-02-06 06:19:29.744669 django-cast-0.2.9/docs/releases/0.1/0.1.23.rst
+-rw-r--r--   0        0        0      356 2023-02-06 06:19:29.744877 django-cast-0.2.9/docs/releases/0.1/0.1.24.rst
+-rw-r--r--   0        0        0      134 2023-02-06 06:19:29.745085 django-cast-0.2.9/docs/releases/0.1/0.1.25.rst
+-rw-r--r--   0        0        0       88 2023-02-06 06:19:29.745283 django-cast-0.2.9/docs/releases/0.1/0.1.26.rst
+-rw-r--r--   0        0        0      221 2023-02-06 06:19:29.745489 django-cast-0.2.9/docs/releases/0.1/0.1.27.rst
+-rw-r--r--   0        0        0      516 2023-02-06 06:19:29.745705 django-cast-0.2.9/docs/releases/0.1/0.1.28.rst
+-rw-r--r--   0        0        0       95 2023-02-06 06:19:29.745924 django-cast-0.2.9/docs/releases/0.1/0.1.29.rst
+-rw-r--r--   0        0        0      159 2023-02-06 06:19:29.746139 django-cast-0.2.9/docs/releases/0.1/0.1.3.rst
+-rw-r--r--   0        0        0      118 2023-02-06 06:19:29.746357 django-cast-0.2.9/docs/releases/0.1/0.1.30.rst
+-rw-r--r--   0        0        0       92 2023-02-06 06:19:29.746563 django-cast-0.2.9/docs/releases/0.1/0.1.31.rst
+-rw-r--r--   0        0        0       61 2023-02-06 06:19:29.746754 django-cast-0.2.9/docs/releases/0.1/0.1.32.rst
+-rw-r--r--   0        0        0       69 2023-02-06 06:19:29.746952 django-cast-0.2.9/docs/releases/0.1/0.1.33.rst
+-rw-r--r--   0        0        0       69 2023-02-06 06:19:29.747146 django-cast-0.2.9/docs/releases/0.1/0.1.34.rst
+-rw-r--r--   0        0        0       98 2023-02-06 06:19:29.747346 django-cast-0.2.9/docs/releases/0.1/0.1.35.rst
+-rw-r--r--   0        0        0       86 2023-02-06 06:19:29.747543 django-cast-0.2.9/docs/releases/0.1/0.1.4.rst
+-rw-r--r--   0        0        0      184 2023-02-06 06:19:29.747910 django-cast-0.2.9/docs/releases/0.1/0.1.5.rst
+-rw-r--r--   0        0        0      543 2023-02-06 06:19:29.748202 django-cast-0.2.9/docs/releases/0.1/0.1.6.rst
+-rw-r--r--   0        0        0       56 2023-02-06 06:19:29.748476 django-cast-0.2.9/docs/releases/0.1/0.1.7.rst
+-rw-r--r--   0        0        0      158 2023-02-06 06:19:29.748680 django-cast-0.2.9/docs/releases/0.1/0.1.8.rst
+-rw-r--r--   0        0        0      266 2023-02-06 06:19:29.748885 django-cast-0.2.9/docs/releases/0.1/0.1.9.rst
+-rw-r--r--   0        0        0      311 2023-02-06 06:19:29.749093 django-cast-0.2.9/docs/releases/0.2.0.rst
+-rw-r--r--   0        0        0      242 2023-02-06 06:19:29.749292 django-cast-0.2.9/docs/releases/0.2.1.rst
+-rw-r--r--   0        0        0      371 2023-02-06 06:19:29.749592 django-cast-0.2.9/docs/releases/0.2.2.rst
+-rw-r--r--   0        0        0      751 2023-02-06 06:19:29.749897 django-cast-0.2.9/docs/releases/0.2.3.rst
+-rw-r--r--   0        0        0      344 2023-02-06 06:19:29.750156 django-cast-0.2.9/docs/releases/0.2.4.rst
+-rw-r--r--   0        0        0      280 2023-02-12 09:48:16.819700 django-cast-0.2.9/docs/releases/0.2.5.rst
+-rw-r--r--   0        0        0      262 2023-02-20 06:17:57.902102 django-cast-0.2.9/docs/releases/0.2.6.rst
+-rw-r--r--   0        0        0      443 2023-03-05 14:24:40.480207 django-cast-0.2.9/docs/releases/0.2.7.rst
+-rw-r--r--   0        0        0      215 2023-03-12 22:53:21.147149 django-cast-0.2.9/docs/releases/0.2.8.rst
+-rw-r--r--   0        0        0      288 2023-03-20 06:09:43.200224 django-cast-0.2.9/docs/releases/0.2.9.rst
+-rw-r--r--   0        0        0      719 2023-03-20 06:09:43.200642 django-cast-0.2.9/docs/releases/index.rst
+-rw-r--r--   0        0        0        5 2022-12-18 08:57:34.962538 django-cast-0.2.9/docs/requirements.txt
+-rw-r--r--   0        0        0     1873 2023-03-20 06:09:43.200911 django-cast-0.2.9/docs/settings.rst
+-rw-r--r--   0        0        0      559 2023-03-12 22:53:21.147515 django-cast-0.2.9/docs/social-media.rst
+-rw-r--r--   0        0        0      852 2023-02-06 06:19:29.750723 django-cast-0.2.9/docs/spamfilter.rst
+-rw-r--r--   0        0        0      628 2023-03-12 22:53:21.147593 django-cast-0.2.9/docs/tests.rst
+-rw-r--r--   0        0        0     2252 2023-03-20 06:09:43.201176 django-cast-0.2.9/docs/themes.rst
+-rw-r--r--   0        0        0     6778 2022-12-18 08:57:34.962979 django-cast-0.2.9/docs_old/Makefile
+-rw-r--r--   0        0        0     3011 2022-12-18 08:57:34.963238 django-cast-0.2.9/docs_old/analytics.rst
+-rw-r--r--   0        0        0       28 2022-12-18 08:57:34.963321 django-cast-0.2.9/docs_old/authors.rst
+-rw-r--r--   0        0        0      725 2022-12-18 08:57:34.963418 django-cast-0.2.9/docs_old/cast.api.rst
+-rw-r--r--   0        0        0     5825 2022-12-18 08:57:34.963493 django-cast-0.2.9/docs_old/cast.migrations.rst
+-rw-r--r--   0        0        0     2130 2022-12-18 08:57:34.963587 django-cast-0.2.9/docs_old/cast.rst
+-rw-r--r--   0        0        0      376 2022-12-18 08:57:34.963662 django-cast-0.2.9/docs_old/cast.templatetags.rst
+-rw-r--r--   0        0        0      601 2022-12-18 08:57:34.963752 django-cast-0.2.9/docs_old/cdn.rst
+-rw-r--r--   0        0        0      871 2022-12-18 08:57:34.963843 django-cast-0.2.9/docs_old/comments.rst
+-rw-r--r--   0        0        0     8272 2022-12-18 08:57:34.964144 django-cast-0.2.9/docs_old/conf.py
+-rw-r--r--   0        0        0     2335 2022-12-18 08:57:34.964250 django-cast-0.2.9/docs_old/content.rst
+-rw-r--r--   0        0        0       33 2022-12-18 08:57:34.964324 django-cast-0.2.9/docs_old/contributing.rst
+-rw-r--r--   0        0        0      405 2022-12-18 08:57:34.964440 django-cast-0.2.9/docs_old/deployment.rst
+-rw-r--r--   0        0        0     2683 2022-12-18 08:57:34.964531 django-cast-0.2.9/docs_old/ec2_install.rst
+-rw-r--r--   0        0        0      106 2022-12-18 08:57:34.964601 django-cast-0.2.9/docs_old/features.rst
+-rw-r--r--   0        0        0     8198 2022-12-18 08:57:34.964750 django-cast-0.2.9/docs_old/heroku.rst
+-rw-r--r--   0        0        0       28 2022-12-18 08:57:34.964818 django-cast-0.2.9/docs_old/history.rst
+-rw-r--r--   0        0        0      463 2022-12-18 08:57:34.965040 django-cast-0.2.9/docs_old/index.rst
+-rw-r--r--   0        0        0     3327 2022-12-18 08:57:34.965129 django-cast-0.2.9/docs_old/local_install.rst
+-rw-r--r--   0        0        0     6467 2022-12-18 08:57:34.965228 django-cast-0.2.9/docs_old/make.bat
+-rw-r--r--   0        0        0       49 2022-12-18 08:57:34.965298 django-cast-0.2.9/docs_old/modules.rst
+-rw-r--r--   0        0        0      926 2022-12-18 08:57:34.965380 django-cast-0.2.9/docs_old/production_services.rst
+-rw-r--r--   0        0        0       27 2022-12-18 08:57:34.965444 django-cast-0.2.9/docs_old/readme.rst
+-rw-r--r--   0        0        0     2833 2022-12-18 08:57:34.965529 django-cast-0.2.9/docs_old/templates.rst
+-rw-r--r--   0        0        0     2184 2022-12-18 08:57:34.965614 django-cast-0.2.9/docs_old/windows_install.rst
+-rw-r--r--   0        0        0        0 2022-11-09 16:01:36.234151 django-cast-0.2.9/example/example_site/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-09 16:01:36.235705 django-cast-0.2.9/example/example_site/settings/__init__.py
+-rw-r--r--   0        0        0     6931 2023-03-12 22:53:21.147806 django-cast-0.2.9/example/example_site/settings/base.py
+-rw-r--r--   0        0        0      536 2023-01-21 14:08:59.179674 django-cast-0.2.9/example/example_site/settings/dev.py
+-rw-r--r--   0        0        0      142 2023-01-21 14:08:59.179913 django-cast-0.2.9/example/example_site/settings/production.py
+-rw-r--r--   0        0        0      191 2023-01-21 14:08:59.180245 django-cast-0.2.9/example/example_site/templates/404.html
+-rw-r--r--   0        0        0      363 2023-01-21 14:08:59.180425 django-cast-0.2.9/example/example_site/templates/500.html
+-rw-r--r--   0        0        0     3440 2023-01-30 05:52:09.403254 django-cast-0.2.9/example/example_site/templates/base.html
+-rw-r--r--   0        0        0      103 2023-01-21 14:08:59.180774 django-cast-0.2.9/example/example_site/templates/pages/about.html
+-rw-r--r--   0        0        0     1820 2023-02-26 07:05:53.137212 django-cast-0.2.9/example/example_site/urls.py
+-rw-r--r--   0        0        0      406 2023-01-21 14:08:59.180960 django-cast-0.2.9/example/example_site/wsgi.py
+-rw-r--r--   0        0        0      849 2022-11-09 16:01:36.237384 django-cast-0.2.9/example/manage.py
+-rw-r--r--   0        0        0      228 2022-11-09 16:01:36.237511 django-cast-0.2.9/example/staticfiles/css/project.css
+-rw-r--r--   0        0        0      100 2022-11-09 16:01:36.237596 django-cast-0.2.9/example/staticfiles/js/project.js
+-rw-r--r--   0        0        0      249 2023-01-21 14:08:59.181336 django-cast-0.2.9/manage.py
+-rw-r--r--   0        0        0    10032 2023-03-05 21:13:19.598511 django-cast-0.2.9/notebooks/api/get_pages_from_production.ipynb
+-rw-r--r--   0        0        0    17098 2022-11-09 16:01:36.238186 django-cast-0.2.9/notebooks/audio/audio_handling.ipynb
+-rw-r--r--   0        0        0    40442 2022-11-09 16:01:36.238884 django-cast-0.2.9/notebooks/audio/chaptermarks_form.ipynb
+-rw-r--r--   0        0        0     3891 2023-01-30 05:54:18.371146 django-cast-0.2.9/notebooks/audio/file_sizes_debug.ipynb
+-rw-r--r--   0        0        0    57507 2022-11-09 16:01:36.239768 django-cast-0.2.9/notebooks/audio/read_chaptermarks_from_audio_file.ipynb
+-rw-r--r--   0        0        0   103147 2022-11-09 16:01:36.240384 django-cast-0.2.9/notebooks/debug/debug.ipynb
+-rw-r--r--   0        0        0    14276 2022-11-09 16:01:36.240722 django-cast-0.2.9/notebooks/debug/debug_add_new_post.ipynb
+-rw-r--r--   0        0        0    49103 2022-11-09 16:01:36.241164 django-cast-0.2.9/notebooks/debug/debug_blog_post_list.ipynb
+-rw-r--r--   0        0        0     4441 2022-11-09 16:01:36.241470 django-cast-0.2.9/notebooks/debug/debug_comments_templates.ipynb
+-rw-r--r--   0        0        0    12251 2022-11-09 16:01:36.241538 django-cast-0.2.9/notebooks/debug/django_upgrade_debug.ipynb
+-rw-r--r--   0        0        0     7022 2022-11-09 16:01:36.241838 django-cast-0.2.9/notebooks/debug/pagination.ipynb
+-rw-r--r--   0        0        0    20426 2022-11-09 16:01:36.242740 django-cast-0.2.9/notebooks/debug/post_get_absolute_url.ipynb
+-rw-r--r--   0        0        0     2767 2022-11-09 16:01:36.243045 django-cast-0.2.9/notebooks/debug/python_3.10_debug.ipynb
+-rw-r--r--   0        0        0    20471 2022-11-09 16:01:36.243288 django-cast-0.2.9/notebooks/debug/remove_obsolete_symlinks.ipynb
+-rw-r--r--   0        0        0     8648 2022-11-09 16:01:36.244543 django-cast-0.2.9/notebooks/debug/render_ajax.ipynb
+-rw-r--r--   0        0        0    40294 2022-11-09 16:01:36.244791 django-cast-0.2.9/notebooks/debug/sync_media_ids.ipynb
+-rw-r--r--   0        0        0    24437 2022-11-09 16:01:36.245204 django-cast-0.2.9/notebooks/debug/test_file_handling.ipynb
+-rw-r--r--   0        0        0    69718 2022-11-09 16:01:36.245680 django-cast-0.2.9/notebooks/debug/video_exploration_foo.ipynb
+-rw-r--r--   0        0        0    23357 2022-11-09 16:01:36.246283 django-cast-0.2.9/notebooks/feed/feed_structure.ipynb
+-rw-r--r--   0        0        0     1192 2023-02-06 06:19:32.679909 django-cast-0.2.9/notebooks/feed/remove_timestamped_model.ipynb
+-rw-r--r--   0        0        0     7199 2023-02-12 09:06:08.029824 django-cast-0.2.9/notebooks/image/from_pillow_to_willow.ipynb
+-rw-r--r--   0        0        0    25495 2022-11-09 16:01:36.246807 django-cast-0.2.9/notebooks/image/gallery_tests.ipynb
+-rw-r--r--   0        0        0    18572 2022-11-09 16:01:36.247244 django-cast-0.2.9/notebooks/logs/broken_access_log.ipynb
+-rw-r--r--   0        0        0    16031 2023-01-06 13:26:12.974612 django-cast-0.2.9/notebooks/moderation/2023-01-04_improve_spamfilter.ipynb
+-rw-r--r--   0        0        0  2650841 2022-12-18 09:06:19.427323 django-cast-0.2.9/notebooks/moderation/comments.json
+-rw-r--r--   0        0        0    82589 2023-01-06 13:26:12.975656 django-cast-0.2.9/notebooks/moderation/comments_api_endpoint_debug.ipynb
+lrwxr-xr-x   0        0        0        0 2022-11-09 16:01:36.248969 django-cast-0.2.9/notebooks/moderation/example_site -> ../../example/example_site
+-rw-r--r--   0        0        0    12907 2022-12-18 09:06:19.427938 django-cast-0.2.9/notebooks/moderation/get_comments_from_production.ipynb
+-rw-r--r--   0        0        0    26385 2022-12-18 09:06:19.428278 django-cast-0.2.9/notebooks/moderation/moderation_debug.ipynb
+-rw-r--r--   0        0        0    53189 2023-01-06 13:26:12.976288 django-cast-0.2.9/notebooks/moderation/naive_bayes.ipynb
+-rw-r--r--   0        0        0    50435 2022-11-09 16:01:36.250271 django-cast-0.2.9/notebooks/moderation/naive_bayes_class.ipynb
+-rw-r--r--   0        0        0    44598 2022-11-09 16:01:36.250570 django-cast-0.2.9/notebooks/moderation/naive_bayes_from_scratch.ipynb
+-rw-r--r--   0        0        0     7256 2022-11-09 16:01:36.250816 django-cast-0.2.9/notebooks/moderation/sms_dataset_to_messages.ipynb
+-rw-r--r--   0        0        0   112037 2022-11-09 16:01:36.251491 django-cast-0.2.9/notebooks/moderation/spamfilter.ipynb
+-rw-r--r--   0        0        0     9070 2022-12-18 09:06:19.428532 django-cast-0.2.9/notebooks/moderation/spamfilter_on_comments_from_db.ipynb
+-rw-r--r--   0        0        0    58099 2022-11-09 16:01:36.252159 django-cast-0.2.9/notebooks/offtopic/dice.ipynb
+-rw-r--r--   0        0        0    45371 2022-11-09 16:01:36.252482 django-cast-0.2.9/notebooks/search/faceted_navigation_debug.ipynb
+-rw-r--r--   0        0        0     1116 2023-01-30 05:54:18.374803 django-cast-0.2.9/notebooks/twitter/player_card.ipynb
+-rw-r--r--   0        0        0    35881 2023-02-06 06:19:32.677260 django-cast-0.2.9/notebooks/twitter/twitter_player_card.ipynb
+-rw-r--r--   0        0        0     4186 2022-11-09 16:01:36.252915 django-cast-0.2.9/notebooks/wagtail/add_child_debug.ipynb
+-rw-r--r--   0        0        0     1981 2023-02-26 08:29:28.223287 django-cast-0.2.9/notebooks/wagtail/api.ipynb
+-rw-r--r--   0        0        0     3420 2023-01-15 12:33:49.375233 django-cast-0.2.9/notebooks/wagtail/code_block.ipynb
+-rw-r--r--   0        0        0    16573 2023-03-05 21:13:19.594358 django-cast-0.2.9/notebooks/wagtail/create_content_wagtail.ipynb
+-rw-r--r--   0        0        0    24960 2022-11-20 05:04:31.320939 django-cast-0.2.9/notebooks/wagtail/missing_audio.ipynb
+-rw-r--r--   0        0        0    17008 2023-03-05 21:13:19.606083 django-cast-0.2.9/notebooks/wagtail/split_post_into_post_and_episode.ipynb
+-rw-r--r--   0        0        0    22262 2023-03-12 22:53:21.148142 django-cast-0.2.9/notebooks/wagtail/template_settings.ipynb
+-rw-r--r--   0        0        0   165131 2022-11-09 16:01:36.253921 django-cast-0.2.9/notebooks/wagtail/test_wagtail_views.ipynb
+-rw-r--r--   0        0        0     9095 2023-01-30 05:20:09.492195 django-cast-0.2.9/notebooks/wagtail/wagtail_get_descendants_of_page_statements.ipynb
+-rw-r--r--   0        0        0    25477 2023-01-06 13:26:12.976885 django-cast-0.2.9/notebooks/wagtail/wagtail_render_post.ipynb
+-rw-r--r--   0        0        0    53276 2022-11-09 16:01:36.255073 django-cast-0.2.9/notebooks/wagtail/wagtail_video_views.ipynb
+-rw-r--r--   0        0        0     3122 2023-03-20 06:09:43.201483 django-cast-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      286 2020-12-14 06:01:37.766654 django-cast-0.2.9/release.txt
+-rw-r--r--   0        0        0      699 2023-01-21 14:08:59.181997 django-cast-0.2.9/runtests.py
+-rw-r--r--   0        0        0      717 2022-12-18 08:57:34.967158 django-cast-0.2.9/setup.cfg
+-rw-r--r--   0        0        0        0 2020-12-14 06:01:37.766864 django-cast-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-02-12 09:06:05.621645 django-cast-0.2.9/tests/admin_test.py
+-rw-r--r--   0        0        0     6841 2023-02-12 09:06:05.621967 django-cast-0.2.9/tests/api_test.py
+-rw-r--r--   0        0        0      692 2023-02-12 09:06:05.622219 django-cast-0.2.9/tests/apps_test.py
+-rw-r--r--   0        0        0    10881 2023-02-12 09:06:05.622532 django-cast-0.2.9/tests/audio_models_test.py
+-rw-r--r--   0        0        0    14880 2023-02-12 09:06:05.622857 django-cast-0.2.9/tests/audio_views_test.py
+-rw-r--r--   0        0        0      984 2023-01-30 05:52:09.405779 django-cast-0.2.9/tests/blocks_test.py
+-rw-r--r--   0        0        0     6990 2023-03-20 06:09:43.201793 django-cast-0.2.9/tests/blog_index_test.py
+-rw-r--r--   0        0        0        0 2023-01-30 05:52:09.406006 django-cast-0.2.9/tests/cast/static/.gitkeep
+-rw-r--r--   0        0        0     4871 2023-02-14 21:21:43.460183 django-cast-0.2.9/tests/comments_test.py
+-rw-r--r--   0        0        0    14597 2023-02-12 09:06:05.623164 django-cast-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0      832 2023-01-30 05:52:09.406659 django-cast-0.2.9/tests/episode_detail_test.py
+-rw-r--r--   0        0        0     1954 2023-02-12 09:06:05.623460 django-cast-0.2.9/tests/factories.py
+-rw-r--r--   0        0        0     6609 2023-02-23 17:07:56.455208 django-cast-0.2.9/tests/feed_test.py
+-rw-r--r--   0        0        0     1149 2023-03-20 06:09:43.202602 django-cast-0.2.9/tests/filter_test.py
+-rw-r--r--   0        0        0      526 2020-12-14 06:01:37.767120 django-cast-0.2.9/tests/fixtures/access.log
+-rw-r--r--   0        0        0     6824 2020-12-14 06:01:37.767199 django-cast-0.2.9/tests/fixtures/test.m4a
+-rw-r--r--   0        0        0      262 2020-12-14 06:01:37.767245 django-cast-0.2.9/tests/fixtures/test.mp4
+-rw-r--r--   0        0        0     4476 2023-02-12 09:06:05.624347 django-cast-0.2.9/tests/forms_test.py
+-rw-r--r--   0        0        0      331 2023-02-12 09:06:05.624566 django-cast-0.2.9/tests/meta_test.py
+-rw-r--r--   0        0        0      435 2023-01-30 05:52:09.407251 django-cast-0.2.9/tests/meta_views_test.py
+-rw-r--r--   0        0        0     7010 2023-03-20 06:09:43.202882 django-cast-0.2.9/tests/models_test.py
+-rw-r--r--   0        0        0     5971 2023-02-12 09:06:05.625193 django-cast-0.2.9/tests/moderation_test.py
+-rw-r--r--   0        0        0     1981 2023-03-20 06:09:43.203179 django-cast-0.2.9/tests/pagination_test.py
+-rw-r--r--   0        0        0     6363 2023-01-30 05:52:09.407682 django-cast-0.2.9/tests/post_add_test.py
+-rw-r--r--   0        0        0      935 2023-01-30 05:52:09.407773 django-cast-0.2.9/tests/post_detail_test.py
+-rw-r--r--   0        0        0     2467 2023-01-30 05:52:09.407881 django-cast-0.2.9/tests/post_media_sync_test.py
+-rw-r--r--   0        0        0      796 2023-02-06 06:19:29.752992 django-cast-0.2.9/tests/post_published_test.py
+-rw-r--r--   0        0        0     5714 2023-03-12 22:53:21.148717 django-cast-0.2.9/tests/settings.py
+-rw-r--r--   0        0        0     3122 2023-03-20 06:09:43.203524 django-cast-0.2.9/tests/theme_test.py
+-rw-r--r--   0        0        0     1792 2023-01-30 05:52:09.408523 django-cast-0.2.9/tests/upload_handler_test.py
+-rw-r--r--   0        0        0      748 2023-02-26 07:05:53.138104 django-cast-0.2.9/tests/urls.py
+-rw-r--r--   0        0        0      447 2023-01-30 05:52:09.408676 django-cast-0.2.9/tests/utils_test.py
+-rw-r--r--   0        0        0    25531 2023-01-30 05:52:09.408915 django-cast-0.2.9/tests/video_dimensions_test.py
+-rw-r--r--   0        0        0     1343 2023-01-30 05:52:09.409123 django-cast-0.2.9/tests/video_upload_test.py
+-rw-r--r--   0        0        0    14012 2023-02-12 09:06:05.625996 django-cast-0.2.9/tests/video_views_test.py
+-rw-r--r--   0        0        0      483 2023-02-07 18:43:34.635097 django-cast-0.2.9/tests/wagtail_image_views_test.py
+-rw-r--r--   0        0        0     1117 2023-02-12 09:06:05.626238 django-cast-0.2.9/tests/widget_test.py
+-rw-r--r--   0        0        0      256 2023-01-30 05:52:09.409560 django-cast-0.2.9/tox.ini
+-rw-r--r--   0        0        0     2706 1970-01-01 00:00:00.000000 django-cast-0.2.9/PKG-INFO
```

### Comparing `django-cast-0.2.8/.github/workflows/workflow.yml` & `django-cast-0.2.9/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/.gitignore` & `django-cast-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/.pre-commit-config.yaml` & `django-cast-0.2.9/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -32,20 +32,20 @@
   - repo: https://github.com/PyCQA/flake8
     # flake8 config is in setup.cfg
     rev: 6.0.0
     hooks:
       - id: flake8
         language_version: python3
   - repo: https://github.com/rtts/djhtml
-    rev: "v2.0.0"  # replace with the latest tag on GitHub
+    rev: "3.0.6"  # replace with the latest tag on GitHub
     hooks:
       - id: djhtml
         args: [-t, "2"]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.0.1'  # Use the sha / tag you want to point at
+    rev: 'v1.1.1'  # Use the sha / tag you want to point at
     hooks:
       - id: mypy
         exclude: "[a-zA-Z]*/(migrations)|(docs)|(example)/(.)*"
         args: [--no-strict-optional,
                --ignore-missing-imports]
         additional_dependencies:
           - crispy_bootstrap4
```

### Comparing `django-cast-0.2.8/CONTRIBUTING.rst` & `django-cast-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/LICENSE` & `django-cast-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/README.md` & `django-cast-0.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![name](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ephes/django-cast)
 
 A blogging/podcasting package based on [Django](https://www.djangoproject.com/)
 and [Wagtail](https://wagtail.org).
 
 After switching to Wagtail, the documentation has to be updated. Stay tuned 😄.
 
-**Documentation for [current version 0.2.8](https://django-cast.readthedocs.io/en/develop/)**
+**Documentation for [current version 0.2.9](https://django-cast.readthedocs.io/en/develop/)**
 
 ## Key Features
 - Responsive images via [wagtail-srcset](https://github.com/ephes/wagtail_srcset)
 - Wagtail as CMS makes it possible for non-technical people to manage the content
   (blog posts, podcast episodes, ...)
 - Podcast support: this package powers [python-podcast.de](https://python-podcast.de/show)
   since 2018 using the [Podlove Web Player](https://podlove.org/podlove-web-player/)
```

### Comparing `django-cast-0.2.8/README_OLD.rst` & `django-cast-0.2.9/README_OLD.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/bootstrap.md` & `django-cast-0.2.9/bootstrap.md`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/admin.py` & `django-cast-0.2.9/cast/admin.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/admin_urls/audio.py` & `django-cast-0.2.9/cast/admin_urls/audio.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/admin_urls/video.py` & `django-cast-0.2.9/cast/admin_urls/video.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/api/serializers.py` & `django-cast-0.2.9/cast/api/serializers.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/api/urls.py` & `django-cast-0.2.9/cast/api/urls.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/api/viewmixins.py` & `django-cast-0.2.9/cast/api/viewmixins.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/api/views.py` & `django-cast-0.2.9/cast/api/views.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/apps.py` & `django-cast-0.2.9/cast/apps.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/blocks.py` & `django-cast-0.2.9/cast/blocks.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/feeds.py` & `django-cast-0.2.9/cast/feeds.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/filters.py` & `django-cast-0.2.9/cast/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from django.db.models.functions import TruncMonth
 from django.forms import Field, Widget
 from django.forms.renderers import BaseRenderer
 from django.forms.utils import flatatt
 from django.http import QueryDict
 from django.utils.datastructures import MultiValueDict
 from django.utils.encoding import force_str
-from django.utils.http import urlencode
 from django.utils.safestring import SafeText, mark_safe
 from django.utils.translation import gettext as _
 from wagtail.models import PageQuerySet
 
 
 class DateFacetWidget(Widget):
     data: QueryDict
@@ -59,21 +58,24 @@
                 output.append(self.render_option(name, selected_choices_set, option_value, option_label))
         return "\n".join(output)
 
     def render_option(self, name: str, selected_choices: set[str], option_value: str, option_label: str) -> str:
         option_value = force_str(option_value)
         if option_label == BLANK_CHOICE_DASH[0][1]:
             option_label = _("All")
-        data = self.data.copy()
+
+        # remove page from querystring, because otherwise the pagination breaks
+        # filters like date facets, str to make mypy happy
+        data_dict = {k: str(v) for k, v in self.data.items() if k != "page"}
+        data = QueryDict("", mutable=True)
+        data.update(data_dict)
+
         data[name] = option_value
         selected = data == self.data or option_value in selected_choices
-        try:
-            url = data.urlencode()
-        except AttributeError:
-            url = urlencode(data)
+        url = data.urlencode()
         option_string = self.option_string()
         return option_string % {
             "attrs": selected and ' class="selected"' or "",
             "query_string": url,
             "label": force_str(option_label),
         }
```

### Comparing `django-cast-0.2.8/cast/forms.py` & `django-cast-0.2.9/cast/forms.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/locale/de/LC_MESSAGES/django.po` & `django-cast-0.2.9/cast/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/.DS_Store` & `django-cast-0.2.9/cast/management/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/.s3_stale.py.swp` & `django-cast-0.2.9/cast/management/commands/.s3_stale.py.swp`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/get_api_token.py` & `django-cast-0.2.9/cast/management/commands/get_api_token.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/s3_backup.py` & `django-cast-0.2.9/cast/management/commands/s3_backup.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/s3_media_sizes.py` & `django-cast-0.2.9/cast/management/commands/s3_media_sizes.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/s3_replace.py` & `django-cast-0.2.9/cast/management/commands/s3_replace.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/s3_restore.py` & `django-cast-0.2.9/cast/management/commands/s3_restore.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/management/commands/s3_stale.py` & `django-cast-0.2.9/cast/management/commands/s3_stale.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0001_initial.py` & `django-cast-0.2.9/cast/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0004_homepage_alias_for_page.py` & `django-cast-0.2.9/cast/migrations/0004_homepage_alias_for_page.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0005_auto_20201024_0613.py` & `django-cast-0.2.9/cast/migrations/0005_auto_20201024_0613.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0006_auto_20210628_1628.py` & `django-cast-0.2.9/cast/migrations/0006_auto_20210628_1628.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0007_alter_post_body.py` & `django-cast-0.2.9/cast/migrations/0007_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0008_auto_20210712_0919.py` & `django-cast-0.2.9/cast/migrations/0008_auto_20210712_0919.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0009_alter_post_body.py` & `django-cast-0.2.9/cast/migrations/0009_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0011_alter_post_body.py` & `django-cast-0.2.9/cast/migrations/0011_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0016_auto_20210830_0422.py` & `django-cast-0.2.9/cast/migrations/0016_auto_20210830_0422.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0017_alter_post_body.py` & `django-cast-0.2.9/cast/migrations/0017_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0020_auto_20210926_1556.py` & `django-cast-0.2.9/cast/migrations/0020_auto_20210926_1556.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0021_spamfilter.py` & `django-cast-0.2.9/cast/migrations/0021_spamfilter.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0022_alter_spamfilter_model.py` & `django-cast-0.2.9/cast/migrations/0022_alter_spamfilter_model.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0023_alter_spamfilter_model.py` & `django-cast-0.2.9/cast/migrations/0023_alter_spamfilter_model.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0024_alter_homepage_body_alter_post_body.py` & `django-cast-0.2.9/cast/migrations/0024_alter_homepage_body_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0026_delete_request_alter_post_body.py` & `django-cast-0.2.9/cast/migrations/0026_delete_request_alter_post_body.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0027_episode.py` & `django-cast-0.2.9/cast/migrations/0027_episode.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0028_rename_and_drop_itune_fields.py` & `django-cast-0.2.9/cast/migrations/0028_rename_and_drop_itune_fields.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0033_add_new_podcast_model.py` & `django-cast-0.2.9/cast/migrations/0033_add_new_podcast_model.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0034_remove_old_podcast_fields_from_blog.py` & `django-cast-0.2.9/cast/migrations/0034_remove_old_podcast_fields_from_blog.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0035_remove_new_prefix_podcast_fields.py` & `django-cast-0.2.9/cast/migrations/0035_remove_new_prefix_podcast_fields.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0036_alter_blog_author.py` & `django-cast-0.2.9/cast/migrations/0036_alter_blog_author.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0037_alter_episode_block_alter_episode_explicit_and_more.py` & `django-cast-0.2.9/cast/migrations/0037_alter_episode_block_alter_episode_explicit_and_more.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0038_alter_episode_keywords.py` & `django-cast-0.2.9/cast/migrations/0038_alter_episode_keywords.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0039_blog_noindex.py` & `django-cast-0.2.9/cast/migrations/0039_blog_noindex.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0040_alter_blog_noindex.py` & `django-cast-0.2.9/cast/migrations/0040_alter_blog_noindex.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0041_templatebasedirectory.py` & `django-cast-0.2.9/cast/migrations/0041_templatebasedirectory.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0043_alter_blog_template_base_dir.py` & `django-cast-0.2.9/cast/migrations/0043_alter_blog_template_base_dir.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/migrations/0044_alter_blog_template_base_dir_and_more.py` & `django-cast-0.2.9/cast/migrations/0044_alter_blog_template_base_dir_and_more.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/models/__init__.py` & `django-cast-0.2.9/cast/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/models/audio.py` & `django-cast-0.2.9/cast/models/audio.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/models/gallery.py` & `django-cast-0.2.9/cast/models/gallery.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/models/index_pages.py` & `django-cast-0.2.9/cast/models/index_pages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import logging
 import uuid
-from typing import Any, Optional, cast
+from datetime import datetime
+from typing import Any
 
 from django.core.paginator import InvalidPage, Paginator
 from django.db import models
 from django.http import Http404, HttpRequest
 from django.http.request import QueryDict
-from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
 from wagtail.admin.panels import FieldPanel
 from wagtail.fields import RichTextField
 from wagtail.models import Page, PageManager
 
 from cast import appsettings
 from cast.filters import PostFilterset
@@ -90,72 +90,49 @@
 
     def get_template(self, request: HttpRequest, *args, **kwargs) -> str:
         template_base_dir = self.get_template_base_dir(request)
         template = f"cast/{template_base_dir}/blog_list_of_posts.html"
         return template
 
     @property
-    def last_build_date(self) -> timezone.datetime:
+    def last_build_date(self) -> datetime:
         return Post.objects.live().descendant_of(self.blog).order_by("-visible_date")[0].visible_date
 
     @property
     def author_name(self) -> str:
         if self.author is not None:
             return self.author
         else:
             return self.owner.get_full_name()
 
     @property
     def unfiltered_published_posts(self) -> models.QuerySet[Post]:
         return Post.objects.live().descendant_of(self).order_by("-visible_date")
 
-    @property
-    def request(self) -> Optional[HttpRequest]:
-        return getattr(self, "_request", None)
-
-    @request.setter
-    def request(self, value: HttpRequest) -> None:
-        self._request = value
-
-    @property
-    def filterset_data(self) -> QueryDict:
-        if self.request is not None:
-            return self.request.GET.copy()
-        else:
-            filterset_data = getattr(self, "_filterset_data", None)
-            if filterset_data is None:
-                return QueryDict()
-            else:
-                filterset_data_as_querydict = cast(QueryDict, filterset_data)  # make mypy happy
-                return filterset_data_as_querydict
+    def get_filterset(self, get_params: QueryDict) -> PostFilterset:
+        return PostFilterset(data=get_params, queryset=self.unfiltered_published_posts, fetch_facet_counts=True)
 
-    @property
-    def filterset(self) -> PostFilterset:
-        return PostFilterset(
-            data=self.filterset_data, queryset=self.unfiltered_published_posts, fetch_facet_counts=True
-        )
-
-    @property
-    def published_posts(self) -> models.QuerySet[Post]:
-        queryset = self.filterset.qs
+    @staticmethod
+    def get_published_posts(filtered_posts: models.QuerySet) -> models.QuerySet[Post]:
+        queryset = filtered_posts
         queryset = (
             queryset.prefetch_related("audios")
             .prefetch_related("images")
             .prefetch_related("videos")
             .prefetch_related("galleries")
             .select_related("owner")
         )
         return queryset
 
-    def paginate_queryset(self, context: ContextDict) -> ContextDict:
-        paginator = Paginator(self.published_posts, appsettings.POST_LIST_PAGINATION)
+    @staticmethod
+    def paginate_queryset(context: ContextDict, posts_queryset: models.QuerySet, get_params: QueryDict) -> ContextDict:
+        paginator = Paginator(posts_queryset, appsettings.POST_LIST_PAGINATION)
         page_from_url = "1"
-        if self.request is not None:
-            if "page" in self.request.GET:
-                page_from_url = self.request.GET["page"]
+        if "page" in get_params:
+            page_from_url = str(get_params["page"])
         try:
             page_number = int(page_from_url)
         except ValueError:
             if page_from_url == "last":
                 page_number = paginator.num_pages
             else:
                 raise Http404(_("Page is not “last”, nor can it be converted to an int."))
@@ -171,33 +148,32 @@
             "is_paginated": page.has_other_pages(),
             "object_list": page.object_list,
             "page_range": page.paginator.get_elided_page_range(page.number, on_each_side=2, on_ends=1),  # type: ignore
         }
         context.update(pagination_context)
         return context
 
-    def get_other_get_params(self) -> str:
-        if self.request is None:
-            return ""
-        get_copy = self.request.GET.copy()
-        parameters = get_copy.pop("page", "") and get_copy.urlencode()
+    @staticmethod
+    def get_other_get_params(get_params: QueryDict) -> str:
+        filtered_get_params = {k: str(v) for k, v in get_params.items() if k != "page"}
+        new_get_params = QueryDict("", mutable=True)
+        new_get_params.update(filtered_get_params)
+        parameters = new_get_params.urlencode()
         if len(parameters) > 0:
             parameters = f"&{parameters}"
         return parameters
 
     def get_context(self, request: HttpRequest, *args, **kwargs) -> ContextDict:
         context = super().get_context(request, *args, **kwargs)
-        self.request = request
-        context["filterset"] = kwargs.get("filterset", self.filterset)
-        context["parameters"] = self.get_other_get_params()
-        context = self.paginate_queryset(context)
+        get_params = request.GET.copy()
+        context["filterset"] = filterset = self.get_filterset(get_params)
+        context["parameters"] = self.get_other_get_params(get_params)
+        context = self.paginate_queryset(context, self.get_published_posts(filterset.qs), get_params)
         context["posts"] = context["object_list"]  # convenience
         context["blog"] = self
-        template_base_dir = TemplateBaseDirectory.for_request(request)
-        print("template_settings base dir: ", template_base_dir.name)
         return context
 
 
 class Podcast(Blog):
     # atm it's only used for podcast image
     itunes_artwork = models.ForeignKey(ItunesArtWork, null=True, blank=True, on_delete=models.SET_NULL)
     itunes_categories = models.CharField(
```

### Comparing `django-cast-0.2.8/cast/models/moderation.py` & `django-cast-0.2.9/cast/models/moderation.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/models/pages.py` & `django-cast-0.2.9/cast/models/pages.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/models/theme.py` & `django-cast-0.2.9/cast/models/theme.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pathlib import Path
 
+from django.conf import settings
 from django.db import models
 from django.template import engines
 from django.template.loaders.base import Loader as BaseLoader
 from django.utils.translation import gettext_lazy as _
 from wagtail.contrib.settings.models import BaseSiteSetting, register_setting
 
 
@@ -80,24 +81,30 @@
 
 
 def get_template_base_dir_choices() -> list[tuple[str, str]]:
     """
     Return a list of choices for the template base directory setting.
     """
     # handle predefined choices
-    choices, predefined = [], set()
+    choices, seen = [], set()
     for template_name in TemplateName:
         choices.append((template_name.value, template_name.label))
-        predefined.add(template_name.value)
+        seen.add(template_name.value)
+
+    # handle custom choices via settings
+    for template_name, display_name in getattr(settings, "CAST_CUSTOM_THEMES", []):
+        if template_name not in seen:
+            choices.append((template_name, display_name))
+            seen.add(template_name)
 
     # search for template base directories
     template_directories = get_template_directories()
     template_base_dir_candidates = get_template_base_dir_candidates(template_directories)
     for candidate in template_base_dir_candidates:
-        if candidate not in predefined:
+        if candidate not in seen:
             choices.append((candidate, candidate))
 
     return choices
 
 
 @register_setting
 class TemplateBaseDirectory(BaseSiteSetting):
```

### Comparing `django-cast-0.2.8/cast/models/video.py` & `django-cast-0.2.9/cast/models/video.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/moderation.py` & `django-cast-0.2.9/cast/moderation.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/runner.py` & `django-cast-0.2.9/cast/runner.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/settings.py` & `django-cast-0.2.9/cast/settings.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/css/cast.css` & `django-cast-0.2.9/cast/static/css/cast.css`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/img/cast/Audio-icon.svg` & `django-cast-0.2.9/cast/static/img/cast/Audio-icon.svg`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/img/cast/Feed-icon.svg` & `django-cast-0.2.9/cast/static/img/cast/Feed-icon.svg`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/img/cast/Video-icon.svg` & `django-cast-0.2.9/cast/static/img/cast/Video-icon.svg`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/gallery.js` & `django-cast-0.2.9/cast/static/js/cast/gallery.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/wagtail/audio-chooser-modal.js` & `django-cast-0.2.9/cast/static/js/cast/wagtail/audio-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/wagtail/audio-chooser-telepath.js` & `django-cast-0.2.9/cast/static/js/cast/wagtail/audio-chooser-telepath.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/wagtail/audio-chooser.js` & `django-cast-0.2.9/cast/static/js/cast/wagtail/audio-chooser.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/wagtail/video-chooser-modal.js` & `django-cast-0.2.9/cast/static/js/cast/wagtail/video-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/wagtail/video-chooser-telepath.js` & `django-cast-0.2.9/cast/static/js/cast/wagtail/video-chooser-telepath.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/wagtail/video-chooser.js` & `django-cast-0.2.9/cast/static/js/cast/wagtail/video-chooser.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/web-player/embed.4.js` & `django-cast-0.2.9/cast/static/js/cast/web-player/embed.4.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/static/js/cast/web-player/embed.5.js` & `django-cast-0.2.9/cast/static/js/cast/web-player/embed.5.js`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/.DS_Store` & `django-cast-0.2.9/cast/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/base.html` & `django-cast-0.2.9/cast/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/add.html` & `django-cast-0.2.9/cast/templates/cast/audio/add.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/chooser_chooser.html` & `django-cast-0.2.9/cast/templates/cast/audio/chooser_chooser.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/chooser_results.html` & `django-cast-0.2.9/cast/templates/cast/audio/chooser_results.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/confirm_delete.html` & `django-cast-0.2.9/cast/templates/cast/audio/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/edit.html` & `django-cast-0.2.9/cast/templates/cast/audio/edit.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/index.html` & `django-cast-0.2.9/cast/templates/cast/audio/index.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/list.html` & `django-cast-0.2.9/cast/templates/cast/audio/list.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/audio/results.html` & `django-cast-0.2.9/cast/templates/cast/audio/results.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/base.html` & `django-cast-0.2.9/cast/templates/cast/base.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/bootstrap4/blog_list_of_posts.html` & `django-cast-0.2.9/cast/templates/cast/bootstrap4/blog_list_of_posts.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "./cast_base.html" %}
+{% extends "./base.html" %}
 {% load wagtailcore_tags %}
 {% load crispy_forms_tags %}
 {% load static %}
 
 {% block body_class %}template-bloglistpage{% endblock %}
 
 {% block meta %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "./cast_base.html" %} {% load wagtailcore_tags %} {% load
+{% extends "./base.html" %} {% load wagtailcore_tags %} {% load
 crispy_forms_tags %} {% load static %} {% block body_class %}template-
 bloglistpage{% endblock %} {% block meta %} {{ block.super }} {% if
 blog.noindex %}
  {% endif %} {% endblock %} {% block content %}
 ****** {{ page.title }} ******
 {{ page.description|richtext }}
 {% block feeds %}
```

### Comparing `django-cast-0.2.8/cast/templates/cast/bootstrap4/pagination.html` & `django-cast-0.2.9/cast/templates/cast/bootstrap4/pagination.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/bootstrap4/post.html` & `django-cast-0.2.9/cast/templates/cast/bootstrap4/post.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends "./cast_base.html" %}
+{% extends "./base.html" %}
 {% load i18n %}
 {% load static %}
 
 {% load wagtailcore_tags %}
 {% load wagtailimages_tags %}
 {% load wagtail_srcset_tags %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends "./cast_base.html" %} {% load i18n %} {% load static %} {% load
+{% extends "./base.html" %} {% load i18n %} {% load static %} {% load
 wagtailcore_tags %} {% load wagtailimages_tags %} {% load wagtail_srcset_tags
 %} {% if page.comments_enabled %} {% load comments %} {% endif %} {% block css
 %} {{ block.super }} {% if page.comments_are_enabled %}
  {% endif %} {% endblock css %} {% block meta %} {{ block.super }} {% if
 page.blog.noindex %}
  {% endif %} {% endblock %} {% block body_class %}template-blogpage{% endblock
 %} {% block title %}{{ page.title }}{% endblock title %} {% block content %} {%
```

### Comparing `django-cast-0.2.8/cast/templates/cast/bootstrap4/post_body.html` & `django-cast-0.2.9/cast/templates/cast/bootstrap4/post_body.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/gallery.html` & `django-cast-0.2.9/cast/templates/cast/gallery.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/plain/base.html` & `django-cast-0.2.9/cast/templates/cast/plain/base.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/plain/blog_list_of_posts.html` & `django-cast-0.2.9/cast/templates/cast/plain/blog_list_of_posts.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/plain/post.html` & `django-cast-0.2.9/cast/templates/cast/plain/post.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/plain/post_body.html` & `django-cast-0.2.9/cast/templates/cast/plain/post_body.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/twitter/card_player.html` & `django-cast-0.2.9/cast/templates/cast/twitter/card_player.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/add.html` & `django-cast-0.2.9/cast/templates/cast/video/add.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/chooser_chooser.html` & `django-cast-0.2.9/cast/templates/cast/video/chooser_chooser.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/chooser_results.html` & `django-cast-0.2.9/cast/templates/cast/video/chooser_results.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/confirm_delete.html` & `django-cast-0.2.9/cast/templates/cast/video/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/edit.html` & `django-cast-0.2.9/cast/templates/cast/video/edit.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/index.html` & `django-cast-0.2.9/cast/templates/cast/video/index.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/list.html` & `django-cast-0.2.9/cast/templates/cast/video/list.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/cast/video/results.html` & `django-cast-0.2.9/cast/templates/cast/video/results.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/comments/comment.html` & `django-cast-0.2.9/cast/templates/comments/comment.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/templates/pagination.html` & `django-cast-0.2.9/cast/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/urls.py` & `django-cast-0.2.9/cast/urls.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/views/audio.py` & `django-cast-0.2.9/cast/views/audio.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/views/meta.py` & `django-cast-0.2.9/cast/views/meta.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/views/video.py` & `django-cast-0.2.9/cast/views/video.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/wagtail_hooks.py` & `django-cast-0.2.9/cast/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/cast/widgets.py` & `django-cast-0.2.9/cast/widgets.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/commands.py` & `django-cast-0.2.9/commands.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/Makefile` & `django-cast-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/conf.py` & `django-cast-0.2.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "Django Cast"
 copyright = "2022, Jochen Wersdörfer"
 author = "Jochen Wersdörfer"
-release = "0.2.8"
+release = "0.2.9"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ["_templates"]
```

### Comparing `django-cast-0.2.8/docs/howto/index.rst` & `django-cast-0.2.9/docs/howto/index.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/images/blog_template_base_dir_setting.png` & `django-cast-0.2.9/docs/images/blog_template_base_dir_setting.png`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/images/cache_file_sizes_admin_action.png` & `django-cast-0.2.9/docs/images/cache_file_sizes_admin_action.png`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/images/spam_filter_performance.png` & `django-cast-0.2.9/docs/images/spam_filter_performance.png`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/images/template_base_dir_setting.png` & `django-cast-0.2.9/docs/images/template_base_dir_setting.png`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/images/twitter_card.png` & `django-cast-0.2.9/docs/images/twitter_card.png`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/make.bat` & `django-cast-0.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/models.rst` & `django-cast-0.2.9/docs/models.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/release.rst` & `django-cast-0.2.9/docs/release.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/releases/0.1/0.1.28.rst` & `django-cast-0.2.9/docs/releases/0.1/0.1.28.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/releases/0.1/0.1.6.rst` & `django-cast-0.2.9/docs/releases/0.1/0.1.6.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/releases/0.2.3.rst` & `django-cast-0.2.9/docs/releases/0.2.3.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/releases/index.rst` & `django-cast-0.2.9/docs/releases/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Versions
 ========
 
 .. toctree::
    :maxdepth: 1
 
+   0.2.9
    0.2.8
    0.2.7
    0.2.6
    0.2.5
    0.2.4
    0.2.3
    0.2.2
```

### Comparing `django-cast-0.2.8/docs/social-media.rst` & `django-cast-0.2.9/docs/social-media.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/spamfilter.rst` & `django-cast-0.2.9/docs/spamfilter.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs/tests.rst` & `django-cast-0.2.9/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/Makefile` & `django-cast-0.2.9/docs_old/Makefile`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/analytics.rst` & `django-cast-0.2.9/docs_old/analytics.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/cast.api.rst` & `django-cast-0.2.9/docs_old/cast.api.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/cast.migrations.rst` & `django-cast-0.2.9/docs_old/cast.migrations.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/cast.rst` & `django-cast-0.2.9/docs_old/cast.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/cdn.rst` & `django-cast-0.2.9/docs_old/cdn.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/comments.rst` & `django-cast-0.2.9/docs_old/comments.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/conf.py` & `django-cast-0.2.9/docs_old/conf.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/content.rst` & `django-cast-0.2.9/docs_old/content.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/ec2_install.rst` & `django-cast-0.2.9/docs_old/ec2_install.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/heroku.rst` & `django-cast-0.2.9/docs_old/heroku.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/local_install.rst` & `django-cast-0.2.9/docs_old/local_install.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/make.bat` & `django-cast-0.2.9/docs_old/make.bat`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/production_services.rst` & `django-cast-0.2.9/docs_old/production_services.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/templates.rst` & `django-cast-0.2.9/docs_old/templates.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/docs_old/windows_install.rst` & `django-cast-0.2.9/docs_old/windows_install.rst`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/example/example_site/settings/base.py` & `django-cast-0.2.9/example/example_site/settings/base.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/example/example_site/settings/dev.py` & `django-cast-0.2.9/example/example_site/settings/dev.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/example/example_site/templates/base.html` & `django-cast-0.2.9/example/example_site/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/example/example_site/urls.py` & `django-cast-0.2.9/example/example_site/urls.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/example/manage.py` & `django-cast-0.2.9/example/manage.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/api/get_pages_from_production.ipynb` & `django-cast-0.2.9/notebooks/api/get_pages_from_production.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/audio/audio_handling.ipynb` & `django-cast-0.2.9/notebooks/audio/audio_handling.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/audio/chaptermarks_form.ipynb` & `django-cast-0.2.9/notebooks/audio/chaptermarks_form.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/audio/file_sizes_debug.ipynb` & `django-cast-0.2.9/notebooks/audio/file_sizes_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/audio/read_chaptermarks_from_audio_file.ipynb` & `django-cast-0.2.9/notebooks/audio/read_chaptermarks_from_audio_file.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/debug.ipynb` & `django-cast-0.2.9/notebooks/debug/debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/debug_add_new_post.ipynb` & `django-cast-0.2.9/notebooks/debug/debug_add_new_post.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/debug_blog_post_list.ipynb` & `django-cast-0.2.9/notebooks/debug/debug_blog_post_list.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/debug_comments_templates.ipynb` & `django-cast-0.2.9/notebooks/debug/debug_comments_templates.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/django_upgrade_debug.ipynb` & `django-cast-0.2.9/notebooks/debug/django_upgrade_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/pagination.ipynb` & `django-cast-0.2.9/notebooks/debug/pagination.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/post_get_absolute_url.ipynb` & `django-cast-0.2.9/notebooks/debug/post_get_absolute_url.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/python_3.10_debug.ipynb` & `django-cast-0.2.9/notebooks/debug/python_3.10_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/remove_obsolete_symlinks.ipynb` & `django-cast-0.2.9/notebooks/debug/remove_obsolete_symlinks.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/render_ajax.ipynb` & `django-cast-0.2.9/notebooks/debug/render_ajax.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/sync_media_ids.ipynb` & `django-cast-0.2.9/notebooks/debug/sync_media_ids.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/test_file_handling.ipynb` & `django-cast-0.2.9/notebooks/debug/test_file_handling.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/debug/video_exploration_foo.ipynb` & `django-cast-0.2.9/notebooks/debug/video_exploration_foo.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/feed/feed_structure.ipynb` & `django-cast-0.2.9/notebooks/feed/feed_structure.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/feed/remove_timestamped_model.ipynb` & `django-cast-0.2.9/notebooks/feed/remove_timestamped_model.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/image/from_pillow_to_willow.ipynb` & `django-cast-0.2.9/notebooks/image/from_pillow_to_willow.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/image/gallery_tests.ipynb` & `django-cast-0.2.9/notebooks/image/gallery_tests.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/logs/broken_access_log.ipynb` & `django-cast-0.2.9/notebooks/logs/broken_access_log.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/2023-01-04_improve_spamfilter.ipynb` & `django-cast-0.2.9/notebooks/moderation/2023-01-04_improve_spamfilter.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/comments.json` & `django-cast-0.2.9/notebooks/moderation/comments.json`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/comments_api_endpoint_debug.ipynb` & `django-cast-0.2.9/notebooks/moderation/comments_api_endpoint_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/get_comments_from_production.ipynb` & `django-cast-0.2.9/notebooks/moderation/get_comments_from_production.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/moderation_debug.ipynb` & `django-cast-0.2.9/notebooks/moderation/moderation_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/naive_bayes.ipynb` & `django-cast-0.2.9/notebooks/moderation/naive_bayes.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/naive_bayes_class.ipynb` & `django-cast-0.2.9/notebooks/moderation/naive_bayes_class.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/naive_bayes_from_scratch.ipynb` & `django-cast-0.2.9/notebooks/moderation/naive_bayes_from_scratch.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/sms_dataset_to_messages.ipynb` & `django-cast-0.2.9/notebooks/moderation/sms_dataset_to_messages.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/spamfilter.ipynb` & `django-cast-0.2.9/notebooks/moderation/spamfilter.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/moderation/spamfilter_on_comments_from_db.ipynb` & `django-cast-0.2.9/notebooks/moderation/spamfilter_on_comments_from_db.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/offtopic/dice.ipynb` & `django-cast-0.2.9/notebooks/offtopic/dice.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/search/faceted_navigation_debug.ipynb` & `django-cast-0.2.9/notebooks/search/faceted_navigation_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/twitter/player_card.ipynb` & `django-cast-0.2.9/notebooks/twitter/player_card.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/twitter/twitter_player_card.ipynb` & `django-cast-0.2.9/notebooks/twitter/twitter_player_card.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/add_child_debug.ipynb` & `django-cast-0.2.9/notebooks/wagtail/add_child_debug.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/api.ipynb` & `django-cast-0.2.9/notebooks/wagtail/api.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/code_block.ipynb` & `django-cast-0.2.9/notebooks/wagtail/code_block.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/create_content_wagtail.ipynb` & `django-cast-0.2.9/notebooks/wagtail/create_content_wagtail.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/missing_audio.ipynb` & `django-cast-0.2.9/notebooks/wagtail/missing_audio.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/split_post_into_post_and_episode.ipynb` & `django-cast-0.2.9/notebooks/wagtail/split_post_into_post_and_episode.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/template_settings.ipynb` & `django-cast-0.2.9/notebooks/wagtail/template_settings.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/test_wagtail_views.ipynb` & `django-cast-0.2.9/notebooks/wagtail/test_wagtail_views.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/wagtail_get_descendants_of_page_statements.ipynb` & `django-cast-0.2.9/notebooks/wagtail/wagtail_get_descendants_of_page_statements.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/wagtail_render_post.ipynb` & `django-cast-0.2.9/notebooks/wagtail/wagtail_render_post.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/notebooks/wagtail/wagtail_video_views.ipynb` & `django-cast-0.2.9/notebooks/wagtail/wagtail_video_views.ipynb`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/pyproject.toml` & `django-cast-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     "django",
     "django-allauth",
     "django-crispy-forms",
     "django-contrib-comments",
     "django-environ",
     "django-filter",
     "django-fluent-comments",
+    "django-htmx",
     "django-model-utils",
     "django-tag-parser",
     "django-threadedcomments",
     "markdown",
     "Pygments",
     "python-akismet",
     "python-slugify",
```

### Comparing `django-cast-0.2.8/runtests.py` & `django-cast-0.2.9/runtests.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/setup.cfg` & `django-cast-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/admin_test.py` & `django-cast-0.2.9/tests/admin_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/api_test.py` & `django-cast-0.2.9/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/apps_test.py` & `django-cast-0.2.9/tests/apps_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/audio_models_test.py` & `django-cast-0.2.9/tests/audio_models_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/audio_views_test.py` & `django-cast-0.2.9/tests/audio_views_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/blocks_test.py` & `django-cast-0.2.9/tests/blocks_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/blog_index_test.py` & `django-cast-0.2.9/tests/blog_index_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
     def test_post_in_blog_index(self, client, post):
         blog_url = post.blog.get_url()
 
         r = client.get(blog_url)
         assert r.status_code == 200
 
-        assert post in r.context["page"].published_posts
+        assert post in r.context["posts"]
 
     def test_unpublished_post_not_in_blog_index(self, client, unpublished_post):
         blog_url = unpublished_post.blog.get_url()
 
         r = client.get(blog_url)
         assert r.status_code == 200
 
-        assert unpublished_post not in r.context["page"].published_posts
+        assert unpublished_post not in r.context["posts"]
 
     def test_post_overview_content_in_blog_index_but_not_detail(self, client, post):
         blog_url = post.blog.get_url()
 
         r = client.get(blog_url)
         assert r.status_code == 200
 
@@ -123,35 +123,35 @@
 
     def test_fulltext_search_all(self, client, post, post_with_search):
         blog_url = post.blog.get_url()
         r = client.get(blog_url)
         assert r.status_code == 200
 
         # assert initially both posts are in the post list
-        assert len(r.context["page"].published_posts) == 2
+        assert len(r.context["posts"]) == 2
 
     def test_fulltext_search_title(self, client, post, post_with_search):
         blog_url = post.blog.get_url()
         blog_url_title = f"{blog_url}?search={post_with_search.title}"
         r = client.get(blog_url_title)
         assert r.status_code == 200
 
         # assert search by title only yields post_with search
-        posts = r.context["page"].published_posts
+        posts = r.context["posts"]
         assert len(posts) == 1
         assert posts[0].pk == post_with_search.pk
 
     def test_fulltext_search_body(self, client, post, post_with_search):
         blog_url = post.blog.get_url()
         blog_url_content = f"{blog_url}?search={post_with_search.query}"
         r = client.get(blog_url_content)
         assert r.status_code == 200
 
         # assert search by title only yields post_with search
-        posts = r.context["page"].published_posts
+        posts = r.context["posts"]
         assert len(posts) == 1
         assert posts[0].pk == post_with_search.pk
 
 
 @pytest.fixture()
 def post_list_paginate_by_1():
     previous = appsettings.POST_LIST_PAGINATION
```

### Comparing `django-cast-0.2.8/tests/comments_test.py` & `django-cast-0.2.9/tests/comments_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/conftest.py` & `django-cast-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/episode_detail_test.py` & `django-cast-0.2.9/tests/episode_detail_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/factories.py` & `django-cast-0.2.9/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/feed_test.py` & `django-cast-0.2.9/tests/feed_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/fixtures/access.log` & `django-cast-0.2.9/tests/fixtures/access.log`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/fixtures/test.m4a` & `django-cast-0.2.9/tests/fixtures/test.m4a`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/forms_test.py` & `django-cast-0.2.9/tests/forms_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/models_test.py` & `django-cast-0.2.9/tests/models_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,43 +64,18 @@
         blog.author = None
         assert blog.author_name == blog.owner.get_full_name()
 
     def test_blog_author_not_null(self, blog):
         blog.author = "Foobar"
         assert blog.author_name == blog.author
 
-    def test_filterset_data_request_is_none(self, blog):
-        blog.request = None
-
-        # blog._filterset_data is None
-        blog._filterset_data = None
-        assert blog.filterset_data == QueryDict()
-
-        # blog._filterset_data is not None
-        blog._filterset_data = QueryDict()
-        assert blog.filterset_data == QueryDict()
-
     def test_paginate_queryset_request_is_none(self, blog):
-        blog.request = None
-        context = blog.paginate_queryset({})
+        context = blog.paginate_queryset({}, blog.get_filterset(QueryDict()).qs, QueryDict())
         assert context["page_obj"].number == 1
 
-    def test_get_other_get_params_request_is_none(self, blog):
-        blog.request = None
-        assert blog.get_other_get_params() == ""
-
-    def test_get_other_get_params_len_parameters_gt_0(self, blog):
-        class Request:
-            GET = QueryDict("foo=bar&bar=foo&page=3")
-
-        request = Request()
-        blog.request = request
-        params = blog.get_other_get_params()
-        assert params == "&foo=bar&bar=foo"
-
 
 class TestPostModel:
     pytestmark = pytest.mark.django_db
 
     def test_post_slug(self, post):
         assert post.get_slug() == "test-entry"
```

### Comparing `django-cast-0.2.8/tests/moderation_test.py` & `django-cast-0.2.9/tests/moderation_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/pagination_test.py` & `django-cast-0.2.9/tests/pagination_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pytest
 from django.core.paginator import Paginator
+from django.http import QueryDict
 from django.shortcuts import render
 from django.test import RequestFactory
 
+from cast.models import Blog
+
 
 @pytest.fixture
 def request_factory():
     return RequestFactory()
 
 
 @pytest.fixture
@@ -43,7 +46,18 @@
 
     # two ellipsis in the middle which are not links
     ellipsis_items = [line for line in html.splitlines() if "…" in line]
     assert len(ellipsis_items) == 2
     assert (
         '<span class="page-link">…</span>' == ellipsis_items[0].strip()
     )  # ellipsis in the middle which is not a link
+
+
+@pytest.mark.parametrize(
+    "query_string, expected_other_get_params",
+    [
+        ("", ""),
+        ("foo=bar&bar=foo&page=3", "&foo=bar&bar=foo"),
+    ],
+)
+def test_get_other_get_params(query_string, expected_other_get_params):
+    assert Blog.get_other_get_params(QueryDict(query_string)) == expected_other_get_params
```

### Comparing `django-cast-0.2.8/tests/post_add_test.py` & `django-cast-0.2.9/tests/post_add_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/post_detail_test.py` & `django-cast-0.2.9/tests/post_detail_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/post_media_sync_test.py` & `django-cast-0.2.9/tests/post_media_sync_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/post_published_test.py` & `django-cast-0.2.9/tests/post_published_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/settings.py` & `django-cast-0.2.9/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/theme_test.py` & `django-cast-0.2.9/tests/theme_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import shutil
 from pathlib import Path
 
+import pytest
 from django.template import engines
 
+from cast.context_processors import site_template_base_dir
 from cast.models.theme import (
     get_required_template_names,
     get_template_base_dir_candidates,
     get_template_base_dir_choices,
     get_template_directories,
 )
 
 
 def create_new_theme(name, invalid=False):
     default_engine = list(engines.all())[0]
     first_template_dir = Path(list(list(default_engine.engine.template_loaders)[0].get_dirs())[0])
-    print(first_template_dir)
 
     new_base_dir = first_template_dir / "cast" / name
     new_base_dir.mkdir(parents=True, exist_ok=True)
 
     required_names = get_required_template_names()
     if invalid:
         required_names = required_names[:-2]  # remove a required name to make it invalid
@@ -67,7 +68,28 @@
         template_loaders = [FakeLoader()]
 
     class FakeContainer:
         engine = FakeEngine()
 
     mocker.patch("cast.models.theme.engines.all", return_value=[FakeContainer()])
     assert get_template_directories() == []
+
+
+def test_cast_custom_theme_settings_show_up(settings):
+    theme_name, theme_display = "my_theme", "My Theme"
+
+    # make sure the custom theme is added to the choices
+    settings.CAST_CUSTOM_THEMES = [(theme_name, theme_display)]
+    custom_choices = get_template_base_dir_choices()
+    assert (theme_name, theme_display) in custom_choices
+
+    # make sure you cannot add predefined themes twice
+    settings.CAST_CUSTOM_THEMES.append((theme_name, theme_display))
+    assert len(get_template_base_dir_choices()) == len(custom_choices)
+
+
+@pytest.mark.django_db
+def test_context_processors_site_template_base_dir(request_factory):
+    request = request_factory.get("/")
+    context = site_template_base_dir(request)
+    assert context["cast_site_template_base_dir"] == "bootstrap4"
+    assert context["cast_base_template"] == "cast/bootstrap4/base.html"
```

### Comparing `django-cast-0.2.8/tests/upload_handler_test.py` & `django-cast-0.2.9/tests/upload_handler_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/urls.py` & `django-cast-0.2.9/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/video_dimensions_test.py` & `django-cast-0.2.9/tests/video_dimensions_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/video_upload_test.py` & `django-cast-0.2.9/tests/video_upload_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/video_views_test.py` & `django-cast-0.2.9/tests/video_views_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/tests/widget_test.py` & `django-cast-0.2.9/tests/widget_test.py`

 * *Files identical despite different names*

### Comparing `django-cast-0.2.8/PKG-INFO` & `django-cast-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cast
-Version: 0.2.8
+Version: 0.2.9
 Summary: Django and Wagtail based blogging / podcasting package
 Keywords: blog,podcast,video,audio
 Author-email: Jochen Wersdörfer <jochen-wagtailsrcset@wersdoerfer.de>, Dominik Geldmacher <oryon@cyberise.de>
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
@@ -25,14 +25,15 @@
 Requires-Dist: django
 Requires-Dist: django-allauth
 Requires-Dist: django-crispy-forms
 Requires-Dist: django-contrib-comments
 Requires-Dist: django-environ
 Requires-Dist: django-filter
 Requires-Dist: django-fluent-comments
+Requires-Dist: django-htmx
 Requires-Dist: django-model-utils
 Requires-Dist: django-tag-parser
 Requires-Dist: django-threadedcomments
 Requires-Dist: markdown
 Requires-Dist: Pygments
 Requires-Dist: python-akismet
 Requires-Dist: python-slugify
```

