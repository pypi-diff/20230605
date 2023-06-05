# Comparing `tmp/req2flatpak-0.1.0.tar.gz` & `tmp/req2flatpak-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "req2flatpak-0.1.0.tar", max compression
+gzip compressed data, was "req2flatpak-0.2.0.tar", max compression
```

## Comparing `req2flatpak-0.1.0.tar` & `req2flatpak-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4956 2022-12-16 11:18:24.975365 req2flatpak-0.1.0/README.rst
--rw-r--r--   0        0        0     1614 2022-12-16 11:18:24.983365 req2flatpak-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0    27101 2022-12-24 08:14:13.385358 req2flatpak-0.1.0/req2flatpak.py
--rw-r--r--   0        0        0     5854 1970-01-01 00:00:00.000000 req2flatpak-0.1.0/setup.py
--rw-r--r--   0        0        0     5618 1970-01-01 00:00:00.000000 req2flatpak-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4916 2023-06-05 14:10:11.464334 req2flatpak-0.2.0/README.rst
+-rw-r--r--   0        0        0     1057 2023-06-05 14:10:11.464334 req2flatpak-0.2.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     1921 2023-06-05 14:10:11.464334 req2flatpak-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0    29404 2023-06-05 14:10:11.464334 req2flatpak-0.2.0/req2flatpak.py
+-rw-r--r--   0        0        0     6762 1970-01-01 00:00:00.000000 req2flatpak-0.2.0/PKG-INFO
```

### Comparing `req2flatpak-0.1.0/README.rst` & `req2flatpak-0.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 generated ``flatpak-builder`` build module. The build module, if included
 into a flatpak-builder build manifest, will install the python packages
 using pip.
 
 Getting Started
 ---------------
 
-Run ``pip install git+https://github.com/johannesjh/req2flatpak``
-to install the latest development version of req2flatpak.
+Run ``pip install req2flatpak``
+to install the latest release of req2flatpak.
 
 It is possible to use req2flatpak from the commandline,
 as well as programmatically from a python script.
 
 Commandline usage means you can invoke req2flatpak’s commandline interface
 as follows, in order to generate a ``flatpak-builder`` build module
 from given python package requirements:
@@ -92,35 +92,41 @@
 
 Comparison between ``flatpak-pip-generator`` and ``req2flatpak.py``:
 Each of the two projects has its own benefits.
 A comparison will likely change over time.
 As in Oct, 2022, in my personal opinion (johannesjh),
 I see the following similarities and differences:
 
--  Both projects generate build modules for flatpak-builder.
--  Both projects consist of a single script file with minimal
+*  Both projects generate build modules for flatpak-builder.
+
+*  Both projects consist of a single script file with minimal
    dependencies, and are thus very easy to install.
--  ``flatpak-pip-generator`` resolves dependencies and freezes
+
+*  ``flatpak-pip-generator`` resolves dependencies and freezes
    dependency versions, whereas ``req2flatpak.py`` asks the user to
    provide a fully resolved list of dependencies with frozen dependency
    versions. Various tools exist which make this easy, e.g.,
    pip, pip-compile and poetry.
--  ``flatpak-pip-generator`` is older and thus likely to be more mature.
+
+*  ``flatpak-pip-generator`` is older and thus likely to be more mature.
    It supports more commandline options and probably has a more complete
    feature set.
--  ``req2flatpak.py`` is faster. The script itself runs faster because
+
+*  ``req2flatpak.py`` is faster. The script itself runs faster because
    it does not need to download package files in order to generate the
    build module. And the flatpak build runs faster because all packages
    (from the entire ``requirements.txt`` file) are installed in a single
    call to ``pip install``.
--  ``req2flatpak.py`` re-implements some functionality of pip. In
+
+*  ``req2flatpak.py`` re-implements some functionality of pip. In
    contrast, ``flatpak-pip-generator`` uses pip’s official
    functionality. Specifically, ``req2flatpak.py`` re-implements how pip
    queries available downloads from pypi and how pip chooses suitable
    downloads to match a given target platform.
