# Comparing `tmp/fake-bpy-module-latest-20230429.tar.gz` & `tmp/fake-bpy-module-latest-20230430.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230429.tar", last modified: Sat Apr 29 06:20:56 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230430.tar", last modified: Sun Apr 30 06:21:34 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230429.tar` & `fake-bpy-module-latest-20230430.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-29 06:19:00.000000 fake-bpy-module-latest-20230429/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-29 06:20:50.000000 fake-bpy-module-latest-20230429/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-29 06:20:51.000000 fake-bpy-module-latest-20230429/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-29 06:20:51.000000 fake-bpy-module-latest-20230429/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-29 06:20:50.000000 fake-bpy-module-latest-20230429/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-29 06:20:50.000000 fake-bpy-module-latest-20230429/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-29 06:20:53.000000 fake-bpy-module-latest-20230429/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-29 06:20:52.000000 fake-bpy-module-latest-20230429/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-29 06:20:51.000000 fake-bpy-module-latest-20230429/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-04-29 06:20:52.000000 fake-bpy-module-latest-20230429/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-29 06:19:19.000000 fake-bpy-module-latest-20230429/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-29 06:19:21.000000 fake-bpy-module-latest-20230429/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-29 06:19:32.000000 fake-bpy-module-latest-20230429/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-29 06:19:32.000000 fake-bpy-module-latest-20230429/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-29 06:20:48.000000 fake-bpy-module-latest-20230429/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-29 06:19:17.000000 fake-bpy-module-latest-20230429/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-29 06:20:30.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-29 06:19:22.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-29 06:19:18.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-29 06:20:36.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-29 06:20:24.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-29 06:20:48.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-29 06:19:22.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-29 06:19:17.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-29 06:19:18.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-29 06:20:28.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-29 06:20:29.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-29 06:20:23.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-29 06:20:23.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-29 06:19:21.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-29 06:20:48.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-29 06:20:28.000000 fake-bpy-module-latest-20230429/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-29 06:19:30.000000 fake-bpy-module-latest-20230429/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-29 06:19:32.000000 fake-bpy-module-latest-20230429/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-29 06:19:19.000000 fake-bpy-module-latest-20230429/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-29 06:20:30.000000 fake-bpy-module-latest-20230429/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-29 06:19:23.000000 fake-bpy-module-latest-20230429/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-29 06:19:21.000000 fake-bpy-module-latest-20230429/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-29 06:20:38.000000 fake-bpy-module-latest-20230429/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-29 06:20:41.000000 fake-bpy-module-latest-20230429/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-29 06:20:35.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-29 06:20:47.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-29 06:19:20.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-29 06:20:30.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-29 06:19:29.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-29 06:20:38.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-29 06:19:20.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-29 06:20:47.000000 fake-bpy-module-latest-20230429/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-29 06:20:37.000000 fake-bpy-module-latest-20230429/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-29 06:19:18.000000 fake-bpy-module-latest-20230429/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-29 06:20:47.000000 fake-bpy-module-latest-20230429/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-29 06:20:47.000000 fake-bpy-module-latest-20230429/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-29 06:19:17.000000 fake-bpy-module-latest-20230429/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-29 06:20:39.000000 fake-bpy-module-latest-20230429/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-29 06:20:44.000000 fake-bpy-module-latest-20230429/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-29 06:20:15.000000 fake-bpy-module-latest-20230429/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-29 06:19:29.000000 fake-bpy-module-latest-20230429/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-29 06:20:46.000000 fake-bpy-module-latest-20230429/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-29 06:19:32.000000 fake-bpy-module-latest-20230429/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-29 06:20:27.000000 fake-bpy-module-latest-20230429/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-29 06:20:16.000000 fake-bpy-module-latest-20230429/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-29 06:20:16.000000 fake-bpy-module-latest-20230429/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-29 06:19:23.000000 fake-bpy-module-latest-20230429/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-29 06:19:07.000000 fake-bpy-module-latest-20230429/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-29 06:20:46.000000 fake-bpy-module-latest-20230429/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-29 06:19:27.000000 fake-bpy-module-latest-20230429/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-29 06:19:18.000000 fake-bpy-module-latest-20230429/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-29 06:19:23.000000 fake-bpy-module-latest-20230429/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-29 06:20:48.000000 fake-bpy-module-latest-20230429/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-29 06:20:39.000000 fake-bpy-module-latest-20230429/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-29 06:19:21.000000 fake-bpy-module-latest-20230429/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-04-29 06:20:23.000000 fake-bpy-module-latest-20230429/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-29 06:20:38.000000 fake-bpy-module-latest-20230429/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-29 06:20:34.000000 fake-bpy-module-latest-20230429/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-29 06:20:15.000000 fake-bpy-module-latest-20230429/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-04-29 06:20:23.000000 fake-bpy-module-latest-20230429/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 06:20:28.000000 fake-bpy-module-latest-20230429/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-29 06:19:00.000000 fake-bpy-module-latest-20230429/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-29 06:18:59.000000 fake-bpy-module-latest-20230429/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-29 06:18:21.000000 fake-bpy-module-latest-20230429/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-29 06:18:57.000000 fake-bpy-module-latest-20230429/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-29 06:18:53.000000 fake-bpy-module-latest-20230429/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-29 06:18:24.000000 fake-bpy-module-latest-20230429/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-29 06:18:54.000000 fake-bpy-module-latest-20230429/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-29 06:18:31.000000 fake-bpy-module-latest-20230429/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-29 06:18:56.000000 fake-bpy-module-latest-20230429/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-29 06:18:24.000000 fake-bpy-module-latest-20230429/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-29 06:18:32.000000 fake-bpy-module-latest-20230429/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-29 06:18:33.000000 fake-bpy-module-latest-20230429/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-29 06:18:38.000000 fake-bpy-module-latest-20230429/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-29 06:18:24.000000 fake-bpy-module-latest-20230429/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-29 06:18:57.000000 fake-bpy-module-latest-20230429/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-29 06:18:54.000000 fake-bpy-module-latest-20230429/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-29 06:18:31.000000 fake-bpy-module-latest-20230429/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-29 06:18:25.000000 fake-bpy-module-latest-20230429/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-29 06:18:33.000000 fake-bpy-module-latest-20230429/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-29 06:18:43.000000 fake-bpy-module-latest-20230429/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-29 06:18:27.000000 fake-bpy-module-latest-20230429/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-29 06:18:30.000000 fake-bpy-module-latest-20230429/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-29 06:18:31.000000 fake-bpy-module-latest-20230429/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-29 06:18:24.000000 fake-bpy-module-latest-20230429/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-04-29 06:18:37.000000 fake-bpy-module-latest-20230429/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-29 06:18:49.000000 fake-bpy-module-latest-20230429/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-29 06:18:35.000000 fake-bpy-module-latest-20230429/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-29 06:18:57.000000 fake-bpy-module-latest-20230429/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-29 06:18:35.000000 fake-bpy-module-latest-20230429/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-29 06:18:54.000000 fake-bpy-module-latest-20230429/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-29 06:18:34.000000 fake-bpy-module-latest-20230429/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-29 06:18:49.000000 fake-bpy-module-latest-20230429/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-29 06:18:48.000000 fake-bpy-module-latest-20230429/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-29 06:18:40.000000 fake-bpy-module-latest-20230429/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-29 06:18:22.000000 fake-bpy-module-latest-20230429/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-29 06:18:52.000000 fake-bpy-module-latest-20230429/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-29 06:18:34.000000 fake-bpy-module-latest-20230429/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-29 06:18:25.000000 fake-bpy-module-latest-20230429/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-29 06:18:40.000000 fake-bpy-module-latest-20230429/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-29 06:18:54.000000 fake-bpy-module-latest-20230429/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-29 06:18:31.000000 fake-bpy-module-latest-20230429/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-29 06:18:32.000000 fake-bpy-module-latest-20230429/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-29 06:18:41.000000 fake-bpy-module-latest-20230429/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-29 06:18:35.000000 fake-bpy-module-latest-20230429/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-29 06:18:22.000000 fake-bpy-module-latest-20230429/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-29 06:18:53.000000 fake-bpy-module-latest-20230429/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-29 06:18:50.000000 fake-bpy-module-latest-20230429/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-29 06:18:24.000000 fake-bpy-module-latest-20230429/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-29 06:18:26.000000 fake-bpy-module-latest-20230429/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-29 06:18:49.000000 fake-bpy-module-latest-20230429/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-29 06:18:30.000000 fake-bpy-module-latest-20230429/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-29 06:18:57.000000 fake-bpy-module-latest-20230429/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-29 06:18:25.000000 fake-bpy-module-latest-20230429/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-29 06:18:56.000000 fake-bpy-module-latest-20230429/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-29 06:18:34.000000 fake-bpy-module-latest-20230429/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-29 06:18:56.000000 fake-bpy-module-latest-20230429/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-29 06:18:28.000000 fake-bpy-module-latest-20230429/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-29 06:18:40.000000 fake-bpy-module-latest-20230429/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    56321 2023-04-29 06:18:27.000000 fake-bpy-module-latest-20230429/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-29 06:18:31.000000 fake-bpy-module-latest-20230429/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-29 06:18:32.000000 fake-bpy-module-latest-20230429/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   245716 2023-04-29 06:18:48.000000 fake-bpy-module-latest-20230429/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-29 06:18:35.000000 fake-bpy-module-latest-20230429/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-29 06:18:24.000000 fake-bpy-module-latest-20230429/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-29 06:18:59.000000 fake-bpy-module-latest-20230429/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3488183 2023-04-29 06:18:21.000000 fake-bpy-module-latest-20230429/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-29 06:18:58.000000 fake-bpy-module-latest-20230429/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-29 06:18:59.000000 fake-bpy-module-latest-20230429/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-29 06:18:59.000000 fake-bpy-module-latest-20230429/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-29 06:19:03.000000 fake-bpy-module-latest-20230429/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-29 06:19:02.000000 fake-bpy-module-latest-20230429/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-29 06:19:01.000000 fake-bpy-module-latest-20230429/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:12:09.000000 fake-bpy-module-latest-20230429/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-29 06:20:49.000000 fake-bpy-module-latest-20230429/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-29 06:19:06.000000 fake-bpy-module-latest-20230429/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-29 06:20:54.000000 fake-bpy-module-latest-20230429/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-29 06:20:56.000000 fake-bpy-module-latest-20230429/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-29 06:20:55.000000 fake-bpy-module-latest-20230429/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-30 06:19:27.000000 fake-bpy-module-latest-20230430/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-30 06:19:35.000000 fake-bpy-module-latest-20230430/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-30 06:19:38.000000 fake-bpy-module-latest-20230430/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-30 06:19:37.000000 fake-bpy-module-latest-20230430/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-30 06:19:39.000000 fake-bpy-module-latest-20230430/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97916 2023-04-30 06:19:36.000000 fake-bpy-module-latest-20230430/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-30 06:19:41.000000 fake-bpy-module-latest-20230430/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-30 06:21:29.000000 fake-bpy-module-latest-20230430/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-30 06:19:55.000000 fake-bpy-module-latest-20230430/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-30 06:20:40.000000 fake-bpy-module-latest-20230430/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-30 06:19:48.000000 fake-bpy-module-latest-20230430/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-30 06:19:48.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-30 06:20:39.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-30 06:19:43.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-30 06:20:41.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-30 06:20:37.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-30 06:20:39.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-30 06:20:41.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-30 06:20:15.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-30 06:20:27.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-30 06:20:38.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-30 06:20:39.000000 fake-bpy-module-latest-20230430/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-30 06:19:57.000000 fake-bpy-module-latest-20230430/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-30 06:20:42.000000 fake-bpy-module-latest-20230430/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-30 06:20:40.000000 fake-bpy-module-latest-20230430/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-30 06:19:43.000000 fake-bpy-module-latest-20230430/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-30 06:20:38.000000 fake-bpy-module-latest-20230430/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-30 06:20:26.000000 fake-bpy-module-latest-20230430/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-30 06:20:23.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-30 06:21:29.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-30 06:20:38.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-30 06:19:42.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-30 06:20:32.000000 fake-bpy-module-latest-20230430/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-30 06:21:30.000000 fake-bpy-module-latest-20230430/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-30 06:20:33.000000 fake-bpy-module-latest-20230430/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-30 06:20:27.000000 fake-bpy-module-latest-20230430/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-30 06:21:31.000000 fake-bpy-module-latest-20230430/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-30 06:19:42.000000 fake-bpy-module-latest-20230430/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-30 06:19:48.000000 fake-bpy-module-latest-20230430/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-30 06:20:31.000000 fake-bpy-module-latest-20230430/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-30 06:20:41.000000 fake-bpy-module-latest-20230430/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-30 06:19:56.000000 fake-bpy-module-latest-20230430/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-30 06:20:29.000000 fake-bpy-module-latest-20230430/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-30 06:19:52.000000 fake-bpy-module-latest-20230430/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-30 06:20:30.000000 fake-bpy-module-latest-20230430/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-30 06:19:58.000000 fake-bpy-module-latest-20230430/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-30 06:19:44.000000 fake-bpy-module-latest-20230430/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-30 06:20:30.000000 fake-bpy-module-latest-20230430/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-30 06:20:15.000000 fake-bpy-module-latest-20230430/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-30 06:20:37.000000 fake-bpy-module-latest-20230430/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-30 06:20:30.000000 fake-bpy-module-latest-20230430/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-30 06:20:15.000000 fake-bpy-module-latest-20230430/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-30 06:21:29.000000 fake-bpy-module-latest-20230430/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-30 06:20:14.000000 fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-04-30 06:20:42.000000 fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-30 06:19:53.000000 fake-bpy-module-latest-20230430/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-30 06:20:03.000000 fake-bpy-module-latest-20230430/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-30 06:21:28.000000 fake-bpy-module-latest-20230430/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-04-30 06:20:23.000000 fake-bpy-module-latest-20230430/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-30 06:20:28.000000 fake-bpy-module-latest-20230430/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-30 06:19:27.000000 fake-bpy-module-latest-20230430/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-30 06:18:43.000000 fake-bpy-module-latest-20230430/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-30 06:18:57.000000 fake-bpy-module-latest-20230430/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-30 06:19:20.000000 fake-bpy-module-latest-20230430/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-30 06:19:21.000000 fake-bpy-module-latest-20230430/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-30 06:19:10.000000 fake-bpy-module-latest-20230430/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-30 06:19:22.000000 fake-bpy-module-latest-20230430/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-30 06:19:13.000000 fake-bpy-module-latest-20230430/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-30 06:19:19.000000 fake-bpy-module-latest-20230430/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-30 06:18:57.000000 fake-bpy-module-latest-20230430/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-30 06:19:03.000000 fake-bpy-module-latest-20230430/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-30 06:18:52.000000 fake-bpy-module-latest-20230430/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-30 06:18:55.000000 fake-bpy-module-latest-20230430/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-30 06:19:12.000000 fake-bpy-module-latest-20230430/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-30 06:19:07.000000 fake-bpy-module-latest-20230430/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-30 06:18:45.000000 fake-bpy-module-latest-20230430/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-04-30 06:18:52.000000 fake-bpy-module-latest-20230430/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-30 06:19:10.000000 fake-bpy-module-latest-20230430/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-30 06:19:13.000000 fake-bpy-module-latest-20230430/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-30 06:18:55.000000 fake-bpy-module-latest-20230430/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-30 06:18:43.000000 fake-bpy-module-latest-20230430/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-30 06:18:57.000000 fake-bpy-module-latest-20230430/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-30 06:19:04.000000 fake-bpy-module-latest-20230430/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-30 06:19:19.000000 fake-bpy-module-latest-20230430/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-30 06:18:50.000000 fake-bpy-module-latest-20230430/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-30 06:18:45.000000 fake-bpy-module-latest-20230430/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-30 06:19:03.000000 fake-bpy-module-latest-20230430/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-30 06:19:05.000000 fake-bpy-module-latest-20230430/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-30 06:19:16.000000 fake-bpy-module-latest-20230430/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-30 06:18:44.000000 fake-bpy-module-latest-20230430/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-30 06:18:56.000000 fake-bpy-module-latest-20230430/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-30 06:19:07.000000 fake-bpy-module-latest-20230430/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-30 06:19:07.000000 fake-bpy-module-latest-20230430/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-30 06:18:58.000000 fake-bpy-module-latest-20230430/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-30 06:19:21.000000 fake-bpy-module-latest-20230430/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-30 06:18:54.000000 fake-bpy-module-latest-20230430/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-30 06:19:24.000000 fake-bpy-module-latest-20230430/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-30 06:18:53.000000 fake-bpy-module-latest-20230430/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56321 2023-04-30 06:19:23.000000 fake-bpy-module-latest-20230430/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-30 06:19:09.000000 fake-bpy-module-latest-20230430/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-30 06:19:21.000000 fake-bpy-module-latest-20230430/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245716 2023-04-30 06:19:03.000000 fake-bpy-module-latest-20230430/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-30 06:19:15.000000 fake-bpy-module-latest-20230430/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-30 06:19:19.000000 fake-bpy-module-latest-20230430/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3488183 2023-04-30 06:18:43.000000 fake-bpy-module-latest-20230430/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-30 06:19:25.000000 fake-bpy-module-latest-20230430/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-30 06:19:30.000000 fake-bpy-module-latest-20230430/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-30 06:19:29.000000 fake-bpy-module-latest-20230430/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-30 06:19:29.000000 fake-bpy-module-latest-20230430/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-30 06:19:29.000000 fake-bpy-module-latest-20230430/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-30 06:19:40.000000 fake-bpy-module-latest-20230430/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-30 06:19:28.000000 fake-bpy-module-latest-20230430/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 06:11:49.000000 fake-bpy-module-latest-20230430/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-30 06:19:33.000000 fake-bpy-module-latest-20230430/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-30 06:19:34.000000 fake-bpy-module-latest-20230430/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 06:21:34.000000 fake-bpy-module-latest-20230430/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-30 06:21:33.000000 fake-bpy-module-latest-20230430/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230429/PKG-INFO` & `fake-bpy-module-latest-20230430/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230429
+Version: 20230430
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230429/README.rst` & `fake-bpy-module-latest-20230430/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/addon_utils.py` & `fake-bpy-module-latest-20230430/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/animsys_refactor.py` & `fake-bpy-module-latest-20230430/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/aud.py` & `fake-bpy-module-latest-20230430/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bgl.py` & `fake-bpy-module-latest-20230430/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230430/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230430/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230430/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230430/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230430/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_math.py` & `fake-bpy-module-latest-20230430/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/__init__.py` & `fake-bpy-module-latest-20230430/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
 import typing
-from . import vertexpaint_dirt
+from . import presets
+from . import console
+from . import image
+from . import node
 from . import screen_play_rendered_anim
-from . import assets
-from . import object_quick_effects
-from . import anim
+from . import constraint
+from . import wm
+from . import freestyle
+from . import bmesh
 from . import mesh
+from . import sequencer
+from . import vertexpaint_dirt
+from . import object
+from . import rigidbody
 from . import object_randomize_transform
 from . import userpref
-from . import object
-from . import node
-from . import view3d
-from . import wm
-from . import uvcalc_transform
-from . import geometry_nodes
-from . import image
-from . import console
-from . import presets
-from . import spreadsheet
+from . import object_quick_effects
 from . import clip
-from . import uvcalc_follow_active
 from . import uvcalc_lightmap
-from . import rigidbody
-from . import add_mesh_torus
-from . import constraint
+from . import spreadsheet
 from . import file
-from . import bmesh
-from . import freestyle
+from . import assets
+from . import geometry_nodes
+from . import view3d
+from . import uvcalc_transform
+from . import uvcalc_follow_active
+from . import anim
 from . import object_align
-from . import sequencer
+from . import add_mesh_torus
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230429/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230430/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/anim.py` & `fake-bpy-module-latest-20230430/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/assets.py` & `fake-bpy-module-latest-20230430/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230430/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/clip.py` & `fake-bpy-module-latest-20230430/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/console.py` & `fake-bpy-module-latest-20230430/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/constraint.py` & `fake-bpy-module-latest-20230430/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/file.py` & `fake-bpy-module-latest-20230430/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230430/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230430/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/image.py` & `fake-bpy-module-latest-20230430/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/mesh.py` & `fake-bpy-module-latest-20230430/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/node.py` & `fake-bpy-module-latest-20230430/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/object.py` & `fake-bpy-module-latest-20230430/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/object_align.py` & `fake-bpy-module-latest-20230430/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230430/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230430/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/presets.py` & `fake-bpy-module-latest-20230430/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230430/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230430/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230430/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230430/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/userpref.py` & `fake-bpy-module-latest-20230430/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230430/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230430/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230430/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230430/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/view3d.py` & `fake-bpy-module-latest-20230430/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_operators/wm.py` & `fake-bpy-module-latest-20230430/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230430/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/__init__.py` & `fake-bpy-module-latest-20230430/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import sys
 import typing
 import bpy_types
 
-from . import space_outliner
-from . import properties_constraint
-from . import properties_workspace
-from . import properties_data_lattice
-from . import properties_data_light
-from . import space_spreadsheet
-from . import properties_scene
-from . import properties_data_camera
-from . import properties_material
-from . import generic_ui_list
-from . import properties_physics_rigidbody_constraint
-from . import properties_physics_dynamicpaint
+from . import properties_physics_fluid
+from . import properties_world
 from . import properties_output
-from . import properties_data_shaderfx
-from . import space_toolsystem_common
-from . import node_add_menu
-from . import properties_data_gpencil
-from . import properties_data_bone
-from . import properties_object
+from . import properties_data_camera
 from . import space_node
-from . import space_statusbar
-from . import space_sequencer
-from . import properties_physics_fluid
-from . import space_dopesheet
-from . import properties_grease_pencil_common
+from . import space_clip
+from . import properties_collection
+from . import properties_data_armature
+from . import space_image
+from . import space_topbar
 from . import node_add_menu_geometry
-from . import space_graph
-from . import properties_mask_common
-from . import properties_animviz
-from . import space_view3d
-from . import space_console
+from . import space_filebrowser
+from . import properties_grease_pencil_common
 from . import space_nla
-from . import space_info
-from . import space_view3d_toolbar
+from . import properties_physics_rigidbody_constraint
 from . import properties_data_pointcloud
-from . import space_toolsystem_toolbar
-from . import properties_data_modifier
-from . import properties_data_curves
-from . import space_image
-from . import properties_freestyle
-from . import utils
+from . import properties_data_metaball
+from . import space_userpref
+from . import properties_constraint
+from . import space_toolsystem_common
+from . import space_spreadsheet
+from . import properties_physics_rigidbody
+from . import space_properties
+from . import properties_data_light
+from . import space_text
+from . import space_view3d_toolbar
+from . import properties_physics_cloth
+from . import properties_particle
+from . import properties_view_layer
 from . import properties_data_lightprobe
 from . import properties_data_mesh
-from . import properties_data_armature
+from . import utils
+from . import properties_data_modifier
+from . import properties_physics_common
+from . import space_graph
+from . import properties_data_curves
 from . import properties_material_gpencil
-from . import properties_physics_field
-from . import space_userpref
-from . import properties_physics_cloth
-from . import properties_data_curve
+from . import generic_ui_list
+from . import properties_data_shaderfx
+from . import space_outliner
+from . import space_info
+from . import space_statusbar
+from . import space_console
 from . import properties_render
-from . import space_topbar
-from . import properties_paint_common
-from . import properties_physics_rigidbody
-from . import space_time
-from . import properties_world
-from . import properties_particle
-from . import space_clip
-from . import space_filebrowser
-from . import space_properties
 from . import properties_texture
-from . import properties_physics_common
-from . import properties_view_layer
-from . import properties_physics_softbody
-from . import properties_collection
-from . import properties_data_speaker
-from . import space_text
+from . import space_sequencer
 from . import properties_data_empty
+from . import properties_physics_field
+from . import properties_paint_common
+from . import properties_data_speaker
+from . import properties_data_gpencil
+from . import properties_data_bone
 from . import properties_data_volume
-from . import properties_data_metaball
+from . import properties_object
+from . import properties_animviz
+from . import properties_data_curve
+from . import properties_data_lattice
+from . import space_dopesheet
+from . import space_toolsystem_toolbar
+from . import properties_material
+from . import space_view3d
+from . import space_time
+from . import node_add_menu
+from . import properties_physics_dynamicpaint
+from . import properties_scene
+from . import properties_freestyle
+from . import properties_mask_common
+from . import properties_physics_softbody
+from . import properties_workspace
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230429/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230430/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230430/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230430/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230430/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_console.py` & `fake-bpy-module-latest-20230430/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230430/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230430/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230430/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_image.py` & `fake-bpy-module-latest-20230430/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_info.py` & `fake-bpy-module-latest-20230430/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230430/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_node.py` & `fake-bpy-module-latest-20230430/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230430/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230430/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230430/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230430/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230430/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_text.py` & `fake-bpy-module-latest-20230430/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_time.py` & `fake-bpy-module-latest-20230430/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230430/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230430/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230430/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230430/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230430/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bl_ui/utils.py` & `fake-bpy-module-latest-20230430/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/blf.py` & `fake-bpy-module-latest-20230430/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bmesh/__init__.py` & `fake-bpy-module-latest-20230430/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bmesh/geometry.py` & `fake-bpy-module-latest-20230430/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bmesh/ops.py` & `fake-bpy-module-latest-20230430/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bmesh/types.py` & `fake-bpy-module-latest-20230430/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bmesh/utils.py` & `fake-bpy-module-latest-20230430/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/app/__init__.py` & `fake-bpy-module-latest-20230430/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 from . import handlers
-from . import timers
 from . import translations
 from . import icons
