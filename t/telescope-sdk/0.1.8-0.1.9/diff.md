# Comparing `tmp/telescope_sdk-0.1.8.tar.gz` & `tmp/telescope_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telescope_sdk-0.1.8.tar", max compression
+gzip compressed data, was "telescope_sdk-0.1.9.tar", max compression
```

## Comparing `telescope_sdk-0.1.8.tar` & `telescope_sdk-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3224 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/README.md
--rw-r--r--   0        0        0      888 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2027 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/telescope_sdk/__init__.py
--rw-r--r--   0        0        0      770 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/telescope_sdk/campaign.py
--rw-r--r--   0        0        0     1360 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/telescope_sdk/campaign_log_event.py
--rw-r--r--   0        0        0     1685 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/telescope_sdk/common.py
--rw-r--r--   0        0        0     3540 2023-02-22 13:38:28.520868 telescope_sdk-0.1.8/telescope_sdk/company.py
--rw-r--r--   0        0        0     1043 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/company_types.py
--rw-r--r--   0        0        0     7996 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/person.py
--rw-r--r--   0        0        0     1081 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/prospect.py
--rw-r--r--   0        0        0      522 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/prospect_interaction_event.py
--rw-r--r--   0        0        0      824 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/recommendation.py
--rw-r--r--   0        0        0      435 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/sequence.py
--rw-r--r--   0        0        0     3982 2023-02-22 13:38:28.524868 telescope_sdk-0.1.8/telescope_sdk/utils.py
--rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 telescope_sdk-0.1.8/setup.py
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 telescope_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3224 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0      888 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2027 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/__init__.py
+-rw-r--r--   0        0        0      770 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/campaign.py
+-rw-r--r--   0        0        0     1360 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/campaign_log_event.py
+-rw-r--r--   0        0        0     1685 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/common.py
+-rw-r--r--   0        0        0     3540 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/company.py
+-rw-r--r--   0        0        0     1043 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/company_types.py
+-rw-r--r--   0        0        0     7996 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/person.py
+-rw-r--r--   0        0        0     1081 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/prospect.py
+-rw-r--r--   0        0        0      588 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/prospect_interaction_event.py
+-rw-r--r--   0        0        0      824 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/recommendation.py
+-rw-r--r--   0        0        0      435 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/sequence.py
+-rw-r--r--   0        0        0     3982 2023-02-22 14:30:18.859458 telescope_sdk-0.1.9/telescope_sdk/utils.py
+-rw-r--r--   0        0        0     4048 1970-01-01 00:00:00.000000 telescope_sdk-0.1.9/setup.py
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 telescope_sdk-0.1.9/PKG-INFO
```

### Comparing `telescope_sdk-0.1.8/README.md` & `telescope_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/pyproject.toml` & `telescope_sdk-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "telescope-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "Telescope Python SDK"
 packages = [{include = "telescope_sdk"}]
 authors = ["Camin McCluskey <camin@gotelescope.ai>",]
 license = "Proprietary"
 readme = "README.md"
 homepage = "https://github.com/telescope-eng/telescope-python-sdk"
 repository = "https://github.com/telescope-eng/telescope-python-sdk"
```

### Comparing `telescope_sdk-0.1.8/telescope_sdk/__init__.py` & `telescope_sdk-0.1.9/telescope_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/campaign.py` & `telescope_sdk-0.1.9/telescope_sdk/campaign.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/campaign_log_event.py` & `telescope_sdk-0.1.9/telescope_sdk/campaign_log_event.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/common.py` & `telescope_sdk-0.1.9/telescope_sdk/common.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/company.py` & `telescope_sdk-0.1.9/telescope_sdk/company.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/company_types.py` & `telescope_sdk-0.1.9/telescope_sdk/company_types.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/person.py` & `telescope_sdk-0.1.9/telescope_sdk/person.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/prospect.py` & `telescope_sdk-0.1.9/telescope_sdk/prospect.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/prospect_interaction_event.py` & `telescope_sdk-0.1.9/telescope_sdk/prospect_interaction_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from telescope_sdk.common import UserFacingDataType
 
 
 class ProspectInteractionEventType(str, Enum):
     PROSPECT_REPLIED_POSITIVE = 'PROSPECT_REPLIED_POSITIVE'
     PROSPECT_REPLIED_NEGATIVE = 'PROSPECT_REPLIED_NEGATIVE'
     PROSPECT_REPLIED_UNKNOWN_SENTIMENT = 'PROSPECT_REPLIED_UNKNOWN_SENTIMENT'
