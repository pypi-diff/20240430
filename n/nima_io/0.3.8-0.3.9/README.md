# Comparing `tmp/nima_io-0.3.8.tar.gz` & `tmp/nima_io-0.3.9.tar.gz`

## Comparing `nima_io-0.3.8.tar` & `nima_io-0.3.9.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nima_io-0.3.8/.gitmodules
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 nima_io-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nima_io-0.3.8/.readthedocs.yml
--rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 nima_io-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 nima_io-0.3.8/cz_customize_info.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/dependabot.yml
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/workflows/ci.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/workflows/constraints.txt
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 nima_io-0.3.8/.github/workflows/docs.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/Makefile
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/click.rst
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/conf.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/make.bat
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/api/api.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/api/nima_io.rst
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/contributing.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/description.rst
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/development.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/ii.rst
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/ii.uml.rst
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/main_module_docstring.rst
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/references/references.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nima_io-0.3.8/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0    45072 2020-02-02 00:00:00.000000 nima_io-0.3.8/examples/mydatafile.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/py.typed
--rw-r--r--   0        0        0    29255 2020-02-02 00:00:00.000000 nima_io-0.3.8/src/nima_io/read.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/conftest.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/data.filenames.md5
--rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/data.filenames.sh
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/data.filenames.txt
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/test_cli.py
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 nima_io-0.3.8/tests/test_read.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nima_io-0.3.8/.gitignore
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nima_io-0.3.8/LICENSE.txt
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 nima_io-0.3.8/README.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 nima_io-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 nima_io-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nima_io-0.3.9/.gitmodules
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 nima_io-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nima_io-0.3.9/.readthedocs.yml
+-rw-r--r--   0        0        0    12949 2020-02-02 00:00:00.000000 nima_io-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 nima_io-0.3.9/cz_customize_info.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nima_io-0.3.9/.github/dependabot.yml
+-rw-r--r--   0        0        0    10681 2020-02-02 00:00:00.000000 nima_io-0.3.9/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 nima_io-0.3.9/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/Makefile
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/click.rst
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/conf.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/make.bat
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/api/api.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/api/nima_io.rst
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/contributing.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/description.rst
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/development.rst
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/ii.rst
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/ii.uml.rst
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/main_module_docstring.rst
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/references/references.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nima_io-0.3.9/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0    45072 2020-02-02 00:00:00.000000 nima_io-0.3.9/examples/mydatafile.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nima_io-0.3.9/src/nima_io/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 nima_io-0.3.9/src/nima_io/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nima_io-0.3.9/src/nima_io/py.typed
+-rw-r--r--   0        0        0    29255 2020-02-02 00:00:00.000000 nima_io-0.3.9/src/nima_io/read.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nima_io-0.3.9/tests/conftest.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 nima_io-0.3.9/tests/data.filenames.md5
+-rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 nima_io-0.3.9/tests/data.filenames.sh
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nima_io-0.3.9/tests/data.filenames.txt
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 nima_io-0.3.9/tests/test_cli.py
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 nima_io-0.3.9/tests/test_read.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 nima_io-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 nima_io-0.3.9/LICENSE.txt
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 nima_io-0.3.9/README.md
+-rw-r--r--   0        0        0     9196 2020-02-02 00:00:00.000000 nima_io-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 nima_io-0.3.9/PKG-INFO
```

### Comparing `nima_io-0.3.8/.pre-commit-config.yaml` & `nima_io-0.3.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ci:
-  autoupdate_commit_msg: "chore: update pre-commit hooks"
+  autoupdate_commit_msg: "build(pre-commit): update hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
       - id: check-added-large-files
@@ -30,29 +30,28 @@
     hooks:
       - id: pretty-format-ini
         args: [--autofix]
       - id: pretty-format-toml
         args: [--autofix]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.2
     hooks:
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: [--fix]
       # Run the formatter.
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         files: \.(yaml|yml|md|html|css|scss|js|json)$
-        types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=preserve]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
       - id: python-use-type-annotations
       - id: rst-backticks