+from . import timers
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def is_job_running(job_type: typing.Optional[str]) -> typing.Any:
     ''' Check whether a job of the given type is running.
```

### Comparing `fake-bpy-module-latest-20230429/bpy/app/handlers.py` & `fake-bpy-module-latest-20230430/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/app/icons.py` & `fake-bpy-module-latest-20230430/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/app/timers.py` & `fake-bpy-module-latest-20230430/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/app/translations.py` & `fake-bpy-module-latest-20230430/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/msgbus.py` & `fake-bpy-module-latest-20230430/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230430/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import sys
 import typing
-from . import node
-from . import rigidbody
+from . import lattice
 from . import armature
-from . import constraint
-from . import script
-from . import gizmogroup
-from . import world
-from . import buttons
+from . import cloth
+from . import boid
+from . import scene
 from . import paint
-from . import surface
+from . import geometry
+from . import object
+from . import gpencil
+from . import dpaint
+from . import marker
+from . import brush
+from . import uilist
+from . import preferences
+from . import rigidbody
+from . import pose
+from . import text
+from . import export_anim
+from . import texture
 from . import ed
+from . import import_scene
 from . import sculpt
-from . import uv
-from . import file
-from . import collection
-from . import cloth
-from . import geometry
-from . import nla
+from . import curve
+from . import action
+from . import material
+from . import spreadsheet
+from . import wm
 from . import paintcurve
+from . import curves
+from . import buttons
+from . import mball
+from . import gizmogroup
 from . import info
-from . import ui
+from . import cycles
+from . import particle
+from . import outliner
+from . import camera
+from . import import_anim
+from . import import_curve
 from . import sequencer
+from . import sound
 from . import fluid
-from . import pose
-from . import font
+from . import transform
 from . import view2d
-from . import boid
-from . import cycles
+from . import palette
+from . import ptcache
 from . import cachefile
-from . import poselib
-from . import view3d
-from . import clip
-from . import export_anim
-from . import texture
-from . import outliner
-from . import mask
+from . import graph
+from . import export_scene
 from . import image
-from . import render
+from . import console
+from . import node
+from . import sculpt_curves
+from . import script
+from . import mask
+from . import font
 from . import workspace
+from . import collection
+from . import poselib
+from . import nla
+from . import render
 from . import import_mesh
-from . import gpencil
-from . import console
 from . import mesh
-from . import uilist
-from . import palette
-from . import export_mesh
-from . import preferences
-from . import lattice
-from . import ptcache
-from . import dpaint
-from . import camera
-from . import import_anim
-from . import export_scene
-from . import wm
-from . import mball
-from . import graph
-from . import sculpt_curves
-from . import material
-from . import screen
-from . import object
+from . import constraint
+from . import world
 from . import anim
-from . import scene
+from . import view3d
 from . import asset
-from . import particle
-from . import marker
-from . import curves
-from . import transform
-from . import text
-from . import brush
-from . import curve
-from . import action
-from . import import_curve
-from . import sound
-from . import import_scene
-from . import spreadsheet
+from . import surface
+from . import clip
+from . import uv
+from . import ui
+from . import export_mesh
+from . import file
+from . import screen
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/action.py` & `fake-bpy-module-latest-20230430/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/anim.py` & `fake-bpy-module-latest-20230430/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/armature.py` & `fake-bpy-module-latest-20230430/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/asset.py` & `fake-bpy-module-latest-20230430/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/boid.py` & `fake-bpy-module-latest-20230430/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/brush.py` & `fake-bpy-module-latest-20230430/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230430/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230430/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/camera.py` & `fake-bpy-module-latest-20230430/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/clip.py` & `fake-bpy-module-latest-20230430/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230430/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/collection.py` & `fake-bpy-module-latest-20230430/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/console.py` & `fake-bpy-module-latest-20230430/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230430/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/curve.py` & `fake-bpy-module-latest-20230430/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/curves.py` & `fake-bpy-module-latest-20230430/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230430/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230430/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/ed.py` & `fake-bpy-module-latest-20230430/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230430/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230430/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230430/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/file.py` & `fake-bpy-module-latest-20230430/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230430/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/font.py` & `fake-bpy-module-latest-20230430/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230430/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230430/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230430/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/graph.py` & `fake-bpy-module-latest-20230430/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/image.py` & `fake-bpy-module-latest-20230430/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230430/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230430/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230430/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230430/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/info.py` & `fake-bpy-module-latest-20230430/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230430/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/marker.py` & `fake-bpy-module-latest-20230430/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/mask.py` & `fake-bpy-module-latest-20230430/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/material.py` & `fake-bpy-module-latest-20230430/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/mball.py` & `fake-bpy-module-latest-20230430/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230430/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/nla.py` & `fake-bpy-module-latest-20230430/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/node.py` & `fake-bpy-module-latest-20230430/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/object.py` & `fake-bpy-module-latest-20230430/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230430/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/paint.py` & `fake-bpy-module-latest-20230430/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230430/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/palette.py` & `fake-bpy-module-latest-20230430/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/particle.py` & `fake-bpy-module-latest-20230430/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/pose.py` & `fake-bpy-module-latest-20230430/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230430/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230430/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230430/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/render.py` & `fake-bpy-module-latest-20230430/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230430/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/scene.py` & `fake-bpy-module-latest-20230430/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/screen.py` & `fake-bpy-module-latest-20230430/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/script.py` & `fake-bpy-module-latest-20230430/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230430/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230430/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230430/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/sound.py` & `fake-bpy-module-latest-20230430/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230430/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/surface.py` & `fake-bpy-module-latest-20230430/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/text.py` & `fake-bpy-module-latest-20230430/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/texture.py` & `fake-bpy-module-latest-20230430/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/transform.py` & `fake-bpy-module-latest-20230430/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/ui.py` & `fake-bpy-module-latest-20230430/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230430/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/uv.py` & `fake-bpy-module-latest-20230430/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230430/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230430/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/wm.py` & `fake-bpy-module-latest-20230430/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230430/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/ops/world.py` & `fake-bpy-module-latest-20230430/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/path.py` & `fake-bpy-module-latest-20230430/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/props.py` & `fake-bpy-module-latest-20230430/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/types.py` & `fake-bpy-module-latest-20230430/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1050 +1,1050 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7370 6163 655f 6f75 746c 696e 6572  i.space_outliner
-00000050: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000060: 6f70 6572 7469 6573 5f63 6f6e 7374 7261  operties_constra
-00000070: 696e 740a 696d 706f 7274 2062 6c5f 7569  int.import bl_ui
-00000080: 2e70 726f 7065 7274 6965 735f 776f 726b  .properties_work
-00000090: 7370 6163 650a 696d 706f 7274 2062 6c5f  space.import bl_
-000000a0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
-000000b0: 7461 5f6c 6174 7469 6365 0a69 6d70 6f72  ta_lattice.impor
-000000c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000000d0: 6573 5f64 6174 615f 6c69 6768 740a 696d  es_data_light.im
-000000e0: 706f 7274 2062 6c5f 6f70 6572 6174 6f72  port bl_operator
-000000f0: 732e 6173 7365 7473 0a69 6d70 6f72 7420  s.assets.import 
-00000100: 626c 5f6f 7065 7261 746f 7273 2e61 6e69  bl_operators.ani
-00000110: 6d0a 696d 706f 7274 2062 6c5f 7569 2e73  m.import bl_ui.s
-00000120: 7061 6365 5f73 7072 6561 6473 6865 6574  pace_spreadsheet
-00000130: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000140: 6f70 6572 7469 6573 5f73 6365 6e65 0a69  operties_scene.i
-00000150: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000160: 6572 7469 6573 5f64 6174 615f 6361 6d65  erties_data_came
-00000170: 7261 0a69 6d70 6f72 7420 626c 5f75 692e  ra.import bl_ui.
-00000180: 7072 6f70 6572 7469 6573 5f6d 6174 6572  properties_mater
-00000190: 6961 6c0a 696d 706f 7274 2062 6c5f 7569  ial.import bl_ui
-000001a0: 2e67 656e 6572 6963 5f75 695f 6c69 7374  .generic_ui_list
-000001b0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-000001c0: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
-000001d0: 5f72 6967 6964 626f 6479 5f63 6f6e 7374  _rigidbody_const
-000001e0: 7261 696e 740a 696d 706f 7274 2062 6c5f  raint.import bl_
-000001f0: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
-00000200: 7973 6963 735f 6479 6e61 6d69 6370 6169  ysics_dynamicpai
-00000210: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
-00000220: 7072 6f70 6572 7469 6573 5f6f 7574 7075  properties_outpu
-00000230: 740a 696d 706f 7274 2062 6c5f 7569 2e70  t.import bl_ui.p
-00000240: 726f 7065 7274 6965 735f 6461 7461 5f73  roperties_data_s
-00000250: 6861 6465 7266 780a 696d 706f 7274 2062  haderfx.import b
-00000260: 6c5f 7569 2e73 7061 6365 5f74 6f6f 6c73  l_ui.space_tools
-00000270: 7973 7465 6d5f 636f 6d6d 6f6e 0a69 6d70  ystem_common.imp
-00000280: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000290: 2e75 7365 7270 7265 660a 696d 706f 7274  .userpref.import
-000002a0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000002b0: 735f 6461 7461 5f67 7065 6e63 696c 0a69  s_data_gpencil.i
-000002c0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000002d0: 6572 7469 6573 5f64 6174 615f 626f 6e65  erties_data_bone
-000002e0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000002f0: 746f 7273 2e6f 626a 6563 740a 696d 706f  tors.object.impo
-00000300: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000310: 6965 735f 6f62 6a65 6374 0a69 6d70 6f72  ies_object.impor
-00000320: 7420 626c 5f75 692e 7370 6163 655f 6e6f  t bl_ui.space_no
-00000330: 6465 0a69 6d70 6f72 7420 626c 5f75 692e  de.import bl_ui.
-00000340: 7370 6163 655f 7374 6174 7573 6261 720a  space_statusbar.
-00000350: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000360: 6365 5f73 6571 7565 6e63 6572 0a69 6d70  ce_sequencer.imp
-00000370: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000380: 2e6e 6f64 650a 696d 706f 7274 2062 6c5f  .node.import bl_
-00000390: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
-000003a0: 7973 6963 735f 666c 7569 640a 696d 706f  ysics_fluid.impo
-000003b0: 7274 2062 6c5f 7569 2e73 7061 6365 5f64  rt bl_ui.space_d
-000003c0: 6f70 6573 6865 6574 0a69 6d70 6f72 7420  opesheet.import 
-000003d0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000003e0: 5f67 7265 6173 655f 7065 6e63 696c 5f63  _grease_pencil_c
-000003f0: 6f6d 6d6f 6e0a 696d 706f 7274 2062 6c5f  ommon.import bl_
-00000400: 6f70 6572 6174 6f72 732e 7669 6577 3364  operators.view3d
-00000410: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000420: 746f 7273 2e77 6d0a 696d 706f 7274 2062  tors.wm.import b
-00000430: 6c5f 7569 2e6e 6f64 655f 6164 645f 6d65  l_ui.node_add_me
-00000440: 6e75 5f67 656f 6d65 7472 790a 696d 706f  nu_geometry.impo
-00000450: 7274 2062 6c5f 7569 2e73 7061 6365 5f67  rt bl_ui.space_g
-00000460: 7261 7068 0a69 6d70 6f72 7420 626c 5f75  raph.import bl_u
-00000470: 692e 7072 6f70 6572 7469 6573 5f6d 6173  i.properties_mas
-00000480: 6b5f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  k_common.import 
-00000490: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-000004a0: 3364 0a69 6d70 6f72 7420 626c 5f75 692e  3d.import bl_ui.
-000004b0: 7370 6163 655f 636f 6e73 6f6c 650a 696d  space_console.im
-000004c0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-000004d0: 5f6e 6c61 0a69 6d70 6f72 7420 626c 5f75  _nla.import bl_u
-000004e0: 692e 7370 6163 655f 696e 666f 0a69 6d70  i.space_info.imp
-000004f0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000500: 7669 6577 3364 5f74 6f6f 6c62 6172 0a69  view3d_toolbar.i
-00000510: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000520: 6572 7469 6573 5f64 6174 615f 706f 696e  erties_data_poin
-00000530: 7463 6c6f 7564 0a69 6d70 6f72 7420 626c  tcloud.import bl
-00000540: 5f75 692e 7370 6163 655f 746f 6f6c 7379  _ui.space_toolsy
-00000550: 7374 656d 5f74 6f6f 6c62 6172 0a69 6d70  stem_toolbar.imp
-00000560: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-00000570: 7469 6573 5f64 6174 615f 6d6f 6469 6669  ties_data_modifi
-00000580: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
-00000590: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-000005a0: 6375 7276 6573 0a69 6d70 6f72 7420 626c  curves.import bl
-000005b0: 5f75 692e 7370 6163 655f 696d 6167 650a  _ui.space_image.
-000005c0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-000005d0: 7065 7274 6965 735f 6672 6565 7374 796c  perties_freestyl
-000005e0: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
-000005f0: 726f 7065 7274 6965 735f 6461 7461 5f6c  roperties_data_l
-00000600: 6967 6874 7072 6f62 650a 696d 706f 7274  ightprobe.import
-00000610: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000620: 735f 6461 7461 5f6d 6573 680a 696d 706f  s_data_mesh.impo
-00000630: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000640: 6965 735f 6461 7461 5f61 726d 6174 7572  ies_data_armatur
-00000650: 650a 696d 706f 7274 2062 6c5f 7569 2e70  e.import bl_ui.p
-00000660: 726f 7065 7274 6965 735f 6d61 7465 7269  roperties_materi
-00000670: 616c 5f67 7065 6e63 696c 0a69 6d70 6f72  al_gpencil.impor
-00000680: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000690: 6573 5f70 6879 7369 6373 5f66 6965 6c64  es_physics_field
-000006a0: 0a69 6d70 6f72 7420 626c 5f75 690a 696d  .import bl_ui.im
-000006b0: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-000006c0: 5f75 7365 7270 7265 660a 696d 706f 7274  _userpref.import
-000006d0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000006e0: 735f 7068 7973 6963 735f 636c 6f74 680a  s_physics_cloth.
-000006f0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000700: 7065 7274 6965 735f 6461 7461 5f63 7572  perties_data_cur
-00000710: 7665 0a69 6d70 6f72 7420 626c 5f75 692e  ve.import bl_ui.
-00000720: 7072 6f70 6572 7469 6573 5f72 656e 6465  properties_rende
-00000730: 720a 696d 706f 7274 2062 6c5f 7569 2e73  r.import bl_ui.s
-00000740: 7061 6365 5f74 6f70 6261 720a 696d 706f  pace_topbar.impo
-00000750: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000760: 6965 735f 7061 696e 745f 636f 6d6d 6f6e  ies_paint_common
-00000770: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000780: 746f 7273 2e70 7265 7365 7473 0a69 6d70  tors.presets.imp
-00000790: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
-000007a0: 7469 6573 5f70 6879 7369 6373 5f72 6967  ties_physics_rig
-000007b0: 6964 626f 6479 0a69 6d70 6f72 7420 626c  idbody.import bl
-000007c0: 5f75 692e 7370 6163 655f 7469 6d65 0a69  _ui.space_time.i
-000007d0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-000007e0: 7273 2e73 7072 6561 6473 6865 6574 0a69  rs.spreadsheet.i
-000007f0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000800: 6572 7469 6573 5f77 6f72 6c64 0a69 6d70  erties_world.imp
-00000810: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000820: 2e63 6c69 700a 696d 706f 7274 2062 6c5f  .clip.import bl_
-00000830: 7569 2e70 726f 7065 7274 6965 735f 7061  ui.properties_pa
-00000840: 7274 6963 6c65 0a69 6d70 6f72 7420 626c  rticle.import bl
-00000850: 5f75 692e 7370 6163 655f 636c 6970 0a69  _ui.space_clip.i
-00000860: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
-00000870: 655f 6669 6c65 6272 6f77 7365 720a 696d  e_filebrowser.im
-00000880: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000890: 5f70 726f 7065 7274 6965 730a 696d 706f  _properties.impo
-000008a0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000008b0: 6965 735f 7465 7874 7572 650a 696d 706f  ies_texture.impo
-000008c0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-000008d0: 6965 735f 7068 7973 6963 735f 636f 6d6d  ies_physics_comm
-000008e0: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
-000008f0: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
-00000900: 6c61 7965 720a 696d 706f 7274 2062 6c5f  layer.import bl_
-00000910: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
-00000920: 7973 6963 735f 736f 6674 626f 6479 0a69  ysics_softbody.i
-00000930: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000940: 6572 7469 6573 5f63 6f6c 6c65 6374 696f  erties_collectio
-00000950: 6e0a 696d 706f 7274 2062 6c5f 6f70 6572  n.import bl_oper
-00000960: 6174 6f72 732e 636f 6e73 7472 6169 6e74  ators.constraint
-00000970: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000980: 746f 7273 2e66 696c 650a 696d 706f 7274  tors.file.import
-00000990: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000009a0: 735f 6461 7461 5f73 7065 616b 6572 0a69  s_data_speaker.i
-000009b0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-000009c0: 7273 2e66 7265 6573 7479 6c65 0a69 6d70  rs.freestyle.imp
-000009d0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-000009e0: 7465 7874 0a69 6d70 6f72 7420 626c 5f75  text.import bl_u
-000009f0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
-00000a00: 615f 656d 7074 790a 696d 706f 7274 2062  a_empty.import b
-00000a10: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000a20: 6461 7461 5f76 6f6c 756d 650a 696d 706f  data_volume.impo
-00000a30: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000a40: 6965 735f 6461 7461 5f6d 6574 6162 616c  ies_data_metabal
-00000a50: 6c0a 0a47 656e 6572 6963 5479 7065 203d  l..GenericType =
+00000040: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000050: 7369 6373 5f66 6c75 6964 0a69 6d70 6f72  sics_fluid.impor
+00000060: 7420 626c 5f6f 7065 7261 746f 7273 2e70  t bl_operators.p
+00000070: 7265 7365 7473 0a69 6d70 6f72 7420 626c  resets.import bl
+00000080: 5f75 692e 7072 6f70 6572 7469 6573 5f77  _ui.properties_w
+00000090: 6f72 6c64 0a69 6d70 6f72 7420 626c 5f75  orld.import bl_u
+000000a0: 692e 7072 6f70 6572 7469 6573 5f6f 7574  i.properties_out
+000000b0: 7075 740a 696d 706f 7274 2062 6c5f 7569  put.import bl_ui
+000000c0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+000000d0: 5f63 616d 6572 610a 696d 706f 7274 2062  _camera.import b
+000000e0: 6c5f 7569 2e73 7061 6365 5f6e 6f64 650a  l_ui.space_node.
+000000f0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+00000100: 6365 5f63 6c69 700a 696d 706f 7274 2062  ce_clip.import b
+00000110: 6c5f 6f70 6572 6174 6f72 732e 6e6f 6465  l_operators.node
+00000120: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000130: 6f70 6572 7469 6573 5f63 6f6c 6c65 6374  operties_collect
+00000140: 696f 6e0a 696d 706f 7274 2062 6c5f 7569  ion.import bl_ui
+00000150: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+00000160: 5f61 726d 6174 7572 650a 696d 706f 7274  _armature.import
+00000170: 2062 6c5f 7569 2e73 7061 6365 5f69 6d61   bl_ui.space_ima
+00000180: 6765 0a69 6d70 6f72 7420 626c 5f75 692e  ge.import bl_ui.
+00000190: 7370 6163 655f 746f 7062 6172 0a69 6d70  space_topbar.imp
+000001a0: 6f72 7420 626c 5f75 692e 6e6f 6465 5f61  ort bl_ui.node_a
+000001b0: 6464 5f6d 656e 755f 6765 6f6d 6574 7279  dd_menu_geometry
+000001c0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
+000001d0: 746f 7273 2e63 6f6e 7374 7261 696e 740a  tors.constraint.
+000001e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000001f0: 6365 5f66 696c 6562 726f 7773 6572 0a69  ce_filebrowser.i
+00000200: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000210: 7273 2e77 6d0a 696d 706f 7274 2062 6c5f  rs.wm.import bl_
+00000220: 7569 2e70 726f 7065 7274 6965 735f 6772  ui.properties_gr
+00000230: 6561 7365 5f70 656e 6369 6c5f 636f 6d6d  ease_pencil_comm
+00000240: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
+00000250: 7370 6163 655f 6e6c 610a 696d 706f 7274  space_nla.import
+00000260: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000270: 735f 7068 7973 6963 735f 7269 6769 6462  s_physics_rigidb
+00000280: 6f64 795f 636f 6e73 7472 6169 6e74 0a69  ody_constraint.i
+00000290: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000002a0: 6572 7469 6573 5f64 6174 615f 706f 696e  erties_data_poin
+000002b0: 7463 6c6f 7564 0a69 6d70 6f72 7420 626c  tcloud.import bl
+000002c0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000002d0: 6174 615f 6d65 7461 6261 6c6c 0a69 6d70  ata_metaball.imp
+000002e0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+000002f0: 7573 6572 7072 6566 0a69 6d70 6f72 7420  userpref.import 
+00000300: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000310: 5f63 6f6e 7374 7261 696e 740a 696d 706f  _constraint.impo
+00000320: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+00000330: 6672 6565 7374 796c 650a 696d 706f 7274  freestyle.import
+00000340: 2062 6c5f 7569 2e73 7061 6365 5f74 6f6f   bl_ui.space_too
+00000350: 6c73 7973 7465 6d5f 636f 6d6d 6f6e 0a69  lsystem_common.i
+00000360: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000370: 655f 7370 7265 6164 7368 6565 740a 696d  e_spreadsheet.im
+00000380: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000390: 7274 6965 735f 7068 7973 6963 735f 7269  rties_physics_ri
+000003a0: 6769 6462 6f64 790a 696d 706f 7274 2062  gidbody.import b
+000003b0: 6c5f 7569 2e73 7061 6365 5f70 726f 7065  l_ui.space_prope
+000003c0: 7274 6965 730a 696d 706f 7274 2062 6c5f  rties.import bl_
+000003d0: 7569 2e70 726f 7065 7274 6965 735f 6461  ui.properties_da
+000003e0: 7461 5f6c 6967 6874 0a69 6d70 6f72 7420  ta_light.import 
+000003f0: 626c 5f75 692e 7370 6163 655f 7465 7874  bl_ui.space_text
+00000400: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000410: 6163 655f 7669 6577 3364 5f74 6f6f 6c62  ace_view3d_toolb
+00000420: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
+00000430: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
+00000440: 6373 5f63 6c6f 7468 0a69 6d70 6f72 7420  cs_cloth.import 
+00000450: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000460: 5f70 6172 7469 636c 650a 696d 706f 7274  _particle.import
+00000470: 2062 6c5f 6f70 6572 6174 6f72 732e 6f62   bl_operators.ob
+00000480: 6a65 6374 0a69 6d70 6f72 7420 626c 5f75  ject.import bl_u
+00000490: 692e 7072 6f70 6572 7469 6573 5f76 6965  i.properties_vie
+000004a0: 775f 6c61 7965 720a 696d 706f 7274 2062  w_layer.import b
+000004b0: 6c5f 6f70 6572 6174 6f72 732e 7573 6572  l_operators.user
+000004c0: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
+000004d0: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+000004e0: 615f 6c69 6768 7470 726f 6265 0a69 6d70  a_lightprobe.imp
+000004f0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000500: 7469 6573 5f64 6174 615f 6d65 7368 0a69  ties_data_mesh.i
+00000510: 6d70 6f72 7420 626c 5f75 690a 696d 706f  mport bl_ui.impo
+00000520: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000530: 6965 735f 6461 7461 5f6d 6f64 6966 6965  ies_data_modifie
+00000540: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
+00000550: 726f 7065 7274 6965 735f 7068 7973 6963  roperties_physic
+00000560: 735f 636f 6d6d 6f6e 0a69 6d70 6f72 7420  s_common.import 
+00000570: 626c 5f75 692e 7370 6163 655f 6772 6170  bl_ui.space_grap
+00000580: 680a 696d 706f 7274 2062 6c5f 7569 2e70  h.import bl_ui.p
+00000590: 726f 7065 7274 6965 735f 6461 7461 5f63  roperties_data_c
+000005a0: 7572 7665 730a 696d 706f 7274 2062 6c5f  urves.import bl_
+000005b0: 6f70 6572 6174 6f72 732e 636c 6970 0a69  operators.clip.i
+000005c0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+000005d0: 6572 7469 6573 5f6d 6174 6572 6961 6c5f  erties_material_
+000005e0: 6770 656e 6369 6c0a 696d 706f 7274 2062  gpencil.import b
+000005f0: 6c5f 7569 2e67 656e 6572 6963 5f75 695f  l_ui.generic_ui_
+00000600: 6c69 7374 0a69 6d70 6f72 7420 626c 5f75  list.import bl_u
+00000610: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000620: 615f 7368 6164 6572 6678 0a69 6d70 6f72  a_shaderfx.impor
+00000630: 7420 626c 5f6f 7065 7261 746f 7273 2e73  t bl_operators.s
+00000640: 7072 6561 6473 6865 6574 0a69 6d70 6f72  preadsheet.impor
+00000650: 7420 626c 5f75 692e 7370 6163 655f 6f75  t bl_ui.space_ou
+00000660: 746c 696e 6572 0a69 6d70 6f72 7420 626c  tliner.import bl
+00000670: 5f75 692e 7370 6163 655f 696e 666f 0a69  _ui.space_info.i
+00000680: 6d70 6f72 7420 626c 5f75 692e 7370 6163  mport bl_ui.spac
+00000690: 655f 7374 6174 7573 6261 720a 696d 706f  e_statusbar.impo
+000006a0: 7274 2062 6c5f 7569 2e73 7061 6365 5f63  rt bl_ui.space_c
+000006b0: 6f6e 736f 6c65 0a69 6d70 6f72 7420 626c  onsole.import bl
+000006c0: 5f75 692e 7072 6f70 6572 7469 6573 5f72  _ui.properties_r
+000006d0: 656e 6465 720a 696d 706f 7274 2062 6c5f  ender.import bl_
+000006e0: 7569 2e70 726f 7065 7274 6965 735f 7465  ui.properties_te
+000006f0: 7874 7572 650a 696d 706f 7274 2062 6c5f  xture.import bl_
+00000700: 7569 2e73 7061 6365 5f73 6571 7565 6e63  ui.space_sequenc
+00000710: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
+00000720: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000730: 656d 7074 790a 696d 706f 7274 2062 6c5f  empty.import bl_
+00000740: 6f70 6572 6174 6f72 732e 6669 6c65 0a69  operators.file.i
+00000750: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000760: 7273 2e61 7373 6574 730a 696d 706f 7274  rs.assets.import
+00000770: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000780: 735f 7068 7973 6963 735f 6669 656c 640a  s_physics_field.
+00000790: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
+000007a0: 6f72 732e 7669 6577 3364 0a69 6d70 6f72  ors.view3d.impor
+000007b0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000007c0: 6573 5f70 6169 6e74 5f63 6f6d 6d6f 6e0a  es_paint_common.
+000007d0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+000007e0: 7065 7274 6965 735f 6461 7461 5f73 7065  perties_data_spe
+000007f0: 616b 6572 0a69 6d70 6f72 7420 626c 5f75  aker.import bl_u
+00000800: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000810: 615f 6770 656e 6369 6c0a 696d 706f 7274  a_gpencil.import
+00000820: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000830: 735f 6461 7461 5f62 6f6e 650a 696d 706f  s_data_bone.impo
+00000840: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+00000850: 616e 696d 0a69 6d70 6f72 7420 626c 5f75  anim.import bl_u
+00000860: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000870: 615f 766f 6c75 6d65 0a69 6d70 6f72 7420  a_volume.import 
+00000880: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000890: 5f6f 626a 6563 740a 696d 706f 7274 2062  _object.import b
+000008a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000008b0: 6461 7461 5f63 7572 7665 0a69 6d70 6f72  data_curve.impor
+000008c0: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000008d0: 6573 5f64 6174 615f 6c61 7474 6963 650a  es_data_lattice.
+000008e0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000008f0: 6365 5f64 6f70 6573 6865 6574 0a69 6d70  ce_dopesheet.imp
+00000900: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
+00000910: 746f 6f6c 7379 7374 656d 5f74 6f6f 6c62  toolsystem_toolb
+00000920: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
+00000930: 7072 6f70 6572 7469 6573 5f6d 6174 6572  properties_mater
+00000940: 6961 6c0a 696d 706f 7274 2062 6c5f 7569  ial.import bl_ui
+00000950: 2e73 7061 6365 5f76 6965 7733 640a 696d  .space_view3d.im
+00000960: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000970: 5f74 696d 650a 696d 706f 7274 2062 6c5f  _time.import bl_
+00000980: 7569 2e70 726f 7065 7274 6965 735f 7068  ui.properties_ph
+00000990: 7973 6963 735f 6479 6e61 6d69 6370 6169  ysics_dynamicpai
+000009a0: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
+000009b0: 7072 6f70 6572 7469 6573 5f73 6365 6e65  properties_scene
+000009c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000009d0: 6f70 6572 7469 6573 5f66 7265 6573 7479  operties_freesty
+000009e0: 6c65 0a69 6d70 6f72 7420 626c 5f75 692e  le.import bl_ui.
+000009f0: 7072 6f70 6572 7469 6573 5f6d 6173 6b5f  properties_mask_
+00000a00: 636f 6d6d 6f6e 0a69 6d70 6f72 7420 626c  common.import bl
+00000a10: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
+00000a20: 6879 7369 6373 5f73 6f66 7462 6f64 790a  hysics_softbody.
+00000a30: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000a40: 7065 7274 6965 735f 776f 726b 7370 6163  perties_workspac
+00000a50: 650a 0a47 656e 6572 6963 5479 7065 203d  e..GenericType =
 00000a60: 2074 7970 696e 672e 5479 7065 5661 7228   typing.TypeVar(
 00000a70: 2247 656e 6572 6963 5479 7065 2229 0a0a  "GenericType")..
-00000a80: 0a63 6c61 7373 2062 7079 5f70 726f 705f  .class bpy_prop_
-00000a90: 636f 6c6c 6563 7469 6f6e 2874 7970 696e  collection(typin
-00000aa0: 672e 4765 6e65 7269 635b 4765 6e65 7269  g.Generic[Generi
-00000ab0: 6354 7970 655d 293a 0a20 2020 2027 2727  cType]):.    '''
-00000ac0: 2062 7569 6c74 2d69 6e20 636c 6173 7320   built-in class 
-00000ad0: 7573 6564 2066 6f72 2061 6c6c 2063 6f6c  used for all col
-00000ae0: 6c65 6374 696f 6e73 2e0a 2020 2020 2727  lections..    ''
-00000af0: 270a 0a20 2020 2064 6566 2066 696e 6428  '..    def find(
-00000b00: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-00000b10: 672e 4f70 7469 6f6e 616c 5b73 7472 5d29  g.Optional[str])
-00000b20: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00000b30: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
-00000b40: 2069 6e64 6578 206f 6620 6120 6b65 7920   index of a key 
-00000b50: 696e 2061 2063 6f6c 6c65 6374 696f 6e20  in a collection 
-00000b60: 6f72 202d 3120 7768 656e 206e 6f74 2066  or -1 when not f
-00000b70: 6f75 6e64 2028 6d61 7463 6865 7320 5079  ound (matches Py
-00000b80: 7468 6f6e 2773 2073 7472 696e 6720 6669  thon's string fi
-00000b90: 6e64 2066 756e 6374 696f 6e20 6f66 2074  nd function of t
-00000ba0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
-00000bb0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-00000bc0: 6579 3a20 5468 6520 6964 656e 7469 6669  ey: The identifi
-00000bd0: 6572 2066 6f72 2074 6865 2063 6f6c 6c65  er for the colle
-00000be0: 6374 696f 6e20 6d65 6d62 6572 2e0a 2020  ction member..  
-00000bf0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-00000c00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00000c10: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
-00000c20: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
-00000c30: 2020 3a72 6574 7572 6e3a 2069 6e64 6578    :return: index
-00000c40: 206f 6620 7468 6520 6b65 792e 0a20 2020   of the key..   
-00000c50: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00000c60: 2070 6173 730a 0a20 2020 2064 6566 2066   pass..    def f
-00000c70: 6f72 6561 6368 5f67 6574 2873 656c 662c  oreach_get(self,
-00000c80: 2061 7474 722c 2073 6571 293a 0a20 2020   attr, seq):.   
-00000c90: 2020 2020 2027 2727 2054 6869 7320 6973       ''' This is
-00000ca0: 2061 2066 756e 6374 696f 6e20 746f 2067   a function to g
-00000cb0: 6976 6520 6661 7374 2061 6363 6573 7320  ive fast access 
-00000cc0: 746f 2061 7474 7269 6275 7465 7320 7769  to attributes wi
-00000cd0: 7468 696e 2061 2063 6f6c 6c65 6374 696f  thin a collectio
-00000ce0: 6e2e 204f 6e6c 7920 776f 726b 7320 666f  n. Only works fo
-00000cf0: 7220 2762 6173 6963 2074 7970 6527 2070  r 'basic type' p
-00000d00: 726f 7065 7274 6965 7320 2862 6f6f 6c2c  roperties (bool,
-00000d10: 2069 6e74 2061 6e64 2066 6c6f 6174 2921   int and float)!
-00000d20: 204d 756c 7469 2d64 696d 656e 7369 6f6e   Multi-dimension
-00000d30: 616c 2061 7272 6179 7320 286c 696b 6520  al arrays (like 
-00000d40: 6172 7261 7920 6f66 2076 6563 746f 7273  array of vectors
-00000d50: 2920 7769 6c6c 2062 6520 666c 6174 7465  ) will be flatte
-00000d60: 6e65 6420 696e 746f 2073 6571 2e0a 0a20  ned into seq... 
-00000d70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00000d80: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00000d90: 2066 6f72 6561 6368 5f73 6574 2873 656c   foreach_set(sel
-00000da0: 662c 2061 7474 722c 2073 6571 293a 0a20  f, attr, seq):. 
-00000db0: 2020 2020 2020 2027 2727 2054 6869 7320         ''' This 
-00000dc0: 6973 2061 2066 756e 6374 696f 6e20 746f  is a function to
-00000dd0: 2067 6976 6520 6661 7374 2061 6363 6573   give fast acces
-00000de0: 7320 746f 2061 7474 7269 6275 7465 7320  s to attributes 
-00000df0: 7769 7468 696e 2061 2063 6f6c 6c65 6374  within a collect
-00000e00: 696f 6e2e 204f 6e6c 7920 776f 726b 7320  ion. Only works 
-00000e10: 666f 7220 2762 6173 6963 2074 7970 6527  for 'basic type'
-00000e20: 2070 726f 7065 7274 6965 7320 2862 6f6f   properties (boo
-00000e30: 6c2c 2069 6e74 2061 6e64 2066 6c6f 6174  l, int and float
-00000e40: 2921 2073 6571 206d 7573 7420 6265 2075  )! seq must be u
-00000e50: 6e69 2d64 696d 656e 7369 6f6e 616c 2c20  ni-dimensional, 
-00000e60: 6d75 6c74 692d 6469 6d65 6e73 696f 6e61  multi-dimensiona
-00000e70: 6c20 6172 7261 7973 2028 6c69 6b65 2061  l arrays (like a
-00000e80: 7272 6179 206f 6620 7665 6374 6f72 7329  rray of vectors)
-00000e90: 2077 696c 6c20 6265 2072 652d 6372 6561   will be re-crea
-00000ea0: 7465 6420 6672 6f6d 2069 742e 0a0a 2020  ted from it...  
-00000eb0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00000ec0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00000ed0: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
-00000ee0: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
-00000ef0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
-00000f00: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-00000f10: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
-00000f20: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
-00000f30: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
-00000f40: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
-00000f50: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00000f60: 6974 656d 2061 7373 6967 6e65 6420 746f  item assigned to
-00000f70: 206b 6579 206f 7220 6465 6661 756c 7420   key or default 
-00000f80: 7768 656e 206e 6f74 2066 6f75 6e64 2028  when not found (
-00000f90: 6d61 7463 6865 7320 5079 7468 6f6e 2773  matches Python's
-00000fa0: 2064 6963 7469 6f6e 6172 7920 6675 6e63   dictionary func
-00000fb0: 7469 6f6e 206f 6620 7468 6520 7361 6d65  tion of the same
-00000fc0: 206e 616d 6529 2e0a 0a20 2020 2020 2020   name)...       
-00000fd0: 203a 7061 7261 6d20 6b65 793a 2054 6865   :param key: The
-00000fe0: 2069 6465 6e74 6966 6965 7220 666f 7220   identifier for 
-00000ff0: 7468 6520 636f 6c6c 6563 7469 6f6e 206d  the collection m
-00001000: 656d 6265 722e 0a20 2020 2020 2020 203a  ember..        :
-00001010: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
-00001020: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00001030: 2020 2020 2020 203a 7061 7261 6d20 6465         :param de
-00001040: 6661 756c 743a 204f 7074 696f 6e61 6c20  fault: Optional 
-00001050: 6172 6775 6d65 6e74 2066 6f72 2074 6865  argument for the
-00001060: 2076 616c 7565 2074 6f20 7265 7475 726e   value to return
-00001070: 2069 6620 2a6b 6579 2a20 6973 206e 6f74   if *key* is not
-00001080: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
-00001090: 3a74 7970 6520 6465 6661 756c 743a 2074  :type default: t
-000010a0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-000010b0: 7970 696e 672e 416e 795d 0a20 2020 2020  yping.Any].     
-000010c0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-000010d0: 6173 730a 0a20 2020 2064 6566 2069 7465  ass..    def ite
-000010e0: 6d73 2873 656c 6629 202d 3e20 7479 7069  ms(self) -> typi
-000010f0: 6e67 2e4c 6973 743a 0a20 2020 2020 2020  ng.List:.       
-00001100: 2027 2727 2052 6574 7572 6e20 7468 6520   ''' Return the 
-00001110: 6964 656e 7469 6669 6572 7320 6f66 2063  identifiers of c
-00001120: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
-00001130: 7320 286d 6174 6368 696e 6720 5079 7468  s (matching Pyth
-00001140: 6f6e 2773 2064 6963 742e 6974 656d 7328  on's dict.items(
-00001150: 2920 6675 6e63 7469 6f6e 616c 6974 7929  ) functionality)
-00001160: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
-00001170: 653a 2074 7970 696e 672e 4c69 7374 0a20  e: typing.List. 
-00001180: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00001190: 286b 6579 2c20 7661 6c75 6529 2070 6169  (key, value) pai
-000011a0: 7273 2066 6f72 2065 6163 6820 6d65 6d62  rs for each memb
-000011b0: 6572 206f 6620 7468 6973 2063 6f6c 6c65  er of this colle
-000011c0: 6374 696f 6e2e 0a20 2020 2020 2020 2027  ction..        '
-000011d0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-000011e0: 0a20 2020 2064 6566 206b 6579 7328 7365  .    def keys(se
-000011f0: 6c66 2920 2d3e 2074 7970 696e 672e 4c69  lf) -> typing.Li
-00001200: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
-00001210: 2027 2727 2052 6574 7572 6e20 7468 6520   ''' Return the 
-00001220: 6964 656e 7469 6669 6572 7320 6f66 2063  identifiers of c
-00001230: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
-00001240: 7320 286d 6174 6368 696e 6720 5079 7468  s (matching Pyth
-00001250: 6f6e 2773 2064 6963 742e 6b65 7973 2829  on's dict.keys()
-00001260: 2066 756e 6374 696f 6e61 6c69 7479 292e   functionality).
-00001270: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00001280: 3a20 7479 7069 6e67 2e4c 6973 745b 7374  : typing.List[st
-00001290: 725d 0a20 2020 2020 2020 203a 7265 7475  r].        :retu
-000012a0: 726e 3a20 7468 6520 6964 656e 7469 6669  rn: the identifi
-000012b0: 6572 7320 666f 7220 6561 6368 206d 656d  ers for each mem
-000012c0: 6265 7220 6f66 2074 6869 7320 636f 6c6c  ber of this coll
-000012d0: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
-000012e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000012f0: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
-00001300: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
-00001310: 2e4c 6973 743a 0a20 2020 2020 2020 2027  .List:.        '
-00001320: 2727 2052 6574 7572 6e20 7468 6520 7661  '' Return the va
-00001330: 6c75 6573 206f 6620 636f 6c6c 6563 7469  lues of collecti
-00001340: 6f6e 2028 6d61 7463 6869 6e67 2050 7974  on (matching Pyt
-00001350: 686f 6e27 7320 6469 6374 2e76 616c 7565  hon's dict.value
-00001360: 7328 2920 6675 6e63 7469 6f6e 616c 6974  s() functionalit
-00001370: 7929 2e0a 0a20 2020 2020 2020 203a 7274  y)...        :rt
-00001380: 7970 653a 2074 7970 696e 672e 4c69 7374  ype: typing.List
-00001390: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000013a0: 3a20 7468 6520 6d65 6d62 6572 7320 6f66  : the members of
-000013b0: 2074 6869 7320 636f 6c6c 6563 7469 6f6e   this collection
-000013c0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-000013d0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000013e0: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
-000013f0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-00001400: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00001410: 5d29 202d 3e20 2747 656e 6572 6963 5479  ]) -> 'GenericTy
-00001420: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
-00001430: 200a 0a20 2020 2020 2020 203a 7061 7261   ..        :para
-00001440: 6d20 6b65 793a 200a 2020 2020 2020 2020  m key: .        
-00001450: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
-00001460: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00001470: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
-00001480: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
-00001490: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-000014a0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000014b0: 6620 5f5f 7365 7469 7465 6d5f 5f28 7365  f __setitem__(se
-000014c0: 6c66 2c20 6b65 793a 2074 7970 696e 672e  lf, key: typing.
-000014d0: 556e 696f 6e5b 696e 742c 2073 7472 5d2c  Union[int, str],
-000014e0: 2076 616c 7565 3a20 2747 656e 6572 6963   value: 'Generic
-000014f0: 5479 7065 2729 3a0a 2020 2020 2020 2020  Type'):.        
-00001500: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-00001510: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-00001520: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-00001530: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00001540: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
-00001550: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
-00001560: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
-00001570: 2027 4765 6e65 7269 6354 7970 6527 0a20   'GenericType'. 
-00001580: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00001590: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-000015a0: 205f 5f64 656c 6974 656d 5f5f 2873 656c   __delitem__(sel
-000015b0: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
-000015c0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2920  nion[int, str]) 
-000015d0: 2d3e 2027 4765 6e65 7269 6354 7970 6527  -> 'GenericType'
-000015e0: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
-000015f0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
-00001600: 6579 3a20 0a20 2020 2020 2020 203a 7479  ey: .        :ty
-00001610: 7065 206b 6579 3a20 7479 7069 6e67 2e55  pe key: typing.U
-00001620: 6e69 6f6e 5b69 6e74 2c20 7374 725d 0a20  nion[int, str]. 
-00001630: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
-00001640: 4765 6e65 7269 6354 7970 6527 0a20 2020  GenericType'.   
-00001650: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00001660: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
-00001670: 5f69 7465 725f 5f28 7365 6c66 2920 2d3e  _iter__(self) ->
-00001680: 2074 7970 696e 672e 4974 6572 6174 6f72   typing.Iterator
-00001690: 5b27 4765 6e65 7269 6354 7970 6527 5d3a  ['GenericType']:
-000016a0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-000016b0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
-000016c0: 7970 696e 672e 4974 6572 6174 6f72 5b27  yping.Iterator['
-000016d0: 4765 6e65 7269 6354 7970 6527 5d0a 2020  GenericType'].  
-000016e0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000016f0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00001700: 5f5f 6e65 7874 5f5f 2873 656c 6629 202d  __next__(self) -
-00001710: 3e20 2747 656e 6572 6963 5479 7065 273a  > 'GenericType':
-00001720: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-00001730: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
-00001740: 4765 6e65 7269 6354 7970 6527 0a20 2020  GenericType'.   
-00001750: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00001760: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
-00001770: 5f6c 656e 5f5f 2873 656c 6629 202d 3e20  _len__(self) -> 
-00001780: 696e 743a 0a20 2020 2020 2020 2027 2727  int:.        '''
-00001790: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
-000017a0: 653a 2069 6e74 0a20 2020 2020 2020 2027  e: int.        '
-000017b0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-000017c0: 0a0a 636c 6173 7320 6270 795f 7374 7275  ..class bpy_stru
-000017d0: 6374 3a0a 2020 2020 2727 2720 6275 696c  ct:.    ''' buil
-000017e0: 742d 696e 2062 6173 6520 636c 6173 7320  t-in base class 
-000017f0: 666f 7220 616c 6c20 636c 6173 7365 7320  for all classes 
-00001800: 696e 2062 7079 2e74 7970 6573 2e0a 2020  in bpy.types..  
-00001810: 2020 2727 270a 0a20 2020 2069 645f 6461    '''..    id_da
-00001820: 7461 203d 204e 6f6e 650a 2020 2020 2727  ta = None.    ''
-00001830: 2720 5468 6520 6062 7079 2e74 7970 6573  ' The `bpy.types
-00001840: 2e49 4460 206f 626a 6563 7420 7468 6973  .ID` object this
-00001850: 2064 6174 6162 6c6f 636b 2069 7320 6672   datablock is fr
-00001860: 6f6d 206f 7220 4e6f 6e65 2c20 286e 6f74  om or None, (not
-00001870: 2061 7661 696c 6162 6c65 2066 6f72 2061   available for a
-00001880: 6c6c 2064 6174 6120 7479 7065 7329 2727  ll data types)''
-00001890: 270a 0a20 2020 2064 6566 2061 735f 706f  '..    def as_po
-000018a0: 696e 7465 7228 7365 6c66 2920 2d3e 2069  inter(self) -> i
-000018b0: 6e74 3a0a 2020 2020 2020 2020 2727 2720  nt:.        ''' 
-000018c0: 5265 7475 726e 7320 7468 6520 6d65 6d6f  Returns the memo
-000018d0: 7279 2061 6464 7265 7373 2077 6869 6368  ry address which
-000018e0: 2068 6f6c 6473 2061 2070 6f69 6e74 6572   holds a pointer
-000018f0: 2074 6f20 426c 656e 6465 7227 7320 696e   to Blender's in
-00001900: 7465 726e 616c 2064 6174 610a 0a20 2020  ternal data..   
-00001910: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00001920: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00001930: 3a20 696e 7420 286d 656d 6f72 7920 6164  : int (memory ad
-00001940: 6472 6573 7329 2e0a 2020 2020 2020 2020  dress)..        
-00001950: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00001960: 0a0a 2020 2020 6465 6620 6472 6976 6572  ..    def driver
-00001970: 5f61 6464 2873 656c 662c 0a20 2020 2020  _add(self,.     
-00001980: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00001990: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
-000019a0: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
-000019b0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-000019c0: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
-000019d0: 6e61 6c5b 696e 745d 203d 202d 3129 202d  nal[int] = -1) -
-000019e0: 3e20 2746 4375 7276 6527 3a0a 2020 2020  > 'FCurve':.    
-000019f0: 2020 2020 2727 2720 4164 6473 2064 7269      ''' Adds dri
-00001a00: 7665 7228 7329 2074 6f20 7468 6520 6769  ver(s) to the gi
-00001a10: 7665 6e20 7072 6f70 6572 7479 0a0a 2020  ven property..  
-00001a20: 2020 2020 2020 3a70 6172 616d 2070 6174        :param pat
-00001a30: 683a 2070 6174 6820 746f 2074 6865 2070  h: path to the p
-00001a40: 726f 7065 7274 7920 746f 2064 7269 7665  roperty to drive
-00001a50: 2c20 616e 616c 6f67 6f75 7320 746f 2074  , analogous to t
-00001a60: 6865 2066 6375 7276 6527 7320 6461 7461  he fcurve's data
-00001a70: 2070 6174 682e 0a20 2020 2020 2020 203a   path..        :
-00001a80: 7479 7065 2070 6174 683a 2074 7970 696e  type path: typin
-00001a90: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-00001aa0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00001ab0: 6e64 6578 3a20 6172 7261 7920 696e 6465  ndex: array inde
-00001ac0: 7820 6f66 2074 6865 2070 726f 7065 7274  x of the propert
-00001ad0: 7920 6472 6976 652e 2044 6566 6175 6c74  y drive. Default
-00001ae0: 7320 746f 202d 3120 666f 7220 616c 6c20  s to -1 for all 
-00001af0: 696e 6469 6365 7320 6f72 2061 2073 696e  indices or a sin
-00001b00: 676c 6520 6368 616e 6e65 6c20 6966 2074  gle channel if t
-00001b10: 6865 2070 726f 7065 7274 7920 6973 206e  he property is n
-00001b20: 6f74 2061 6e20 6172 7261 792e 0a20 2020  ot an array..   
-00001b30: 2020 2020 203a 7479 7065 2069 6e64 6578       :type index
+00000a80: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
+00000a90: 743a 0a20 2020 2027 2727 2062 7569 6c74  t:.    ''' built
+00000aa0: 2d69 6e20 6261 7365 2063 6c61 7373 2066  -in base class f
+00000ab0: 6f72 2061 6c6c 2063 6c61 7373 6573 2069  or all classes i
+00000ac0: 6e20 6270 792e 7479 7065 732e 0a20 2020  n bpy.types..   
+00000ad0: 2027 2727 0a0a 2020 2020 6964 5f64 6174   '''..    id_dat
+00000ae0: 6120 3d20 4e6f 6e65 0a20 2020 2027 2727  a = None.    '''
+00000af0: 2054 6865 2060 6270 792e 7479 7065 732e   The `bpy.types.
+00000b00: 4944 6020 6f62 6a65 6374 2074 6869 7320  ID` object this 
+00000b10: 6461 7461 626c 6f63 6b20 6973 2066 726f  datablock is fro
+00000b20: 6d20 6f72 204e 6f6e 652c 2028 6e6f 7420  m or None, (not 
+00000b30: 6176 6169 6c61 626c 6520 666f 7220 616c  available for al
+00000b40: 6c20 6461 7461 2074 7970 6573 2927 2727  l data types)'''
+00000b50: 0a0a 2020 2020 6465 6620 6173 5f70 6f69  ..    def as_poi
+00000b60: 6e74 6572 2873 656c 6629 202d 3e20 696e  nter(self) -> in
+00000b70: 743a 0a20 2020 2020 2020 2027 2727 2052  t:.        ''' R
+00000b80: 6574 7572 6e73 2074 6865 206d 656d 6f72  eturns the memor
+00000b90: 7920 6164 6472 6573 7320 7768 6963 6820  y address which 
+00000ba0: 686f 6c64 7320 6120 706f 696e 7465 7220  holds a pointer 
+00000bb0: 746f 2042 6c65 6e64 6572 2773 2069 6e74  to Blender's int
+00000bc0: 6572 6e61 6c20 6461 7461 0a0a 2020 2020  ernal data..    
+00000bd0: 2020 2020 3a72 7479 7065 3a20 696e 740a      :rtype: int.
+00000be0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00000bf0: 2069 6e74 2028 6d65 6d6f 7279 2061 6464   int (memory add
+00000c00: 7265 7373 292e 0a20 2020 2020 2020 2027  ress)..        '
+00000c10: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00000c20: 0a20 2020 2064 6566 2064 7269 7665 725f  .    def driver_
+00000c30: 6164 6428 7365 6c66 2c0a 2020 2020 2020  add(self,.      
+00000c40: 2020 2020 2020 2020 2020 2020 2070 6174               pat
+00000c50: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+00000c60: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
+00000c70: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00000c80: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00000c90: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
+00000ca0: 2027 4643 7572 7665 273a 0a20 2020 2020   'FCurve':.     
+00000cb0: 2020 2027 2727 2041 6464 7320 6472 6976     ''' Adds driv
+00000cc0: 6572 2873 2920 746f 2074 6865 2067 6976  er(s) to the giv
+00000cd0: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
+00000ce0: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
+00000cf0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
+00000d00: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
+00000d10: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
+00000d20: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
+00000d30: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
+00000d40: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
+00000d50: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00000d60: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+00000d70: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
+00000d80: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00000d90: 2064 7269 7665 2e20 4465 6661 756c 7473   drive. Defaults
+00000da0: 2074 6f20 2d31 2066 6f72 2061 6c6c 2069   to -1 for all i
+00000db0: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
+00000dc0: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
+00000dd0: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
+00000de0: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
+00000df0: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
+00000e00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00000e10: 5b69 6e74 5d0a 2020 2020 2020 2020 3a72  [int].        :r
+00000e20: 7479 7065 3a20 2746 4375 7276 6527 0a20  type: 'FCurve'. 
+00000e30: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00000e40: 5468 6520 6472 6976 6572 2873 2920 6164  The driver(s) ad
+00000e50: 6465 642e 0a20 2020 2020 2020 2027 2727  ded..        '''
+00000e60: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00000e70: 2020 2064 6566 2064 7269 7665 725f 7265     def driver_re
+00000e80: 6d6f 7665 2873 656c 662c 0a20 2020 2020  move(self,.     
+00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ea0: 2070 6174 683a 2074 7970 696e 672e 4f70   path: typing.Op
+00000eb0: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
+00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ed0: 2020 2069 6e64 6578 3a20 7479 7069 6e67     index: typing
+00000ee0: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
+00000ef0: 202d 3129 202d 3e20 626f 6f6c 3a0a 2020   -1) -> bool:.  
+00000f00: 2020 2020 2020 2727 2720 5265 6d6f 7665        ''' Remove
+00000f10: 2064 7269 7665 7228 7329 2066 726f 6d20   driver(s) from 
+00000f20: 7468 6520 6769 7665 6e20 7072 6f70 6572  the given proper
+00000f30: 7479 0a0a 2020 2020 2020 2020 3a70 6172  ty..        :par
+00000f40: 616d 2070 6174 683a 2070 6174 6820 746f  am path: path to
+00000f50: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
+00000f60: 2064 7269 7665 2c20 616e 616c 6f67 6f75   drive, analogou
+00000f70: 7320 746f 2074 6865 2066 6375 7276 6527  s to the fcurve'
+00000f80: 7320 6461 7461 2070 6174 682e 0a20 2020  s data path..   
+00000f90: 2020 2020 203a 7479 7065 2070 6174 683a       :type path:
+00000fa0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00000fb0: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
+00000fc0: 6172 616d 2069 6e64 6578 3a20 6172 7261  aram index: arra
+00000fd0: 7920 696e 6465 7820 6f66 2074 6865 2070  y index of the p
+00000fe0: 726f 7065 7274 7920 6472 6976 652e 2044  roperty drive. D
+00000ff0: 6566 6175 6c74 7320 746f 202d 3120 666f  efaults to -1 fo
+00001000: 7220 616c 6c20 696e 6469 6365 7320 6f72  r all indices or
+00001010: 2061 2073 696e 676c 6520 6368 616e 6e65   a single channe
+00001020: 6c20 6966 2074 6865 2070 726f 7065 7274  l if the propert
+00001030: 7920 6973 206e 6f74 2061 6e20 6172 7261  y is not an arra
+00001040: 792e 0a20 2020 2020 2020 203a 7479 7065  y..        :type
+00001050: 2069 6e64 6578 3a20 7479 7069 6e67 2e4f   index: typing.O
+00001060: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
+00001070: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00001080: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+00001090: 6e3a 2053 7563 6365 7373 206f 6620 6472  n: Success of dr
+000010a0: 6976 6572 2072 656d 6f76 616c 2e0a 2020  iver removal..  
+000010b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000010c0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+000010d0: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
+000010e0: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
+000010f0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
+00001100: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00001110: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+00001120: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00001130: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
+00001140: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
+00001150: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00001160: 6375 7374 6f6d 2070 726f 7065 7274 7920  custom property 
+00001170: 6173 7369 676e 6564 2074 6f20 6b65 7920  assigned to key 
+00001180: 6f72 2064 6566 6175 6c74 2077 6865 6e20  or default when 
+00001190: 6e6f 7420 666f 756e 6420 286d 6174 6368  not found (match
+000011a0: 6573 2050 7974 686f 6e27 7320 6469 6374  es Python's dict
+000011b0: 696f 6e61 7279 2066 756e 6374 696f 6e20  ionary function 
+000011c0: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
+000011d0: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
+000011e0: 616d 206b 6579 3a20 5468 6520 6b65 7920  am key: The key 
+000011f0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00001200: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
+00001210: 7274 792e 0a20 2020 2020 2020 203a 7479  rty..        :ty
+00001220: 7065 206b 6579 3a20 7479 7069 6e67 2e4f  pe key: typing.O
+00001230: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
+00001240: 2020 2020 203a 7061 7261 6d20 6465 6661       :param defa
+00001250: 756c 743a 204f 7074 696f 6e61 6c20 6172  ult: Optional ar
+00001260: 6775 6d65 6e74 2066 6f72 2074 6865 2076  gument for the v
+00001270: 616c 7565 2074 6f20 7265 7475 726e 2069  alue to return i
+00001280: 6620 2a6b 6579 2a20 6973 206e 6f74 2066  f *key* is not f
+00001290: 6f75 6e64 2e0a 2020 2020 2020 2020 3a74  ound..        :t
+000012a0: 7970 6520 6465 6661 756c 743a 2074 7970  ype default: typ
+000012b0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+000012c0: 696e 672e 416e 795d 0a20 2020 2020 2020  ing.Any].       
+000012d0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+000012e0: 730a 0a20 2020 2064 6566 2069 645f 7072  s..    def id_pr
+000012f0: 6f70 6572 7469 6573 5f63 6c65 6172 2873  operties_clear(s
+00001300: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
+00001310: 2720 0a0a 2020 2020 2020 2020 2727 270a  ' ..        '''.
+00001320: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00001330: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
+00001340: 6965 735f 656e 7375 7265 2873 656c 6629  ies_ensure(self)
+00001350: 202d 3e20 7479 7069 6e67 2e41 6e79 3a0a   -> typing.Any:.
+00001360: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+00001370: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
+00001380: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
+00001390: 203a 7265 7475 726e 3a20 7468 6520 7061   :return: the pa
+000013a0: 7265 6e74 2067 726f 7570 2066 6f72 2061  rent group for a
+000013b0: 6e20 524e 4120 7374 7275 6374 2773 2063  n RNA struct's c
+000013c0: 7573 746f 6d20 4944 5072 6f70 6572 7469  ustom IDProperti
+000013d0: 6573 2e0a 2020 2020 2020 2020 2727 270a  es..        '''.
+000013e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000013f0: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
+00001400: 6965 735f 7569 2873 656c 662c 206b 6579  ies_ui(self, key
+00001410: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00001420: 6c5b 7479 7069 6e67 2e41 6e79 5d29 202d  l[typing.Any]) -
+00001430: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
+00001440: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
+00001450: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
+00001460: 2053 7472 696e 6720 6e61 6d65 206f 6620   String name of 
+00001470: 7468 6520 7072 6f70 6572 7479 2e0a 2020  the property..  
+00001480: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00001490: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000014a0: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
+000014b0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
+000014c0: 696e 672e 416e 790a 2020 2020 2020 2020  ing.Any.        
+000014d0: 3a72 6574 7572 6e3a 2052 6574 7572 6e20  :return: Return 
+000014e0: 616e 206f 626a 6563 7420 7573 6564 2074  an object used t
+000014f0: 6f20 6d61 6e61 6765 2061 6e20 4944 5072  o manage an IDPr
+00001500: 6f70 6572 7479 2773 2055 4920 6461 7461  operty's UI data
+00001510: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00001520: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00001530: 6465 6620 6973 5f70 726f 7065 7274 795f  def is_property_
+00001540: 6869 6464 656e 2873 656c 662c 2070 726f  hidden(self, pro
+00001550: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
+00001560: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
+00001570: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
+00001580: 6973 2068 6964 6465 6e2e 0a0a 2020 2020  is hidden...    
+00001590: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+000015a0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000015b0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
+000015c0: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
+000015d0: 656e 2e0a 2020 2020 2020 2020 2727 270a  en..        '''.
+000015e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000015f0: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
+00001600: 795f 6f76 6572 7269 6461 626c 655f 6c69  y_overridable_li
+00001610: 6272 6172 7928 7365 6c66 2c20 7072 6f70  brary(self, prop
+00001620: 6572 7479 2920 2d3e 2062 6f6f 6c3a 0a20  erty) -> bool:. 
+00001630: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
+00001640: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
+00001650: 7320 6f76 6572 7269 6461 626c 652e 0a0a  s overridable...
+00001660: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00001670: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
+00001680: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
+00001690: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
+000016a0: 6f76 6572 7269 6461 626c 652e 0a20 2020  overridable..   
+000016b0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+000016c0: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
+000016d0: 735f 7072 6f70 6572 7479 5f72 6561 646f  s_property_reado
+000016e0: 6e6c 7928 7365 6c66 2c20 7072 6f70 6572  nly(self, proper
+000016f0: 7479 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ty) -> bool:.   
+00001700: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
+00001710: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
+00001720: 7265 6164 6f6e 6c79 2e0a 0a20 2020 2020  readonly...     
+00001730: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
+00001740: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001750: 2054 7275 6520 7768 656e 2074 6865 2070   True when the p
+00001760: 726f 7065 7274 7920 6973 2072 6561 646f  roperty is reado
+00001770: 6e6c 7920 286e 6f74 2077 7269 7461 626c  nly (not writabl
+00001780: 6529 2e0a 2020 2020 2020 2020 2727 270a  e)..        '''.
+00001790: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+000017a0: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
+000017b0: 795f 7365 7428 7365 6c66 2c20 7072 6f70  y_set(self, prop
+000017c0: 6572 7479 2c0a 2020 2020 2020 2020 2020  erty,.          
+000017d0: 2020 2020 2020 2020 2020 2020 2020 6768                gh
+000017e0: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
+000017f0: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
+00001800: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
+00001810: 2020 2020 2727 2720 4368 6563 6b20 6966      ''' Check if
+00001820: 2061 2070 726f 7065 7274 7920 6973 2073   a property is s
+00001830: 6574 2c20 7573 6520 666f 7220 7465 7374  et, use for test
+00001840: 696e 6720 6f70 6572 6174 6f72 2070 726f  ing operator pro
+00001850: 7065 7274 6965 732e 0a0a 2020 2020 2020  perties...      
+00001860: 2020 3a70 6172 616d 2067 686f 7374 3a20    :param ghost: 
+00001870: 5573 6564 2066 6f72 206f 7065 7261 746f  Used for operato
+00001880: 7273 2074 6861 7420 7265 2d72 756e 2077  rs that re-run w
+00001890: 6974 6820 7072 6576 696f 7573 2073 6574  ith previous set
+000018a0: 7469 6e67 732e 2049 6e20 7468 6973 2063  tings. In this c
+000018b0: 6173 6520 7468 6520 7072 6f70 6572 7479  ase the property
+000018c0: 2069 7320 6e6f 7420 6d61 726b 6564 2061   is not marked a
+000018d0: 7320 7365 742c 2079 6574 2074 6865 2076  s set, yet the v
+000018e0: 616c 7565 2066 726f 6d20 7468 6520 7072  alue from the pr
+000018f0: 6576 696f 7573 2065 7865 6375 7469 6f6e  evious execution
+00001900: 2069 7320 7573 6564 2e20 496e 2072 6172   is used. In rar
+00001910: 6520 6361 7365 7320 796f 7520 6d61 7920  e cases you may 
+00001920: 7761 6e74 2074 6f20 7365 7420 7468 6973  want to set this
+00001930: 206f 7074 696f 6e20 746f 2066 616c 7365   option to false
+00001940: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00001950: 6768 6f73 743a 2074 7970 696e 672e 4f70  ghost: typing.Op
+00001960: 7469 6f6e 616c 5b62 6f6f 6c5d 0a20 2020  tional[bool].   
+00001970: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00001980: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+00001990: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
+000019a0: 2070 726f 7065 7274 7920 6861 7320 6265   property has be
+000019b0: 656e 2073 6574 2e0a 2020 2020 2020 2020  en set..        
+000019c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000019d0: 0a0a 2020 2020 6465 6620 6974 656d 7328  ..    def items(
+000019e0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
+000019f0: 416e 793a 0a20 2020 2020 2020 2027 2727  Any:.        '''
+00001a00: 2052 6574 7572 6e73 2074 6865 2069 7465   Returns the ite
+00001a10: 6d73 206f 6620 7468 6973 206f 626a 6563  ms of this objec
+00001a20: 7473 2063 7573 746f 6d20 7072 6f70 6572  ts custom proper
+00001a30: 7469 6573 2028 6d61 7463 6865 7320 5079  ties (matches Py
+00001a40: 7468 6f6e 2773 2064 6963 7469 6f6e 6172  thon's dictionar
+00001a50: 7920 6675 6e63 7469 6f6e 206f 6620 7468  y function of th
+00001a60: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
+00001a70: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+00001a80: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
+00001a90: 2020 3a72 6574 7572 6e3a 2063 7573 746f    :return: custo
+00001aa0: 6d20 7072 6f70 6572 7479 206b 6579 2c20  m property key, 
+00001ab0: 7661 6c75 6520 7061 6972 732e 0a20 2020  value pairs..   
+00001ac0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001ad0: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
+00001ae0: 6579 6672 616d 655f 6465 6c65 7465 280a  eyframe_delete(.
+00001af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001b00: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00001b10: 7461 5f70 6174 683a 2074 7970 696e 672e  ta_path: typing.
+00001b20: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
+00001b30: 2020 2020 2020 2020 2020 2069 6e64 6578             index
 00001b40: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001b50: 6c5b 696e 745d 0a20 2020 2020 2020 203a  l[int].        :
-00001b60: 7274 7970 653a 2027 4643 7572 7665 270a  rtype: 'FCurve'.
-00001b70: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00001b80: 2054 6865 2064 7269 7665 7228 7329 2061   The driver(s) a
-00001b90: 6464 6564 2e0a 2020 2020 2020 2020 2727  dded..        ''
-00001ba0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00001bb0: 2020 2020 6465 6620 6472 6976 6572 5f72      def driver_r
-00001bc0: 656d 6f76 6528 7365 6c66 2c0a 2020 2020  emove(self,.    
-00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001be0: 2020 7061 7468 3a20 7479 7069 6e67 2e4f    path: typing.O
-00001bf0: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
-00001c20: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
-00001c30: 3d20 2d31 2920 2d3e 2062 6f6f 6c3a 0a20  = -1) -> bool:. 
-00001c40: 2020 2020 2020 2027 2727 2052 656d 6f76         ''' Remov
-00001c50: 6520 6472 6976 6572 2873 2920 6672 6f6d  e driver(s) from
-00001c60: 2074 6865 2067 6976 656e 2070 726f 7065   the given prope
-00001c70: 7274 790a 0a20 2020 2020 2020 203a 7061  rty..        :pa
-00001c80: 7261 6d20 7061 7468 3a20 7061 7468 2074  ram path: path t
-00001c90: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
-00001ca0: 6f20 6472 6976 652c 2061 6e61 6c6f 676f  o drive, analogo
-00001cb0: 7573 2074 6f20 7468 6520 6663 7572 7665  us to the fcurve
-00001cc0: 2773 2064 6174 6120 7061 7468 2e0a 2020  's data path..  
-00001cd0: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
-00001ce0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001cf0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
-00001d00: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
-00001d10: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
-00001d20: 7072 6f70 6572 7479 2064 7269 7665 2e20  property drive. 
-00001d30: 4465 6661 756c 7473 2074 6f20 2d31 2066  Defaults to -1 f
-00001d40: 6f72 2061 6c6c 2069 6e64 6963 6573 206f  or all indices o
-00001d50: 7220 6120 7369 6e67 6c65 2063 6861 6e6e  r a single chann
-00001d60: 656c 2069 6620 7468 6520 7072 6f70 6572  el if the proper
-00001d70: 7479 2069 7320 6e6f 7420 616e 2061 7272  ty is not an arr
-00001d80: 6179 2e0a 2020 2020 2020 2020 3a74 7970  ay..        :typ
-00001d90: 6520 696e 6465 783a 2074 7970 696e 672e  e index: typing.
-00001da0: 4f70 7469 6f6e 616c 5b69 6e74 5d0a 2020  Optional[int].  
-00001db0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
-00001dc0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
-00001dd0: 726e 3a20 5375 6363 6573 7320 6f66 2064  rn: Success of d
-00001de0: 7269 7665 7220 7265 6d6f 7661 6c2e 0a20  river removal.. 
-00001df0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00001e00: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00001e10: 2067 6574 2873 656c 662c 0a20 2020 2020   get(self,.     
-00001e20: 2020 2020 2020 206b 6579 3a20 7479 7069         key: typi
-00001e30: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00001e40: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
-00001e50: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
-00001e60: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
-00001e70: 795d 203d 204e 6f6e 6529 3a0a 2020 2020  y] = None):.    
-00001e80: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
-00001e90: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
-00001ea0: 2063 7573 746f 6d20 7072 6f70 6572 7479   custom property
-00001eb0: 2061 7373 6967 6e65 6420 746f 206b 6579   assigned to key
-00001ec0: 206f 7220 6465 6661 756c 7420 7768 656e   or default when
-00001ed0: 206e 6f74 2066 6f75 6e64 2028 6d61 7463   not found (matc
-00001ee0: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
-00001ef0: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
-00001f00: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
-00001f10: 6529 2e0a 0a20 2020 2020 2020 203a 7061  e)...        :pa
-00001f20: 7261 6d20 6b65 793a 2054 6865 206b 6579  ram key: The key
-00001f30: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00001f40: 2074 6865 2063 7573 746f 6d20 7072 6f70   the custom prop
-00001f50: 6572 7479 2e0a 2020 2020 2020 2020 3a74  erty..        :t
-00001f60: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
-00001f70: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
-00001f80: 2020 2020 2020 3a70 6172 616d 2064 6566        :param def
-00001f90: 6175 6c74 3a20 4f70 7469 6f6e 616c 2061  ault: Optional a
-00001fa0: 7267 756d 656e 7420 666f 7220 7468 6520  rgument for the 
-00001fb0: 7661 6c75 6520 746f 2072 6574 7572 6e20  value to return 
-00001fc0: 6966 202a 6b65 792a 2069 7320 6e6f 7420  if *key* is not 
-00001fd0: 666f 756e 642e 0a20 2020 2020 2020 203a  found..        :
-00001fe0: 7479 7065 2064 6566 6175 6c74 3a20 7479  type default: ty
-00001ff0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00002000: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
-00002010: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00002020: 7373 0a0a 2020 2020 6465 6620 6964 5f70  ss..    def id_p
-00002030: 726f 7065 7274 6965 735f 636c 6561 7228  roperties_clear(
-00002040: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
-00002050: 2727 200a 0a20 2020 2020 2020 2027 2727  '' ..        '''
-00002060: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00002070: 2020 2064 6566 2069 645f 7072 6f70 6572     def id_proper
-00002080: 7469 6573 5f65 6e73 7572 6528 7365 6c66  ties_ensure(self
-00002090: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
-000020a0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-000020b0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
-000020c0: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
-000020d0: 2020 3a72 6574 7572 6e3a 2074 6865 2070    :return: the p
-000020e0: 6172 656e 7420 6772 6f75 7020 666f 7220  arent group for 
-000020f0: 616e 2052 4e41 2073 7472 7563 7427 7320  an RNA struct's 
-00002100: 6375 7374 6f6d 2049 4450 726f 7065 7274  custom IDPropert
-00002110: 6965 732e 0a20 2020 2020 2020 2027 2727  ies..        '''
-00002120: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00002130: 2020 2064 6566 2069 645f 7072 6f70 6572     def id_proper
-00002140: 7469 6573 5f75 6928 7365 6c66 2c20 6b65  ties_ui(self, ke
-00002150: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
-00002160: 616c 5b74 7970 696e 672e 416e 795d 2920  al[typing.Any]) 
-00002170: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
-00002180: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
-00002190: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-000021a0: 2020 5374 7269 6e67 206e 616d 6520 6f66    String name of
-000021b0: 2074 6865 2070 726f 7065 7274 792e 0a20   the property.. 
-000021c0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
-000021d0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-000021e0: 6c5b 7479 7069 6e67 2e41 6e79 5d0a 2020  l[typing.Any].  
-000021f0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
-00002200: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
-00002210: 203a 7265 7475 726e 3a20 5265 7475 726e   :return: Return
-00002220: 2061 6e20 6f62 6a65 6374 2075 7365 6420   an object used 
-00002230: 746f 206d 616e 6167 6520 616e 2049 4450  to manage an IDP
-00002240: 726f 7065 7274 7927 7320 5549 2064 6174  roperty's UI dat
-00002250: 612e 0a20 2020 2020 2020 2027 2727 0a20  a..        '''. 
-00002260: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00002270: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
-00002280: 5f68 6964 6465 6e28 7365 6c66 2c20 7072  _hidden(self, pr
-00002290: 6f70 6572 7479 2920 2d3e 2062 6f6f 6c3a  operty) -> bool:
-000022a0: 0a20 2020 2020 2020 2027 2727 2043 6865  .        ''' Che
-000022b0: 636b 2069 6620 6120 7072 6f70 6572 7479  ck if a property
-000022c0: 2069 7320 6869 6464 656e 2e0a 0a20 2020   is hidden...   
-000022d0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-000022e0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-000022f0: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
-00002300: 2070 726f 7065 7274 7920 6973 2068 6964   property is hid
-00002310: 6465 6e2e 0a20 2020 2020 2020 2027 2727  den..        '''
-00002320: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00002330: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
-00002340: 7479 5f6f 7665 7272 6964 6162 6c65 5f6c  ty_overridable_l
-00002350: 6962 7261 7279 2873 656c 662c 2070 726f  ibrary(self, pro
-00002360: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
-00002370: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
-00002380: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
-00002390: 6973 206f 7665 7272 6964 6162 6c65 2e0a  is overridable..
-000023a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-000023b0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
-000023c0: 6574 7572 6e3a 2054 7275 6520 7768 656e  eturn: True when
-000023d0: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
-000023e0: 206f 7665 7272 6964 6162 6c65 2e0a 2020   overridable..  
-000023f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00002400: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00002410: 6973 5f70 726f 7065 7274 795f 7265 6164  is_property_read
-00002420: 6f6e 6c79 2873 656c 662c 2070 726f 7065  only(self, prope
-00002430: 7274 7929 202d 3e20 626f 6f6c 3a0a 2020  rty) -> bool:.  
-00002440: 2020 2020 2020 2727 2720 4368 6563 6b20        ''' Check 
-00002450: 6966 2061 2070 726f 7065 7274 7920 6973  if a property is
-00002460: 2072 6561 646f 6e6c 792e 0a0a 2020 2020   readonly...    
-00002470: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-00002480: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00002490: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
-000024a0: 7072 6f70 6572 7479 2069 7320 7265 6164  property is read
-000024b0: 6f6e 6c79 2028 6e6f 7420 7772 6974 6162  only (not writab
-000024c0: 6c65 292e 0a20 2020 2020 2020 2027 2727  le)..        '''
-000024d0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000024e0: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
-000024f0: 7479 5f73 6574 2873 656c 662c 2070 726f  ty_set(self, pro
-00002500: 7065 7274 792c 0a20 2020 2020 2020 2020  perty,.         
-00002510: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-00002520: 686f 7374 3a20 7479 7069 6e67 2e4f 7074  host: typing.Opt
-00002530: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
-00002540: 7565 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ue) -> bool:.   
-00002550: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
-00002560: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
-00002570: 7365 742c 2075 7365 2066 6f72 2074 6573  set, use for tes
-00002580: 7469 6e67 206f 7065 7261 746f 7220 7072  ting operator pr
-00002590: 6f70 6572 7469 6573 2e0a 0a20 2020 2020  operties...     
-000025a0: 2020 203a 7061 7261 6d20 6768 6f73 743a     :param ghost:
-000025b0: 2055 7365 6420 666f 7220 6f70 6572 6174   Used for operat
-000025c0: 6f72 7320 7468 6174 2072 652d 7275 6e20  ors that re-run 
-000025d0: 7769 7468 2070 7265 7669 6f75 7320 7365  with previous se
-000025e0: 7474 696e 6773 2e20 496e 2074 6869 7320  ttings. In this 
-000025f0: 6361 7365 2074 6865 2070 726f 7065 7274  case the propert
-00002600: 7920 6973 206e 6f74 206d 6172 6b65 6420  y is not marked 
-00002610: 6173 2073 6574 2c20 7965 7420 7468 6520  as set, yet the 
-00002620: 7661 6c75 6520 6672 6f6d 2074 6865 2070  value from the p
-00002630: 7265 7669 6f75 7320 6578 6563 7574 696f  revious executio
-00002640: 6e20 6973 2075 7365 642e 2049 6e20 7261  n is used. In ra
-00002650: 7265 2063 6173 6573 2079 6f75 206d 6179  re cases you may
-00002660: 2077 616e 7420 746f 2073 6574 2074 6869   want to set thi
-00002670: 7320 6f70 7469 6f6e 2074 6f20 6661 6c73  s option to fals
-00002680: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
-00002690: 2067 686f 7374 3a20 7479 7069 6e67 2e4f   ghost: typing.O
-000026a0: 7074 696f 6e61 6c5b 626f 6f6c 5d0a 2020  ptional[bool].  
-000026b0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
-000026c0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
-000026d0: 726e 3a20 5472 7565 2077 6865 6e20 7468  rn: True when th
-000026e0: 6520 7072 6f70 6572 7479 2068 6173 2062  e property has b
-000026f0: 6565 6e20 7365 742e 0a20 2020 2020 2020  een set..       
-00002700: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00002710: 730a 0a20 2020 2064 6566 2069 7465 6d73  s..    def items
-00002720: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
-00002730: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
-00002740: 2720 5265 7475 726e 7320 7468 6520 6974  ' Returns the it
-00002750: 656d 7320 6f66 2074 6869 7320 6f62 6a65  ems of this obje
-00002760: 6374 7320 6375 7374 6f6d 2070 726f 7065  cts custom prope
-00002770: 7274 6965 7320 286d 6174 6368 6573 2050  rties (matches P
-00002780: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
-00002790: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
-000027a0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
-000027b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000027c0: 7479 7069 6e67 2e41 6e79 0a20 2020 2020  typing.Any.     
-000027d0: 2020 203a 7265 7475 726e 3a20 6375 7374     :return: cust
-000027e0: 6f6d 2070 726f 7065 7274 7920 6b65 792c  om property key,
-000027f0: 2076 616c 7565 2070 6169 7273 2e0a 2020   value pairs..  
-00002800: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00002810: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00002820: 6b65 7966 7261 6d65 5f64 656c 6574 6528  keyframe_delete(
-00002830: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002840: 662c 0a20 2020 2020 2020 2020 2020 2064  f,.            d
-00002850: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
-00002860: 2e4f 7074 696f 6e61 6c5b 7374 725d 2c0a  .Optional[str],.
-00002870: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00002880: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
-00002890: 616c 5b69 6e74 5d20 3d20 2d31 2c0a 2020  al[int] = -1,.  
-000028a0: 2020 2020 2020 2020 2020 6672 616d 653a            frame:
-000028b0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000028c0: 5b66 6c6f 6174 5d20 3d20 2762 7079 2e63  [float] = 'bpy.c
-000028d0: 6f6e 7465 7874 2e73 6365 6e65 2e66 7261  ontext.scene.fra
-000028e0: 6d65 5f63 7572 7265 6e74 272c 0a20 2020  me_current',.   
-000028f0: 2020 2020 2020 2020 2067 726f 7570 3a20           group: 
-00002900: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00002910: 7374 725d 203d 2022 2229 202d 3e20 626f  str] = "") -> bo
-00002920: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
-00002930: 5265 6d6f 7665 2061 206b 6579 6672 616d  Remove a keyfram
-00002940: 6520 6672 6f6d 2074 6869 7320 7072 6f70  e from this prop
-00002950: 6572 7469 6573 2066 6375 7276 652e 0a0a  erties fcurve...
-00002960: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00002970: 6174 615f 7061 7468 3a20 7061 7468 2074  ata_path: path t
-00002980: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
-00002990: 6f20 7265 6d6f 7665 2061 206b 6579 2c20  o remove a key, 
-000029a0: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
-000029b0: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
-000029c0: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
-000029d0: 7065 2064 6174 615f 7061 7468 3a20 7479  pe data_path: ty
-000029e0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-000029f0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
-00002a00: 6d20 696e 6465 783a 2061 7272 6179 2069  m index: array i
-00002a10: 6e64 6578 206f 6620 7468 6520 7072 6f70  ndex of the prop
-00002a20: 6572 7479 2074 6f20 7265 6d6f 7665 2061  erty to remove a
-00002a30: 206b 6579 2e20 4465 6661 756c 7473 2074   key. Defaults t
-00002a40: 6f20 2d31 2072 656d 6f76 696e 6720 616c  o -1 removing al
-00002a50: 6c20 696e 6469 6365 7320 6f72 2061 2073  l indices or a s
-00002a60: 696e 676c 6520 6368 616e 6e65 6c20 6966  ingle channel if
-00002a70: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
-00002a80: 206e 6f74 2061 6e20 6172 7261 792e 0a20   not an array.. 
-00002a90: 2020 2020 2020 203a 7479 7065 2069 6e64         :type ind
-00002aa0: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
-00002ab0: 6e61 6c5b 696e 745d 0a20 2020 2020 2020  nal[int].       
-00002ac0: 203a 7061 7261 6d20 6672 616d 653a 2054   :param frame: T
-00002ad0: 6865 2066 7261 6d65 206f 6e20 7768 6963  he frame on whic
-00002ae0: 6820 7468 6520 6b65 7966 7261 6d65 2069  h the keyframe i
-00002af0: 7320 6465 6c65 7465 642c 2064 6566 6175  s deleted, defau
-00002b00: 6c74 696e 6720 746f 2074 6865 2063 7572  lting to the cur
-00002b10: 7265 6e74 2066 7261 6d65 2e0a 2020 2020  rent frame..    
-00002b20: 2020 2020 3a74 7970 6520 6672 616d 653a      :type frame:
-00002b30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002b40: 5b66 6c6f 6174 5d0a 2020 2020 2020 2020  [float].        
-00002b50: 3a70 6172 616d 2067 726f 7570 3a20 5468  :param group: Th
-00002b60: 6520 6e61 6d65 206f 6620 7468 6520 6772  e name of the gr
-00002b70: 6f75 7020 7468 6520 462d 4375 7276 6520  oup the F-Curve 
-00002b80: 7368 6f75 6c64 2062 6520 6164 6465 6420  should be added 
-00002b90: 746f 2069 6620 6974 2064 6f65 736e 2774  to if it doesn't
-00002ba0: 2065 7869 7374 2079 6574 2e0a 2020 2020   exist yet..    
-00002bb0: 2020 2020 3a74 7970 6520 6772 6f75 703a      :type group:
-00002bc0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002bd0: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
-00002be0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
-00002bf0: 2020 203a 7265 7475 726e 3a20 5375 6363     :return: Succ
-00002c00: 6573 7320 6f66 206b 6579 6672 616d 6520  ess of keyframe 
-00002c10: 6465 6c65 7469 6f6e 2e0a 2020 2020 2020  deletion..      
-00002c20: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00002c30: 7373 0a0a 2020 2020 6465 6620 6b65 7966  ss..    def keyf
-00002c40: 7261 6d65 5f69 6e73 6572 7428 0a20 2020  rame_insert(.   
-00002c50: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00002c60: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00002c70: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
-00002c80: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
-00002c90: 2020 2020 2020 2020 696e 6465 783a 2074          index: t
-00002ca0: 7970 696e 672e 4f70 7469 6f6e 616c 5b69  yping.Optional[i
-00002cb0: 6e74 5d20 3d20 2d31 2c0a 2020 2020 2020  nt] = -1,.      
-00002cc0: 2020 2020 2020 6672 616d 653a 2074 7970        frame: typ
-00002cd0: 696e 672e 4f70 7469 6f6e 616c 5b66 6c6f  ing.Optional[flo
-00002ce0: 6174 5d20 3d20 2762 7079 2e63 6f6e 7465  at] = 'bpy.conte
-00002cf0: 7874 2e73 6365 6e65 2e66 7261 6d65 5f63  xt.scene.frame_c
-00002d00: 7572 7265 6e74 272c 0a20 2020 2020 2020  urrent',.       
-00002d10: 2020 2020 2067 726f 7570 3a20 7479 7069       group: typi
-00002d20: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00002d30: 203d 2022 222c 0a20 2020 2020 2020 2020   = "",.         
-00002d40: 2020 206f 7074 696f 6e73 3a20 7479 7069     options: typi
-00002d50: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00002d60: 6e67 2e41 6e79 5d20 3d20 2773 6574 2829  ng.Any] = 'set()
-00002d70: 2729 202d 3e20 626f 6f6c 3a0a 2020 2020  ') -> bool:.    
-00002d80: 2020 2020 2727 2720 496e 7365 7274 2061      ''' Insert a
-00002d90: 206b 6579 6672 616d 6520 6f6e 2074 6865   keyframe on the
-00002da0: 2070 726f 7065 7274 7920 6769 7665 6e2c   property given,
-00002db0: 2061 6464 696e 6720 6663 7572 7665 7320   adding fcurves 
-00002dc0: 616e 6420 616e 696d 6174 696f 6e20 6461  and animation da
-00002dd0: 7461 2077 6865 6e20 6e65 6365 7373 6172  ta when necessar
-00002de0: 792e 2054 6869 7320 6973 2074 6865 206d  y. This is the m
-00002df0: 6f73 7420 7369 6d70 6c65 2065 7861 6d70  ost simple examp
-00002e00: 6c65 206f 6620 696e 7365 7274 696e 6720  le of inserting 
-00002e10: 6120 6b65 7966 7261 6d65 2066 726f 6d20  a keyframe from 
-00002e20: 7079 7468 6f6e 2e20 4e6f 7465 2074 6861  python. Note tha
-00002e30: 7420 7768 656e 206b 6579 696e 6720 6461  t when keying da
-00002e40: 7461 2070 6174 6873 2077 6869 6368 2063  ta paths which c
-00002e50: 6f6e 7461 696e 206e 6573 7465 6420 7072  ontain nested pr
-00002e60: 6f70 6572 7469 6573 2074 6869 7320 6d75  operties this mu
-00002e70: 7374 2062 6520 646f 6e65 2066 726f 6d20  st be done from 
-00002e80: 7468 6520 6049 4460 2073 7562 636c 6173  the `ID` subclas
-00002e90: 732c 2069 6e20 7468 6973 2063 6173 6520  s, in this case 
-00002ea0: 7468 6520 6041 726d 6174 7572 6560 2072  the `Armature` r
-00002eb0: 6174 6865 7220 7468 616e 2074 6865 2062  ather than the b
-00002ec0: 6f6e 652e 0a0a 2020 2020 2020 2020 3a70  one...        :p
-00002ed0: 6172 616d 2064 6174 615f 7061 7468 3a20  aram data_path: 
-00002ee0: 7061 7468 2074 6f20 7468 6520 7072 6f70  path to the prop
-00002ef0: 6572 7479 2074 6f20 6b65 792c 2061 6e61  erty to key, ana
-00002f00: 6c6f 676f 7573 2074 6f20 7468 6520 6663  logous to the fc
-00002f10: 7572 7665 2773 2064 6174 6120 7061 7468  urve's data path
-00002f20: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00002f30: 6461 7461 5f70 6174 683a 2074 7970 696e  data_path: typin
-00002f40: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-00002f50: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00002f60: 6e64 6578 3a20 6172 7261 7920 696e 6465  ndex: array inde
-00002f70: 7820 6f66 2074 6865 2070 726f 7065 7274  x of the propert
-00002f80: 7920 746f 206b 6579 2e20 4465 6661 756c  y to key. Defaul
-00002f90: 7473 2074 6f20 2d31 2077 6869 6368 2077  ts to -1 which w
-00002fa0: 696c 6c20 6b65 7920 616c 6c20 696e 6469  ill key all indi
-00002fb0: 6365 7320 6f72 2061 2073 696e 676c 6520  ces or a single 
-00002fc0: 6368 616e 6e65 6c20 6966 2074 6865 2070  channel if the p
-00002fd0: 726f 7065 7274 7920 6973 206e 6f74 2061  roperty is not a
-00002fe0: 6e20 6172 7261 792e 0a20 2020 2020 2020  n array..       
-00002ff0: 203a 7479 7065 2069 6e64 6578 3a20 7479   :type index: ty
-00003000: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00003010: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
-00003020: 6d20 6672 616d 653a 2054 6865 2066 7261  m frame: The fra
-00003030: 6d65 206f 6e20 7768 6963 6820 7468 6520  me on which the 
-00003040: 6b65 7966 7261 6d65 2069 7320 696e 7365  keyframe is inse
-00003050: 7274 6564 2c20 6465 6661 756c 7469 6e67  rted, defaulting
-00003060: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
-00003070: 6672 616d 652e 0a20 2020 2020 2020 203a  frame..        :
-00003080: 7479 7065 2066 7261 6d65 3a20 7479 7069  type frame: typi
-00003090: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
-000030a0: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
-000030b0: 6d20 6772 6f75 703a 2054 6865 206e 616d  m group: The nam
-000030c0: 6520 6f66 2074 6865 2067 726f 7570 2074  e of the group t
-000030d0: 6865 2046 2d43 7572 7665 2073 686f 756c  he F-Curve shoul
-000030e0: 6420 6265 2061 6464 6564 2074 6f20 6966  d be added to if
-000030f0: 2069 7420 646f 6573 6e27 7420 6578 6973   it doesn't exis
-00003100: 7420 7965 742e 0a20 2020 2020 2020 203a  t yet..        :
-00003110: 7479 7065 2067 726f 7570 3a20 7479 7069  type group: typi
-00003120: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00003130: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003140: 666c 6167 3a20 0a20 2020 2020 2020 203a  flag: .        :
-00003150: 7479 7065 2066 6c61 673a 2074 7970 696e  type flag: typin
-00003160: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00003170: 672e 5365 745d 0a20 2020 2020 2020 203a  g.Set].        :
-00003180: 7061 7261 6d20 6f70 7469 6f6e 733a 2020  param options:  
-00003190: 2d20 6060 494e 5345 5254 4b45 595f 4e45  - ``INSERTKEY_NE
-000031a0: 4544 4544 6060 204f 6e6c 7920 696e 7365  EDED`` Only inse
-000031b0: 7274 206b 6579 6672 616d 6573 2077 6865  rt keyframes whe
-000031c0: 7265 2074 6865 7927 7265 206e 6565 6465  re they're neede
-000031d0: 6420 696e 2074 6865 2072 656c 6576 616e  d in the relevan
-000031e0: 7420 462d 4375 7276 6573 2e20 2d20 6060  t F-Curves. - ``
-000031f0: 494e 5345 5254 4b45 595f 5649 5355 414c  INSERTKEY_VISUAL
-00003200: 6060 2049 6e73 6572 7420 6b65 7966 7261  `` Insert keyfra
-00003210: 6d65 7320 6261 7365 6420 6f6e 2027 7669  mes based on 'vi
-00003220: 7375 616c 2074 7261 6e73 666f 726d 7327  sual transforms'
-00003230: 2e20 2d20 6060 494e 5345 5254 4b45 595f  . - ``INSERTKEY_
-00003240: 5859 5a5f 544f 5f52 4742 6060 2043 6f6c  XYZ_TO_RGB`` Col
-00003250: 6f72 2066 6f72 206e 6577 6c79 2061 6464  or for newly add
-00003260: 6564 2074 7261 6e73 666f 726d 6174 696f  ed transformatio
-00003270: 6e20 462d 4375 7276 6573 2028 4c6f 6361  n F-Curves (Loca
-00003280: 7469 6f6e 2c20 526f 7461 7469 6f6e 2c20  tion, Rotation, 
-00003290: 5363 616c 6529 2069 7320 6261 7365 6420  Scale) is based 
-000032a0: 6f6e 2074 6865 2074 7261 6e73 666f 726d  on the transform
-000032b0: 2061 7869 732e 202d 2060 6049 4e53 4552   axis. - ``INSER
-000032c0: 544b 4559 5f52 4550 4c41 4345 6060 204f  TKEY_REPLACE`` O
-000032d0: 6e6c 7920 7265 706c 6163 6520 616c 7265  nly replace alre
-000032e0: 6164 7920 6578 6973 7469 6e67 206b 6579  ady existing key
-000032f0: 6672 616d 6573 2e20 2d20 6060 494e 5345  frames. - ``INSE
-00003300: 5254 4b45 595f 4156 4149 4c41 424c 4560  RTKEY_AVAILABLE`
-00003310: 6020 4f6e 6c79 2069 6e73 6572 7420 696e  ` Only insert in
-00003320: 746f 2061 6c72 6561 6479 2065 7869 7374  to already exist
-00003330: 696e 6720 462d 4375 7276 6573 2e20 2d20  ing F-Curves. - 
-00003340: 6060 494e 5345 5254 4b45 595f 4359 434c  ``INSERTKEY_CYCL
-00003350: 455f 4157 4152 4560 6020 5461 6b65 2063  E_AWARE`` Take c
-00003360: 7963 6c69 6320 6578 7472 6170 6f6c 6174  yclic extrapolat
-00003370: 696f 6e20 696e 746f 2061 6363 6f75 6e74  ion into account
-00003380: 2028 4379 636c 652d 4177 6172 6520 4b65   (Cycle-Aware Ke
-00003390: 7969 6e67 206f 7074 696f 6e29 2e0a 2020  ying option)..  
-000033a0: 2020 2020 2020 3a74 7970 6520 6f70 7469        :type opti
-000033b0: 6f6e 733a 2074 7970 696e 672e 4f70 7469  ons: typing.Opti
-000033c0: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
-000033d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-000033e0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
-000033f0: 6574 7572 6e3a 2053 7563 6365 7373 206f  eturn: Success o
-00003400: 6620 6b65 7966 7261 6d65 2069 6e73 6572  f keyframe inser
-00003410: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
-00003420: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00003430: 2020 2020 6465 6620 6b65 7973 2873 656c      def keys(sel
-00003440: 6629 202d 3e20 7479 7069 6e67 2e41 6e79  f) -> typing.Any
-00003450: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00003460: 7475 726e 7320 7468 6520 6b65 7973 206f  turns the keys o
-00003470: 6620 7468 6973 206f 626a 6563 7473 2063  f this objects c
-00003480: 7573 746f 6d20 7072 6f70 6572 7469 6573  ustom properties
-00003490: 2028 6d61 7463 6865 7320 5079 7468 6f6e   (matches Python
-000034a0: 2773 2064 6963 7469 6f6e 6172 7920 6675  's dictionary fu
-000034b0: 6e63 7469 6f6e 206f 6620 7468 6520 7361  nction of the sa
-000034c0: 6d65 206e 616d 6529 2e0a 0a20 2020 2020  me name)...     
-000034d0: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
-000034e0: 672e 416e 790a 2020 2020 2020 2020 3a72  g.Any.        :r
-000034f0: 6574 7572 6e3a 2063 7573 746f 6d20 7072  eturn: custom pr
-00003500: 6f70 6572 7479 206b 6579 732e 0a20 2020  operty keys..   
-00003510: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00003520: 2070 6173 730a 0a20 2020 2064 6566 2070   pass..    def p
-00003530: 6174 685f 6672 6f6d 5f69 6428 7365 6c66  ath_from_id(self
-00003540: 2c20 7072 6f70 6572 7479 3a20 7479 7069  , property: typi
-00003550: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00003560: 203d 2022 2229 202d 3e20 7374 723a 0a20   = "") -> str:. 
-00003570: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-00003580: 6e73 2074 6865 2064 6174 6120 7061 7468  ns the data path
-00003590: 2066 726f 6d20 7468 6520 4944 2074 6f20   from the ID to 
-000035a0: 7468 6973 206f 626a 6563 7420 2873 7472  this object (str
-000035b0: 696e 6729 2e0a 0a20 2020 2020 2020 203a  ing)...        :
-000035c0: 7061 7261 6d20 7072 6f70 6572 7479 3a20  param property: 
-000035d0: 4f70 7469 6f6e 616c 2070 726f 7065 7274  Optional propert
-000035e0: 7920 6e61 6d65 2077 6869 6368 2063 616e  y name which can
-000035f0: 2062 6520 7573 6564 2069 6620 7468 6520   be used if the 
-00003600: 7061 7468 2069 7320 746f 2061 2070 726f  path is to a pro
-00003610: 7065 7274 7920 6f66 2074 6869 7320 6f62  perty of this ob
-00003620: 6a65 6374 2e0a 2020 2020 2020 2020 3a74  ject..        :t
-00003630: 7970 6520 7072 6f70 6572 7479 3a20 7479  ype property: ty
-00003640: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-00003650: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
-00003660: 653a 2073 7472 0a20 2020 2020 2020 203a  e: str.        :
-00003670: 7265 7475 726e 3a20 6062 7079 2e74 7970  return: `bpy.typ
-00003680: 6573 2e62 7079 5f73 7472 7563 742e 6964  es.bpy_struct.id
-00003690: 5f64 6174 6160 2074 6f20 7468 6973 2073  _data` to this s
-000036a0: 7472 7563 7420 616e 6420 7072 6f70 6572  truct and proper
-000036b0: 7479 2028 7768 656e 2067 6976 656e 292e  ty (when given).
-000036c0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000036d0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000036e0: 6566 2070 6174 685f 7265 736f 6c76 6528  ef path_resolve(
-000036f0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00003700: 2020 2020 2020 2020 2020 2070 6174 683a             path:
-00003710: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00003720: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
-00003730: 2020 2020 2020 2020 2020 2020 636f 6572              coer
-00003740: 6365 3a20 7479 7069 6e67 2e4f 7074 696f  ce: typing.Optio
-00003750: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-00003760: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
-00003770: 6574 7572 6e73 2074 6865 2070 726f 7065  eturns the prope
-00003780: 7274 7920 6672 6f6d 2074 6865 2070 6174  rty from the pat
-00003790: 682c 2072 6169 7365 2061 6e20 6578 6365  h, raise an exce
-000037a0: 7074 696f 6e20 7768 656e 206e 6f74 2066  ption when not f
-000037b0: 6f75 6e64 2e0a 0a20 2020 2020 2020 203a  ound...        :
-000037c0: 7061 7261 6d20 7061 7468 3a20 7061 7468  param path: path
-000037d0: 2077 6869 6368 2074 6869 7320 7072 6f70   which this prop
-000037e0: 6572 7479 2072 6573 6f6c 7665 732e 0a20  erty resolves.. 
-000037f0: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
-00003800: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
-00003810: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
-00003820: 3a70 6172 616d 2063 6f65 7263 653a 206f  :param coerce: o
-00003830: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
-00003840: 2c20 7768 656e 2054 7275 652c 2074 6865  , when True, the
-00003850: 2070 726f 7065 7274 7920 7769 6c6c 2062   property will b
-00003860: 6520 636f 6e76 6572 7465 6420 696e 746f  e converted into
-00003870: 2069 7473 2050 7974 686f 6e20 7265 7072   its Python repr
-00003880: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
-00003890: 2020 2020 3a74 7970 6520 636f 6572 6365      :type coerce
-000038a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-000038b0: 6c5b 626f 6f6c 5d0a 2020 2020 2020 2020  l[bool].        
-000038c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000038d0: 0a0a 2020 2020 6465 6620 706f 7028 7365  ..    def pop(se
-000038e0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-000038f0: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
-00003900: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
-00003910: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
-00003920: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00003930: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
-00003940: 6e65 293a 0a20 2020 2020 2020 2027 2727  ne):.        '''
-00003950: 2052 656d 6f76 6520 616e 6420 7265 7475   Remove and retu
-00003960: 726e 2074 6865 2076 616c 7565 206f 6620  rn the value of 
-00003970: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
-00003980: 7274 7920 6173 7369 676e 6564 2074 6f20  rty assigned to 
-00003990: 6b65 7920 6f72 2064 6566 6175 6c74 2077  key or default w
-000039a0: 6865 6e20 6e6f 7420 666f 756e 6420 286d  hen not found (m
-000039b0: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
-000039c0: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
-000039d0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
-000039e0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
-000039f0: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
-00003a00: 6b65 7920 6173 736f 6369 6174 6564 2077  key associated w
-00003a10: 6974 6820 7468 6520 6375 7374 6f6d 2070  ith the custom p
-00003a20: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
-00003a30: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
-00003a40: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-00003a50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003a60: 6465 6661 756c 743a 204f 7074 696f 6e61  default: Optiona
-00003a70: 6c20 6172 6775 6d65 6e74 2066 6f72 2074  l argument for t
-00003a80: 6865 2076 616c 7565 2074 6f20 7265 7475  he value to retu
-00003a90: 726e 2069 6620 2a6b 6579 2a20 6973 206e  rn if *key* is n
-00003aa0: 6f74 2066 6f75 6e64 2e0a 2020 2020 2020  ot found..      
-00003ab0: 2020 3a74 7970 6520 6465 6661 756c 743a    :type default:
-00003ac0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00003ad0: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
-00003ae0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00003af0: 2070 6173 730a 0a20 2020 2064 6566 2070   pass..    def p
-00003b00: 726f 7065 7274 795f 6f76 6572 7269 6461  roperty_overrida
-00003b10: 626c 655f 6c69 6272 6172 795f 7365 7428  ble_library_set(
-00003b20: 7365 6c66 2c20 7072 6f70 6572 7479 2c20  self, property, 
-00003b30: 6f76 6572 7269 6461 626c 6529 202d 3e20  overridable) -> 
-00003b40: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
-00003b50: 2720 4465 6669 6e65 2061 2070 726f 7065  ' Define a prope
-00003b60: 7274 7920 6173 206f 7665 7272 6964 6162  rty as overridab
-00003b70: 6c65 206f 7220 6e6f 7420 286f 6e6c 7920  le or not (only 
-00003b80: 666f 7220 6375 7374 6f6d 2070 726f 7065  for custom prope
-00003b90: 7274 6965 7321 292e 0a0a 2020 2020 2020  rties!)...      
-00003ba0: 2020 3a72 7479 7065 3a20 626f 6f6c 0a20    :rtype: bool. 
-00003bb0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00003bc0: 5472 7565 2077 6865 6e20 7468 6520 6f76  True when the ov
-00003bd0: 6572 7269 6461 626c 6520 7374 6174 7573  erridable status
-00003be0: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00003bf0: 2077 6173 2073 7563 6365 7373 6675 6c6c   was successfull
-00003c00: 7920 7365 742e 0a20 2020 2020 2020 2027  y set..        '
-00003c10: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00003c20: 0a20 2020 2064 6566 2070 726f 7065 7274  .    def propert
-00003c30: 795f 756e 7365 7428 7365 6c66 2c20 7072  y_unset(self, pr
-00003c40: 6f70 6572 7479 293a 0a20 2020 2020 2020  operty):.       
-00003c50: 2027 2727 2055 6e73 6574 2061 2070 726f   ''' Unset a pro
-00003c60: 7065 7274 792c 2077 696c 6c20 7573 6520  perty, will use 
-00003c70: 6465 6661 756c 7420 7661 6c75 6520 6166  default value af
-00003c80: 7465 7277 6172 642e 0a0a 2020 2020 2020  terward...      
-00003c90: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003ca0: 7373 0a0a 2020 2020 6465 6620 7479 7065  ss..    def type
-00003cb0: 5f72 6563 6173 7428 7365 6c66 2920 2d3e  _recast(self) ->
-00003cc0: 2027 6270 795f 7374 7275 6374 273a 0a20   'bpy_struct':. 
-00003cd0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-00003ce0: 6e20 6120 6e65 7720 696e 7374 616e 6365  n a new instance
-00003cf0: 2c20 7468 6973 2069 7320 6e65 6564 6564  , this is needed
-00003d00: 2062 6563 6175 7365 2074 7970 6573 2073   because types s
-00003d10: 7563 6820 6173 2074 6578 7475 7265 7320  uch as textures 
-00003d20: 6361 6e20 6265 2063 6861 6e67 6564 2061  can be changed a
-00003d30: 7420 7275 6e74 696d 652e 0a0a 2020 2020  t runtime...    
-00003d40: 2020 2020 3a72 7479 7065 3a20 2762 7079      :rtype: 'bpy
-00003d50: 5f73 7472 7563 7427 0a20 2020 2020 2020  _struct'.       
-00003d60: 203a 7265 7475 726e 3a20 6120 6e65 7720   :return: a new 
-00003d70: 696e 7374 616e 6365 206f 6620 7468 6973  instance of this
-00003d80: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-00003d90: 2074 7970 6520 696e 6974 6961 6c69 7a65   type initialize
-00003da0: 6420 6167 6169 6e2e 0a20 2020 2020 2020  d again..       
-00003db0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00003dc0: 730a 0a20 2020 2064 6566 2076 616c 7565  s..    def value
-00003dd0: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
-00003de0: 672e 416e 793a 0a20 2020 2020 2020 2027  g.Any:.        '
-00003df0: 2727 2052 6574 7572 6e73 2074 6865 2076  '' Returns the v
-00003e00: 616c 7565 7320 6f66 2074 6869 7320 6f62  alues of this ob
-00003e10: 6a65 6374 7320 6375 7374 6f6d 2070 726f  jects custom pro
-00003e20: 7065 7274 6965 7320 286d 6174 6368 6573  perties (matches
-00003e30: 2050 7974 686f 6e27 7320 6469 6374 696f   Python's dictio
-00003e40: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
-00003e50: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
-00003e60: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00003e70: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
-00003e80: 2020 2020 203a 7265 7475 726e 3a20 6375       :return: cu
-00003e90: 7374 6f6d 2070 726f 7065 7274 7920 7661  stom property va
-00003ea0: 6c75 6573 2e0a 2020 2020 2020 2020 2727  lues..        ''
-00003eb0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00003ec0: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
-00003ed0: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
-00003ee0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00003ef0: 2073 7472 5d29 202d 3e20 2774 7970 696e   str]) -> 'typin
-00003f00: 672e 416e 7927 3a0a 2020 2020 2020 2020  g.Any':.        
-00003f10: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-00003f20: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-00003f30: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-00003f40: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-00003f50: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
-00003f60: 7970 653a 2027 7479 7069 6e67 2e41 6e79  ype: 'typing.Any
-00003f70: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
-00003f80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003f90: 6465 6620 5f5f 7365 7469 7465 6d5f 5f28  def __setitem__(
-00003fa0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
-00003fb0: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
-00003fc0: 5d2c 2076 616c 7565 3a20 2774 7970 696e  ], value: 'typin
-00003fd0: 672e 416e 7927 293a 0a20 2020 2020 2020  g.Any'):.       
-00003fe0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00003ff0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
-00004000: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
-00004010: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00004020: 2073 7472 5d0a 2020 2020 2020 2020 3a70   str].        :p
-00004030: 6172 616d 2076 616c 7565 3a20 0a20 2020  aram value: .   
-00004040: 2020 2020 203a 7479 7065 2076 616c 7565       :type value
-00004050: 3a20 2774 7970 696e 672e 416e 7927 0a20  : 'typing.Any'. 
-00004060: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00004070: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00004080: 205f 5f64 656c 6974 656d 5f5f 2873 656c   __delitem__(sel
-00004090: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
-000040a0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2920  nion[int, str]) 
-000040b0: 2d3e 2027 7479 7069 6e67 2e41 6e79 273a  -> 'typing.Any':
-000040c0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
-000040d0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
-000040e0: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
-000040f0: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
-00004100: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
-00004110: 2020 2020 2020 3a72 7479 7065 3a20 2774        :rtype: 't
-00004120: 7970 696e 672e 416e 7927 0a20 2020 2020  yping.Any'.     
+00001b50: 6c5b 696e 745d 203d 202d 312c 0a20 2020  l[int] = -1,.   
+00001b60: 2020 2020 2020 2020 2066 7261 6d65 3a20           frame: 
+00001b70: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001b80: 666c 6f61 745d 203d 2027 6270 792e 636f  float] = 'bpy.co
+00001b90: 6e74 6578 742e 7363 656e 652e 6672 616d  ntext.scene.fram
+00001ba0: 655f 6375 7272 656e 7427 2c0a 2020 2020  e_current',.    
+00001bb0: 2020 2020 2020 2020 6772 6f75 703a 2074          group: t
+00001bc0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+00001bd0: 7472 5d20 3d20 2222 2920 2d3e 2062 6f6f  tr] = "") -> boo
+00001be0: 6c3a 0a20 2020 2020 2020 2027 2727 2052  l:.        ''' R
+00001bf0: 656d 6f76 6520 6120 6b65 7966 7261 6d65  emove a keyframe
+00001c00: 2066 726f 6d20 7468 6973 2070 726f 7065   from this prope
+00001c10: 7274 6965 7320 6663 7572 7665 2e0a 0a20  rties fcurve... 
+00001c20: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
+00001c30: 7461 5f70 6174 683a 2070 6174 6820 746f  ta_path: path to
+00001c40: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
+00001c50: 2072 656d 6f76 6520 6120 6b65 792c 2061   remove a key, a
+00001c60: 6e61 6c6f 676f 7573 2074 6f20 7468 6520  nalogous to the 
+00001c70: 6663 7572 7665 2773 2064 6174 6120 7061  fcurve's data pa
+00001c80: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
+00001c90: 6520 6461 7461 5f70 6174 683a 2074 7970  e data_path: typ
+00001ca0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00001cb0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00001cc0: 2069 6e64 6578 3a20 6172 7261 7920 696e   index: array in
+00001cd0: 6465 7820 6f66 2074 6865 2070 726f 7065  dex of the prope
+00001ce0: 7274 7920 746f 2072 656d 6f76 6520 6120  rty to remove a 
+00001cf0: 6b65 792e 2044 6566 6175 6c74 7320 746f  key. Defaults to
+00001d00: 202d 3120 7265 6d6f 7669 6e67 2061 6c6c   -1 removing all
+00001d10: 2069 6e64 6963 6573 206f 7220 6120 7369   indices or a si
+00001d20: 6e67 6c65 2063 6861 6e6e 656c 2069 6620  ngle channel if 
+00001d30: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
+00001d40: 6e6f 7420 616e 2061 7272 6179 2e0a 2020  not an array..  
+00001d50: 2020 2020 2020 3a74 7970 6520 696e 6465        :type inde
+00001d60: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00001d70: 616c 5b69 6e74 5d0a 2020 2020 2020 2020  al[int].        
+00001d80: 3a70 6172 616d 2066 7261 6d65 3a20 5468  :param frame: Th
+00001d90: 6520 6672 616d 6520 6f6e 2077 6869 6368  e frame on which
+00001da0: 2074 6865 206b 6579 6672 616d 6520 6973   the keyframe is
+00001db0: 2064 656c 6574 6564 2c20 6465 6661 756c   deleted, defaul
+00001dc0: 7469 6e67 2074 6f20 7468 6520 6375 7272  ting to the curr
+00001dd0: 656e 7420 6672 616d 652e 0a20 2020 2020  ent frame..     
+00001de0: 2020 203a 7479 7065 2066 7261 6d65 3a20     :type frame: 
+00001df0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001e00: 666c 6f61 745d 0a20 2020 2020 2020 203a  float].        :
+00001e10: 7061 7261 6d20 6772 6f75 703a 2054 6865  param group: The
+00001e20: 206e 616d 6520 6f66 2074 6865 2067 726f   name of the gro
+00001e30: 7570 2074 6865 2046 2d43 7572 7665 2073  up the F-Curve s
+00001e40: 686f 756c 6420 6265 2061 6464 6564 2074  hould be added t
+00001e50: 6f20 6966 2069 7420 646f 6573 6e27 7420  o if it doesn't 
+00001e60: 6578 6973 7420 7965 742e 0a20 2020 2020  exist yet..     
+00001e70: 2020 203a 7479 7065 2067 726f 7570 3a20     :type group: 
+00001e80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00001e90: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00001ea0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00001eb0: 2020 3a72 6574 7572 6e3a 2053 7563 6365    :return: Succe
+00001ec0: 7373 206f 6620 6b65 7966 7261 6d65 2064  ss of keyframe d
+00001ed0: 656c 6574 696f 6e2e 0a20 2020 2020 2020  eletion..       
+00001ee0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00001ef0: 730a 0a20 2020 2064 6566 206b 6579 6672  s..    def keyfr
+00001f00: 616d 655f 696e 7365 7274 280a 2020 2020  ame_insert(.    
+00001f10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00001f20: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
+00001f30: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
+00001f40: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
+00001f50: 2020 2020 2020 2069 6e64 6578 3a20 7479         index: ty
+00001f60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
+00001f70: 745d 203d 202d 312c 0a20 2020 2020 2020  t] = -1,.       
+00001f80: 2020 2020 2066 7261 6d65 3a20 7479 7069       frame: typi
+00001f90: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
+00001fa0: 745d 203d 2027 6270 792e 636f 6e74 6578  t] = 'bpy.contex
+00001fb0: 742e 7363 656e 652e 6672 616d 655f 6375  t.scene.frame_cu
+00001fc0: 7272 656e 7427 2c0a 2020 2020 2020 2020  rrent',.        
+00001fd0: 2020 2020 6772 6f75 703a 2074 7970 696e      group: typin
+00001fe0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
+00001ff0: 3d20 2222 2c0a 2020 2020 2020 2020 2020  = "",.          
+00002000: 2020 6f70 7469 6f6e 733a 2074 7970 696e    options: typin
+00002010: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00002020: 672e 416e 795d 203d 2027 7365 7428 2927  g.Any] = 'set()'
+00002030: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00002040: 2020 2027 2727 2049 6e73 6572 7420 6120     ''' Insert a 
+00002050: 6b65 7966 7261 6d65 206f 6e20 7468 6520  keyframe on the 
+00002060: 7072 6f70 6572 7479 2067 6976 656e 2c20  property given, 
+00002070: 6164 6469 6e67 2066 6375 7276 6573 2061  adding fcurves a
+00002080: 6e64 2061 6e69 6d61 7469 6f6e 2064 6174  nd animation dat
+00002090: 6120 7768 656e 206e 6563 6573 7361 7279  a when necessary
+000020a0: 2e20 5468 6973 2069 7320 7468 6520 6d6f  . This is the mo
+000020b0: 7374 2073 696d 706c 6520 6578 616d 706c  st simple exampl
+000020c0: 6520 6f66 2069 6e73 6572 7469 6e67 2061  e of inserting a
+000020d0: 206b 6579 6672 616d 6520 6672 6f6d 2070   keyframe from p
+000020e0: 7974 686f 6e2e 204e 6f74 6520 7468 6174  ython. Note that
+000020f0: 2077 6865 6e20 6b65 7969 6e67 2064 6174   when keying dat
+00002100: 6120 7061 7468 7320 7768 6963 6820 636f  a paths which co
+00002110: 6e74 6169 6e20 6e65 7374 6564 2070 726f  ntain nested pro
+00002120: 7065 7274 6965 7320 7468 6973 206d 7573  perties this mus
+00002130: 7420 6265 2064 6f6e 6520 6672 6f6d 2074  t be done from t
+00002140: 6865 2060 4944 6020 7375 6263 6c61 7373  he `ID` subclass
+00002150: 2c20 696e 2074 6869 7320 6361 7365 2074  , in this case t
+00002160: 6865 2060 4172 6d61 7475 7265 6020 7261  he `Armature` ra
+00002170: 7468 6572 2074 6861 6e20 7468 6520 626f  ther than the bo
+00002180: 6e65 2e0a 0a20 2020 2020 2020 203a 7061  ne...        :pa
+00002190: 7261 6d20 6461 7461 5f70 6174 683a 2070  ram data_path: p
+000021a0: 6174 6820 746f 2074 6865 2070 726f 7065  ath to the prope
+000021b0: 7274 7920 746f 206b 6579 2c20 616e 616c  rty to key, anal
+000021c0: 6f67 6f75 7320 746f 2074 6865 2066 6375  ogous to the fcu
+000021d0: 7276 6527 7320 6461 7461 2070 6174 682e  rve's data path.
+000021e0: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
+000021f0: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
+00002200: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00002210: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
+00002220: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
+00002230: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00002240: 2074 6f20 6b65 792e 2044 6566 6175 6c74   to key. Default
+00002250: 7320 746f 202d 3120 7768 6963 6820 7769  s to -1 which wi
+00002260: 6c6c 206b 6579 2061 6c6c 2069 6e64 6963  ll key all indic
+00002270: 6573 206f 7220 6120 7369 6e67 6c65 2063  es or a single c
+00002280: 6861 6e6e 656c 2069 6620 7468 6520 7072  hannel if the pr
+00002290: 6f70 6572 7479 2069 7320 6e6f 7420 616e  operty is not an
+000022a0: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+000022b0: 3a74 7970 6520 696e 6465 783a 2074 7970  :type index: typ
+000022c0: 696e 672e 4f70 7469 6f6e 616c 5b69 6e74  ing.Optional[int
+000022d0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+000022e0: 2066 7261 6d65 3a20 5468 6520 6672 616d   frame: The fram
+000022f0: 6520 6f6e 2077 6869 6368 2074 6865 206b  e on which the k
+00002300: 6579 6672 616d 6520 6973 2069 6e73 6572  eyframe is inser
+00002310: 7465 642c 2064 6566 6175 6c74 696e 6720  ted, defaulting 
+00002320: 746f 2074 6865 2063 7572 7265 6e74 2066  to the current f
+00002330: 7261 6d65 2e0a 2020 2020 2020 2020 3a74  rame..        :t
+00002340: 7970 6520 6672 616d 653a 2074 7970 696e  ype frame: typin
+00002350: 672e 4f70 7469 6f6e 616c 5b66 6c6f 6174  g.Optional[float
+00002360: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
+00002370: 2067 726f 7570 3a20 5468 6520 6e61 6d65   group: The name
+00002380: 206f 6620 7468 6520 6772 6f75 7020 7468   of the group th
+00002390: 6520 462d 4375 7276 6520 7368 6f75 6c64  e F-Curve should
+000023a0: 2062 6520 6164 6465 6420 746f 2069 6620   be added to if 
+000023b0: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
+000023c0: 2079 6574 2e0a 2020 2020 2020 2020 3a74   yet..        :t
+000023d0: 7970 6520 6772 6f75 703a 2074 7970 696e  ype group: typin
+000023e0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+000023f0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
+00002400: 6c61 673a 200a 2020 2020 2020 2020 3a74  lag: .        :t
+00002410: 7970 6520 666c 6167 3a20 7479 7069 6e67  ype flag: typing
+00002420: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+00002430: 2e53 6574 5d0a 2020 2020 2020 2020 3a70  .Set].        :p
+00002440: 6172 616d 206f 7074 696f 6e73 3a20 202d  aram options:  -
+00002450: 2060 6049 4e53 4552 544b 4559 5f4e 4545   ``INSERTKEY_NEE
+00002460: 4445 4460 6020 4f6e 6c79 2069 6e73 6572  DED`` Only inser
+00002470: 7420 6b65 7966 7261 6d65 7320 7768 6572  t keyframes wher
+00002480: 6520 7468 6579 2772 6520 6e65 6564 6564  e they're needed
+00002490: 2069 6e20 7468 6520 7265 6c65 7661 6e74   in the relevant
+000024a0: 2046 2d43 7572 7665 732e 202d 2060 6049   F-Curves. - ``I
+000024b0: 4e53 4552 544b 4559 5f56 4953 5541 4c60  NSERTKEY_VISUAL`
+000024c0: 6020 496e 7365 7274 206b 6579 6672 616d  ` Insert keyfram
+000024d0: 6573 2062 6173 6564 206f 6e20 2776 6973  es based on 'vis
+000024e0: 7561 6c20 7472 616e 7366 6f72 6d73 272e  ual transforms'.
+000024f0: 202d 2060 6049 4e53 4552 544b 4559 5f58   - ``INSERTKEY_X
+00002500: 595a 5f54 4f5f 5247 4260 6020 436f 6c6f  YZ_TO_RGB`` Colo
+00002510: 7220 666f 7220 6e65 776c 7920 6164 6465  r for newly adde
+00002520: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
+00002530: 2046 2d43 7572 7665 7320 284c 6f63 6174   F-Curves (Locat
+00002540: 696f 6e2c 2052 6f74 6174 696f 6e2c 2053  ion, Rotation, S
+00002550: 6361 6c65 2920 6973 2062 6173 6564 206f  cale) is based o
+00002560: 6e20 7468 6520 7472 616e 7366 6f72 6d20  n the transform 
+00002570: 6178 6973 2e20 2d20 6060 494e 5345 5254  axis. - ``INSERT
+00002580: 4b45 595f 5245 504c 4143 4560 6020 4f6e  KEY_REPLACE`` On
+00002590: 6c79 2072 6570 6c61 6365 2061 6c72 6561  ly replace alrea
+000025a0: 6479 2065 7869 7374 696e 6720 6b65 7966  dy existing keyf
+000025b0: 7261 6d65 732e 202d 2060 6049 4e53 4552  rames. - ``INSER
+000025c0: 544b 4559 5f41 5641 494c 4142 4c45 6060  TKEY_AVAILABLE``
+000025d0: 204f 6e6c 7920 696e 7365 7274 2069 6e74   Only insert int
+000025e0: 6f20 616c 7265 6164 7920 6578 6973 7469  o already existi
+000025f0: 6e67 2046 2d43 7572 7665 732e 202d 2060  ng F-Curves. - `
+00002600: 6049 4e53 4552 544b 4559 5f43 5943 4c45  `INSERTKEY_CYCLE
+00002610: 5f41 5741 5245 6060 2054 616b 6520 6379  _AWARE`` Take cy
+00002620: 636c 6963 2065 7874 7261 706f 6c61 7469  clic extrapolati
+00002630: 6f6e 2069 6e74 6f20 6163 636f 756e 7420  on into account 
+00002640: 2843 7963 6c65 2d41 7761 7265 204b 6579  (Cycle-Aware Key
+00002650: 696e 6720 6f70 7469 6f6e 292e 0a20 2020  ing option)..   
+00002660: 2020 2020 203a 7479 7065 206f 7074 696f       :type optio
+00002670: 6e73 3a20 7479 7069 6e67 2e4f 7074 696f  ns: typing.Optio
+00002680: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d0a  nal[typing.Any].
+00002690: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000026a0: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
+000026b0: 7475 726e 3a20 5375 6363 6573 7320 6f66  turn: Success of
+000026c0: 206b 6579 6672 616d 6520 696e 7365 7274   keyframe insert
+000026d0: 696f 6e2e 0a20 2020 2020 2020 2027 2727  ion..        '''
+000026e0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000026f0: 2020 2064 6566 206b 6579 7328 7365 6c66     def keys(self
+00002700: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
+00002710: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
+00002720: 7572 6e73 2074 6865 206b 6579 7320 6f66  urns the keys of
+00002730: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
+00002740: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
+00002750: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
+00002760: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
+00002770: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
+00002780: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
+00002790: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
+000027a0: 2e41 6e79 0a20 2020 2020 2020 203a 7265  .Any.        :re
+000027b0: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
+000027c0: 7065 7274 7920 6b65 7973 2e0a 2020 2020  perty keys..    
+000027d0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000027e0: 7061 7373 0a0a 2020 2020 6465 6620 7061  pass..    def pa
+000027f0: 7468 5f66 726f 6d5f 6964 2873 656c 662c  th_from_id(self,
+00002800: 2070 726f 7065 7274 793a 2074 7970 696e   property: typin
+00002810: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
+00002820: 3d20 2222 2920 2d3e 2073 7472 3a0a 2020  = "") -> str:.  
+00002830: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+00002840: 7320 7468 6520 6461 7461 2070 6174 6820  s the data path 
+00002850: 6672 6f6d 2074 6865 2049 4420 746f 2074  from the ID to t
+00002860: 6869 7320 6f62 6a65 6374 2028 7374 7269  his object (stri
+00002870: 6e67 292e 0a0a 2020 2020 2020 2020 3a70  ng)...        :p
+00002880: 6172 616d 2070 726f 7065 7274 793a 204f  aram property: O
+00002890: 7074 696f 6e61 6c20 7072 6f70 6572 7479  ptional property
+000028a0: 206e 616d 6520 7768 6963 6820 6361 6e20   name which can 
+000028b0: 6265 2075 7365 6420 6966 2074 6865 2070  be used if the p
+000028c0: 6174 6820 6973 2074 6f20 6120 7072 6f70  ath is to a prop
+000028d0: 6572 7479 206f 6620 7468 6973 206f 626a  erty of this obj
+000028e0: 6563 742e 0a20 2020 2020 2020 203a 7479  ect..        :ty
+000028f0: 7065 2070 726f 7065 7274 793a 2074 7970  pe property: typ
+00002900: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+00002910: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
+00002920: 3a20 7374 720a 2020 2020 2020 2020 3a72  : str.        :r
+00002930: 6574 7572 6e3a 2060 6270 792e 7479 7065  eturn: `bpy.type
+00002940: 732e 6270 795f 7374 7275 6374 2e69 645f  s.bpy_struct.id_
+00002950: 6461 7461 6020 746f 2074 6869 7320 7374  data` to this st
+00002960: 7275 6374 2061 6e64 2070 726f 7065 7274  ruct and propert
+00002970: 7920 2877 6865 6e20 6769 7665 6e29 2e0a  y (when given)..
+00002980: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00002990: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000029a0: 6620 7061 7468 5f72 6573 6f6c 7665 2873  f path_resolve(s
+000029b0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+000029c0: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
+000029d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000029e0: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
+000029f0: 2020 2020 2020 2020 2020 2063 6f65 7263             coerc
+00002a00: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+00002a10: 616c 5b62 6f6f 6c5d 203d 2054 7275 6529  al[bool] = True)
+00002a20: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
+00002a30: 7475 726e 7320 7468 6520 7072 6f70 6572  turns the proper
+00002a40: 7479 2066 726f 6d20 7468 6520 7061 7468  ty from the path
+00002a50: 2c20 7261 6973 6520 616e 2065 7863 6570  , raise an excep
+00002a60: 7469 6f6e 2077 6865 6e20 6e6f 7420 666f  tion when not fo
+00002a70: 756e 642e 0a0a 2020 2020 2020 2020 3a70  und...        :p
+00002a80: 6172 616d 2070 6174 683a 2070 6174 6820  aram path: path 
+00002a90: 7768 6963 6820 7468 6973 2070 726f 7065  which this prope
+00002aa0: 7274 7920 7265 736f 6c76 6573 2e0a 2020  rty resolves..  
+00002ab0: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
+00002ac0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00002ad0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00002ae0: 7061 7261 6d20 636f 6572 6365 3a20 6f70  param coerce: op
+00002af0: 7469 6f6e 616c 2061 7267 756d 656e 742c  tional argument,
+00002b00: 2077 6865 6e20 5472 7565 2c20 7468 6520   when True, the 
+00002b10: 7072 6f70 6572 7479 2077 696c 6c20 6265  property will be
+00002b20: 2063 6f6e 7665 7274 6564 2069 6e74 6f20   converted into 
+00002b30: 6974 7320 5079 7468 6f6e 2072 6570 7265  its Python repre
+00002b40: 7365 6e74 6174 696f 6e2e 0a20 2020 2020  sentation..     
+00002b50: 2020 203a 7479 7065 2063 6f65 7263 653a     :type coerce:
+00002b60: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00002b70: 5b62 6f6f 6c5d 0a20 2020 2020 2020 2027  [bool].        '
+00002b80: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00002b90: 0a20 2020 2064 6566 2070 6f70 2873 656c  .    def pop(sel
+00002ba0: 662c 0a20 2020 2020 2020 2020 2020 206b  f,.            k
+00002bb0: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
+00002bc0: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
+00002bd0: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
+00002be0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+00002bf0: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
+00002c00: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
+00002c10: 5265 6d6f 7665 2061 6e64 2072 6574 7572  Remove and retur
+00002c20: 6e20 7468 6520 7661 6c75 6520 6f66 2074  n the value of t
+00002c30: 6865 2063 7573 746f 6d20 7072 6f70 6572  he custom proper
+00002c40: 7479 2061 7373 6967 6e65 6420 746f 206b  ty assigned to k
+00002c50: 6579 206f 7220 6465 6661 756c 7420 7768  ey or default wh
+00002c60: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
+00002c70: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
+00002c80: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
+00002c90: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
+00002ca0: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
+00002cb0: 7061 7261 6d20 6b65 793a 2054 6865 206b  param key: The k
+00002cc0: 6579 2061 7373 6f63 6961 7465 6420 7769  ey associated wi
+00002cd0: 7468 2074 6865 2063 7573 746f 6d20 7072  th the custom pr
+00002ce0: 6f70 6572 7479 2e0a 2020 2020 2020 2020  operty..        
+00002cf0: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
+00002d00: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00002d10: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00002d20: 6566 6175 6c74 3a20 4f70 7469 6f6e 616c  efault: Optional
+00002d30: 2061 7267 756d 656e 7420 666f 7220 7468   argument for th
+00002d40: 6520 7661 6c75 6520 746f 2072 6574 7572  e value to retur
+00002d50: 6e20 6966 202a 6b65 792a 2069 7320 6e6f  n if *key* is no
+00002d60: 7420 666f 756e 642e 0a20 2020 2020 2020  t found..       
+00002d70: 203a 7479 7065 2064 6566 6175 6c74 3a20   :type default: 
+00002d80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002d90: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
+00002da0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00002db0: 7061 7373 0a0a 2020 2020 6465 6620 7072  pass..    def pr
+00002dc0: 6f70 6572 7479 5f6f 7665 7272 6964 6162  operty_overridab
+00002dd0: 6c65 5f6c 6962 7261 7279 5f73 6574 2873  le_library_set(s
+00002de0: 656c 662c 2070 726f 7065 7274 792c 206f  elf, property, o
+00002df0: 7665 7272 6964 6162 6c65 2920 2d3e 2062  verridable) -> b
+00002e00: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
+00002e10: 2044 6566 696e 6520 6120 7072 6f70 6572   Define a proper
+00002e20: 7479 2061 7320 6f76 6572 7269 6461 626c  ty as overridabl
+00002e30: 6520 6f72 206e 6f74 2028 6f6e 6c79 2066  e or not (only f
+00002e40: 6f72 2063 7573 746f 6d20 7072 6f70 6572  or custom proper
+00002e50: 7469 6573 2129 2e0a 0a20 2020 2020 2020  ties!)...       
+00002e60: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+00002e70: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
+00002e80: 7275 6520 7768 656e 2074 6865 206f 7665  rue when the ove
+00002e90: 7272 6964 6162 6c65 2073 7461 7475 7320  rridable status 
+00002ea0: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
+00002eb0: 7761 7320 7375 6363 6573 7366 756c 6c79  was successfully
+00002ec0: 2073 6574 2e0a 2020 2020 2020 2020 2727   set..        ''
+00002ed0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00002ee0: 2020 2020 6465 6620 7072 6f70 6572 7479      def property
+00002ef0: 5f75 6e73 6574 2873 656c 662c 2070 726f  _unset(self, pro
+00002f00: 7065 7274 7929 3a0a 2020 2020 2020 2020  perty):.        
+00002f10: 2727 2720 556e 7365 7420 6120 7072 6f70  ''' Unset a prop
+00002f20: 6572 7479 2c20 7769 6c6c 2075 7365 2064  erty, will use d
+00002f30: 6566 6175 6c74 2076 616c 7565 2061 6674  efault value aft
+00002f40: 6572 7761 7264 2e0a 0a20 2020 2020 2020  erward...       
+00002f50: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00002f60: 730a 0a20 2020 2064 6566 2074 7970 655f  s..    def type_
+00002f70: 7265 6361 7374 2873 656c 6629 202d 3e20  recast(self) -> 
+00002f80: 2762 7079 5f73 7472 7563 7427 3a0a 2020  'bpy_struct':.  
+00002f90: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
+00002fa0: 2061 206e 6577 2069 6e73 7461 6e63 652c   a new instance,
+00002fb0: 2074 6869 7320 6973 206e 6565 6465 6420   this is needed 
+00002fc0: 6265 6361 7573 6520 7479 7065 7320 7375  because types su
+00002fd0: 6368 2061 7320 7465 7874 7572 6573 2063  ch as textures c
+00002fe0: 616e 2062 6520 6368 616e 6765 6420 6174  an be changed at
+00002ff0: 2072 756e 7469 6d65 2e0a 0a20 2020 2020   runtime...     
+00003000: 2020 203a 7274 7970 653a 2027 6270 795f     :rtype: 'bpy_
+00003010: 7374 7275 6374 270a 2020 2020 2020 2020  struct'.        
+00003020: 3a72 6574 7572 6e3a 2061 206e 6577 2069  :return: a new i
+00003030: 6e73 7461 6e63 6520 6f66 2074 6869 7320  nstance of this 
+00003040: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
+00003050: 7479 7065 2069 6e69 7469 616c 697a 6564  type initialized
+00003060: 2061 6761 696e 2e0a 2020 2020 2020 2020   again..        
+00003070: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00003080: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
+00003090: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+000030a0: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
+000030b0: 2720 5265 7475 726e 7320 7468 6520 7661  ' Returns the va
+000030c0: 6c75 6573 206f 6620 7468 6973 206f 626a  lues of this obj
+000030d0: 6563 7473 2063 7573 746f 6d20 7072 6f70  ects custom prop
+000030e0: 6572 7469 6573 2028 6d61 7463 6865 7320  erties (matches 
+000030f0: 5079 7468 6f6e 2773 2064 6963 7469 6f6e  Python's diction
+00003100: 6172 7920 6675 6e63 7469 6f6e 206f 6620  ary function of 
+00003110: 7468 6520 7361 6d65 206e 616d 6529 2e0a  the same name)..
+00003120: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00003130: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
+00003140: 2020 2020 3a72 6574 7572 6e3a 2063 7573      :return: cus
+00003150: 746f 6d20 7072 6f70 6572 7479 2076 616c  tom property val
+00003160: 7565 732e 0a20 2020 2020 2020 2027 2727  ues..        '''
+00003170: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00003180: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
+00003190: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
+000031a0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+000031b0: 7374 725d 2920 2d3e 2027 7479 7069 6e67  str]) -> 'typing
+000031c0: 2e41 6e79 273a 0a20 2020 2020 2020 2027  .Any':.        '
+000031d0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
+000031e0: 7261 6d20 6b65 793a 200a 2020 2020 2020  ram key: .      
+000031f0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
+00003200: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
+00003210: 7472 5d0a 2020 2020 2020 2020 3a72 7479  tr].        :rty
+00003220: 7065 3a20 2774 7970 696e 672e 416e 7927  pe: 'typing.Any'
+00003230: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00003240: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00003250: 6566 205f 5f73 6574 6974 656d 5f5f 2873  ef __setitem__(s
+00003260: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
+00003270: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
+00003280: 2c20 7661 6c75 653a 2027 7479 7069 6e67  , value: 'typing
+00003290: 2e41 6e79 2729 3a0a 2020 2020 2020 2020  .Any'):.        
+000032a0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+000032b0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+000032c0: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+000032d0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+000032e0: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
+000032f0: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
+00003300: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
+00003310: 2027 7479 7069 6e67 2e41 6e79 270a 2020   'typing.Any'.  
+00003320: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00003330: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00003340: 5f5f 6465 6c69 7465 6d5f 5f28 7365 6c66  __delitem__(self
+00003350: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
+00003360: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
+00003370: 3e20 2774 7970 696e 672e 416e 7927 3a0a  > 'typing.Any':.
+00003380: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
+00003390: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
+000033a0: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
+000033b0: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
+000033c0: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
+000033d0: 2020 2020 203a 7274 7970 653a 2027 7479       :rtype: 'ty
+000033e0: 7069 6e67 2e41 6e79 270a 2020 2020 2020  ping.Any'.      
+000033f0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00003400: 7373 0a0a 0a63 6c61 7373 2062 7079 5f70  ss...class bpy_p
+00003410: 726f 705f 636f 6c6c 6563 7469 6f6e 2874  rop_collection(t
+00003420: 7970 696e 672e 4765 6e65 7269 635b 4765  yping.Generic[Ge
+00003430: 6e65 7269 6354 7970 655d 293a 0a20 2020  nericType]):.   
+00003440: 2027 2727 2062 7569 6c74 2d69 6e20 636c   ''' built-in cl
+00003450: 6173 7320 7573 6564 2066 6f72 2061 6c6c  ass used for all
+00003460: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
+00003470: 2020 2727 270a 0a20 2020 2064 6566 2066    '''..    def f
+00003480: 696e 6428 7365 6c66 2c20 6b65 793a 2074  ind(self, key: t
+00003490: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+000034a0: 7472 5d29 202d 3e20 696e 743a 0a20 2020  tr]) -> int:.   
+000034b0: 2020 2020 2027 2727 2052 6574 7572 6e73       ''' Returns
+000034c0: 2074 6865 2069 6e64 6578 206f 6620 6120   the index of a 
+000034d0: 6b65 7920 696e 2061 2063 6f6c 6c65 6374  key in a collect
+000034e0: 696f 6e20 6f72 202d 3120 7768 656e 206e  ion or -1 when n
+000034f0: 6f74 2066 6f75 6e64 2028 6d61 7463 6865  ot found (matche
+00003500: 7320 5079 7468 6f6e 2773 2073 7472 696e  s Python's strin
+00003510: 6720 6669 6e64 2066 756e 6374 696f 6e20  g find function 
+00003520: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
+00003530: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
+00003540: 616d 206b 6579 3a20 5468 6520 6964 656e  am key: The iden
+00003550: 7469 6669 6572 2066 6f72 2074 6865 2063  tifier for the c
+00003560: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
+00003570: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00003580: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
+00003590: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
+000035a0: 2020 3a72 7479 7065 3a20 696e 740a 2020    :rtype: int.  
+000035b0: 2020 2020 2020 3a72 6574 7572 6e3a 2069        :return: i
+000035c0: 6e64 6578 206f 6620 7468 6520 6b65 792e  ndex of the key.
+000035d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000035e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000035f0: 6566 2066 6f72 6561 6368 5f67 6574 2873  ef foreach_get(s
+00003600: 656c 662c 2061 7474 722c 2073 6571 293a  elf, attr, seq):
+00003610: 0a20 2020 2020 2020 2027 2727 2054 6869  .        ''' Thi
+00003620: 7320 6973 2061 2066 756e 6374 696f 6e20  s is a function 
+00003630: 746f 2067 6976 6520 6661 7374 2061 6363  to give fast acc
+00003640: 6573 7320 746f 2061 7474 7269 6275 7465  ess to attribute
+00003650: 7320 7769 7468 696e 2061 2063 6f6c 6c65  s within a colle
+00003660: 6374 696f 6e2e 204f 6e6c 7920 776f 726b  ction. Only work
+00003670: 7320 666f 7220 2762 6173 6963 2074 7970  s for 'basic typ
+00003680: 6527 2070 726f 7065 7274 6965 7320 2862  e' properties (b
+00003690: 6f6f 6c2c 2069 6e74 2061 6e64 2066 6c6f  ool, int and flo
+000036a0: 6174 2921 204d 756c 7469 2d64 696d 656e  at)! Multi-dimen
+000036b0: 7369 6f6e 616c 2061 7272 6179 7320 286c  sional arrays (l
+000036c0: 696b 6520 6172 7261 7920 6f66 2076 6563  ike array of vec
+000036d0: 746f 7273 2920 7769 6c6c 2062 6520 666c  tors) will be fl
+000036e0: 6174 7465 6e65 6420 696e 746f 2073 6571  attened into seq
+000036f0: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
+00003700: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00003710: 2064 6566 2066 6f72 6561 6368 5f73 6574   def foreach_set
+00003720: 2873 656c 662c 2061 7474 722c 2073 6571  (self, attr, seq
+00003730: 293a 0a20 2020 2020 2020 2027 2727 2054  ):.        ''' T
+00003740: 6869 7320 6973 2061 2066 756e 6374 696f  his is a functio
+00003750: 6e20 746f 2067 6976 6520 6661 7374 2061  n to give fast a
+00003760: 6363 6573 7320 746f 2061 7474 7269 6275  ccess to attribu
+00003770: 7465 7320 7769 7468 696e 2061 2063 6f6c  tes within a col
+00003780: 6c65 6374 696f 6e2e 204f 6e6c 7920 776f  lection. Only wo
+00003790: 726b 7320 666f 7220 2762 6173 6963 2074  rks for 'basic t
+000037a0: 7970 6527 2070 726f 7065 7274 6965 7320  ype' properties 
+000037b0: 2862 6f6f 6c2c 2069 6e74 2061 6e64 2066  (bool, int and f
+000037c0: 6c6f 6174 2921 2073 6571 206d 7573 7420  loat)! seq must 
+000037d0: 6265 2075 6e69 2d64 696d 656e 7369 6f6e  be uni-dimension
+000037e0: 616c 2c20 6d75 6c74 692d 6469 6d65 6e73  al, multi-dimens
+000037f0: 696f 6e61 6c20 6172 7261 7973 2028 6c69  ional arrays (li
+00003800: 6b65 2061 7272 6179 206f 6620 7665 6374  ke array of vect
+00003810: 6f72 7329 2077 696c 6c20 6265 2072 652d  ors) will be re-
+00003820: 6372 6561 7465 6420 6672 6f6d 2069 742e  created from it.
+00003830: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+00003840: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00003850: 6465 6620 6765 7428 7365 6c66 2c0a 2020  def get(self,.  
+00003860: 2020 2020 2020 2020 2020 6b65 793a 2074            key: t
+00003870: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+00003880: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
+00003890: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
+000038a0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+000038b0: 2e41 6e79 5d20 3d20 4e6f 6e65 293a 0a20  .Any] = None):. 
+000038c0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+000038d0: 6e73 2074 6865 2076 616c 7565 206f 6620  ns the value of 
+000038e0: 7468 6520 6974 656d 2061 7373 6967 6e65  the item assigne
+000038f0: 6420 746f 206b 6579 206f 7220 6465 6661  d to key or defa
+00003900: 756c 7420 7768 656e 206e 6f74 2066 6f75  ult when not fou
+00003910: 6e64 2028 6d61 7463 6865 7320 5079 7468  nd (matches Pyth
+00003920: 6f6e 2773 2064 6963 7469 6f6e 6172 7920  on's dictionary 
+00003930: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
+00003940: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
+00003950: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
+00003960: 2054 6865 2069 6465 6e74 6966 6965 7220   The identifier 
+00003970: 666f 7220 7468 6520 636f 6c6c 6563 7469  for the collecti
+00003980: 6f6e 206d 656d 6265 722e 0a20 2020 2020  on member..     
+00003990: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+000039a0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+000039b0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
+000039c0: 6d20 6465 6661 756c 743a 204f 7074 696f  m default: Optio
+000039d0: 6e61 6c20 6172 6775 6d65 6e74 2066 6f72  nal argument for
+000039e0: 2074 6865 2076 616c 7565 2074 6f20 7265   the value to re
+000039f0: 7475 726e 2069 6620 2a6b 6579 2a20 6973  turn if *key* is
+00003a00: 206e 6f74 2066 6f75 6e64 2e0a 2020 2020   not found..    
+00003a10: 2020 2020 3a74 7970 6520 6465 6661 756c      :type defaul
+00003a20: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
+00003a30: 616c 5b74 7970 696e 672e 416e 795d 0a20  al[typing.Any]. 
+00003a40: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00003a50: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00003a60: 2069 7465 6d73 2873 656c 6629 202d 3e20   items(self) -> 
+00003a70: 7479 7069 6e67 2e4c 6973 743a 0a20 2020  typing.List:.   
+00003a80: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
+00003a90: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
+00003aa0: 6f66 2063 6f6c 6c65 6374 696f 6e20 6d65  of collection me
+00003ab0: 6d62 6572 7320 286d 6174 6368 696e 6720  mbers (matching 
+00003ac0: 5079 7468 6f6e 2773 2064 6963 742e 6974  Python's dict.it
+00003ad0: 656d 7328 2920 6675 6e63 7469 6f6e 616c  ems() functional
+00003ae0: 6974 7929 2e0a 0a20 2020 2020 2020 203a  ity)...        :
+00003af0: 7274 7970 653a 2074 7970 696e 672e 4c69  rtype: typing.Li
+00003b00: 7374 0a20 2020 2020 2020 203a 7265 7475  st.        :retu
+00003b10: 726e 3a20 286b 6579 2c20 7661 6c75 6529  rn: (key, value)
+00003b20: 2070 6169 7273 2066 6f72 2065 6163 6820   pairs for each 
+00003b30: 6d65 6d62 6572 206f 6620 7468 6973 2063  member of this c
+00003b40: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
+00003b50: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+00003b60: 6173 730a 0a20 2020 2064 6566 206b 6579  ass..    def key
+00003b70: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
+00003b80: 672e 4c69 7374 5b73 7472 5d3a 0a20 2020  g.List[str]:.   
+00003b90: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
+00003ba0: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
+00003bb0: 6f66 2063 6f6c 6c65 6374 696f 6e20 6d65  of collection me
+00003bc0: 6d62 6572 7320 286d 6174 6368 696e 6720  mbers (matching 
+00003bd0: 5079 7468 6f6e 2773 2064 6963 742e 6b65  Python's dict.ke
+00003be0: 7973 2829 2066 756e 6374 696f 6e61 6c69  ys() functionali
+00003bf0: 7479 292e 0a0a 2020 2020 2020 2020 3a72  ty)...        :r
+00003c00: 7479 7065 3a20 7479 7069 6e67 2e4c 6973  type: typing.Lis
+00003c10: 745b 7374 725d 0a20 2020 2020 2020 203a  t[str].        :
+00003c20: 7265 7475 726e 3a20 7468 6520 6964 656e  return: the iden
+00003c30: 7469 6669 6572 7320 666f 7220 6561 6368  tifiers for each
+00003c40: 206d 656d 6265 7220 6f66 2074 6869 7320   member of this 
+00003c50: 636f 6c6c 6563 7469 6f6e 2e0a 2020 2020  collection..    
+00003c60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+00003c70: 7061 7373 0a0a 2020 2020 6465 6620 7661  pass..    def va
+00003c80: 6c75 6573 2873 656c 6629 202d 3e20 7479  lues(self) -> ty
+00003c90: 7069 6e67 2e4c 6973 743a 0a20 2020 2020  ping.List:.     
+00003ca0: 2020 2027 2727 2052 6574 7572 6e20 7468     ''' Return th
+00003cb0: 6520 7661 6c75 6573 206f 6620 636f 6c6c  e values of coll
+00003cc0: 6563 7469 6f6e 2028 6d61 7463 6869 6e67  ection (matching
+00003cd0: 2050 7974 686f 6e27 7320 6469 6374 2e76   Python's dict.v
+00003ce0: 616c 7565 7328 2920 6675 6e63 7469 6f6e  alues() function
+00003cf0: 616c 6974 7929 2e0a 0a20 2020 2020 2020  ality)...       
+00003d00: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
+00003d10: 4c69 7374 0a20 2020 2020 2020 203a 7265  List.        :re
+00003d20: 7475 726e 3a20 7468 6520 6d65 6d62 6572  turn: the member
+00003d30: 7320 6f66 2074 6869 7320 636f 6c6c 6563  s of this collec
+00003d40: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
+00003d50: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003d60: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
+00003d70: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
+00003d80: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00003d90: 2073 7472 5d29 202d 3e20 2747 656e 6572   str]) -> 'Gener
+00003da0: 6963 5479 7065 273a 0a20 2020 2020 2020  icType':.       
+00003db0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00003dc0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
+00003dd0: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
+00003de0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00003df0: 2073 7472 5d0a 2020 2020 2020 2020 3a72   str].        :r
+00003e00: 7479 7065 3a20 2747 656e 6572 6963 5479  type: 'GenericTy
+00003e10: 7065 270a 2020 2020 2020 2020 2727 270a  pe'.        '''.
+00003e20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00003e30: 2020 6465 6620 5f5f 7365 7469 7465 6d5f    def __setitem_
+00003e40: 5f28 7365 6c66 2c20 6b65 793a 2074 7970  _(self, key: typ
+00003e50: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
+00003e60: 7472 5d2c 2076 616c 7565 3a20 2747 656e  tr], value: 'Gen
+00003e70: 6572 6963 5479 7065 2729 3a0a 2020 2020  ericType'):.    
+00003e80: 2020 2020 2727 2720 0a0a 2020 2020 2020      ''' ..      
+00003e90: 2020 3a70 6172 616d 206b 6579 3a20 0a20    :param key: . 
+00003ea0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+00003eb0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
+00003ec0: 6e74 2c20 7374 725d 0a20 2020 2020 2020  nt, str].       
+00003ed0: 203a 7061 7261 6d20 7661 6c75 653a 200a   :param value: .
+00003ee0: 2020 2020 2020 2020 3a74 7970 6520 7661          :type va
+00003ef0: 6c75 653a 2027 4765 6e65 7269 6354 7970  lue: 'GenericTyp
+00003f00: 6527 0a20 2020 2020 2020 2027 2727 0a20  e'.        '''. 
+00003f10: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00003f20: 2064 6566 205f 5f64 656c 6974 656d 5f5f   def __delitem__
+00003f30: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
+00003f40: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
+00003f50: 725d 2920 2d3e 2027 4765 6e65 7269 6354  r]) -> 'GenericT
+00003f60: 7970 6527 3a0a 2020 2020 2020 2020 2727  ype':.        ''
+00003f70: 2720 0a0a 2020 2020 2020 2020 3a70 6172  ' ..        :par
+00003f80: 616d 206b 6579 3a20 0a20 2020 2020 2020  am key: .       
+00003f90: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
+00003fa0: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
+00003fb0: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
+00003fc0: 653a 2027 4765 6e65 7269 6354 7970 6527  e: 'GenericType'
+00003fd0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00003fe0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+00003ff0: 6566 205f 5f69 7465 725f 5f28 7365 6c66  ef __iter__(self
+00004000: 2920 2d3e 2074 7970 696e 672e 4974 6572  ) -> typing.Iter
+00004010: 6174 6f72 5b27 4765 6e65 7269 6354 7970  ator['GenericTyp
+00004020: 6527 5d3a 0a20 2020 2020 2020 2027 2727  e']:.        '''
+00004030: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
+00004040: 653a 2074 7970 696e 672e 4974 6572 6174  e: typing.Iterat
+00004050: 6f72 5b27 4765 6e65 7269 6354 7970 6527  or['GenericType'
+00004060: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
+00004070: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00004080: 6465 6620 5f5f 6e65 7874 5f5f 2873 656c  def __next__(sel
+00004090: 6629 202d 3e20 2747 656e 6572 6963 5479  f) -> 'GenericTy
+000040a0: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
+000040b0: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
+000040c0: 653a 2027 4765 6e65 7269 6354 7970 6527  e: 'GenericType'
+000040d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000040e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000040f0: 6566 205f 5f6c 656e 5f5f 2873 656c 6629  ef __len__(self)
+00004100: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00004110: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00004120: 7274 7970 653a 2069 6e74 0a20 2020 2020  rtype: int.     
 00004130: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 00004140: 6173 730a 0a0a 636c 6173 7320 6270 795f  ass...class bpy_
 00004150: 7072 6f70 5f61 7272 6179 2874 7970 696e  prop_array(typin
 00004160: 672e 4765 6e65 7269 635b 4765 6e65 7269  g.Generic[Generi
 00004170: 6354 7970 655d 293a 0a20 2020 2064 6566  cType]):.    def
 00004180: 2066 6f72 6561 6368 5f67 6574 2873 656c   foreach_get(sel
 00004190: 662c 2061 7474 722c 2073 6571 293a 0a20  f, attr, seq):. 
@@ -23163,16 +23163,16 @@
 0005a7a0: 3a20 2745 7665 6e74 272c 0a20 2020 2020  : 'Event',.     
 0005a7b0: 2020 2020 2020 2020 2074 7765 616b 3a20           tweak: 
 0005a7c0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
 0005a7d0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
 0005a7e0: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 0005a7f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 0005a800: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-0005a810: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
-0005a820: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
+0005a810: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
+0005a820: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
 0005a830: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
 0005a840: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
 0005a850: 6f6e 7465 7874 3a20 0a20 2020 2020 2020  ontext: .       
 0005a860: 203a 7479 7065 2063 6f6e 7465 7874 3a20   :type context: 
 0005a870: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 0005a880: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 0005a890: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
@@ -23181,42 +23181,42 @@
 0005a8c0: 616b 3a20 5477 6561 6b0a 2020 2020 2020  ak: Tweak.      
 0005a8d0: 2020 3a74 7970 6520 7477 6561 6b3a 2074    :type tweak: t
 0005a8e0: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
 0005a8f0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
 0005a900: 696e 672e 5365 745b 696e 745d 5d0a 2020  ing.Set[int]].  
 0005a910: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 0005a920: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-0005a930: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
-0005a940: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
+0005a930: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
+0005a940: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
 0005a950: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 0005a960: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 0005a970: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 0005a980: 2020 2064 6566 2073 6574 7570 2873 656c     def setup(sel
 0005a990: 6629 3a0a 2020 2020 2020 2020 2727 2720  f):.        ''' 
 0005a9a0: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
 0005a9b0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 0005a9c0: 6465 6620 696e 766f 6b65 2873 656c 662c  def invoke(self,
 0005a9d0: 2063 6f6e 7465 7874 3a20 2743 6f6e 7465   context: 'Conte
 0005a9e0: 7874 272c 2065 7665 6e74 3a20 2745 7665  xt', event: 'Eve
 0005a9f0: 6e74 270a 2020 2020 2020 2020 2020 2020  nt'.            
 0005aa00: 2020 2029 202d 3e20 7479 7069 6e67 2e55     ) -> typing.U
 0005aa10: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0005aa20: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-0005aa30: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+0005aa20: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+0005aa30: 5b69 6e74 5d5d 3a0a 2020 2020 2020 2020  [int]]:.        
 0005aa40: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
 0005aa50: 6172 616d 2063 6f6e 7465 7874 3a20 0a20  aram context: . 
 0005aa60: 2020 2020 2020 203a 7479 7065 2063 6f6e         :type con
 0005aa70: 7465 7874 3a20 2743 6f6e 7465 7874 270a  text: 'Context'.
 0005aa80: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 0005aa90: 7665 6e74 3a20 0a20 2020 2020 2020 203a  vent: .        :
 0005aaa0: 7479 7065 2065 7665 6e74 3a20 2745 7665  type event: 'Eve
 0005aab0: 6e74 270a 2020 2020 2020 2020 3a72 7479  nt'.        :rty
 0005aac0: 7065 3a20 7479 7069 6e67 2e55 6e69 6f6e  pe: typing.Union
-0005aad0: 5b74 7970 696e 672e 5365 745b 696e 745d  [typing.Set[int]
-0005aae0: 2c20 7479 7069 6e67 2e53 6574 5b73 7472  , typing.Set[str
+0005aad0: 5b74 7970 696e 672e 5365 745b 7374 725d  [typing.Set[str]
+0005aae0: 2c20 7479 7069 6e67 2e53 6574 5b69 6e74  , typing.Set[int
 0005aaf0: 5d5d 0a20 2020 2020 2020 203a 7265 7475  ]].        :retu
 0005ab00: 726e 3a20 7265 7375 6c74 0a20 2020 2020  rn: result.     
 0005ab10: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 0005ab20: 6173 730a 0a20 2020 2064 6566 2065 7869  ass..    def exi
 0005ab30: 7428 7365 6c66 2c20 636f 6e74 6578 743a  t(self, context:
 0005ab40: 2027 436f 6e74 6578 7427 2c20 6361 6e63   'Context', canc
 0005ab50: 656c 3a20 7479 7069 6e67 2e4f 7074 696f  el: typing.Optio
@@ -27339,24 +27339,24 @@
 0006aca0: 6e5b 7374 722c 2074 7970 696e 672e 416e  n[str, typing.An
 0006acb0: 795d 203d 204e 6f6e 650a 2020 2020 2727  y] = None.    ''
 0006acc0: 2720 0a0a 2020 2020 3a74 7970 653a 2074  ' ..    :type: t
 0006acd0: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 0006ace0: 2074 7970 696e 672e 416e 795d 0a20 2020   typing.Any].   
 0006acf0: 2027 2727 0a0a 2020 2020 626c 5f6f 7074   '''..    bl_opt
 0006ad00: 696f 6e73 3a20 7479 7069 6e67 2e55 6e69  ions: typing.Uni
-0006ad10: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-0006ad20: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-0006ad30: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+0006ad10: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+0006ad20: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+0006ad30: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
 0006ad40: 2727 2720 4b65 7969 6e67 2053 6574 206f  ''' Keying Set o
 0006ad50: 7074 696f 6e73 2074 6f20 7573 6520 7768  ptions to use wh
 0006ad60: 656e 2069 6e73 6572 7469 6e67 206b 6579  en inserting key
 0006ad70: 6672 616d 6573 0a0a 2020 2020 3a74 7970  frames..    :typ
 0006ad80: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-0006ad90: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-0006ada0: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+0006ad90: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+0006ada0: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 0006adb0: 5d0a 2020 2020 2727 270a 0a20 2020 2064  ].    '''..    d
 0006adc0: 6566 2070 6f6c 6c28 7365 6c66 2c20 636f  ef poll(self, co
 0006add0: 6e74 6578 743a 2074 7970 696e 672e 4f70  ntext: typing.Op
 0006ade0: 7469 6f6e 616c 5b27 436f 6e74 6578 7427  tional['Context'
 0006adf0: 5d29 3a0a 2020 2020 2020 2020 2727 2720  ]):.        ''' 
 0006ae00: 5465 7374 2069 6620 4b65 7969 6e67 2053  Test if Keying S
 0006ae10: 6574 2063 616e 2062 6520 7573 6564 206f  et can be used o
@@ -28100,23 +28100,23 @@
 0006dc30: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
 0006dc40: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 0006dc50: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 0006dc60: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0006dc70: 2e41 6e79 5d0a 2020 2020 2727 270a 0a20  .Any].    '''.. 
 0006dc80: 2020 2062 6c5f 6f70 7469 6f6e 733a 2074     bl_options: t
 0006dc90: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-0006dca0: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
-0006dcb0: 696e 672e 5365 745b 7374 725d 5d20 3d20  ing.Set[str]] = 
+0006dca0: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
+0006dcb0: 696e 672e 5365 745b 696e 745d 5d20 3d20  ing.Set[int]] = 
 0006dcc0: 4e6f 6e65 0a20 2020 2027 2727 204f 7074  None.    ''' Opt
 0006dcd0: 696f 6e73 2066 6f72 2074 6869 7320 6f70  ions for this op
 0006dce0: 6572 6174 6f72 2074 7970 650a 0a20 2020  erator type..   
 0006dcf0: 203a 7479 7065 3a20 7479 7069 6e67 2e55   :type: typing.U
 0006dd00: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-0006dd10: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-0006dd20: 5b73 7472 5d5d 0a20 2020 2027 2727 0a0a  [str]].    '''..