--  ``req2flatpak.py`` prefers binary wheels, whereas
+
+*  ``req2flatpak.py`` prefers binary wheels, whereas
    ``flatpak-pip-generator`` prefers source packages.
 
 License
 -------
 
 req2flatpak is MIT-licensed, see the ``COPYING`` file.
```

### Comparing `req2flatpak-0.1.0/pyproject.toml` & `req2flatpak-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,76 @@
+[build-system]
+requires      = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
-name = "req2flatpak"
-version = "0.1.0"
+name        = "req2flatpak"
+version     = "0.2.0"
 description = "Generates a flatpak-builder build module for installing python packages defined in requirements.txt files."
-authors = ["johannesjh <johannesjh@users.noreply.github.com>"]
-license = "MIT"
-readme = "README.rst"
+authors     = ["johannesjh <johannesjh@users.noreply.github.com>"]
+license     = "MIT"
+readme      = ["README.rst", "docs/source/changelog.rst"]
 
 [tool.poetry.scripts]
 req2flatpak = 'req2flatpak:main'
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python    = "^3.7.2"
 packaging = { version = "^21.3", optional = true }
+pyyaml    = { version = "^6.0", optional = true }
+
+[tool.poetry.extras]
+packaging = ["packaging"]
+yaml      = ["pyyaml"]
 
 [tool.poetry.group.lint.dependencies]
 pylama = { extras = [
     "mypy",
     "pylint",
     "eradicate",
     "toml",
 ], version = "^8.4.1" }
 bandit = { extras = ["toml"], version = "^1.7.4" }
-types-setuptools = "^65.5.0.2" # type stubs for mypy linting
+
+# type stubs for mypy linting
+types-setuptools = "^65.5.0.2"
+types-pyyaml     = "^6.0.12.8"
 
 # [tool.poetry.group.tests.dependencies]
+pydocstyle = "<6.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^5.3.0"
-sphinx-argparse = "^0.3.2"
+sphinx                           = "^5.3.0"
+sphinx-argparse                  = "^0.4.0"
+sphinx-rtd-theme                 = "^1.2.0"
 sphinx-rtd-theme-github-versions = "^1.1"
 
-[tool.poetry.extras]
-packaging = ["packaging"]
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
 [tool.isort]
-profile = "black"
+profile        = "black"
 skip_gitignore = true
 
 [tool.pylama]
 max_line_length = 88
-concurrent = true
-linters = "pycodestyle,pydocstyle,pyflakes,pylint,eradicate,mypy"
+concurrent      = true
+linters         = "pycodestyle,pydocstyle,pyflakes,pylint,eradicate,mypy"
 
 [tool.pylama.linter.pycodestyle]
 ignore = "W503,E203,E501"
 
 # [tool.pycodestyle] -> see setup.cfg
 
 [tool.pylama.linter.pydocstyle]
 ignore = "D202,D203,D205,D401,D212"
 
 [tool.pydocstyle]
 ignore = ["D202", "D203", "D205", "D401", "D212"]
 
 [tool.pylint]
 format.max-line-length = 88
-main.disable = ["C0301"]            # ignore line-too-long
-basic.good-names = ["e", "f", "py"]
+main.disable           = ["C0301"]        # ignore line-too-long
+basic.good-names       = ["e", "f", "py"]
 
 [tool.bandit]
 exclude_dirs = ['tests']
```

### Comparing `req2flatpak-0.1.0/req2flatpak.py` & `req2flatpak-0.2.0/req2flatpak.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,24 +60,27 @@
 )
 from urllib.parse import urlparse
 
 import pkg_resources
 
 logger = logging.getLogger(__name__)
 
+try:
+    import yaml
+except ImportError:
+    yaml = None  # type: ignore
 
 # =============================================================================
 # Helper functions / semi vendored code
 # =============================================================================
 
 try:
     # added with py 3.8
     from functools import cached_property  # type: ignore[attr-defined]
 except ImportError:
-
     # Inspired by the implementation in the standard library
     # pylint: disable=invalid-name,too-few-public-methods
     class cached_property:  # type: ignore[no-redef]
         """A property-like wrapper that caches the value."""
 
         def __init__(self, func):
             """Init."""