+    PROSPECT_BOUNCE_NOTIFICATION = 'PROSPECT_BOUNCE_NOTIFICATION'
 
 
 class ProspectInteractionEvent(UserFacingDataType):
     campaign_id: str
     prospect_id: str
     type: ProspectInteractionEventType
     text_reply: Optional[str] = None
```

### Comparing `telescope_sdk-0.1.8/telescope_sdk/recommendation.py` & `telescope_sdk-0.1.9/telescope_sdk/recommendation.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/telescope_sdk/utils.py` & `telescope_sdk-0.1.9/telescope_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `telescope_sdk-0.1.8/setup.py` & `telescope_sdk-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['flake8>=5.0,<6.0', 'pycountry>=22.3.5,<23.0.0', 'pydantic>=1.7,<2.0']
 
 setup_kwargs = {
     'name': 'telescope-sdk',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Telescope Python SDK',
     'long_description': '# Telescope Python SDK\n\nPackage containing Pydantic models representing the entities used in Telescope backend systems. The source of truth\nfor these types lives [here](https://gotelescope.atlassian.net/wiki/spaces/~62cc5da0bb346bdf82fa14f7/pages/32899073/Data+model+changes+move+to+Person).\n\nSee [Deployment](#deployment) for instructions on how to publish a new version of this package.\n\n## Usage\n\n```bash\n$ pip install telescope-sdk\n```\n\nTo construct an entity (e.g. Person) you can use the constructor \n(please note Pydantic only accepts keyword arguments):\n\n```python\nfrom telescope_sdk import Person\nperson = Person(\n    id="123",\n    first_name="John Doe",\n    ...\n    )\n```\n\nOr, to construct from a Python dictionary object:\n\n```python\nperson = Person.parse_obj({\n    "id": "123",\n    "first_name": "John Doe",\n    ...\n    })\n```\n\nIf you are mapping from [PDL](https://docs.peopledatalabs.com/docs/fields) types, use the `from_pdl` method:\n\n```python\nperson = Person.from_pdl({\n    "id": "123",\n    "firstName": "John Doe",\n    ...\n    })\n```\n\n* Please note that unless a field is set as "Strict", it will automatically attempt to cast any input, \n  and only throw an error if casting fails \n\n## Development\n\nTo make changes to this package clone the repo and follow the steps below. Please ensure that any changes to the code\nbase are synced with the documentation linked above.\n\n### Installation\n\nFirst set up a virtual environment to isolate dependencies. You can do this in many ways but as an example:\n\n```bash\n$ pyenv virtualenv 3.10.0 <chosen-virtualenv-name>\n$ pyenv activate <chosen-virtualenv-name>\n```\n\nNote this codebase takes advantage of features from Python 3.10+ therefore you may run into errors if you attempt to use\nan earlier Python version.\n\nThis project relies on Poetry for dependency management. To install Poetry follow the instructions\n[here](https://python-poetry.org/docs/#installing-with-pipx) (recommend using [pipx](https://pypa.github.io/pipx/) to\ninstall Poetry globally but manage in virtualenv).\n\nNow ensure you have Make on your machine then run\n\n```bash\n$ make install\n```\n\nThis will install the package and its dependencies in [editable mode](https://setuptools.pypa.io/en/latest/userguide/development_mode.html).\n\n### Testing\n\nTo run tests locally, run the following command:\n\n```bash\n$ make test\n```\n\n### Linting\n\nTo run linting locally, run the following command:\n\n```bash\n$ make lint\n```\n\n## Deployment\n\nA new package version is published to PyPI whenever a new release is created on GitHub. To create a new release follow\nthe following steps, from the `master` branch:\n\n1. Update the version number in `pyproject.toml` to the new version number (use semantic versioning).\n2. Create a new release on GitHub with the same version number as the one in `pyproject.toml`.\n3. Draft release notes for the new version. These will be used as the package description on PyPI.\n4. The new version will be published to [PyPI](https://pypi.org/) automatically.\n\nOn pushes to the `master` branch, the `sandbox-deploy` job will run and publish a new version of the package to\n[TestPyPI](https://test.pypi.org/). This is useful for testing changes to the package before publishing to PyPI.\n',
     'author': 'Camin McCluskey',
     'author_email': 'camin@gotelescope.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/telescope-eng/telescope-python-sdk',
```

### Comparing `telescope_sdk-0.1.8/PKG-INFO` & `telescope_sdk-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telescope-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Telescope Python SDK
 Home-page: https://github.com/telescope-eng/telescope-python-sdk
 License: Proprietary
 Keywords: telescope,sdk
 Author: Camin McCluskey
 Author-email: camin@gotelescope.ai
 Requires-Python: >=3.7,<4.0
```