+0006dd10: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+0006dd20: 5b69 6e74 5d5d 0a20 2020 2027 2727 0a0a  [int]].    '''..
 0006dd30: 2020 2020 626c 5f74 7261 6e73 6c61 7469      bl_translati
 0006dd40: 6f6e 5f63 6f6e 7465 7874 3a20 7479 7069  on_context: typi
 0006dd50: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 7479  ng.Union[str, ty
 0006dd60: 7069 6e67 2e41 6e79 5d20 3d20 4e6f 6e65  ping.Any] = None
 0006dd70: 0a20 2020 2027 2727 200a 0a20 2020 203a  .    ''' ..    :
 0006dd80: 7479 7065 3a20 7479 7069 6e67 2e55 6e69  type: typing.Uni
 0006dd90: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
@@ -28151,27 +28151,27 @@
 0006df60: 5072 6f70 6572 7469 6573 2720 3d20 4e6f  Properties' = No
 0006df70: 6e65 0a20 2020 2027 2727 200a 0a20 2020  ne.    ''' ..   
 0006df80: 203a 7479 7065 3a20 274f 7065 7261 746f   :type: 'Operato
 0006df90: 7250 726f 7065 7274 6965 7327 0a20 2020  rProperties'.   
 0006dfa0: 2027 2727 0a0a 2020 2020 6465 6620 7265   '''..    def re
 0006dfb0: 706f 7274 2873 656c 662c 2074 7970 653a  port(self, type:
 0006dfc0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-0006dfd0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-0006dfe0: 7970 696e 672e 5365 745b 7374 725d 5d2c  yping.Set[str]],