@@ -98,14 +101,18 @@
             val = cache.get(self.attrname, _None)
             if val is _None:
                 val = self.func(instance)
                 cache[self.attrname] = val
             return val
 
 
+class InvalidWheelFilename(Exception):
+    """An invalid wheel filename was found, users should refer to PEP 427."""
+
+
 try:
     # use packaging.tags functionality if available
     from packaging.utils import parse_wheel_filename
 
     def tags_from_wheel_filename(filename: str) -> Set[str]:
         """
         Parses a wheel filename into a list of compatible platform tags.
@@ -120,15 +127,14 @@
     # that is heavily inspired by / almost vendored from the `packaging` package:
     def tags_from_wheel_filename(filename: str) -> Set[str]:
         """
         Parses a wheel filename into a list of compatible platform tags.
 
         Implemented as (semi-)vendored functionality in req2flatpak.
         """
-        InvalidWheelFilename = Exception
         Tag = Tuple[str, str, str]
 
         # the following code is based on packaging.tags.parse_tag,
         # it is needed for the parse_wheel_filename function:
         def parse_tag(tag: str) -> FrozenSet[Tag]:
             tags: Set[Tag] = set()
             interpreters, abis, platforms = tag.split("-")
@@ -223,14 +229,25 @@
         if not self.is_sdist and self.is_wheel and self.tags:
             if any(tag.endswith("x86_64") for tag in self.tags):
                 return "x86_64"
             if any(tag.endswith("aarch64") for tag in self.tags):
                 return "aarch64"
         return None
 
+    def __lt__(self, other):
+        """Makes this class sortable."""
+        # Note: Implementing __lt__ is sufficient to make a class sortable,
+        # see, e.g., https://stackoverflow.com/a/7152796
+
+        def sort_keys(download: Download) -> Tuple[str, str, str]:
+            """A tuple of package, version and architecture is used as key for sorting."""
+            return download.package, download.version, download.arch or ""
+
+        return sort_keys(self) < sort_keys(other)
+
 
 @dataclass(frozen=True)
 class Release(Requirement):
     """Represents a package release as name, version, and downloads."""
 
     package: str
     version: str
@@ -304,15 +321,15 @@
             return cls.from_python_version_and_arch(minor_version=int(minor), arch=arch)
         except AttributeError:
             logger.warning("Could not parse platform string %s", platform_string)
             return None
 
     @classmethod
     def from_python_version_and_arch(
-        cls, minor_version: int = None, arch="x86_64"
+        cls, minor_version: Optional[int] = None, arch="x86_64"
     ) -> Platform:
         """
         Returns a platform object that roughly describes a cpython installation on linux.
 
         The tags in the platform object are a rough approximation, trying to match what
         `packaging.tags.sys_tags` would return if invoked on a linux system with cpython.
         No guarantees are made about how closely this approximation matches a real system.
@@ -329,15 +346,15 @@
             python_tags=list(
                 cls._cp3_linux_tags(minor_version=minor_version, arch=arch)
             ),
         )
 
     @classmethod
     def _cp3_linux_tags(
-        cls, minor_version: int = None, arch="x86_64"
+        cls, minor_version: Optional[int] = None, arch="x86_64"
     ) -> Generator[str, None, None]:
         """Yields python platform tags for cpython3 on linux."""
         # pylint: disable=too-many-branches
 
         assert minor_version is not None
         assert arch in ["x86_64", "aarch64"]
 
@@ -533,17 +550,15 @@
         """
         Yields suitable downloads for a specific platform.
 
         The order of downloads matches the order of platform tags, i.e.,
         preferred downloads are returned first.
         """
         cache = set()
-        for (platform_tag, download) in product(
-            platform.python_tags, release.downloads
-        ):
+        for platform_tag, download in product(platform.python_tags, release.downloads):
             if download in cache:
                 continue
             if wheels_only and not download.is_wheel:
                 continue
             if sdists_only and not download.is_sdist:
                 continue
             if cls.matches(download, platform_tag):
@@ -602,37 +617,52 @@
                 "sha256": download.sha256,
             }
             if download.arch:
                 source["only-arches"] = [download.arch]
             return source
 
         def sources(downloads: Iterable[Download]) -> List[dict]:
