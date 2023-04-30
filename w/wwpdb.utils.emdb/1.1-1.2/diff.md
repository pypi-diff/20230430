# Comparing `tmp/wwpdb.utils.emdb-1.1.tar.gz` & `tmp/wwpdb.utils.emdb-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.1.tar", last modified: Fri Mar 17 18:46:32 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.2.tar", last modified: Sun Apr 30 13:10:36 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.1.tar` & `wwpdb.utils.emdb-1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.963534 wwpdb.utils.emdb-1.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-03-17 18:46:32.963534 wwpdb.utils.emdb-1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-03-17 18:46:32.967534 wwpdb.utils.emdb-1.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2223 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.959534 wwpdb.utils.emdb-1.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.959534 wwpdb.utils.emdb-1.1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.959534 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.963534 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   662511 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  1660130 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)      329 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.963534 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   217615 2023-03-17 18:45:20.000000 wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 18:46:32.959534 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-03-17 18:46:32.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-03-17 18:46:32.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-17 18:46:32.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-03-17 18:46:32.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-03-17 18:46:15.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-03-17 18:46:32.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-03-17 18:46:32.000000 wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-30 13:10:36.631974 wwpdb.utils.emdb-1.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2223 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.619974 wwpdb.utils.emdb-1.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.623974 wwpdb.utils.emdb-1.2/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.623974 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   663967 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  1660129 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      329 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.627974 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   217704 2023-04-30 13:09:34.000000 wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-30 13:10:36.623974 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-30 13:10:22.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-30 13:10:36.000000 wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.1/PKG-INFO` & `wwpdb.utils.emdb-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.1
+Version: 1.2
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.1/setup.py` & `wwpdb.utils.emdb-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.3.0"
+        XML_OUT_VERSION = "3.0.3.2"
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
         EM_DEPUI = "em_depui"
@@ -182,14 +182,15 @@
         PDBX_ENTITY_NONPOLY = "pdbx_entity_nonpoly"
         PDBX_DEPOSITOR_INFO = "pdbx_struct_ref_seq_depositor_info"
         STRUCT_REF = "struct_ref"
         PDBX_OBS_SPR = "pdbx_database_PDB_obs_spr"
         PDBX_AUDIT_SUPPORT = "pdbx_audit_support"
         PDBX_CONTACT_AUTHOR = "pdbx_contact_author"
         STRUCT = "struct"
+        STRUCT_KEYWORDS = "struct_keywords"
         PDBX_DICT_ITEM_MAPPING = "pdbx_dict_item_mapping"
 
         # Keys
         K_EM_DIFFRACTION_STATS_ID = "em_diffraction_stats_id"
         K_SAMPLE_SUPPORT_ID = "sample_support_id"
         K_IMAGE_PROCESSING_ID = "image_processing_id"
         K_IMAGE_RECORDING_ID = "image_recording_id"
@@ -611,14 +612,15 @@
             "_em_admin.deposition_date": '<xs:element name="deposition" type="xs:date">',
             "_em_admin.header_release_date": '<xs:element name="header_release" type="xs:date" minOccurs="0">',
             "_em_admin.map_release_date": '<xs:element name="map_release" type="xs:date" minOccurs="0">',
             "_em_admin.obsoleted_date": '<xs:element name="obsolete" type="xs:date" minOccurs="0">',
             "_em_admin.last_update": '<xs:element name="update" type="xs:date">',  # noqa: F601 pylint: disable=duplicate-key
             "_em_admin.title": '<xs:element name="title" type="xs:token">',
             "_em_admin.details": '<xs:element name="details" type="xs:token" minOccurs="0">',
+            "_em_admin.keywords": '<xs:element name="keywords" type="xs:token" minOccurs="0">',
             "_em_euler_angle_assignment.type": '<xs:element name="type">',
             "_em_euler_angle_assignment.proj_matching_num_projections": '<xs:element name="number_reference_projections" type="xs:positiveInteger" minOccurs="0"/>',
             "_em_euler_angle_assignment.proj_matching_merit_function": '<xs:element name="merit_function" type="xs:token" minOccurs="0"/>',
             "_em_euler_angle_assignment.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_em_euler_angle_assignment.proj_matching_angular_sampling": '<xs:element name="angular_sampling" minOccurs="0">',
             "_em_author_list.identifier_ORCID": '<xs:attribute name="ORCID" type="ORCID_type"/>',
             "_em_db_reference.access_code": '<xs:element name="emdb_id" type="emdb_id_type"/>',