+0006dfd0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+0006dfe0: 7970 696e 672e 5365 745b 696e 745d 5d2c  yping.Set[int]],
 0006dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 0006e000: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 0006e010: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 0006e020: 672e 416e 795d 293a 0a20 2020 2020 2020  g.Any]):.       
 0006e030: 2027 2727 2072 6570 6f72 740a 0a20 2020   ''' report..   
 0006e040: 2020 2020 203a 7061 7261 6d20 7479 7065       :param type
 0006e050: 3a20 5479 7065 0a20 2020 2020 2020 203a  : Type.        :
 0006e060: 7479 7065 2074 7970 653a 2074 7970 696e  type type: typin
 0006e070: 672e 556e 696f 6e5b 7479 7069 6e67 2e53  g.Union[typing.S
-0006e080: 6574 5b69 6e74 5d2c 2074 7970 696e 672e  et[int], typing.
-0006e090: 5365 745b 7374 725d 5d0a 2020 2020 2020  Set[str]].      
+0006e080: 6574 5b73 7472 5d2c 2074 7970 696e 672e  et[str], typing.
+0006e090: 5365 745b 696e 745d 5d0a 2020 2020 2020  Set[int]].      
 0006e0a0: 2020 3a70 6172 616d 206d 6573 7361 6765    :param message
 0006e0b0: 3a20 5265 706f 7274 204d 6573 7361 6765  : Report Message
 0006e0c0: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
 0006e0d0: 6573 7361 6765 3a20 7479 7069 6e67 2e55  essage: typing.U
 0006e0e0: 6e69 6f6e 5b73 7472 2c20 7479 7069 6e67  nion[str, typing
 0006e0f0: 2e41 6e79 5d0a 2020 2020 2020 2020 2727  .Any].        ''
 0006e100: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
@@ -37222,23 +37222,23 @@
 00091650: 6f6e 5b73 7472 2c20 7479 7069 6e67 2e41  on[str, typing.A
 00091660: 6e79 5d20 3d20 4e6f 6e65 0a20 2020 2027  ny] = None.    '
 00091670: 2727 200a 0a20 2020 203a 7479 7065 3a20  '' ..    :type: 
 00091680: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 00091690: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 000916a0: 2020 2727 270a 0a20 2020 2062 6c5f 6f70    '''..    bl_op
 000916b0: 7469 6f6e 733a 2074 7970 696e 672e 556e  tions: typing.Un