-            sorted_downloads = sorted(
-                downloads, key=lambda d: (d.package, d.version, d.arch)
-            )
-            return [source(download) for download in sorted_downloads]
+            return [source(download) for download in sorted(downloads)]
 
         return {
             "name": module_name,
             "buildsystem": "simple",
             "build-commands": [
                 pip_install_template + " ".join([req.package for req in requirements])
             ],
             "sources": sources(downloads),
         }
 
     @classmethod
     def build_module_as_str(cls, *args, **kwargs) -> str:
         """
-        Generates a build module for inclusion in a flatpak-builder build manifest.
+        Generate JSON build module for inclusion in a flatpak-builder build manifest.
 
         The args and kwargs are the same as in
         :py:meth:`~req2flatpak.FlatpakGenerator.build_module`
         """
-        return json.dumps(cls.build_module(*args, **kwargs), indent=2)
+        return json.dumps(cls.build_module(*args, **kwargs), indent=4)
+
+    @classmethod
+    def build_module_as_yaml_str(cls, *args, **kwargs) -> str:
+        """
+        Generate YAML build module for inclusion in a flatpak-builder build manifest.
+
+        The args and kwargs are the same as in
+        :py:meth:`~req2flatpak.FlatpakGenerator.build_module`
+        """
+        # optional dependency, not imported at top
+        if not yaml:
+            raise ImportError(
+                "Package `pyyaml` has to be installed for the yaml format."
+            )
+
+        return yaml.dump(
+            cls.build_module(*args, **kwargs), default_flow_style=False, sort_keys=False
+        )
 
 
 # =============================================================================
 # CLI commandline interface
 # =============================================================================
 
 
@@ -662,19 +692,29 @@
     parser.add_argument(
         "--cache",
         action="store_true",
         default=False,
         help="Uses a persistent cache when querying pypi.",
     )
     parser.add_argument(
+        "--yaml",
+        action="store_true",
+        help="Write YAML instead of the default JSON.  Needs the 'pyyaml' package.",
+    )
+
+    parser.add_argument(
         "--outfile",
         "-o",
         nargs="?",
         type=argparse.FileType("w"),
         default=sys.stdout,
+        help="""
+            By default, writes JSON but specify a '.yaml' extension and YAML
+            will be written instead, provided you have the 'pyyaml' package.
+        """,
     )
     parser.add_argument(
         "--platform-info",
         action="store_true",
         default=False,
         help="Prints information about the current platform.",
     )
@@ -683,29 +723,41 @@
         action="store_true",
         default=False,
         help="Prints installed packages in requirements.txt format.",
     )
     return parser
 
 
-def main():
+def main():  # pylint: disable=too-many-branches
     """Main function that provides req2flatpak's commandline interface."""
 
     # process commandline arguments
     parser = cli_parser()
     options = parser.parse_args()
 
     # stream output to a file or to stdout
-    output_stream = options.outfile if hasattr(options.outfile, "write") else sys.stdout
+    if hasattr(options.outfile, "write"):
+        output_stream = options.outfile
+        if pathlib.Path(output_stream.name).suffix.casefold() in (".yaml", ".yml"):
+            options.yaml = True
+    else:
+        output_stream = sys.stdout
+
+    if options.yaml and not yaml:
+        parser.error(
+            "Outputing YAML requires 'pyyaml' package: try 'pip install pyyaml'"
+        )
 
     # print platform info if requested, and exit
     if options.platform_info:
-        json.dump(
-            asdict(PlatformFactory.from_current_interpreter()), output_stream, indent=4
-        )
+        info = asdict(PlatformFactory.from_current_interpreter())
+        if options.yaml:
+            yaml.dump(info, output_stream, default_flow_style=False, sort_keys=False)
+        else:
+            json.dump(info, output_stream, indent=4)
         parser.exit()
 
     # print installed packages if requested, and exit
     if options.installed_packages:
         # pylint: disable=not-an-iterable
         pkgs = {p.key: p.version for p in pkg_resources.working_set}
         for pkg, version in pkgs.items():