@@ -82,12 +81,12 @@
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.10.0.1
     hooks:
       - id: shellcheck
         args: [-x]
 
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.21.3
+    rev: v3.24.0
     hooks:
       - id: commitizen
       - id: commitizen-branch
         stages: [push]
```

### Comparing `nima_io-0.3.8/.readthedocs.yml` & `nima_io-0.3.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/CHANGELOG.md` & `nima_io-0.3.9/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,63 @@
 <!-- markdownlint-disable MD024 -->
 <!-- vale write-good.TooWordy = NO -->
 
 # Changelog
 
+## v0.3.9 (2024-04-30)
+
+### Build
+
+- Update loci to 7.3.0
+- **pre-commit**: update hooks (#144)
+- **deps**: update pytest requirement from <=8.1.2 to <=8.2.0 (#143)
+- **deps**: update pytest requirement from <=8.1.1 to <=8.1.2 (#142)
+- **deps**: update ruff requirement from <=0.4.1 to <=0.4.2 (#141)
+- **deps**: update mypy requirement from <=1.9.0 to <=1.10.0 (#140)
+- **deps**: bump hatch from 1.9.4 to 1.9.7 in /.github/workflows (#139)
+- **deps**: update coverage[toml] requirement from <=7.4.4 to <=7.5.0 (#138)
+- **deps**: update scikit-image requirement from <=0.23.1 to <=0.23.2 (#136)
+- **deps**: update ruff requirement from <=0.4.0 to <=0.4.1 (#135)
+- **deps**: update sphinx requirement from <=7.3.6 to <=7.3.7 (#134)
+- **deps**: update commitizen requirement from <=3.22.0 to <=3.24.0 (#133)
+- **deps**: update ruff requirement from <=0.3.7 to <=0.4.0 (#132)
+- **deps**: update sphinx requirement from <=7.3.5 to <=7.3.6 (#131)
+- **deps**: update sphinx-autodoc-typehints requirement from <=2.0.1 to <=2.1.0 (#130)
+- **deps**: update sphinx requirement from <=7.2.6 to <=7.3.5 (#129)
+- **deps**: bump codecov/codecov-action from 4.2.0 to 4.3.0 (#119)
+- **fix**: message_template and prettier
+- **deps**: update ruff requirement from <=0.3.6 to <=0.3.7 (#124)
+- **deps**: update commitizen requirement from <=3.21.3 to <=3.22.0 (#123)
+- **deps**: update ruff requirement from <=0.3.5 to <=0.3.6 (#122)
+- **deps-dev**: update sphinx-autodoc-typehints requirement (#121)
+- **deps-dev**: update scikit-image requirement (#120)
+
+### CI/CD
+
+- rename pip caches
+- MacOS requires update of jdk from 8 to 11
+- Deploy pages also for pull request
+- Merge docs into ci
+- automerge fixes
+- Move auto_merge into ci workflow
+- **fix**: Add auto_merge workflow for dependabot labeled pr
+- **fix**: Add auto_merge workflow for dependabot labeled pr
+- Add auto_merge workflow for dependabot labeled pr
+
+### Refactor
+
+- cache pip
+
+### chore
+
+- Modify pre-commit update message
+- update pre-commit hooks (#137)
+- **build**: Adjust pre-commit config and pyproject.toml
+- update pre-commit hooks (#125)
+
 ## v0.3.8 (2024-04-10)
 
 ### Fix
 
 - license
 
 ## v0.3.7 (2024-04-10)
```

### Comparing `nima_io-0.3.8/cz_customize_info.txt` & `nima_io-0.3.9/cz_customize_info.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/.github/workflows/ci.yml` & `nima_io-0.3.9/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# Run lint, mypy, and xdoctest, and pytest with coverage
+# CI Workflow
+# This workflow runs linting, type checking, and testing (pytest with coverage),
+# builds documentation, and deploys it to GitHub Pages.
 name: CI
 
 on:
   workflow_dispatch:
   pull_request:
     paths-ignore:
       - "docs/**"
       - "*.md"
   push:
     paths-ignore:
-      - "docs/**"
       - "*.md"
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
-  STABLE_PYTHON_VERSION: "3.11"
-  # PYTHONUNBUFFERED: "1"
+  STABLE_PYTHON_VERSION: "3.12"
+  PYTHONUNBUFFERED: "1"
   FORCE_COLOR: "1"
 
 jobs:
   pre-commit:
     name: Lint
     runs-on: "ubuntu-latest"
     steps:
@@ -30,19 +31,19 @@
         uses: actions/checkout@v4
 
       - name: Set up Python-${{ env.STABLE_PYTHON_VERSION }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ env.STABLE_PYTHON_VERSION }}
 
-      - name: Set up JDK 8
+      - name: Set up JDK 11
         uses: actions/setup-java@v4
         with:
           distribution: "adopt"
-          java-version: 8
+          java-version: 11
 
       - name: Display JAVA version
         run: java -version
 
       - name: Cache pip
         id: cache-pip
         uses: actions/cache@v4
@@ -77,19 +78,19 @@
         uses: actions/checkout@v4
 
       - name: Set up Python-${{ matrix.python }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
 
-      - name: Set up JDK 8
+      - name: Set up JDK 11
         uses: actions/setup-java@v4
         with:
           distribution: "adopt"
-          java-version: 8
+          java-version: 11
 
       - name: Display JAVA version
         run: java -version
 
       - name: Cache tests/data
         id: cache-data
         uses: actions/cache@v4
@@ -109,21 +110,30 @@
 
       - name: List cached data files
         if: "!startsWith(matrix.os , 'windows-')"
         run: |
           echo "Listing files in tests/data"
           ls -a tests/data
 
+      # TODO: check
+      - name: Setup pip cache directory
+        run: |
+          mkdir -p ~/.cache/pip
+        if: runner.os == 'macOS'
+
       - name: Cache pip
         id: cache-pip
         uses: actions/cache@v4
         with:
           path: ~/.cache/pip
-          key: ${{ runner.os }}|pip|${{ matrix.python }}|-${{ hashFiles('**/constraints.txt', '**/pyproject.toml') }}
+          key: ${{ runner.os }}|pip|${{ matrix.python }}|${{ hashFiles('**/constraints.txt', '**/pyproject.toml') }}
+          restore-keys: |
+            ${{ runner.os }}|pip|${{ matrix.python }}|
           enableCrossOsArchive: true
+          fail-on-cache-miss: false
 
       - name: Install pip and hatch
         run: |
           python -m pip install --constraint=.github/workflows/constraints.txt pip hatch
 
       - name: Run pytest and coverage
         if: matrix.tests == 'pytest'
@@ -131,15 +141,15 @@
 
       - name: Run coverage
         if: matrix.tests == 'pytest'
         run: hatch run tests.py${{ matrix.python }}:cov
 
       - name: Upload coverage report
         if: matrix.tests == 'pytest'
-        uses: codecov/codecov-action@v4.2.0
+        uses: codecov/codecov-action@v4.3.0
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
 
       - name: Run mypy
         if: matrix.tests == 'mypy'
         run: hatch run tests.py${{ matrix.python }}:type
 
@@ -166,19 +176,19 @@
         id: version
         run: |
           echo ${{ github.event.head_commit.message }}
           ver=`echo ${{ github.event.head_commit.message }} | awk '{ print $NF }'`
           echo "ver=${ver}" >> $GITHUB_OUTPUT
           echo "ver=${ver}" >> $GITHUB_ENV
 
-      - name: Set up JDK 8
+      - name: Set up JDK 11
         uses: actions/setup-java@v4
         with:
           distribution: "adopt"
-          java-version: 8
+          java-version: 11
 
       - name: Cache pip
         id: cache-pip
         uses: actions/cache@v4
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}|pip|${{ env.STABLE_PYTHON_VERSION }}|${{ hashFiles('**/constraints.txt', '**/pyproject.toml') }}
@@ -219,7 +229,123 @@
         with:
           python-version: ${{ env.STABLE_PYTHON_VERSION }}
 
       - name: Build and publish
         run: |
           pipx run hatch build
           pipx run hatch publish --user=__token__ --auth=${{ secrets.PYPI_TOKEN }}
+
+  docs_build:
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout Repository
+        uses: actions/checkout@v4
+
+      - name: Set up Python ${{ env.STABLE_PYTHON_VERSION }}
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ env.STABLE_PYTHON_VERSION }}
+
+      - name: Set up JDK 11
+        uses: actions/setup-java@v4
+        with:
+          distribution: "adopt"
+          java-version: 11
+
+      - name: Display JAVA version
+        run: java -version
+
+      - name: Install binaries for docs
+        run: |
+          sudo add-apt-repository ppa:openjdk-r/ppa
+          sudo apt-get update
+          sudo apt-get install -y pandoc
+          sudo apt-get install -y plantuml
+
+      - name: Cache tests/data
+        id: cache-data
+        uses: actions/cache@v4
+        with:
+          path: tests/data
+          key: ${{ hashFiles('tests/data.filenames.md5') }}
+          enableCrossOsArchive: true
+
+      - name: Download tests data files
+        if: steps.cache-data.outputs.cache-hit != 'true' && matrix.tests != 'mypy'
+        run: |
+          base_url="https://gin.g-node.org/darosio/imgread-testdata/raw/master/"
+          wget -P tests/data/ -i tests/data.filenames.txt -B "$base_url"
+          files=($(<tests/data.filenames.txt))
+          echo "files=${files[*]}" >> $GITHUB_OUTPUT
+
+      - name: List cached data files
+        run: |
+          echo "Listing files in tests/data"
+          ls -a tests/data
+
+      - name: Cache pip
+        id: cache-pip
+        uses: actions/cache@v4
+        with:
+          path: ~/.cache/pip
+          key: ${{ runner.os }}|pip|${{ env.STABLE_PYTHON_VERSION }}|-${{ hashFiles('**/constraints.txt', '**/pyproject.toml') }}
+          enableCrossOsArchive: true
+
+      - name: Install pip and hatch
+        run: |
+          python -m pip install --constraint=.github/workflows/constraints.txt pip hatch
+
+      - name: Run hatch
+        run: hatch run docs
+
+      - name: Upload artifact
+        uses: actions/upload-pages-artifact@v3
+        with:
+          name: github-pages
+          path: "./docs/_build"
+
+  docs_deploy:
+    runs-on: ubuntu-latest
+    if: ${{ github.ref == 'refs/heads/main' }}
+    # if: ${{  (github.event_name == 'pull_request' && github.event.pull_request.merged == true) }}
+    # if: ${{  (github.event_name == 'pull_request' && github.event.pull_request.base.ref == 'main') }}
+    needs: [docs_build]
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    # Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
+    permissions:
+      contents: read
+      pages: write
+      id-token: write
+    steps:
+      - name: Download artifact
+        uses: actions/download-artifact@v4
+        with:
+          name: github-pages
+      - name: Deploy to GitHub Pages
+        id: deployment
+        uses: actions/deploy-pages@v4
+
+  auto_merge_deps:
+    name: Auto Merge dependencies labeled PRs
+    needs: [pre-commit, tests, docs_build]
+    # Run only on pull_request labeled dependencies (e.g. by dependabot) or
+    # with the pre-commit ci commit message.
+    if: >
+      startsWith(github.event.pull_request.title, 'build(pre-commit): update hooks') ||
+      contains(github.event.pull_request.labels.*.name, 'dependencies')
+    runs-on: ubuntu-latest
+    permissions:
+      contents: write
+    steps:
+      - name: Checkout code
+        uses: actions/checkout@v4
+
+      - name: Merge PR
+        uses: pascalgn/automerge-action@v0.16.3
+        env:
+          GITHUB_TOKEN: "${{ secrets.GITHUB_TOKEN }}"
+          MERGE_LABELS: ""
+          MERGE_METHOD: squash
+          DELETE_BRANCH_AFTER_MERGE: true
+          LOG: "TRACE" # or DEBUG
```

### Comparing `nima_io-0.3.8/docs/Makefile` & `nima_io-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/docs/conf.py` & `nima_io-0.3.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "NImA-io"
-release = "0.3.8"
+release = "0.3.9"
 author = "Daniele Arosio"
 copyright = f"2023, {author}"  # noqa: A001
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
```

### Comparing `nima_io-0.3.8/docs/index.rst` & `nima_io-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/docs/make.bat` & `nima_io-0.3.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/docs/references/contributing.rst` & `nima_io-0.3.9/docs/references/contributing.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/docs/references/development.rst` & `nima_io-0.3.9/docs/references/development.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/docs/references/ii.uml.rst` & `nima_io-0.3.9/docs/references/ii.uml.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/docs/references/main_module_docstring.rst` & `nima_io-0.3.9/docs/references/main_module_docstring.rst`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/examples/mydatafile.txt` & `nima_io-0.3.9/examples/mydatafile.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/src/nima_io/__main__.py` & `nima_io-0.3.9/src/nima_io/__main__.py`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/src/nima_io/read.py` & `nima_io-0.3.9/src/nima_io/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 Pixels = Any
 Image = Any
 ChannelSeparator = Any
 OMEPyramidStore = Any
 
 
 def start_loci(
-    version: str = "7.1.0", java_memory: str = "4g", debug_level: str = "INFO"
+    version: str = "7.3.0", java_memory: str = "4g", debug_level: str = "INFO"
 ) -> None:
     """Initialize the loci package and associated classes.
 
     This function starts the Java Virtual Machine (JVM), configures endpoints,
     and initializes global variables for the loci package and related classes.
 
     Global Variables
@@ -46,15 +46,15 @@
         Global variable for the Pixels class from the ome.xml.model package.
     Image: ome.xml.model.Image
         Global variable for the Image class from the ome.xml.model package.
 
     Parameters
     ----------
     version : str, optional
-        Version of Bioformats to use (default "7.1.0").
+        Version of Bioformats to use (default "7.3.0").
     java_memory : str, optional
         Maximum memory for JVM (default "4g").
     debug_level : str, optional
         Logging level for Java process "ERROR", "WARN", "INFO", "DEBUG", "TRACE"
         (default "INFO").
 
     """
```

### Comparing `nima_io-0.3.8/tests/data.filenames.md5` & `nima_io-0.3.9/tests/data.filenames.md5`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/tests/data.filenames.sh` & `nima_io-0.3.9/tests/data.filenames.sh`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/tests/test_cli.py` & `nima_io-0.3.9/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # tests path
 tpath = Path(__file__).parent
 datafolder = tpath / "data"
 
 
 def test_version() -> None:
     """Report correct version."""
-    expected_version = "0.3.8"
+    expected_version = "0.3.9"
     runner = CliRunner()
     result = runner.invoke(imgdiff, ["--version"])
     assert result.output.startswith(expected_version)
 
 
 @pytest.fixture(
     params=[
```

### Comparing `nima_io-0.3.8/tests/test_read.py` & `nima_io-0.3.9/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/.gitignore` & `nima_io-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/LICENSE.txt` & `nima_io-0.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nima_io-0.3.8/README.md` & `nima_io-0.3.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 <!-- [![RtD](https://readthedocs.org/projects/nima_io/badge/)](https://nima_io.readthedocs.io/) -->
 
 This is a helper library designed for reading microscopy data supported by
 [Bioformats](https://www.openmicroscopy.org/bio-formats/) using Python. The
 package also includes a command-line interface for assessing differences between
 images.
 
-- Version: "0.3.8"
+- Version: "0.3.9"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/nima_io/)
 using `pip`:
 
     pip install nima_io
```

### Comparing `nima_io-0.3.8/pyproject.toml` & `nima_io-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,44 +41,44 @@
   "Open Microscopy",
   "Tiled Images"
 ]
 license = "BSD-3-Clause"
 name = "nima_io"
 readme = "README.md"
 requires-python = ">=3.10, <3.13"
-version = "0.3.8"
+version = "0.3.9"
 
 [project.optional-dependencies]
 dev = [
-  "commitizen <= 3.21.3",
+  "commitizen <= 3.24.0",
   "ipykernel",
   "jupyter",
   # "jupyterlab",
-  "ruff <= 0.3.5",
+  "ruff <= 0.4.2",
   "pre-commit <= 3.7.0",
   "pylsp-mypy",
   "ruff-lsp",
-  "scikit-image <= 0.22.0",
+  "scikit-image <= 0.23.2",
   "matplotlib <= 3.8.4"
 ]
 docs = [
   "autodocsumm <= 0.2.12",
   "nbsphinx <= 0.9.3",
   "pydata-sphinx-theme <= 0.15.2",
-  "Sphinx <= 7.2.6",
+  "Sphinx <= 7.3.7",
   "sphinx-click <= 5.1.0",
-  "sphinx_autodoc_typehints <= 2.0.0",
+  "sphinx_autodoc_typehints <= 2.1.0",
   "sphinxcontrib-plantuml <= 0.29",
   "xmltodict"
 ]
 tests = [
-  "coverage[toml] <= 7.4.4",
-  "mypy <= 1.9.0",
+  "coverage[toml] <= 7.5.0",
+  "mypy <= 1.10.0",
   "pygments <= 2.17.2",  # color xdoctest
-  "pytest <= 8.1.1",
+  "pytest <= 8.2.0",
   "types-click <= 7.1.8",
   "xdoctest <= 1.1.3"
 ]
 
 [project.scripts]
 imgdiff = "nima_io.__main__:imgdiff"
 
@@ -91,41 +91,24 @@
 Homepage = "https://github.com/darosio/nima_io"
 
 [tool.bandit]
 skips = ["B101", "B603"]
 # exclude_dirs = ["tests"]
 tests = ["B201", "B301"]
 
-[tool.black]
-exclude = '''
-/(
-    \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-)/
-'''
-line-length = 88
-skip-string-normalization = false
-
 [tool.codespell]
 count = ''
 ignore-words-list = 'ciao'
 quiet-level = 3
 skip = 'examples/general_reading_and_development.ipynb,aics_et_al.ipynb'
 
 [tool.commitizen]
 name = "cz_customize"
 tag_format = "v$version"
-version = "0.3.8"
+version = "0.3.9"
 version_files = [
   "pyproject.toml:version",
   "docs/conf.py:release",
   "README.md:Version",
   "tests/test_cli.py:expected_version"
 ]
 
@@ -137,15 +120,15 @@
 changelog_pattern = "^(feat|fix|docs|style|refactor|perf|test|build|ci)?(\\(.*\\))?(!)?"
 commit_parser = "^(?P<change_type>feat|fix|docs|style|refactor|perf|test|build|ci|chore|revert)(?:\\((?P<scope>[^()\r\n]*)\\)|\\()?(?P<breaking>!)?:\\s(?P<message>.*)?"
 example = """fix(parser): correct minor typos in code\n
 see the issue for details on the typos fixed\n
 closes issue #12
 """
 info_path = "cz_customize_info.txt"
-message_template = "change_type: if show_message  message endif"
+message_template = "{{change_type}}:{% if show_message %} {{message}}{% endif %}"
 schema = """
 <type>(<scope>): <subject>
 <BLANK LINE>
 <body>
 <BLANK LINE>
 (BREAKING CHANGE: )<footer>
 """
@@ -210,15 +193,15 @@
 init = [
   "pre-commit --version",
   "pre-commit install",
   "pre-commit install --hook-type commit-msg --hook-type pre-push"
 ]
 lint = [
   "pre-commit --version",
-  "pre-commit run --all-files --show-diff-on-failure {args}"  # No need for --hook-stage=manual
+  "pre-commit run --all-files --show-diff-on-failure {args}"
 ]
 
 [tool.hatch.envs.tests]
 features = ["tests"]
 template = "tests"
 
 [[tool.hatch.envs.tests.matrix]]
@@ -227,17 +210,15 @@
 [tool.hatch.envs.tests.scripts]
 all = ["test", "type", "xdoc", "cov"]
 cov = [
   "coverage combine",
   "coverage report",
   "coverage xml"
 ]
-test = [
-  "coverage run -p -m pytest -v"
-]
+test = "coverage run -p -m pytest -v"
 type = "mypy src tests docs/conf.py"
 xdoc = "python -m xdoctest nima_io all"
 
 [tool.isort]
 combine_as_imports = true
 force_single_line = false
 include_trailing_comma = true
```

### Comparing `nima_io-0.3.8/PKG-INFO` & `nima_io-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nima_io
-Version: 0.3.8
+Version: 0.3.9
 Summary: A project to read microscopy files.
 Project-URL: Bug Tracker, https://github.com/darosio/nima_io/issues
 Project-URL: Changelog, https://github.com/darosio/nima_io/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://nima-io.readthedocs.io
 Project-URL: Github releases, https://github.com/darosio/nima_io/releases
 Project-URL: Homepage, https://github.com/darosio/nima_io
 Author-email: Daniele Arosio <darosio@duck.com>
@@ -32,37 +32,37 @@
 Requires-Dist: numpy<=1.26.4
 Requires-Dist: pims<=0.6.1
 Requires-Dist: pyometiff<=1.0.0
 Requires-Dist: readlif<=0.6.5
 Requires-Dist: scyjava<=1.9.1
 Requires-Dist: setuptools
 Provides-Extra: dev
-Requires-Dist: commitizen<=3.21.3; extra == 'dev'
+Requires-Dist: commitizen<=3.24.0; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: jupyter; extra == 'dev'
 Requires-Dist: matplotlib<=3.8.4; extra == 'dev'
 Requires-Dist: pre-commit<=3.7.0; extra == 'dev'
 Requires-Dist: pylsp-mypy; extra == 'dev'
 Requires-Dist: ruff-lsp; extra == 'dev'
-Requires-Dist: ruff<=0.3.5; extra == 'dev'
-Requires-Dist: scikit-image<=0.22.0; extra == 'dev'
+Requires-Dist: ruff<=0.4.2; extra == 'dev'
+Requires-Dist: scikit-image<=0.23.2; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodocsumm<=0.2.12; extra == 'docs'
 Requires-Dist: nbsphinx<=0.9.3; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme<=0.15.2; extra == 'docs'
-Requires-Dist: sphinx-autodoc-typehints<=2.0.0; extra == 'docs'
+Requires-Dist: sphinx-autodoc-typehints<=2.1.0; extra == 'docs'
 Requires-Dist: sphinx-click<=5.1.0; extra == 'docs'
-Requires-Dist: sphinx<=7.2.6; extra == 'docs'
+Requires-Dist: sphinx<=7.3.7; extra == 'docs'
 Requires-Dist: sphinxcontrib-plantuml<=0.29; extra == 'docs'
 Requires-Dist: xmltodict; extra == 'docs'
 Provides-Extra: tests
-Requires-Dist: coverage[toml]<=7.4.4; extra == 'tests'
-Requires-Dist: mypy<=1.9.0; extra == 'tests'
+Requires-Dist: coverage[toml]<=7.5.0; extra == 'tests'
+Requires-Dist: mypy<=1.10.0; extra == 'tests'
 Requires-Dist: pygments<=2.17.2; extra == 'tests'
-Requires-Dist: pytest<=8.1.1; extra == 'tests'
+Requires-Dist: pytest<=8.2.0; extra == 'tests'
 Requires-Dist: types-click<=7.1.8; extra == 'tests'
 Requires-Dist: xdoctest<=1.1.3; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # NImA-io
 
 [![PyPI](https://img.shields.io/pypi/v/nima_io.svg)](https://pypi.org/project/nima_io/)
@@ -73,15 +73,15 @@
 <!-- [![RtD](https://readthedocs.org/projects/nima_io/badge/)](https://nima_io.readthedocs.io/) -->
 
 This is a helper library designed for reading microscopy data supported by
 [Bioformats](https://www.openmicroscopy.org/bio-formats/) using Python. The
 package also includes a command-line interface for assessing differences between
 images.
 
-- Version: "0.3.8"
+- Version: "0.3.9"
 
 ## Installation
 
 You can get the library directly from [PyPI](https://pypi.org/project/nima_io/)
 using `pip`:
 
     pip install nima_io
```