-000916c0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
-000916d0: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
-000916e0: 7374 725d 5d20 3d20 4e6f 6e65 0a20 2020  str]] = None.   
+000916c0: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
+000916d0: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
+000916e0: 696e 745d 5d20 3d20 4e6f 6e65 0a20 2020  int]] = None.   
 000916f0: 2027 2727 204f 7074 696f 6e73 2066 6f72   ''' Options for
 00091700: 2074 6869 7320 6f70 6572 6174 6f72 2074   this operator t
 00091710: 7970 650a 0a20 2020 203a 7479 7065 3a20  ype..    :type: 
 00091720: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-00091730: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
-00091740: 7069 6e67 2e53 6574 5b73 7472 5d5d 0a20  ping.Set[str]]. 
+00091730: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
+00091740: 7069 6e67 2e53 6574 5b69 6e74 5d5d 0a20  ping.Set[int]]. 
 00091750: 2020 2027 2727 0a0a 2020 2020 626c 5f74     '''..    bl_t
 00091760: 7261 6e73 6c61 7469 6f6e 5f63 6f6e 7465  ranslation_conte
 00091770: 7874 3a20 7479 7069 6e67 2e55 6e69 6f6e  xt: typing.Union
 00091780: 5b73 7472 2c20 7479 7069 6e67 2e41 6e79  [str, typing.Any
 00091790: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 000917a0: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 000917b0: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
@@ -37305,27 +37305,27 @@
 00091b80: 7065 7274 7920 7768 656e 2065 7870 616e  perty when expan
 00091b90: 6469 6e67 2061 6e20 6f70 6572 6174 6f72  ding an operator
 00091ba0: 2069 6e74 6f20 6120 6d65 6e75 2e0a 0a20   into a menu... 
 00091bb0: 2020 203a 7479 7065 3a20 7374 720a 2020     :type: str.  
 00091bc0: 2020 2727 270a 0a20 2020 2064 6566 2072    '''..    def r
 00091bd0: 6570 6f72 7428 7365 6c66 2c20 7479 7065  eport(self, type
 00091be0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b74  : typing.Union[t
-00091bf0: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
-00091c00: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
+00091bf0: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
+00091c00: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
 00091c10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00091c20: 206d 6573 7361 6765 3a20 7479 7069 6e67   message: typing
 00091c30: 2e55 6e69 6f6e 5b73 7472 2c20 7479 7069  .Union[str, typi
 00091c40: 6e67 2e41 6e79 5d29 3a0a 2020 2020 2020  ng.Any]):.      
 00091c50: 2020 2727 2720 7265 706f 7274 0a0a 2020    ''' report..  
 00091c60: 2020 2020 2020 3a70 6172 616d 2074 7970        :param typ
 00091c70: 653a 2054 7970 650a 2020 2020 2020 2020  e: Type.        
 00091c80: 3a74 7970 6520 7479 7065 3a20 7479 7069  :type type: typi
 00091c90: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-00091ca0: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-00091cb0: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
+00091ca0: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+00091cb0: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
 00091cc0: 2020 203a 7061 7261 6d20 6d65 7373 6167     :param messag
 00091cd0: 653a 2052 6570 6f72 7420 4d65 7373 6167  e: Report Messag
 00091ce0: 650a 2020 2020 2020 2020 3a74 7970 6520  e.        :type 
 00091cf0: 6d65 7373 6167 653a 2074 7970 696e 672e  message: typing.
 00091d00: 556e 696f 6e5b 7374 722c 2074 7970 696e  Union[str, typin
 00091d10: 672e 416e 795d 0a20 2020 2020 2020 2027  g.Any].        '
 00091d20: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
@@ -37350,26 +37350,26 @@
 00091e50: 436f 6e74 6578 7427 0a20 2020 2020 2020  Context'.       
 00091e60: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
 00091e70: 730a 0a20 2020 2064 6566 2065 7865 6375  s..    def execu
 00091e80: 7465 2873 656c 662c 2063 6f6e 7465 7874  te(self, context
 00091e90: 3a20 2743 6f6e 7465 7874 270a 2020 2020  : 'Context'.    
 00091ea0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
 00091eb0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-00091ec0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-00091ed0: 7970 696e 672e 5365 745b 7374 725d 5d3a  yping.Set[str]]:
+00091ec0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+00091ed0: 7970 696e 672e 5365 745b 696e 745d 5d3a  yping.Set[int]]:
 00091ee0: 0a20 2020 2020 2020 2027 2727 2045 7865  .        ''' Exe
 00091ef0: 6375 7465 2074 6865 206f 7065 7261 746f  cute the operato
 00091f00: 720a 0a20 2020 2020 2020 203a 7061 7261  r..        :para
 00091f10: 6d20 636f 6e74 6578 743a 200a 2020 2020  m context: .    
 00091f20: 2020 2020 3a74 7970 6520 636f 6e74 6578      :type contex
 00091f30: 743a 2027 436f 6e74 6578 7427 0a20 2020  t: 'Context'.   
 00091f40: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
 00091f50: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-00091f60: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
-00091f70: 672e 5365 745b 7374 725d 5d0a 2020 2020  g.Set[str]].    
+00091f60: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
+00091f70: 672e 5365 745b 696e 745d 5d0a 2020 2020  g.Set[int]].    
 00091f80: 2020 2020 3a72 6574 7572 6e3a 2072 6573      :return: res
 00091f90: 756c 740a 2020 2020 2020 2020 2727 270a  ult.        '''.
 00091fa0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
 00091fb0: 2020 6465 6620 6368 6563 6b28 7365 6c66    def check(self
 00091fc0: 2c20 636f 6e74 6578 743a 2027 436f 6e74  , context: 'Cont
 00091fd0: 6578 7427 2920 2d3e 2062 6f6f 6c3a 0a20  ext') -> bool:. 
 00091fe0: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
@@ -37387,53 +37387,53 @@
 000920a0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
 000920b0: 730a 0a20 2020 2064 6566 2069 6e76 6f6b  s..    def invok
 000920c0: 6528 7365 6c66 2c20 636f 6e74 6578 743a  e(self, context:
 000920d0: 2027 436f 6e74 6578 7427 2c20 6576 656e   'Context', even
 000920e0: 743a 2027 4576 656e 7427 0a20 2020 2020  t: 'Event'.     
 000920f0: 2020 2020 2020 2020 2020 2920 2d3e 2074            ) -> t
 00092100: 7970 696e 672e 556e 696f 6e5b 7479 7069  yping.Union[typi
-00092110: 6e67 2e53 6574 5b69 6e74 5d2c 2074 7970  ng.Set[int], typ
-00092120: 696e 672e 5365 745b 7374 725d 5d3a 0a20  ing.Set[str]]:. 
+00092110: 6e67 2e53 6574 5b73 7472 5d2c 2074 7970  ng.Set[str], typ
+00092120: 696e 672e 5365 745b 696e 745d 5d3a 0a20  ing.Set[int]]:. 
 00092130: 2020 2020 2020 2027 2727 2049 6e76 6f6b         ''' Invok
 00092140: 6520 7468 6520 6f70 6572 6174 6f72 0a0a  e the operator..
 00092150: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
 00092160: 6f6e 7465 7874 3a20 0a20 2020 2020 2020  ontext: .       
 00092170: 203a 7479 7065 2063 6f6e 7465 7874 3a20   :type context: 
 00092180: 2743 6f6e 7465 7874 270a 2020 2020 2020  'Context'.      
 00092190: 2020 3a70 6172 616d 2065 7665 6e74 3a20    :param event: 
 000921a0: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
 000921b0: 7665 6e74 3a20 2745 7665 6e74 270a 2020  vent: 'Event'.  
 000921c0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
 000921d0: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-000921e0: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
-000921f0: 6e67 2e53 6574 5b73 7472 5d5d 0a20 2020  ng.Set[str]].   
+000921e0: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
+000921f0: 6e67 2e53 6574 5b69 6e74 5d5d 0a20 2020  ng.Set[int]].   
 00092200: 2020 2020 203a 7265 7475 726e 3a20 7265       :return: re
 00092210: 7375 6c74 0a20 2020 2020 2020 2027 2727  sult.        '''
 00092220: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
 00092230: 2020 2064 6566 206d 6f64 616c 2873 656c     def modal(sel
 00092240: 662c 2063 6f6e 7465 7874 3a20 2743 6f6e  f, context: 'Con
 00092250: 7465 7874 272c 2065 7665 6e74 3a20 2745  text', event: 'E
 00092260: 7665 6e74 270a 2020 2020 2020 2020 2020  vent'.          
 00092270: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
 00092280: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-00092290: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-000922a0: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
+00092290: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+000922a0: 745b 696e 745d 5d3a 0a20 2020 2020 2020  t[int]]:.       
 000922b0: 2027 2727 204d 6f64 616c 206f 7065 7261   ''' Modal opera
 000922c0: 746f 7220 6675 6e63 7469 6f6e 0a0a 2020  tor function..  
 000922d0: 2020 2020 2020 3a70 6172 616d 2063 6f6e        :param con
 000922e0: 7465 7874 3a20 0a20 2020 2020 2020 203a  text: .        :
 000922f0: 7479 7065 2063 6f6e 7465 7874 3a20 2743  type context: 'C
 00092300: 6f6e 7465 7874 270a 2020 2020 2020 2020  ontext'.        
 00092310: 3a70 6172 616d 2065 7665 6e74 3a20 0a20  :param event: . 
 00092320: 2020 2020 2020 203a 7479 7065 2065 7665         :type eve
 00092330: 6e74 3a20 2745 7665 6e74 270a 2020 2020  nt: 'Event'.    
 00092340: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
 00092350: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-00092360: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-00092370: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
+00092360: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+00092370: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
 00092380: 2020 203a 7265 7475 726e 3a20 7265 7375     :return: resu
 00092390: 6c74 0a20 2020 2020 2020 2027 2727 0a20  lt.        '''. 
 000923a0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 000923b0: 2064 6566 2064 7261 7728 7365 6c66 2c20   def draw(self, 
 000923c0: 636f 6e74 6578 743a 2027 436f 6e74 6578  context: 'Contex
 000923d0: 7427 293a 0a20 2020 2020 2020 2027 2727  t'):.        '''
 000923e0: 2044 7261 7720 6675 6e63 7469 6f6e 2066   Draw function f
@@ -47082,29 +47082,29 @@
 000b7e90: 2020 203a 7479 7065 206d 656d 6f72 795f     :type memory_
 000b7ea0: 7065 616b 3a20 7479 7069 6e67 2e4f 7074  peak: typing.Opt
 000b7eb0: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
 000b7ec0: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
 000b7ed0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
 000b7ee0: 6465 6620 7265 706f 7274 2873 656c 662c  def report(self,
 000b7ef0: 2074 7970 653a 2074 7970 696e 672e 556e   type: typing.Un
-000b7f00: 696f 6e5b 7479 7069 6e67 2e53 6574 5b69  ion[typing.Set[i
-000b7f10: 6e74 5d2c 2074 7970 696e 672e 5365 745b  nt], typing.Set[
-000b7f20: 7374 725d 5d2c 0a20 2020 2020 2020 2020  str]],.         
+000b7f00: 696f 6e5b 7479 7069 6e67 2e53 6574 5b73  ion[typing.Set[s
+000b7f10: 7472 5d2c 2074 7970 696e 672e 5365 745b  tr], typing.Set[
+000b7f20: 696e 745d 5d2c 0a20 2020 2020 2020 2020  int]],.         
 000b7f30: 2020 2020 2020 6d65 7373 6167 653a 2074        message: t
 000b7f40: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
 000b7f50: 2074 7970 696e 672e 416e 795d 293a 0a20   typing.Any]):. 
 000b7f60: 2020 2020 2020 2027 2727 2052 6570 6f72         ''' Repor
 000b7f70: 7420 696e 666f 2c20 7761 726e 696e 6720  t info, warning 
 000b7f80: 6f72 2065 7272 6f72 206d 6573 7361 6765  or error message
 000b7f90: 730a 0a20 2020 2020 2020 203a 7061 7261  s..        :para
 000b7fa0: 6d20 7479 7065 3a20 5479 7065 0a20 2020  m type: Type.   
 000b7fb0: 2020 2020 203a 7479 7065 2074 7970 653a       :type type:
 000b7fc0: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-000b7fd0: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-000b7fe0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+000b7fd0: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+000b7fe0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 000b7ff0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
 000b8000: 6573 7361 6765 3a20 5265 706f 7274 204d  essage: Report M
 000b8010: 6573 7361 6765 0a20 2020 2020 2020 203a  essage.        :
 000b8020: 7479 7065 206d 6573 7361 6765 3a20 7479  type message: ty
 000b8030: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 000b8040: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
 000b8050: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
@@ -66601,23 +66601,23 @@
 00104280: 2066 6163 6573 2077 6974 6820 7468 6520   faces with the 
 00104290: 6375 7272 656e 746c 7920 6469 7370 6c61  currently displa
 001042a0: 7965 6420 696d 6167 6520 6173 7369 676e  yed image assign
 001042b0: 6564 0a0a 2020 2020 3a74 7970 653a 2062  ed..    :type: b
 001042c0: 6f6f 6c0a 2020 2020 2727 270a 0a20 2020  ool.    '''..   
 001042d0: 2073 6e61 705f 656c 656d 656e 7473 3a20   snap_elements: 
 001042e0: 7479 7069 6e67 2e55 6e69 6f6e 5b74 7970  typing.Union[typ
-001042f0: 696e 672e 5365 745b 696e 745d 2c20 7479  ing.Set[int], ty
-00104300: 7069 6e67 2e53 6574 5b73 7472 5d5d 203d  ping.Set[str]] =
+001042f0: 696e 672e 5365 745b 7374 725d 2c20 7479  ing.Set[str], ty
+00104300: 7069 6e67 2e53 6574 5b69 6e74 5d5d 203d  ping.Set[int]] =
 00104310: 204e 6f6e 650a 2020 2020 2727 2720 5479   None.    ''' Ty
 00104320: 7065 206f 6620 656c 656d 656e 7420 746f  pe of element to
 00104330: 2073 6e61 7020 746f 0a0a 2020 2020 3a74   snap to..    :t
 00104340: 7970 653a 2074 7970 696e 672e 556e 696f  ype: typing.Unio
-00104350: 6e5b 7479 7069 6e67 2e53 6574 5b69 6e74  n[typing.Set[int
-00104360: 5d2c 2074 7970 696e 672e 5365 745b 7374  ], typing.Set[st
-00104370: 725d 5d0a 2020 2020 2727 270a 0a20 2020  r]].    '''..   
+00104350: 6e5b 7479 7069 6e67 2e53 6574 5b73 7472  n[typing.Set[str
+00104360: 5d2c 2074 7970 696e 672e 5365 745b 696e  ], typing.Set[in
+00104370: 745d 5d0a 2020 2020 2727 270a 0a20 2020  t]].    '''..   
 00104380: 2073 6e61 705f 6661 6365 5f6e 6561 7265   snap_face_neare
 00104390: 7374 5f73 7465 7073 3a20 696e 7420 3d20  st_steps: int = 
 001043a0: 4e6f 6e65 0a20 2020 2027 2727 204e 756d  None.    ''' Num
 001043b0: 6265 7220 6f66 2073 7465 7073 2074 6f20  ber of steps to 
 001043c0: 6272 6561 6b20 7472 616e 7366 6f72 6d61  break transforma
 001043d0: 7469 6f6e 2069 6e74 6f20 666f 7220 6661  tion into for fa
 001043e0: 6365 206e 6561 7265 7374 2073 6e61 7070  ce nearest snapp