@@ -751,18 +803,29 @@
         releases = PypiClient.get_releases(requirements)
 
     # choose suitable downloads for the target platforms
     downloads = {
         DownloadChooser.wheel_or_sdist(release, platform)
         for release in releases
         for platform in platforms
+        if platform
     }
 
     # generate flatpak-builder build module
-    build_module = FlatpakGenerator.build_module(requirements, downloads)
-
-    # write output
-    json.dump(build_module, output_stream, indent=4)
+    if options.yaml:
+        try:
+            name = pathlib.Path(__file__).name
+        except NameError:
+            name = "req2flatpak"
+        output_stream.write(f"# Generated by {name} {' '.join(sys.argv[1:])}\n")
+        output_stream.write(
+            FlatpakGenerator.build_module_as_yaml_str(requirements, downloads)
+        )
+    else:
+        # write json
+        output_stream.write(
+            FlatpakGenerator.build_module_as_str(requirements, downloads)
+        )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `req2flatpak-0.1.0/setup.py` & `req2flatpak-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,188 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: req2flatpak
+Version: 0.2.0
+Summary: Generates a flatpak-builder build module for installing python packages defined in requirements.txt files.
+License: MIT
+Author: johannesjh
+Author-email: johannesjh@users.noreply.github.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: packaging
+Provides-Extra: yaml
+Requires-Dist: packaging (>=21.3,<22.0) ; extra == "packaging"
+Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
+Description-Content-Type: text/x-rst
 
-modules = \
-['req2flatpak']
-extras_require = \
-{'packaging': ['packaging>=21.3,<22.0']}
-
-entry_points = \
-{'console_scripts': ['req2flatpak = req2flatpak:main']}
-
-setup_kwargs = {
-    'name': 'req2flatpak',
-    'version': '0.1.0',
-    'description': 'Generates a flatpak-builder build module for installing python packages defined in requirements.txt files.',
-    'long_description': "req2flatpak\n===========\n\n.. inclusion-marker-do-not-remove\n\n``req2flatpak`` is a script to convert python package requirements\nto a flatpak-builder build module.\nThe module will install the required python packages\nas part of a flatpak build.\n\n\nIntended Use\n------------\n\nreq2flatpak is for programmers\nwho want to package a python application using flatpak.\n\nThe req2flatpak script takes python package requirements as input, e.g., as\n``requirements.txt`` file. It allows to specify the target platform’s\npython version and architecture. The script outputs an automatically\ngenerated ``flatpak-builder`` build module. The build module, if included\ninto a flatpak-builder build manifest, will install the python packages\nusing pip.\n\nGetting Started\n---------------\n\nRun ``pip install git+https://github.com/johannesjh/req2flatpak``\nto install the latest development version of req2flatpak.\n\nIt is possible to use req2flatpak from the commandline,\nas well as programmatically from a python script.\n\nCommandline usage means you can invoke req2flatpak’s commandline interface\nas follows, in order to generate a ``flatpak-builder`` build module\nfrom given python package requirements:\n\n.. code:: bash\n\n   ./req2flatpak.py --requirements-file requirements.txt --target-platforms 310-x86_64 310-aarch64\n\nWhen invoked like this, req2flatpak will\nread the requirements file,\nquery pypi about available downloads for the requirements,\nchoose appropriate downloads for the specified target platforms,\nand generate a flatpak-builder build module.\nThe module, if included in a flatpak-builder build manifest,\nwill install the required packages using pip.\n\nThe commandline option to define target platforms uses the format ``<pythonversion>-<architecture>``.\nTo learn more about available commandline options,\nrun ``req2flatpak.py --help``.\n\nProgrammatic usage is also possible.\nThis means you can invoke functionality from req2flatpak in your own python script,\nallowing you to tweak the desired behavior in many ways.\nThe `documentation <https://johannesjh.github.io/req2flatpak/>`__\ndescribes req2flatpak's python api and includes code examples\nto help you get started quickly.\n\n\nDocumentation\n-------------\n\nSee https://johannesjh.github.io/req2flatpak/\n\n\nContributing\n------------\n\nreq2flatpak is developed in an open-source, community-driven way, as a\nvoluntary effort in the authors’ free time.\n\nAll contributions are greatly appreciated… pull requests are welcome,\nand so are bug reports and suggestions for improvement.\nSee req2flatpak’s documentation for how to set up a development environment\nand how to contribute back to req2flatpak.\n\nRelated Work\n------------\n\nThe\n`flatpak-pip-generator <https://github.com/flatpak/flatpak-builder-tools/blob/master/pip/flatpak-pip-generator>`__\nscript is very similar to this project. Both scripts basically serve the same purpose,\nand this project took a lot of inspiration from\nflatpak-pip-generator. In fact, this project was created when we\ndiscussed feature request\n`#296 <https://github.com/flatpak/flatpak-builder-tools/issues/296>`__\nin flatpak-pip-generator. A prototype followed from this feature\nrequest, and since it was written from scratch, the prototype became\nthis separate project.\n\nComparison between ``flatpak-pip-generator`` and ``req2flatpak.py``:\nEach of the two projects has its own benefits.\nA comparison will likely change over time.\nAs in Oct, 2022, in my personal opinion (johannesjh),\nI see the following similarities and differences:\n\n-  Both projects generate build modules for flatpak-builder.\n-  Both projects consist of a single script file with minimal\n   dependencies, and are thus very easy to install.\n-  ``flatpak-pip-generator`` resolves dependencies and freezes\n   dependency versions, whereas ``req2flatpak.py`` asks the user to\n   provide a fully resolved list of dependencies with frozen dependency\n   versions. Various tools exist which make this easy, e.g.,\n   pip, pip-compile and poetry.\n-  ``flatpak-pip-generator`` is older and thus likely to be more mature.\n   It supports more commandline options and probably has a more complete\n   feature set.\n-  ``req2flatpak.py`` is faster. The script itself runs faster because\n   it does not need to download package files in order to generate the\n   build module. And the flatpak build runs faster because all packages\n   (from the entire ``requirements.txt`` file) are installed in a single\n   call to ``pip install``.\n-  ``req2flatpak.py`` re-implements some functionality of pip. In\n   contrast, ``flatpak-pip-generator`` uses pip’s official\n   functionality. Specifically, ``req2flatpak.py`` re-implements how pip\n   queries available downloads from pypi and how pip chooses suitable\n   downloads to match a given target platform.\n-  ``req2flatpak.py`` prefers binary wheels, whereas\n   ``flatpak-pip-generator`` prefers source packages.\n\nLicense\n-------\n\nreq2flatpak is MIT-licensed, see the ``COPYING`` file.\n",
-    'author': 'johannesjh',
-    'author_email': 'johannesjh@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'py_modules': modules,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4.0.0',
-}
+req2flatpak
+===========
 