@@ -704,14 +706,15 @@
             "_em_volume_selection.num_tomograms": '<xs:element name="number_tomograms" type="xs:positiveInteger"/>',
             "_em_volume_selection.num_volumes_extracted": '<xs:element name="number_images_used" type="xs:positiveInteger"/>',
             "_em_volume_selection.reference_model": '<xs:element name="reference_model" type="xs:token" minOccurs="0">',
             "_em_volume_selection.method": '<xs:element name="method" type="xs:string" minOccurs="0">',
             "_em_volume_selection.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_pdbx_database_status.process_site": '<xs:element name="processing_site" minOccurs="0">',
             "_struct.title": '<xs:element name="title" type="xs:token">',
+            "_struct_keywords.text": '<xs:element name="keywords" type="xs:string" minOccurs="0">',
             "_citation.title": '<xs:element name="title" type="xs:token"/>',
             "_citation.journal_full": '<xs:element name="journal" type="xs:token" minOccurs="0"/>',
             "_citation.journal_abbrev": '<xs:element name="journal_abbreviation" type="xs:token"/>',
             "_citation.country": '<xs:element name="country" type="xs:token" minOccurs="0"/>',
             "_citation.journal_issue": '<xs:element name="issue" type="xs:positiveInteger" minOccurs="0"/>',
             "_citation.journal_volume": '<xs:element name="volume" type="xs:string" nillable="true" minOccurs="0"/>',
             "_citation.page_first": '<xs:element name="first_page" type="page_type" nillable="false" minOccurs="0"/>',
@@ -1332,14 +1335,15 @@
                 const.PDBX_DATABASE_STATUS,
                 const.PDBX_ENTITY_NONPOLY,
                 const.PDBX_DEPOSITOR_INFO,
                 const.PDBX_OBS_SPR,
                 const.PDBX_AUDIT_SUPPORT,
                 const.PDBX_CONTACT_AUTHOR,
                 const.STRUCT,
+                const.STRUCT_KEYWORDS,
                 const.PDBX_ENTITY_SRC_SYN,
                 const.EM_SUPERSEDE,
                 const.EM_OBSOLETE,
             ],
         )
         self.cif = Cif(container)
         if container is not None or container == {}:
@@ -2481,15 +2485,15 @@
                         """
                         if same_as_pdb == "YES":
                             # CIF: _audit_author
                             set_cif_value(author_with_ORCID.set_ORCID, "identifier_ORCID", const.AUDIT_AUTHOR, cif_list=auth_in)
                             author = get_cif_value("name", const.AUDIT_AUTHOR, cif_list=auth_in)
                         else:
                             # CIF: _em_author_list
-                            set_cif_value(author_with_ORCID.set_ORCID, "identifier_ORCID", const.EM_AUTHOR_LIST)
+                            set_cif_value(author_with_ORCID.set_ORCID, "identifier_ORCID", const.EM_AUTHOR_LIST, cif_list=auth_in)
                             author = get_cif_value("author", const.EM_AUTHOR_LIST, cif_list=auth_in)
 
                         fmt_auth = format_author(author)
                         if fmt_auth != "":
                             author_with_ORCID.set_valueOf_(fmt_auth)
                         else:
                             txt = u"Author (%s) is not added to the list of authors as the format is wrong." % author
@@ -2518,19 +2522,20 @@
                 """
                 EMDB administration details
                 XSD: <xs:element name="details" type="xs:token" minOccurs="0">
                 CIF: _em_admin.details
                 Deprecated (2014-10-21)
                 """
 
-            def set_el_keywords():
+            def set_el_keywords(admin, key_words):
                 """
