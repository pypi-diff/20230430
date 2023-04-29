# Comparing `tmp/acrclient-0.2.0.tar.gz` & `tmp/acrclient-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrclient-0.2.0.tar", max compression
+gzip compressed data, was "acrclient-0.3.0.tar", max compression
```

## Comparing `acrclient-0.2.0.tar` & `acrclient-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     2287 2023-02-18 19:03:26.248509 acrclient-0.2.0/README.md
--rw-r--r--   0        0        0       27 2023-02-18 19:03:26.248509 acrclient-0.2.0/acrclient/__init__.py
--rw-r--r--   0        0        0     3724 2023-02-18 19:03:26.248509 acrclient-0.2.0/acrclient/client.py
--rw-r--r--   0        0        0      664 2023-02-18 19:03:26.248509 acrclient-0.2.0/acrclient/models.py
--rw-r--r--   0        0        0        0 2023-02-18 19:03:26.248509 acrclient-0.2.0/acrclient/py.typed
--rw-r--r--   0        0        0     1468 2023-02-18 19:04:12.200450 acrclient-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 acrclient-0.2.0/setup.py
--rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 acrclient-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2287 2023-04-29 23:12:33.634727 acrclient-0.3.0/README.md
+-rw-r--r--   0        0        0      307 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/__init__.py
+-rw-r--r--   0        0        0     4983 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/client.py
+-rw-r--r--   0        0        0      664 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/models.py
+-rw-r--r--   0        0        0        0 2023-04-29 23:12:33.634727 acrclient-0.3.0/acrclient/py.typed
+-rw-r--r--   0        0        0     1672 2023-04-29 23:13:06.026890 acrclient-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 acrclient-0.3.0/PKG-INFO
```

### Comparing `acrclient-0.2.0/README.md` & `acrclient-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `acrclient-0.2.0/acrclient/client.py` & `acrclient-0.3.0/acrclient/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,63 +18,68 @@
 
     def __call__(self, request: PreparedRequest) -> PreparedRequest:
         request.headers["Authorization"] = f"Bearer {self.bearer_token}"
         return request
 
 
 class Client:
-    """ACRCloud client to fetch metadata.
+    """Client class with various methods to call ACRCloud API v2 endpoints.
 
-    >>> bearer_token = "bearer-token"
-    >>> config = Client.Config(retries= 5, backoff_factor= 0.1)
-    >>> client = Client(bearer_token, config=config)
+    Examples:
+        Create an instance with configuration.
+        ```python
+        >>> bearer_token = "bearer-token"
+        >>> config = Client.Config(retries= 5, backoff_factor= 0.1)
+        >>> client = Client(bearer_token, config=config)
 