+.. inclusion-marker-do-not-remove
+
+``req2flatpak`` is a script to convert python package requirements
+to a flatpak-builder build module.
+The module will install the required python packages
+as part of a flatpak build.
+
+
+Intended Use
+------------
+
+req2flatpak is for programmers
+who want to package a python application using flatpak.
+
+The req2flatpak script takes python package requirements as input, e.g., as
+``requirements.txt`` file. It allows to specify the target platform’s
+python version and architecture. The script outputs an automatically
+generated ``flatpak-builder`` build module. The build module, if included
+into a flatpak-builder build manifest, will install the python packages
+using pip.
+
+Getting Started
+---------------
+
+Run ``pip install req2flatpak``
+to install the latest release of req2flatpak.
+
+It is possible to use req2flatpak from the commandline,
+as well as programmatically from a python script.
+
+Commandline usage means you can invoke req2flatpak’s commandline interface
+as follows, in order to generate a ``flatpak-builder`` build module
+from given python package requirements:
+
+.. code:: bash
+
+   ./req2flatpak.py --requirements-file requirements.txt --target-platforms 310-x86_64 310-aarch64
+
+When invoked like this, req2flatpak will
+read the requirements file,
+query pypi about available downloads for the requirements,
+choose appropriate downloads for the specified target platforms,
+and generate a flatpak-builder build module.
+The module, if included in a flatpak-builder build manifest,
+will install the required packages using pip.
+
+The commandline option to define target platforms uses the format ``<pythonversion>-<architecture>``.
+To learn more about available commandline options,
+run ``req2flatpak.py --help``.
+
+Programmatic usage is also possible.
+This means you can invoke functionality from req2flatpak in your own python script,
+allowing you to tweak the desired behavior in many ways.
+The `documentation <https://johannesjh.github.io/req2flatpak/>`__
+describes req2flatpak's python api and includes code examples
+to help you get started quickly.
+
+
+Documentation
+-------------
+
+See https://johannesjh.github.io/req2flatpak/
+
+
+Contributing
+------------
+
+req2flatpak is developed in an open-source, community-driven way, as a
+voluntary effort in the authors’ free time.
+
+All contributions are greatly appreciated… pull requests are welcome,
+and so are bug reports and suggestions for improvement.
+See req2flatpak’s documentation for how to set up a development environment
+and how to contribute back to req2flatpak.
+
+Related Work
+------------
+
+The
+`flatpak-pip-generator <https://github.com/flatpak/flatpak-builder-tools/blob/master/pip/flatpak-pip-generator>`__
+script is very similar to this project. Both scripts basically serve the same purpose,
+and this project took a lot of inspiration from
+flatpak-pip-generator. In fact, this project was created when we
+discussed feature request
+`#296 <https://github.com/flatpak/flatpak-builder-tools/issues/296>`__
+in flatpak-pip-generator. A prototype followed from this feature
+request, and since it was written from scratch, the prototype became
+this separate project.
+
+Comparison between ``flatpak-pip-generator`` and ``req2flatpak.py``:
+Each of the two projects has its own benefits.
+A comparison will likely change over time.
+As in Oct, 2022, in my personal opinion (johannesjh),
+I see the following similarities and differences:
+
+*  Both projects generate build modules for flatpak-builder.
+
+*  Both projects consist of a single script file with minimal
+   dependencies, and are thus very easy to install.
+
+*  ``flatpak-pip-generator`` resolves dependencies and freezes
+   dependency versions, whereas ``req2flatpak.py`` asks the user to
+   provide a fully resolved list of dependencies with frozen dependency
+   versions. Various tools exist which make this easy, e.g.,
+   pip, pip-compile and poetry.
+
+*  ``flatpak-pip-generator`` is older and thus likely to be more mature.
+   It supports more commandline options and probably has a more complete
+   feature set.
+
+*  ``req2flatpak.py`` is faster. The script itself runs faster because
+   it does not need to download package files in order to generate the
+   build module. And the flatpak build runs faster because all packages
+   (from the entire ``requirements.txt`` file) are installed in a single
+   call to ``pip install``.
+
+*  ``req2flatpak.py`` re-implements some functionality of pip. In
+   contrast, ``flatpak-pip-generator`` uses pip’s official
+   functionality. Specifically, ``req2flatpak.py`` re-implements how pip
+   queries available downloads from pypi and how pip chooses suitable
+   downloads to match a given target platform.
+
+*  ``req2flatpak.py`` prefers binary wheels, whereas
+   ``flatpak-pip-generator`` prefers source packages.
+
+License
+-------
+
+req2flatpak is MIT-licensed, see the ``COPYING`` file.
+
+Changelog
+=========
+
+..
+   This changelog is written by hand.
+   Newest releases are added to the top of the file.
+
+
+v0.2 (2023-06-04) "Yaml"
+------------------------
+
+Highlight: req2flatpak can now generate yaml output.
+
+Features:
+
+- Adds yaml output.
+  It is now possible to generate yaml output by specifying a ``.yaml`` file extension
+  or by specifying the ``--yaml`` commandline option.
+
+Bugfixes:
+
+- Fixes sorting when architecture is None - `#34 <https://github.com/johannesjh/req2flatpak/pull/34>`_
+- Fixes exception handling with invalid platforms - `#39 <https://github.com/johannesjh/req2flatpak/pull/39>`_
+
+
+v0.1 (2022-12-23) "Initial Release"
+-----------------------------------
+
+Highlight: This is the initial release of req2flatpak.
+
+Features:
+
+- Generates a flatpak-builder build module for given python package requirements; the module will install the required packages as part of a flatpak build.
+- This initial release already comes with documentation, a clean code style, and automated tests that are run using continuous integration.
 
-setup(**setup_kwargs)
```