-                XSD: <name="keywords" type="xs:string" xs:element minOccurs="0">
+                XSD: <name="z" type="xs:string" xs:element minOccurs="0">
                 DEPRECATED 2014-10-21
                 """
+                set_cif_value(admin.set_keywords, "text", const.STRUCT_KEYWORDS, cif_list=key_words)
 
             def set_el_replace_existing_entry():
                 """
                 XSD: <xs:element name="replace_existing_entry" type="xs:boolean">
                 CIF: _em_admin.replace_existing_entry_flag NO
                 DEPRECATED (2014-10-21)
                 """
@@ -2557,15 +2562,19 @@
             # element 9
             set_el_title(admin)
             # element 10
             set_el_authors_list(admin)
             # element 11
             set_el_details()
             # element 12
-            set_el_keywords()
+            keywords_in = make_dict(const.STRUCT_KEYWORDS, "entry_id")
+            for key_words in keywords_in.values():
+                pdbx_keywords = get_cif_value("text", const.STRUCT_KEYWORDS, cif_list=key_words)
+                if pdbx_keywords is not None:
+                    set_el_keywords(admin, key_words)
             # element 13
             set_el_replace_existing_entry()
 
         def set_crossreferences_type(cross_references):
             """
             Sets <xs:complexType name="crossreferences_type"> as
             ...a sequence of 4 elements
@@ -8472,16 +8481,15 @@
                         set_el_choices(st_map, sm_in)
                         # element 1
                         set_el_details(st_map, sm_in)
 
                     for sm_in in st_mod_dict_in[ip_id_in]:
                         st_map = emdb.starting_map_type()
                         set_starting_map_type(st_map, sm_in)