@@ -108240,16 +108240,16 @@
 001a6cf0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
 001a6d00: 2020 2020 2020 2020 2020 2020 2020 6576                ev
 001a6d10: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
 001a6d20: 6f6e 616c 5b27 4576 656e 7427 5d0a 2020  onal['Event'].  
 001a6d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a6d40: 2020 2020 2020 2020 2029 202d 3e20 7479           ) -> ty
 001a6d50: 7069 6e67 2e55 6e69 6f6e 5b74 7970 696e  ping.Union[typin
-001a6d60: 672e 5365 745b 696e 745d 2c20 7479 7069  g.Set[int], typi
-001a6d70: 6e67 2e53 6574 5b73 7472 5d5d 3a0a 2020  ng.Set[str]]:.  
+001a6d60: 672e 5365 745b 7374 725d 2c20 7479 7069  g.Set[str], typi
+001a6d70: 6e67 2e53 6574 5b69 6e74 5d5d 3a0a 2020  ng.Set[int]]:.  
 001a6d80: 2020 2020 2020 2727 2720 4f70 6572 6174        ''' Operat
 001a6d90: 6f72 2070 6f70 7570 2069 6e76 6f6b 6520  or popup invoke 
 001a6da0: 2873 686f 7720 6f70 6572 6174 6f72 2070  (show operator p
 001a6db0: 726f 7065 7274 6965 7320 616e 6420 6578  roperties and ex
 001a6dc0: 6563 7574 6520 6974 2061 7574 6f6d 6174  ecute it automat
 001a6dd0: 6963 616c 6c79 206f 6e20 6368 616e 6765  ically on change
 001a6de0: 7329 0a0a 2020 2020 2020 2020 3a70 6172  s)..        :par
@@ -108261,16 +108261,16 @@
 001a6e40: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
 001a6e50: 2065 7665 6e74 3a20 4576 656e 740a 2020   event: Event.  
 001a6e60: 2020 2020 2020 3a74 7970 6520 6576 656e        :type even
 001a6e70: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
 001a6e80: 616c 5b27 4576 656e 7427 5d0a 2020 2020  al['Event'].    
 001a6e90: 2020 2020 3a72 7479 7065 3a20 7479 7069      :rtype: typi
 001a6ea0: 6e67 2e55 6e69 6f6e 5b74 7970 696e 672e  ng.Union[typing.
-001a6eb0: 5365 745b 696e 745d 2c20 7479 7069 6e67  Set[int], typing
-001a6ec0: 2e53 6574 5b73 7472 5d5d 0a20 2020 2020  .Set[str]].     
+001a6eb0: 5365 745b 7374 725d 2c20 7479 7069 6e67  Set[str], typing
+001a6ec0: 2e53 6574 5b69 6e74 5d5d 0a20 2020 2020  .Set[int]].     
 001a6ed0: 2020 203a 7265 7475 726e 3a20 7265 7375     :return: resu
 001a6ee0: 6c74 0a20 2020 2020 2020 2027 2727 0a20  lt.        '''. 
 001a6ef0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
 001a6f00: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
 001a6f10: 2020 6465 6620 696e 766f 6b65 5f70 726f    def invoke_pro
 001a6f20: 7073 5f64 6961 6c6f 6728 0a20 2020 2020  ps_dialog(.     
 001a6f30: 2020 2020 2020 2063 6c73 2c0a 2020 2020         cls,.    
@@ -108278,16 +108278,16 @@
 001a6f50: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
 001a6f60: 6c5b 274f 7065 7261 746f 7227 5d2c 0a20  l['Operator'],. 
 001a6f70: 2020 2020 2020 2020 2020 2077 6964 7468             width
 001a6f80: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
 001a6f90: 6c5b 7479 7069 6e67 2e41 6e79 5d20 3d20  l[typing.Any] = 
 001a6fa0: 3330 300a 2020 2020 2920 2d3e 2074 7970  300.    ) -> typ
 001a6fb0: 696e 672e 556e 696f 6e5b 7479 7069 6e67  ing.Union[typing
-001a6fc0: 2e53 6574 5b69 6e74 5d2c 2074 7970 696e  .Set[int], typin
-001a6fd0: 672e 5365 745b 7374 725d 5d3a 0a20 2020  g.Set[str]]:.   
+001a6fc0: 2e53 6574 5b73 7472 5d2c 2074 7970 696e  .Set[str], typin
+001a6fd0: 672e 5365 745b 696e 745d 5d3a 0a20 2020  g.Set[int]]:.   
 001a6fe0: 2020 2020 2027 2727 204f 7065 7261 746f       ''' Operato
 001a6ff0: 7220 6469 616c 6f67 2028 6e6f 6e2d 6175  r dialog (non-au
 001a7000: 746f 6578 6563 2070 6f70 7570 2920 696e  toexec popup) in
 001a7010: 766f 6b65 2028 7368 6f77 206f 7065 7261  voke (show opera
 001a7020: 746f 7220 7072 6f70 6572 7469 6573 2061  tor properties a
 001a7030: 6e64 206f 6e6c 7920 6578 6563 7574 6520  nd only execute 
 001a7040: 6974 206f 6e20 636c 6963 6b20 6f6e 204f  it on click on O
@@ -108301,16 +108301,16 @@
 001a70c0: 203a 7061 7261 6d20 7769 6474 683a 2057   :param width: W
 001a70d0: 6964 7468 206f 6620 7468 6520 706f 7075  idth of the popu
 001a70e0: 700a 2020 2020 2020 2020 3a74 7970 6520  p.        :type 
 001a70f0: 7769 6474 683a 2074 7970 696e 672e 4f70  width: typing.Op
 001a7100: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
 001a7110: 795d 0a20 2020 2020 2020 203a 7274 7970  y].        :rtyp
 001a7120: 653a 2074 7970 696e 672e 556e 696f 6e5b  e: typing.Union[
-001a7130: 7479 7069 6e67 2e53 6574 5b69 6e74 5d2c  typing.Set[int],
-001a7140: 2074 7970 696e 672e 5365 745b 7374 725d   typing.Set[str]
+001a7130: 7479 7069 6e67 2e53 6574 5b73 7472 5d2c  typing.Set[str],
+001a7140: 2074 7970 696e 672e 5365 745b 696e 745d   typing.Set[int]
 001a7150: 5d0a 2020 2020 2020 2020 3a72 6574 7572  ].        :retur
 001a7160: 6e3a 2072 6573 756c 740a 2020 2020 2020  n: result.      
 001a7170: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 001a7180: 7373 0a0a 2020 2020 4063 6c61 7373 6d65  ss..    @classme
 001a7190: 7468 6f64 0a20 2020 2064 6566 2069 6e76  thod.    def inv
 001a71a0: 6f6b 655f 7365 6172 6368 5f70 6f70 7570  oke_search_popup
 001a71b0: 2863 6c73 2c20 6f70 6572 6174 6f72 3a20  (cls, operator: 
@@ -108343,17 +108343,17 @@
 001a7360: 5b27 4f70 6572 6174 6f72 275d 2c0a 2020  ['Operator'],.  
 001a7370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a7380: 2020 2077 6964 7468 3a20 7479 7069 6e67     width: typing
 001a7390: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
 001a73a0: 2e41 6e79 5d20 3d20 3330 300a 2020 2020  .Any] = 300.    
 001a73b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a73c0: 2029 202d 3e20 7479 7069 6e67 2e55 6e69   ) -> typing.Uni
-001a73d0: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-001a73e0: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-001a73f0: 7472 5d5d 3a0a 2020 2020 2020 2020 2727  tr]]:.        ''
+001a73d0: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+001a73e0: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+001a73f0: 6e74 5d5d 3a0a 2020 2020 2020 2020 2727  nt]]:.        ''
 001a7400: 2720 4f70 6572 6174 6f72 2070 6f70 7570  ' Operator popup
 001a7410: 2069 6e76 6f6b 6520 286f 6e6c 7920 7368   invoke (only sh
 001a7420: 6f77 7320 6f70 6572 6174 6f72 2773 2070  ows operator's p
 001a7430: 726f 7065 7274 6965 732c 2077 6974 686f  roperties, witho
 001a7440: 7574 2065 7865 6375 7469 6e67 2069 7429  ut executing it)
 001a7450: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
 001a7460: 206f 7065 7261 746f 723a 204f 7065 7261   operator: Opera
@@ -108365,32 +108365,32 @@
 001a74c0: 6964 7468 3a20 5769 6474 6820 6f66 2074  idth: Width of t
 001a74d0: 6865 2070 6f70 7570 0a20 2020 2020 2020  he popup.       
 001a74e0: 203a 7479 7065 2077 6964 7468 3a20 7479   :type width: ty
 001a74f0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
 001a7500: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
 001a7510: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 001a7520: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a7530: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-001a7540: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
+001a7530: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+001a7540: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
 001a7550: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 001a7560: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 001a7570: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
 001a7580: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
 001a7590: 6465 6620 696e 766f 6b65 5f63 6f6e 6669  def invoke_confi
 001a75a0: 726d 2863 6c73 2c20 6f70 6572 6174 6f72  rm(cls, operator
 001a75b0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
 001a75c0: 6c5b 274f 7065 7261 746f 7227 5d2c 0a20  l['Operator'],. 
 001a75d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 001a75e0: 2020 2020 2020 6576 656e 743a 2074 7970        event: typ
 001a75f0: 696e 672e 4f70 7469 6f6e 616c 5b27 4576  ing.Optional['Ev
 001a7600: 656e 7427 5d0a 2020 2020 2020 2020 2020  ent'].          
 001a7610: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
 001a7620: 3e20 7479 7069 6e67 2e55 6e69 6f6e 5b74  > typing.Union[t
-001a7630: 7970 696e 672e 5365 745b 696e 745d 2c20  yping.Set[int], 
-001a7640: 7479 7069 6e67 2e53 6574 5b73 7472 5d5d  typing.Set[str]]
+001a7630: 7970 696e 672e 5365 745b 7374 725d 2c20  yping.Set[str], 
+001a7640: 7479 7069 6e67 2e53 6574 5b69 6e74 5d5d  typing.Set[int]]
 001a7650: 3a0a 2020 2020 2020 2020 2727 2720 4f70  :.        ''' Op
 001a7660: 6572 6174 6f72 2063 6f6e 6669 726d 6174  erator confirmat
 001a7670: 696f 6e20 706f 7075 7020 286f 6e6c 7920  ion popup (only 
 001a7680: 746f 206c 6574 2075 7365 7220 636f 6e66  to let user conf
 001a7690: 6972 6d20 7468 6520 6578 6563 7574 696f  irm the executio
 001a76a0: 6e2c 206e 6f20 6f70 6572 6174 6f72 2070  n, no operator p
 001a76b0: 726f 7065 7274 6965 7320 7368 6f77 6e29  roperties shown)
