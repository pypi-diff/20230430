# Comparing `tmp/openapi-python-client-0.9.1.tar.gz` & `tmp/openapi-python-client-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi-python-client-0.9.1.tar", max compression
+gzip compressed data, was "openapi-python-client-0.9.2.tar", max compression
```

## Comparing `openapi-python-client-0.9.1.tar` & `openapi-python-client-0.9.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    18847 2021-05-13 01:17:27.643262 openapi-python-client-0.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2021-05-13 01:17:27.643262 openapi-python-client-0.9.1/LICENSE
--rw-r--r--   0        0        0     7288 2021-05-13 01:17:27.643262 openapi-python-client-0.9.1/README.md
--rw-r--r--   0        0        0    12412 2021-05-13 01:17:27.643262 openapi-python-client-0.9.1/openapi_python_client/__init__.py
--rw-r--r--   0        0        0       28 2021-05-13 01:17:27.643262 openapi-python-client-0.9.1/openapi_python_client/__main__.py
--rw-r--r--   0        0        0     5874 2021-05-13 01:17:27.643262 openapi-python-client-0.9.1/openapi_python_client/cli.py
--rw-r--r--   0        0        0      809 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/config.py
--rw-r--r--   0        0        0      179 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/__init__.py
--rw-r--r--   0        0        0     1109 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/errors.py
--rw-r--r--   0        0        0    15096 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/openapi.py
--rw-r--r--   0        0        0    21980 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/properties/__init__.py
--rw-r--r--   0        0        0     2384 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/properties/converter.py
--rw-r--r--   0        0        0     2133 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/properties/enum_property.py
--rw-r--r--   0        0        0     8633 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/properties/model_property.py
--rw-r--r--   0        0        0     3778 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/properties/property.py
--rw-r--r--   0        0        0     2631 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/properties/schemas.py
--rw-r--r--   0        0        0     2395 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/parser/responses.py
--rw-r--r--   0        0        0       26 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/py.typed
--rw-r--r--   0        0        0     1327 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/__init__.py
--rw-r--r--   0        0        0     1064 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/LICENSE
--rw-r--r--   0        0        0     1812 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/README.md
--rw-r--r--   0        0        0     1772 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/__init__.py
--rw-r--r--   0        0        0     4769 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/components.py
--rw-r--r--   0        0        0      762 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/contact.py
--rw-r--r--   0        0        0     1234 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/discriminator.py
--rw-r--r--   0        0        0     2941 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/encoding.py
--rw-r--r--   0        0        0     1446 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/example.py
--rw-r--r--   0        0        0      650 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/external_documentation.py
--rw-r--r--   0        0        0      949 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/header.py
--rw-r--r--   0        0        0     1877 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/info.py
--rw-r--r--   0        0        0      510 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/license.py
--rw-r--r--   0        0        0     2825 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/link.py
--rw-r--r--   0        0        0     2903 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/media_type.py
--rw-r--r--   0        0        0     1579 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/oauth_flow.py
--rw-r--r--   0        0        0      773 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/oauth_flows.py
--rw-r--r--   0        0        0     2129 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/open_api.py
--rw-r--r--   0        0        0     5667 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/operation.py
--rw-r--r--   0        0        0     7551 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/parameter.py
--rw-r--r--   0        0        0     4335 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/path_item.py
--rw-r--r--   0        0        0     1011 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/paths.py
--rw-r--r--   0        0        0      823 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/reference.py
--rw-r--r--   0        0        0     3054 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/request_body.py
--rw-r--r--   0        0        0     3125 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/response.py
--rw-r--r--   0        0        0     2042 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/responses.py
--rw-r--r--   0        0        0    21321 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/schema.py
--rw-r--r--   0        0        0     1322 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/security_requirement.py
--rw-r--r--   0        0        0     3058 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/security_scheme.py
--rw-r--r--   0        0        0     1778 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/server.py
--rw-r--r--   0        0        0     1005 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/server_variable.py
--rw-r--r--   0        0        0      839 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/tag.py
--rw-r--r--   0        0        0     1807 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/xml.py
--rw-r--r--   0        0        0      211 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/schema/parameter_location.py
--rw-r--r--   0        0        0      195 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/.gitignore.jinja
--rw-r--r--   0        0        0     2904 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/README.md.jinja
--rw-r--r--   0        0        0     1575 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/client.py.jinja
--rw-r--r--   0        0        0     4677 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/endpoint_macros.py.jinja
--rw-r--r--   0        0        0     4053 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/endpoint_module.py.jinja
--rw-r--r--   0        0        0      224 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/int_enum.py.jinja
--rw-r--r--   0        0        0     4946 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/model.py.jinja
--rw-r--r--   0        0        0      122 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/models_init.py.jinja
--rw-r--r--   0        0        0       74 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/package_init.py.jinja
--rw-r--r--   0        0        0     1005 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/date_property.py.jinja
--rw-r--r--   0        0        0     1057 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/datetime_property.py.jinja
--rw-r--r--   0        0        0     1086 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/enum_property.py.jinja
--rw-r--r--   0        0        0     1077 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/file_property.py.jinja
--rw-r--r--   0        0        0     2318 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/list_property.py.jinja
--rw-r--r--   0        0        0     1082 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/model_property.py.jinja
--rw-r--r--   0        0        0      330 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/none_property.py.jinja
--rw-r--r--   0        0        0      956 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/property_macros.py.jinja
--rw-r--r--   0        0        0     3317 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/union_property.py.jinja
--rw-r--r--   0        0        0      689 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/pyproject.toml.jinja
--rw-r--r--   0        0        0      233 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/pyproject_no_poetry.toml.jinja
--rw-r--r--   0        0        0      697 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/setup.py.jinja
--rw-r--r--   0        0        0      225 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/str_enum.py.jinja
--rw-r--r--   0        0        0     1021 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/templates/types.py.jinja
--rw-r--r--   0        0        0     1956 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/openapi_python_client/utils.py
--rw-r--r--   0        0        0     2254 2021-05-13 01:17:27.647262 openapi-python-client-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8965 2021-05-13 01:17:53.103884 openapi-python-client-0.9.1/setup.py
--rw-r--r--   0        0        0     8711 2021-05-13 01:17:53.104359 openapi-python-client-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    19024 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/LICENSE
+-rw-r--r--   0        0        0     7288 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/README.md
+-rw-r--r--   0        0        0    12412 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/__init__.py
+-rw-r--r--   0        0        0       28 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/__main__.py
+-rw-r--r--   0        0        0     6028 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/cli.py
+-rw-r--r--   0        0        0      809 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/config.py
+-rw-r--r--   0        0        0      179 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/__init__.py
+-rw-r--r--   0        0        0     1109 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/errors.py
+-rw-r--r--   0        0        0    15096 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/openapi.py
+-rw-r--r--   0        0        0    21980 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/properties/__init__.py
+-rw-r--r--   0        0        0     2384 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/properties/converter.py
+-rw-r--r--   0        0        0     2133 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/properties/enum_property.py
+-rw-r--r--   0        0        0     8633 2021-06-14 00:39:51.120875 openapi-python-client-0.9.2/openapi_python_client/parser/properties/model_property.py
+-rw-r--r--   0        0        0     3778 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/parser/properties/property.py
+-rw-r--r--   0        0        0     2631 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/parser/properties/schemas.py
+-rw-r--r--   0        0        0     2395 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/parser/responses.py
+-rw-r--r--   0        0        0       26 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/py.typed
+-rw-r--r--   0        0        0     1327 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/__init__.py
+-rw-r--r--   0        0        0     1064 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/LICENSE
+-rw-r--r--   0        0        0     1812 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/README.md
+-rw-r--r--   0        0        0     1772 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/__init__.py
+-rw-r--r--   0        0        0     4769 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/components.py
+-rw-r--r--   0        0        0      762 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/contact.py
+-rw-r--r--   0        0        0     1234 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/discriminator.py
+-rw-r--r--   0        0        0     2941 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/encoding.py
+-rw-r--r--   0        0        0     1446 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/example.py
+-rw-r--r--   0        0        0      650 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/external_documentation.py
+-rw-r--r--   0        0        0      949 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/header.py
+-rw-r--r--   0        0        0     1877 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/info.py
+-rw-r--r--   0        0        0      510 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/license.py
+-rw-r--r--   0        0        0     2825 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/link.py
+-rw-r--r--   0        0        0     2903 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/media_type.py
+-rw-r--r--   0        0        0     1579 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/oauth_flow.py
+-rw-r--r--   0        0        0      773 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/oauth_flows.py
+-rw-r--r--   0        0        0     2129 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/open_api.py
+-rw-r--r--   0        0        0     5667 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/operation.py
+-rw-r--r--   0        0        0     7551 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/parameter.py
+-rw-r--r--   0        0        0     4335 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/path_item.py
+-rw-r--r--   0        0        0     1011 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/paths.py
+-rw-r--r--   0        0        0      823 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/reference.py
+-rw-r--r--   0        0        0     3054 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/request_body.py
+-rw-r--r--   0        0        0     3125 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/response.py
+-rw-r--r--   0        0        0     2042 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/responses.py
+-rw-r--r--   0        0        0    21321 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/schema.py
+-rw-r--r--   0        0        0     1322 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/security_requirement.py
+-rw-r--r--   0        0        0     3058 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/security_scheme.py
+-rw-r--r--   0        0        0     1778 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/server.py
+-rw-r--r--   0        0        0     1005 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/server_variable.py
+-rw-r--r--   0        0        0      839 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/tag.py
+-rw-r--r--   0        0        0     1807 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/xml.py
+-rw-r--r--   0        0        0      211 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/schema/parameter_location.py
+-rw-r--r--   0        0        0      195 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/.gitignore.jinja
+-rw-r--r--   0        0        0     2904 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/README.md.jinja
+-rw-r--r--   0        0        0     1575 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/client.py.jinja
+-rw-r--r--   0        0        0     4677 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/endpoint_macros.py.jinja
+-rw-r--r--   0        0        0     4031 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/endpoint_module.py.jinja
+-rw-r--r--   0        0        0      224 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/int_enum.py.jinja
+-rw-r--r--   0        0        0     4946 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/model.py.jinja
+-rw-r--r--   0        0        0      122 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/models_init.py.jinja
+-rw-r--r--   0        0        0       74 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/package_init.py.jinja
+-rw-r--r--   0        0        0     1005 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/date_property.py.jinja
+-rw-r--r--   0        0        0     1057 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/datetime_property.py.jinja
+-rw-r--r--   0        0        0     1086 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/enum_property.py.jinja
+-rw-r--r--   0        0        0     1077 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/file_property.py.jinja
+-rw-r--r--   0        0        0     2318 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/list_property.py.jinja
+-rw-r--r--   0        0        0     1082 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/model_property.py.jinja
+-rw-r--r--   0        0        0      330 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/none_property.py.jinja
+-rw-r--r--   0        0        0      956 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/property_macros.py.jinja
+-rw-r--r--   0        0        0     3317 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/union_property.py.jinja
+-rw-r--r--   0        0        0      689 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/pyproject.toml.jinja
+-rw-r--r--   0        0        0      233 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/pyproject_no_poetry.toml.jinja
+-rw-r--r--   0        0        0      697 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/setup.py.jinja
+-rw-r--r--   0        0        0      225 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/str_enum.py.jinja
+-rw-r--r--   0        0        0     1021 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/templates/types.py.jinja
+-rw-r--r--   0        0        0     1956 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/openapi_python_client/utils.py
+-rw-r--r--   0        0        0     2254 2021-06-14 00:39:51.124876 openapi-python-client-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8965 2021-06-14 00:40:15.397153 openapi-python-client-0.9.2/setup.py
+-rw-r--r--   0        0        0     8711 2021-06-14 00:40:15.397817 openapi-python-client-0.9.2/PKG-INFO
```

### Comparing `openapi-python-client-0.9.1/CHANGELOG.md` & `openapi-python-client-0.9.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.9.2
+
+### Features
+
+- Add option to fail on warning [#427]. Thanks @forest-benchling!
+
+### Fixes
+
+- Properly strip out `UNSET` values from form data [#430]. Thanks @p1-ra!
+
 ## 0.9.1
 
 ### Features
 
 - Allow references to non-object, non-enum types [#371][#418][#425]. Thanks @p1-ra!
 - Allow for attrs 21.x in generated clients [#412]
 - Allow for using any version of Black [#416] [#411]. Thanks @christhekeele!
```

### Comparing `openapi-python-client-0.9.1/LICENSE` & `openapi-python-client-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/README.md` & `openapi-python-client-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/__init__.py` & `openapi-python-client-0.9.2/openapi_python_client/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/cli.py` & `openapi-python-client-0.9.2/openapi_python_client/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     if isinstance(e, ParseError) and e.data is not None:
         formatted_data = pformat(e.data)
         typer.secho(formatted_data, fg=color, err=True)
 
     typer.echo()
 
 
-def handle_errors(errors: Sequence[GeneratorError]) -> None:
+def handle_errors(errors: Sequence[GeneratorError], fail_on_warning: bool = False) -> None:
     """Turn custom errors into formatted error messages"""
     if len(errors) == 0:
         return
     error_level = ErrorLevel.WARNING
     message = "Warning(s) encountered while generating. Client was generated, but some pieces may be missing"
     header_color = typer.colors.BRIGHT_YELLOW
     color = typer.colors.YELLOW
@@ -87,15 +87,15 @@
     typer.secho(
         f"If you believe this was a mistake or this tool is missing a feature you need, "
         f"please open an issue at {gh_link}",
         fg=typer.colors.BLUE,
         err=True,
     )
 
-    if error_level == ErrorLevel.ERROR:
+    if error_level == ErrorLevel.ERROR or fail_on_warning:
         raise typer.Exit(code=1)
 
 
 custom_template_path_options = {
     "help": "A path to a directory containing custom template(s)",
     "file_okay": False,
     "dir_okay": True,
@@ -115,14 +115,15 @@
 def generate(
     url: Optional[str] = typer.Option(None, help="A URL to read the JSON from"),
     path: Optional[pathlib.Path] = typer.Option(None, help="A path to the JSON file"),
     custom_template_path: Optional[pathlib.Path] = typer.Option(None, **custom_template_path_options),  # type: ignore
     meta: MetaType = _meta_option,
     file_encoding: str = typer.Option("utf-8", help="Encoding used when writing generated"),
     config_path: Optional[pathlib.Path] = CONFIG_OPTION,
+    fail_on_warning: bool = False,
 ) -> None:
     """Generate a new OpenAPI Client library"""
     from . import create_new_client
 
     if not url and not path:
         typer.secho("You must either provide --url or --path", fg=typer.colors.RED)
         raise typer.Exit(code=1)
@@ -141,25 +142,26 @@
         url=url,
         path=path,
         meta=meta,
         custom_template_path=custom_template_path,
         file_encoding=file_encoding,
         config=config,
     )
-    handle_errors(errors)
+    handle_errors(errors, fail_on_warning)
 
 
 @app.command()
 def update(
     url: Optional[str] = typer.Option(None, help="A URL to read the JSON from"),
     path: Optional[pathlib.Path] = typer.Option(None, help="A path to the JSON file"),
     custom_template_path: Optional[pathlib.Path] = typer.Option(None, **custom_template_path_options),  # type: ignore
     meta: MetaType = _meta_option,
     file_encoding: str = typer.Option("utf-8", help="Encoding used when writing generated"),
     config_path: Optional[pathlib.Path] = CONFIG_OPTION,
+    fail_on_warning: bool = False,
 ) -> None:
     """Update an existing OpenAPI Client library"""
     from . import update_existing_client
 
     if not url and not path:
         typer.secho("You must either provide --url or --path", fg=typer.colors.RED)
         raise typer.Exit(code=1)
@@ -178,8 +180,8 @@
         url=url,
         path=path,
         meta=meta,
         custom_template_path=custom_template_path,
         file_encoding=file_encoding,
         config=config,
     )
-    handle_errors(errors)
+    handle_errors(errors, fail_on_warning)
```

### Comparing `openapi-python-client-0.9.1/openapi_python_client/config.py` & `openapi-python-client-0.9.2/openapi_python_client/config.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/errors.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/errors.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/openapi.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/openapi.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/properties/__init__.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/properties/converter.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/properties/converter.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/properties/enum_property.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/properties/enum_property.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/properties/model_property.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/properties/model_property.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/properties/property.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/properties/property.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/properties/schemas.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/properties/schemas.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/parser/responses.py` & `openapi-python-client-0.9.2/openapi_python_client/parser/responses.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/__init__.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/LICENSE` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/README.md` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/README.md`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/__init__.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/components.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/components.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/contact.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/contact.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/discriminator.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/discriminator.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/encoding.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/encoding.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/example.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/example.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/external_documentation.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/external_documentation.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/header.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/header.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/info.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/info.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/link.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/link.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/media_type.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/media_type.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/oauth_flow.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/oauth_flows.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/open_api.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/open_api.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/operation.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/operation.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/parameter.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/parameter.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/path_item.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/path_item.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/paths.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/paths.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/reference.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/reference.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/request_body.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/request_body.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/response.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/response.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/responses.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/responses.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/schema.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/security_requirement.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/security_requirement.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/security_scheme.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/security_scheme.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/server.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/server.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/server_variable.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/server_variable.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/tag.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/tag.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/schema/openapi_schema_pydantic/xml.py` & `openapi-python-client-0.9.2/openapi_python_client/schema/openapi_schema_pydantic/xml.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/README.md.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/client.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/client.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/endpoint_macros.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/endpoint_macros.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/endpoint_module.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/endpoint_module.py.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
-from attr import asdict
 
 from ...client import AuthenticatedClient, Client
 from ...types import Response, UNSET{% if endpoint.multipart_body_class %}, File {% endif %}
 
 {% for relative in endpoint.relative_imports %}
 {{ relative }}
 {% endfor %}
@@ -48,15 +47,15 @@
 
     return {
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         {% if endpoint.form_body_class %}
-        "data": asdict(form_data),
+        "data": form_data.to_dict(),
         {% elif endpoint.multipart_body_class %}
         "files": files,
         "data": data,
         {% elif endpoint.json_body %}
         "json": {{ "json_" + endpoint.json_body.python_name }},
         {% endif %}
         {% if endpoint.query_parameters %}
```

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/model.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/model.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/date_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/date_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/datetime_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/datetime_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/enum_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/enum_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/file_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/file_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/list_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/list_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/model_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/model_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/property_macros.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/property_macros.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/property_templates/union_property.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/property_templates/union_property.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/pyproject.toml.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/pyproject.toml.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/setup.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/setup.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/templates/types.py.jinja` & `openapi-python-client-0.9.2/openapi_python_client/templates/types.py.jinja`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/openapi_python_client/utils.py` & `openapi-python-client-0.9.2/openapi_python_client/utils.py`

 * *Files identical despite different names*

### Comparing `openapi-python-client-0.9.1/pyproject.toml` & `openapi-python-client-0.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openapi-python-client"
-version = "0.9.1"
+version = "0.9.2"
 description = "Generate modern Python clients from OpenAPI"
 repository = "https://github.com/triaxtec/openapi-python-client"
 license = "MIT"
 keywords=["OpenAPI", "Client", "Generator"]
 authors = ["Dylan Anthony <danthony@triaxtec.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `openapi-python-client-0.9.1/setup.py` & `openapi-python-client-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  ':sys_platform == "win32"': ['colorama>=0.4.3,<0.5.0']}
 
 entry_points = \
 {'console_scripts': ['openapi-python-client = openapi_python_client.cli:app']}
 
 setup_kwargs = {
     'name': 'openapi-python-client',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Generate modern Python clients from OpenAPI',
     'long_description': '![Run Checks](https://github.com/triaxtec/openapi-python-client/workflows/Run%20Checks/badge.svg)\n[![codecov](https://codecov.io/gh/triaxtec/openapi-python-client/branch/main/graph/badge.svg)](https://codecov.io/gh/triaxtec/openapi-python-client)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n[![Generic badge](https://img.shields.io/badge/type_checked-mypy-informational.svg)](https://mypy.readthedocs.io/en/stable/introduction.html)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![PyPI version shields.io](https://img.shields.io/pypi/v/openapi-python-client.svg)](https://pypi.python.org/pypi/openapi-python-client/)\n[![Downloads](https://static.pepy.tech/personalized-badge/openapi-python-client?period=total&units=international_system&left_color=blue&right_color=green&left_text=Downloads)](https://pepy.tech/project/openapi-python-client)\n\n# openapi-python-client\n\nGenerate modern Python clients from OpenAPI 3.x documents.\n\n_This generator does not support OpenAPI 2.x FKA Swagger. If you need to use an older document, try upgrading it to\nversion 3 first with one of many available converters._\n\n**This project is still in development and does not support all OpenAPI features**\n\n## Why This?\n\nThe Python clients generated by openapi-generator support Python 2 and therefore come with a lot of baggage. This tool\naims to generate clients which:\n\n1. Use all the latest and greatest Python features like type annotations and dataclasses\n1. Don\'t carry around a bunch of compatibility code for older version of Python (e.g. the `six` package)\n1. Have better documentation and more obvious usage instructions\n\nAdditionally, because this generator is written in Python, it should be more accessible to contribution by the people\nusing it (Python developers).\n\n## Installation\n\nI recommend you install with [pipx](https://pipxproject.github.io/pipx/) so you don\'t conflict with any other packages\nyou might have: `pipx install openapi-python-client`.\n\nBetter yet, use `pipx run openapi-python-client <normal params / options>` to always use the latest version of the generator.\n\nYou can install with normal pip if you want to though: `pip install openapi-python-client`\n\nThen, if you want tab completion: `openapi-python-client --install-completion`\n\n## Usage\n\n### Create a new client\n\n`openapi-python-client generate --url https://my.api.com/openapi.json`\n\nThis will generate a new client library named based on the title in your OpenAPI spec. For example, if the title\nof your API is "My API", the expected output will be "my-api-client". If a folder already exists by that name, you\'ll\nget an error.\n\nIf you have an `openapi.json` file available on disk, in any CLI invocation you can build off that instead by replacing `--url` with a `--path`:\n\n`openapi-python-client generate --path location/on/disk/openapi.json`\n\n### Update an existing client\n\n`openapi-python-client update --url https://my.api.com/openapi.json`\n\n> For more usage details run `openapi-python-client --help` or read [usage](usage.md)\n\n### Using custom templates\n\nThis feature leverages Jinja2\'s [ChoiceLoader](https://jinja.palletsprojects.com/en/2.11.x/api/#jinja2.ChoiceLoader) and [FileSystemLoader](https://jinja.palletsprojects.com/en/2.11.x/api/#jinja2.FileSystemLoader). This means you do _not_ need to customize every template. Simply copy the template(s) you want to customize from [the default template directory](openapi_python_client/templates) to your own custom template directory (file names _must_ match exactly) and pass the template directory through the `custom-template-path` flag to the `generate` and `update` commands. For instance,\n\n```\nopenapi-python-client update \\\n  --url https://my.api.com/openapi.json \\\n  --custom-template-path=relative/path/to/mytemplates\n```\n\n_Be forewarned, this is a beta-level feature in the sense that the API exposed in the templates is undocumented and unstable._\n\n## What You Get\n\n1. A `pyproject.toml` file with some basic metadata intended to be used with [Poetry].\n1. A `README.md` you\'ll most definitely need to update with your project\'s details\n1. A Python module named just like the auto-generated project name (e.g. "my_api_client") which contains:\n   1. A `client` module which will have both a `Client` class and an `AuthenticatedClient` class. You\'ll need these\n      for calling the functions in the `api` module.\n   1. An `api` module which will contain one module for each tag in your OpenAPI spec, as well as a `default` module\n      for endpoints without a tag. Each of these modules in turn contains one function for calling each endpoint.\n   1. A `models` module which has all the classes defined by the various schemas in your OpenAPI spec\n\nFor a full example you can look at the `end_to_end_tests` directory which has an `openapi.json` file.\n"golden-record" in that same directory is the generated client from that OpenAPI document.\n\n## OpenAPI features supported\n\n1. All HTTP Methods\n1. JSON and form bodies, path and query parameters\n1. File uploads with multipart/form-data bodies\n1. float, string, int, date, datetime, string enums, and custom schemas or lists containing any of those\n1. html/text or application/json responses containing any of the previous types\n1. Bearer token security\n\n## Configuration\n\nYou can pass a YAML (or JSON) file to openapi-python-client with the `--config` option in order to change some behavior.\nThe following parameters are supported:\n\n### class_overrides\n\nUsed to change the name of generated model classes. This param should be a mapping of existing class name\n(usually a key in the "schemas" section of your OpenAPI document) to class_name and module_name. As an example, if the\nname of the a model in OpenAPI (and therefore the generated class name) was something like "\\_PrivateInternalLongName"\nand you want the generated client\'s model to be called "ShortName" in a module called "short_name" you could do this:\n\nExample:\n\n```yaml\nclass_overrides:\n  _PrivateInternalLongName:\n    class_name: ShortName\n    module_name: short_name\n```\n\nThe easiest way to find what needs to be overridden is probably to generate your client and go look at everything in the\nmodels folder.\n\n### project_name_override and package_name_override\n\nUsed to change the name of generated client library project/package. If the project name is changed but an override for the package name\nisn\'t provided, the package name will be converted from the project name using the standard convention (replacing `-`\'s with `_`\'s).\n\nExample:\n\n```yaml\nproject_name_override: my-special-project-name\npackage_name_override: my_extra_special_package_name\n```\n\n### field_prefix\n\nWhen generating properties, the `name` attribute of the OpenAPI schema will be used. When the `name` is not a valid\nPython identifier (e.g. begins with a number) this string will be prepended. Defaults to "field\\_".\n\nExample:\n\n```yaml\nfield_prefix: attr_\n```\n\n### package_version_override\n\nSpecify the package version of the generated client. If unset, the client will use the version of the OpenAPI spec.\n\nExample:\n\n```yaml\npackage_version_override: 1.2.3\n```\n\n[changelog.md]: CHANGELOG.md\n[poetry]: https://python-poetry.org/\n',
     'author': 'Dylan Anthony',
     'author_email': 'danthony@triaxtec.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/triaxtec/openapi-python-client',
```

### Comparing `openapi-python-client-0.9.1/PKG-INFO` & `openapi-python-client-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-python-client
-Version: 0.9.1
+Version: 0.9.2
 Summary: Generate modern Python clients from OpenAPI
 Home-page: https://github.com/triaxtec/openapi-python-client
 License: MIT
 Keywords: OpenAPI,Client,Generator
 Author: Dylan Anthony
 Author-email: danthony@triaxtec.com
 Requires-Python: >=3.6.2,<4.0.0
```