-                        if st_map.hasContent_():
-                            im_proc.add_startup_model(st_map)
+                        im_proc.add_startup_model(st_map)
 
                 def set_final_reconstruction(final_rec, ip_id_in, final_dicts):
                     """
                     Final reconstruction for every method but non-subtomographs
 
                     @param ip_id_in: image processing id
                     @param im_proc: image processing object
@@ -10996,15 +11004,21 @@
                                             set_cif_value(chain.set_number_of_copies_in_final_model, "number_of_copies_in_final_model", const.EM_3D_FITTING_LIST, cif_list=model_in)
 
                                         def set_el_source_name(chain, model_in):
                                             """
                                             XSD: <xs:element name="source_name" type="xs:string"  minOccurs="0" maxOccurs="1">
                                             CIF: _em_3d_fitting_list.source_name SwissModel
                                             """
+                                            access_code = get_cif_value("pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
+                                            sourcename = get_cif_value("source_name", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             set_cif_value(chain.set_source_name, "source_name", const.EM_3D_FITTING_LIST, cif_list=model_in)
+                                            if sourcename == "PDB" and access_code is None:
+                                                txt = u"Error! Missing PDB ID. If initial model is from PDB, then access code is mandatory."
+                                                self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
+                                                self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
                                         def set_el_initial_model_type(chain, model_in):
                                             """
                                             XSD: <xs:element name="initial_model_type" type="xs:string"  minOccurs="0" maxOccurs="1">
                                             CIF: _em_3d_fitting_list.type experimental model
                                             """
                                             set_cif_value(chain.set_initial_model_type, "type", const.EM_3D_FITTING_LIST, cif_list=model_in)
```

### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Fri Mar  3 15:24:47 2023 by generateDS.py version 2.29.5.
+# Generated Fri Mar 24 10:07:40 2023 by generateDS.py version 2.29.5.
 # Python 2.7.15 | packaged by conda-forge | (default, Mar  5 2020, 14:58:04)  [GCC Clang 9.0.1 ]
 #
 # Command line options:
 #   ('--root-element', 'emd')
 #   ('-f', '')
-#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_3_0/emdb.py')
+#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_3_2/emdb.py')
 #   ('--no-warnings', '')
 #   ('--external-encoding', 'utf-8')
 #
 # Command line arguments:
-#   emdb-schemas/emdb_schemas/v3/v3_0_3_0/emdb.xsd
+#   emdb-schemas/emdb_schemas/v3/v3_0_3_2/emdb.xsd
 #
 # Command line:
-#   emdb_config/emdb_config/modified_generateDS/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_3_0/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_3_0/emdb.xsd
+#   emdb_config/emdb_config/modified_generateDS/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_3_2/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_3_2/emdb.xsd
 #
 # Current working directory (os.getcwd()):
 #   IdeaProjects
 #
 
 import sys
 import re as re_
@@ -735,15 +735,15 @@
 # Data representation classes.
 #
 
 
 class entry_type(GeneratedsSuper):
     subclass = None
     superclass = None
-    def __init__(self, emdb_id=None, version='3.0.3.0', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None):
+    def __init__(self, emdb_id=None, version='3.0.3.2', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None):
         self.original_tagname_ = None
         self.emdb_id = _cast(None, emdb_id)
         self.version = _cast(None, version)
         self.admin = admin
         self.crossreferences = crossreferences
         self.sample = sample
         self.structure_determination_list = structure_determination_list
@@ -32404,15 +32404,15 @@
                     break
             if not enumeration_respectee:
                 warnings_.warn('Value "%(value)s" does not match xsd enumeration restriction on source_nameType' % {"value" : value.encode("utf-8")} )
     def validate_initial_model_typeType(self, value):
         # Validate type initial_model_typeType, a restriction on xs:string.
         if value is not None and Validate_simpletypes_:
             value = str(value)
-            enumerations = ['experimental model', 'in silico model', 'intergrative model', 'other']
+            enumerations = ['experimental model', 'in silico model', 'integrative model', 'other']
             enumeration_respectee = False
             for enum in enumerations:
                 if value == enum:
                     enumeration_respectee = True
                     break
             if not enumeration_respectee:
                 warnings_.warn('Value "%(value)s" does not match xsd enumeration restriction on initial_model_typeType' % {"value" : value.encode("utf-8")} )
```

### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 0% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.1/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.2/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.3.0"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.3.2"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -2558,14 +2558,15 @@
       <xs:enumeration value="GENERIC TVIPS (2k x 2k)"/>
       <xs:enumeration value="GENERIC TVIPS (4k x 4k)"/>
       <xs:enumeration value="KODAK 4489 FILM"/>
       <xs:enumeration value="KODAK SO-163 FILM"/>
       <xs:enumeration value="OTHER"/>
       <xs:enumeration value="PROSCAN TEM-PIV (2k x 2k)"/>
       <xs:enumeration value="SIA 15C (3k x 3k)"/>
+      <xs:enumeration value="TFS FALCON 4i (4k x 4x)"/>
       <xs:enumeration value="TVIPS TEMCAM-F216 (2k x 2k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F224 (2k x 2k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F415 (4k x 4k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F416 (4k x 4k)"/>
       <xs:enumeration value="TVIPS TEMCAM-F816 (8k x 8k)"/>
     </xs:restriction>
   </xs:simpleType>
@@ -3073,15 +3074,15 @@
             </xs:sequence>
           </xs:complexType>
         </xs:element>
         <xs:element name="orthogonal_tilt" minOccurs="0">
           <xs:complexType>
             <xs:sequence>
               <xs:element name="software_list" type="software_list_type" minOccurs="0"/>
-              <xs:element name="number_images" type="xs:positiveInteger"/>
+              <xs:element name="number_images" type="xs:positiveInteger" minOccurs="0"/>
               <xs:element name="tilt_angle1" minOccurs="0">
                 <xs:complexType>
                   <xs:simpleContent>
                     <xs:extension base="allowed_tilt_angle1Orthogonal">
                       <xs:attribute name="units" type="xs:token" fixed="degrees" use="required"/>
                     </xs:extension>
                   </xs:simpleContent>
@@ -3125,15 +3126,15 @@
     <xs:restriction base="xs:float">
       <xs:minInclusive value="30"/>
       <xs:maxInclusive value="50"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="pdb_model_type">
     <xs:sequence>
-      <xs:element name="pdb_id" type="pdb_code_type"/>
+      <xs:element name="pdb_id" type="pdb_code_type" minOccurs="0"/>
       <xs:element name="chain_id_list" type="chain_type" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
   <xs:simpleType name="pdb_code_type">
     <xs:restriction base="xs:token">
       <xs:pattern value="\d[\dA-Za-z]{3}"/>
     </xs:restriction>
@@ -3834,15 +3835,15 @@
                     </xs:simpleType>
                   </xs:element>
                   <xs:element maxOccurs="1" minOccurs="0" name="initial_model_type">
                     <xs:simpleType>
                       <xs:restriction base="xs:string">
                         <xs:enumeration value="experimental model"/>
                         <xs:enumeration value="in silico model"/>
-                        <xs:enumeration value="intergrative model"/>
+                        <xs:enumeration value="integrative model"/>
                         <xs:enumeration value="other"/>
                       </xs:restriction>
                     </xs:simpleType>
                   </xs:element>
                 </xs:sequence>
               </xs:complexType>
             </xs:element>
```

### Comparing `wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.1
+Version: 1.2
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.1/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.2/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