-    :param str bearer_token
-        The bearer token for ACRCloud.
+        ```
     """
 
     class Config:
-        """Configuration for acrclient.
-
-        :param int retries
-            Total number of retries to allow.
-
-        :param float backoff_factor
-            A backoff factor to apply between attempts after the second try
-            (most errors are resolved immediately by a second try without a
-            delay). urllib3 will sleep for::
-                {backoff factor} * (2 ** ({number of total retries} - 1))
-            seconds. If the backoff_factor is 0.1, then :func:`Retry.sleep` will sleep
-            for [0.0s, 0.2s, 0.4s, ...] between retries. It will never be longer
-            than `backoff_max`.
-            By default, backoff is set to 0.1.
-        """
+        """Configuration for acrclient."""
 
         def __init__(
             self,
             retries: Union[bool | int | None] = 5,
             backoff_factor: float = 0.1,
-        ):
+        ) -> None:
+            """
+            Parameters:
+                retries: Total number of retries to allow.
+
+                backoff_factor: A backoff factor to apply between attempts after the
+                    second try (most errors are resolved immediately by a second try
+                    without a delay). urllib3 will sleep for::
+                        {backoff factor} * (2 ** ({number of total retries} - 1))
+                    seconds. If the backoff_factor is 0.1, then :func:`Retry.sleep`
+                    will sleep for [0.0s, 0.2s, 0.4s, ...] between retries. It will
+                    never be longer than `backoff_max`.
+                    By default, backoff is set to 0.1.
+            """
             self._retries: Union[bool | int | None] = retries
             self._backoff_factor: float = backoff_factor
 
         @property
-        def retries(self):
+        def retries(self) -> Union[bool | int | None]:
             return self._retries
 
         @property
-        def backoff_factor(self):
+        def backoff_factor(self) -> float:
             return self._backoff_factor
 
     def __init__(
         self,
         bearer_token: str,
         base_url: str = "https://eu-api-v2.acrcloud.com",
         config: Optional[Config] = None,
-    ):
+    ) -> None:
+        """
+        Parameters:
+            bearer_token: The bearer token for ACRCloud.
+        """
         self.base_url: str = base_url
 
         self._config: Optional[Client.Config] = config or Client.Config()
         self._auth: _Auth = _Auth(bearer_token=bearer_token)
         self._session = Session()
         self._session.mount(
             "https://",
@@ -82,34 +87,71 @@
                 max_retries=Retry(
                     total=self._config.retries,
                     backoff_factor=self._config.backoff_factor,
                 )
             ),
         )
 
-    def get(self, path: str, params: Any = None, **kwargs) -> Response:
-        """Fetch JSON data from ACRCloud API with set Access Key param."""
+    def get(
+        self,
+        path: str,
+        params: Any = None,
+        **kwargs: Any,
+    ) -> Response:
+        """Fetch JSON data from ACRCloud API with set Access Key param.
+
+        Parameters:
+            path: URL path
+            params: Parameters for request (usually used as GET params)
+            **kwargs: Get passed to `requests.get`
+        Returns:
+            Response object
+        """
         url = f"{self.base_url}{path}"
         if not kwargs.get("timeout"):
             kwargs["timeout"] = 60
 
         # pylint: disable-next=missing-timeout
         response = self._session.get(url=url, auth=self._auth, params=params, **kwargs)
         response.raise_for_status()
         return response
 
-    def json(self, path: str, params: Any = None, **kwargs) -> Any:
+    def json(
+        self,
+        path: str,
+        params: Any = None,
+        **kwargs: Any,
+    ) -> Any:
+        """Get the json results of a get call.
+
+        Parameters:
+            path: URL path
+            params: Parameters for request (usually used as GET params)
+            **kwargs: Get passed to `requests.get`
+        Returns:
+            Data from API
+        """
         response = self.get(path, params=params, **kwargs)
         return response.json()
 
     def get_bm_cs_projects_results(
         self,
         project_id: int,
         stream_id: str,
         params: Optional[GetBmCsProjectsResultsParams] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> Any:
+        """Get Custom Broadcast Monitoring Streams Results from ACRCloud.
+
+        Parameters:
+            project_id: Custom Broadcast Monitoring Project ID
+            stream_id: Custom Broadcast Monitoring Stream ID
+            params: GET parameters for request
+            **kwargs: Get passed to `requests.get`
+        Returns:
+            Data from API
+        """
         return self.json(
             path=f"/api/bm-cs-projects/{project_id}/streams/{stream_id}/results",
             params=params,
             **kwargs,
         ).get("data")
```

### Comparing `acrclient-0.2.0/acrclient/models.py` & `acrclient-0.3.0/acrclient/models.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.2.0/pyproject.toml` & `acrclient-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "acrclient"
-version = "v0.2.0"
-description = "API wrapper for the v2 ACRCloud API."
+version = "v0.3.0"
+description = "API wrapper for the v2 ACRCloud API"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-v3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
@@ -15,43 +15,49 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = ">=2.28.2"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-wheel = "^0.38.4"
+wheel = "^0.40.0"
 types-requests = "^2.28.11"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.6.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
 freezegun = "^1.2.2"
 requests-mock = "^1.10.0"
-black = "^23.1.0"
+black = "^23.3.0"
 isort = "^5.11.4"
-Markdown = "^3.4.1"
+Markdown = "^3.3"
 pytest-mypy = "^0.10.3"
 pytest-pylint = "^0.19.0"
 pytest-random-order = "^1.1.0"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
+mkdocs-material = "^9.1"
+mkdocs = "^1.4.2"
+mkdocs-gen-files = "^0.5.0"
+mkdocs-literate-nav = "^0.6.0"
+mkdocs-section-index = "^0.3.5"
 
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.messages_control]
 # C0114 = missing-module-docstring
 # C0116 = missing-function-docstring
 disable = ["C0114","C0116"]
 
 [tool.pytest.ini_options]
 minversion = "7.2"
-addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=acrclient --cov-fail-under=100 --pylint --mypy"
+addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=acrclient --cov-fail-under=100 --ignore=docs/ --pylint --mypy"
 filterwarnings = [
     "ignore::pytest.PytestRemovedIn8Warning:pytest_pylint",
     "ignore::DeprecationWarning:pytest_pylint",
     "ignore::DeprecationWarning:pylint"
 ]
 
 [build-system]
```

### Comparing `acrclient-0.2.0/setup.py` & `acrclient-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,96 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: acrclient
+Version: 0.3.0
+Summary: API wrapper for the v2 ACRCloud API
+License: AGPL-v3
+Author: RaBe IT-Reaktion
+Author-email: it@rabe.ch
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: requests (>=2.28.2)
+Description-Content-Type: text/markdown
 