@@ -108403,16 +108403,16 @@
 001a7720: 2020 2020 2020 2020 3a70 6172 616d 2065          :param e
 001a7730: 7665 6e74 3a20 4576 656e 740a 2020 2020  vent: Event.    
 001a7740: 2020 2020 3a74 7970 6520 6576 656e 743a      :type event:
 001a7750: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
 001a7760: 5b27 4576 656e 7427 5d0a 2020 2020 2020  ['Event'].      
 001a7770: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
 001a7780: 2e55 6e69 6f6e 5b74 7970 696e 672e 5365  .Union[typing.Se
-001a7790: 745b 696e 745d 2c20 7479 7069 6e67 2e53  t[int], typing.S
-001a77a0: 6574 5b73 7472 5d5d 0a20 2020 2020 2020  et[str]].       
+001a7790: 745b 7374 725d 2c20 7479 7069 6e67 2e53  t[str], typing.S
+001a77a0: 6574 5b69 6e74 5d5d 0a20 2020 2020 2020  et[int]].       
 001a77b0: 203a 7265 7475 726e 3a20 7265 7375 6c74   :return: result
 001a77c0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
 001a77d0: 2020 2020 2070 6173 730a 0a20 2020 2040       pass..    @
 001a77e0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
 001a77f0: 6465 6620 706f 706d 656e 755f 6265 6769  def popmenu_begi
 001a7800: 6e5f 5f69 6e74 6572 6e61 6c28 636c 732c  n__internal(cls,
 001a7810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
@@ -114395,22 +114395,22 @@
 001beda0: 6d65 7472 7920 746f 2066 6f72 6d20 706c  metry to form pl
 001bedb0: 616e 6172 2070 6f6c 7967 6f6e 732e 0a0a  anar polygons...
 001bedc0: 2020 2020 3a74 7970 653a 2074 7970 696e      :type: typin
 001bedd0: 672e 556e 696f 6e5b 7374 722c 2069 6e74  g.Union[str, int
 001bede0: 5d0a 2020 2020 2727 270a 0a20 2020 2064  ].    '''..    d
 001bedf0: 656c 696d 6974 3a20 7479 7069 6e67 2e55  elimit: typing.U
 001bee00: 6e69 6f6e 5b74 7970 696e 672e 5365 745b  nion[typing.Set[
-001bee10: 696e 745d 2c20 7479 7069 6e67 2e53 6574  int], typing.Set
-001bee20: 5b73 7472 5d5d 203d 204e 6f6e 650a 2020  [str]] = None.  
+001bee10: 7374 725d 2c20 7479 7069 6e67 2e53 6574  str], typing.Set
+001bee20: 5b69 6e74 5d5d 203d 204e 6f6e 650a 2020  [int]] = None.  
 001bee30: 2020 2727 2720 4c69 6d69 7420 6d65 7267    ''' Limit merg
 001bee40: 696e 6720 6765 6f6d 6574 7279 0a0a 2020  ing geometry..  
 001bee50: 2020 3a74 7970 653a 2074 7970 696e 672e    :type: typing.
 001bee60: 556e 696f 6e5b 7479 7069 6e67 2e53 6574  Union[typing.Set
-001bee70: 5b69 6e74 5d2c 2074 7970 696e 672e 5365  [int], typing.Se
-001bee80: 745b 7374 725d 5d0a 2020 2020 2727 270a  t[str]].    '''.
+001bee70: 5b73 7472 5d2c 2074 7970 696e 672e 5365  [str], typing.Se
+001bee80: 745b 696e 745d 5d0a 2020 2020 2727 270a  t[int]].    '''.
 001bee90: 0a20 2020 2066 6163 655f 636f 756e 743a  .    face_count:
 001beea0: 2069 6e74 203d 204e 6f6e 650a 2020 2020   int = None.    
 001beeb0: 2727 2720 5468 6520 6375 7272 656e 7420  ''' The current 
 001beec0: 6e75 6d62 6572 206f 6620 6661 6365 7320  number of faces 
 001beed0: 696e 2074 6865 2064 6563 696d 6174 6564  in the decimated
 001beee0: 206d 6573 680a 0a20 2020 203a 7479 7065   mesh..    :type
 001beef0: 3a20 696e 740a 2020 2020 2727 270a 0a20  : int.    '''.. 
@@ -115678,21 +115678,21 @@
 001c3dd0: 5061 7468 2074 6f20 6578 7465 726e 616c  Path to external
 001c3de0: 2064 6973 706c 6163 656d 656e 7473 2066   displacements f
 001c3df0: 696c 650a 0a20 2020 203a 7479 7065 3a20  ile..    :type: 
 001c3e00: 7479 7069 6e67 2e55 6e69 6f6e 5b73 7472  typing.Union[str
 001c3e10: 2c20 7479 7069 6e67 2e41 6e79 5d0a 2020  , typing.Any].  
 001c3e20: 2020 2727 270a 0a20 2020 2066 6c69 705f    '''..    flip_
 001c3e30: 6178 6973 3a20 7479 7069 6e67 2e55 6e69  axis: typing.Uni
-001c3e40: 6f6e 5b74 7970 696e 672e 5365 745b 696e  on[typing.Set[in
-001c3e50: 745d 2c20 7479 7069 6e67 2e53 6574 5b73  t], typing.Set[s
-001c3e60: 7472 5d5d 203d 204e 6f6e 650a 2020 2020  tr]] = None.    
+001c3e40: 6f6e 5b74 7970 696e 672e 5365 745b 7374  on[typing.Set[st
+001c3e50: 725d 2c20 7479 7069 6e67 2e53 6574 5b69  r], typing.Set[i
+001c3e60: 6e74 5d5d 203d 204e 6f6e 650a 2020 2020  nt]] = None.    
 001c3e70: 2727 2720 0a0a 2020 2020 3a74 7970 653a  ''' ..    :type:
 001c3e80: 2074 7970 696e 672e 556e 696f 6e5b 7479   typing.Union[ty
-001c3e90: 7069 6e67 2e53 6574 5b69 6e74 5d2c 2074  ping.Set[int], t
-001c3ea0: 7970 696e 672e 5365 745b 7374 725d 5d0a  yping.Set[str]].
+001c3e90: 7069 6e67 2e53 6574 5b73 7472 5d2c 2074  ping.Set[str], t
+001c3ea0: 7970 696e 672e 5365 745b 696e 745d 5d0a  yping.Set[int]].
 001c3eb0: 2020 2020 2727 270a 0a20 2020 2066 6f72      '''..    for
 001c3ec0: 7761 7264 5f61 7869 733a 2074 7970 696e  ward_axis: typin
 001c3ed0: 672e 556e 696f 6e5b 7374 722c 2069 6e74  g.Union[str, int
 001c3ee0: 5d20 3d20 4e6f 6e65 0a20 2020 2027 2727  ] = None.    '''
 001c3ef0: 200a 0a20 2020 203a 7479 7065 3a20 7479   ..    :type: ty
 001c3f00: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
 001c3f10: 696e 745d 0a20 2020 2027 2727 0a0a 2020  int].    '''..
```

### Comparing `fake-bpy-module-latest-20230429/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230430/bpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/utils/previews.py` & `fake-bpy-module-latest-20230430/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy/utils/units.py` & `fake-bpy-module-latest-20230430/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence'],
+        Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Object', 'bpy.types.Action', 'bpy.types.Sequence']
+    :type object_action_pairs: typing.Union['bpy.types.Sequence', 'bpy.types.Action', 'bpy.types.Object']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230430/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230430/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/bpy_types.py` & `fake-bpy-module-latest-20230430/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230429
+Version: 20230430
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230429/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230430/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230430/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/functions.py` & `fake-bpy-module-latest-20230430/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/predicates.py` & `fake-bpy-module-latest-20230430/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/shaders.py` & `fake-bpy-module-latest-20230430/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/types.py` & `fake-bpy-module-latest-20230430/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230430/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230430/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/capabilities.py` & `fake-bpy-module-latest-20230430/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/matrix.py` & `fake-bpy-module-latest-20230430/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/platform.py` & `fake-bpy-module-latest-20230430/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/shader.py` & `fake-bpy-module-latest-20230430/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/state.py` & `fake-bpy-module-latest-20230430/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/texture.py` & `fake-bpy-module-latest-20230430/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu/types.py` & `fake-bpy-module-latest-20230430/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu_extras/batch.py` & `fake-bpy-module-latest-20230430/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/gpu_extras/presets.py` & `fake-bpy-module-latest-20230430/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/idprop/types.py` & `fake-bpy-module-latest-20230430/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/imbuf/__init__.py` & `fake-bpy-module-latest-20230430/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/imbuf/types.py` & `fake-bpy-module-latest-20230430/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/keyingsets_builtins.py` & `fake-bpy-module-latest-20230430/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/keyingsets_utils.py` & `fake-bpy-module-latest-20230430/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/mathutils/__init__.py` & `fake-bpy-module-latest-20230430/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230430/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/mathutils/geometry.py` & `fake-bpy-module-latest-20230430/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/mathutils/kdtree.py` & `fake-bpy-module-latest-20230430/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/mathutils/noise.py` & `fake-bpy-module-latest-20230430/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/nodeitems_builtins.py` & `fake-bpy-module-latest-20230430/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/nodeitems_utils.py` & `fake-bpy-module-latest-20230430/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/rna_info.py` & `fake-bpy-module-latest-20230430/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/rna_keymap_ui.py` & `fake-bpy-module-latest-20230430/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/rna_prop_ui.py` & `fake-bpy-module-latest-20230430/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/rna_xml.py` & `fake-bpy-module-latest-20230430/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230429/setup.py` & `fake-bpy-module-latest-20230430/setup.py`

 * *Files identical despite different names*