-packages = \
-['acrclient']
+# Python ACR Client module
 
-package_data = \
-{'': ['*']}
+Contains a simple client for calling the v2 endpoints of the [ACRCloud](https://www.acrcloud.com) API.
 
-install_requires = \
-['requests>=2.28.2']
-
-setup_kwargs = {
-    'name': 'acrclient',
-    'version': '0.2.0',
-    'description': 'API wrapper for the v2 ACRCloud API.',
-    'long_description': '# Python ACR Client module\n\nContains a simple client for calling the v2 endpoints of the [ACRCloud](https://www.acrcloud.com) API.\n\n## Installation\n\n```bash\npoetry add acrclient\n\n# or on old setup style projects\npip -m install acrclient\n```\n\n## Usage\n\n```python\n>>> from acrclient import Client\n>>> client = Client(bearer_token="bearer-token")\n\n```\n\n## Development\n\n```bash\n# setup a dev env\npython -mvenv env\n. env/bin/activate\n\n# install a modern poetry version\npython -mpip install poetry>=1.2.0\n\n# install deps and dev version\npoetry install\n\n# make changes, run tests\npoetry run pytest\n```\n\n## Release Management\n\nThe CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).\nThere is a GitHub Action in [.github/workflows/semantic-release.yaml](./.github/workflows/semantic-release.yaml)\nthat uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new\nreleases.\n\nThe commit message should be structured as follows:\n\n```\n<type>[optional scope]: <description>\n\n[optional body]\n\n[optional footer(s)]\n```\n\nThe commit contains the following structural elements, to communicate intent to the consumers of your library:\n\n1. **fix:** a commit of the type `fix` patches gets released with a PATCH version bump\n1. **feat:** a commit of the type `feat` gets released as a MINOR version bump\n1. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:` gets released as a MAJOR version bump\n1. types other than `fix:` and `feat:` are allowed and don\'t trigger a release\n\nIf a commit does not contain a conventional commit style message you can fix\nit during the squash and merge operation on the PR.\n\nOnce a commit has landed on the `main` branch a release will be created and automatically published to [pypi](https://pypi.org/)\nusing the GitHub Action in [.github/workflows/release.yaml](./.github/workflows/release.yaml) which uses [poetry](https://python-poetry.org/)\nto publish the package to pypi.\n\n## License\n\nThis package is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, version 3 of the License.\n\n## Copyright\n\nCopyright (c) 2023 [Radio Bern RaBe](http://www.rabe.ch)\n',
-    'author': 'RaBe IT-Reaktion',
-    'author_email': 'it@rabe.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+## Installation
 
+```bash
+poetry add acrclient
+
+# or on old setup style projects
+pip -m install acrclient
+```
+
+## Usage
+
+```python
+>>> from acrclient import Client
+>>> client = Client(bearer_token="bearer-token")
+
+```
+
+## Development
+
+```bash
+# setup a dev env
+python -mvenv env
+. env/bin/activate
+
+# install a modern poetry version
+python -mpip install poetry>=1.2.0
+
+# install deps and dev version
+poetry install
+
+# make changes, run tests
+poetry run pytest
+```
+
+## Release Management
+
+The CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).
+There is a GitHub Action in [.github/workflows/semantic-release.yaml](./.github/workflows/semantic-release.yaml)
+that uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new
+releases.
+
+The commit message should be structured as follows:
+
+```
+<type>[optional scope]: <description>
+
+[optional body]
+
+[optional footer(s)]
+```
+
+The commit contains the following structural elements, to communicate intent to the consumers of your library:
+
+1. **fix:** a commit of the type `fix` patches gets released with a PATCH version bump
+1. **feat:** a commit of the type `feat` gets released as a MINOR version bump
+1. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:` gets released as a MAJOR version bump
+1. types other than `fix:` and `feat:` are allowed and don't trigger a release
+
+If a commit does not contain a conventional commit style message you can fix
+it during the squash and merge operation on the PR.
+
+Once a commit has landed on the `main` branch a release will be created and automatically published to [pypi](https://pypi.org/)
+using the GitHub Action in [.github/workflows/release.yaml](./.github/workflows/release.yaml) which uses [poetry](https://python-poetry.org/)
+to publish the package to pypi.
+
+## License
+
+This package is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, version 3 of the License.
+
+## Copyright
+
+Copyright (c) 2023 [Radio Bern RaBe](http://www.rabe.ch)
 
-setup(**setup_kwargs)
```

