# Comparing `tmp/sourcesage-4.1.2.tar.gz` & `tmp/sourcesage-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.1.2.tar", last modified: Sun Apr  7 15:47:49 2024, max compression
+gzip compressed data, was "sourcesage-4.1.4.tar", last modified: Tue Apr 30 06:23:24 2024, max compression
```

## Comparing `sourcesage-4.1.2.tar` & `sourcesage-4.1.4.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.374963 sourcesage-4.1.2/
--rw-rw-rw-   0        0        0     1082 2024-04-04 07:13:56.000000 sourcesage-4.1.2/LICENSE
--rw-rw-rw-   0        0        0    15649 2024-04-07 15:47:49.374963 sourcesage-4.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    15251 2024-04-07 15:45:44.000000 sourcesage-4.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 15:47:49.374963 sourcesage-4.1.2/setup.cfg
--rw-rw-rw-   0        0        0      915 2024-04-07 15:47:47.000000 sourcesage-4.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.282126 sourcesage-4.1.2/sourcesage/
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/__init__.py
--rw-rw-rw-   0        0        0     1441 2024-04-07 15:31:18.000000 sourcesage-4.1.2/sourcesage/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.320073 sourcesage-4.1.2/sourcesage/config/
--rw-rw-rw-   0        0        0      306 2024-04-07 15:31:18.000000 sourcesage-4.1.2/sourcesage/config/.SourceSageignore
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.323112 sourcesage-4.1.2/sourcesage/config/ISSUES_RESOLVE/
--rw-rw-rw-   0        0        0     1113 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.333311 sourcesage-4.1.2/sourcesage/config/STAGE_INFO/
--rw-rw-rw-   0        0        0     1319 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
--rw-rw-rw-   0        0        0     1127 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.334874 sourcesage-4.1.2/sourcesage/config/__pycache__/
--rw-rw-rw-   0        0        0     3229 2024-04-04 16:07:17.000000 sourcesage-4.1.2/sourcesage/config/__pycache__/constants.cpython-311.pyc
--rw-rw-rw-   0        0        0     1773 2024-04-07 15:31:18.000000 sourcesage-4.1.2/sourcesage/config/constants.py
--rw-rw-rw-   0        0        0      590 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/config/language_map.json
--rw-rw-rw-   0        0        0     4932 2024-04-07 15:31:18.000000 sourcesage-4.1.2/sourcesage/core.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.370674 sourcesage-4.1.2/sourcesage/modules/
--rw-rw-rw-   0        0        0     3915 2024-04-07 15:45:44.000000 sourcesage-4.1.2/sourcesage/modules/ChangelogGenerator.py
--rw-rw-rw-   0        0        0     1440 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/ChangelogUtils.py
--rw-rw-rw-   0        0        0     4171 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/DiffChangelogGenerator.py
--rw-rw-rw-   0        0        0     1073 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/EnvFileHandler.py
--rw-rw-rw-   0        0        0      836 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/GitHubIssueRetrieve.py
--rw-rw-rw-   0        0        0     1291 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/GitHubUtils.py
--rw-rw-rw-   0        0        0     2227 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/IssuesToMarkdown.py
--rw-rw-rw-   0        0        0     3036 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/StageInfoGenerator.py
--rw-rw-rw-   0        0        0     2778 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/StagedDiffGenerator.py
--rw-rw-rw-   0        0        0        0 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/__init__.py
--rw-rw-rw-   0        0        0      930 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/file_utils.py
--rw-rw-rw-   0        0        0     3261 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/markdown_utils.py
--rw-rw-rw-   0        0        0     1115 2024-04-04 15:59:17.000000 sourcesage-4.1.2/sourcesage/modules/source_sage.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.316289 sourcesage-4.1.2/sourcesage.egg-info/
--rw-rw-rw-   0        0        0    15649 2024-04-07 15:47:49.000000 sourcesage-4.1.2/sourcesage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2024-04-07 15:47:49.000000 sourcesage-4.1.2/sourcesage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 15:47:49.000000 sourcesage-4.1.2/sourcesage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-07 15:47:49.000000 sourcesage-4.1.2/sourcesage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-07 15:47:49.000000 sourcesage-4.1.2/sourcesage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 15:47:49.000000 sourcesage-4.1.2/sourcesage.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 15:47:49.372676 sourcesage-4.1.2/tests/
--rw-rw-rw-   0        0        0     3207 2024-04-07 15:31:18.000000 sourcesage-4.1.2/tests/test_sourcesage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.732770 sourcesage-4.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 06:23:20.000000 sourcesage-4.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-30 06:23:24.732770 sourcesage-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-04-30 06:23:20.000000 sourcesage-4.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 06:23:24.732770 sourcesage-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-30 06:23:20.000000 sourcesage-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.728770 sourcesage-4.1.4/sourcesage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.728770 sourcesage-4.1.4/sourcesage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/config/.SourceSageignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.728770 sourcesage-4.1.4/sourcesage/config/ISSUES_RESOLVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.732770 sourcesage-4.1.4/sourcesage/config/STAGE_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/config/language_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.732770 sourcesage-4.1.4/sourcesage/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/ChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/ChangelogUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/DiffChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/EnvFileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/IssuesToMarkdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/StageInfoGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/StagedDiffGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/markdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 06:23:20.000000 sourcesage-4.1.4/sourcesage/modules/source_sage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.732770 sourcesage-4.1.4/sourcesage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-30 06:23:24.000000 sourcesage-4.1.4/sourcesage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 06:23:24.000000 sourcesage-4.1.4/sourcesage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 06:23:24.000000 sourcesage-4.1.4/sourcesage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 06:23:24.000000 sourcesage-4.1.4/sourcesage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 06:23:24.000000 sourcesage-4.1.4/sourcesage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 06:23:24.000000 sourcesage-4.1.4/sourcesage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 06:23:24.732770 sourcesage-4.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-30 06:23:20.000000 sourcesage-4.1.4/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.1.2/PKG-INFO` & `sourcesage-4.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,229 +1,232 @@
-Metadata-Version: 2.1
-Name: sourcesage
-Version: 4.1.2
-Home-page: https://github.com/Sunwood-ai-labs/SourceSage
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: loguru
-Requires-Dist: GitPython
-Requires-Dist: requests
-Requires-Dist: art
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
-<br>
-<h1 align="center">SourceSage</h1>
-<h2 align="center">
-  ～Transforming code for AI～
-
-  <br>
-  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
-  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
-  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
-  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
-  <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
-
-  <br>
-
-</h2>
-
-
-</p>
-
-
-
-SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
-
-**このリポジトリ自体もSourceSageを活用しており、リリースノートやREADME、コミットメッセージの9割はSourceSage X クロードで生成しています。**
-
-
-## 更新内容
-
-- [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
-  - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
-  - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
-  - CLI引数の追加とコアモジュールの修正
-  - プロジェクトの構成とファイルの変更によるシンプル化
-  - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
-- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
-  - README.mdのセットアップ手順と実行手順を簡素化
-  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
-  - テスト実行方法のドキュメントを更新
-- [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
-  - コードの品質と保守性を向上させるためのリファクタリングと機能改善
-  - コミットメッセージのフォーマットとタイプの説明を追加
-  - コマンドラインからソースコードのリポジトリパスを取得するように修正
-  - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
-- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
-  - [IssueWise](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
-  - [CommitCraft](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
-  - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
-- [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
-  - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
-  - 言語ごとのシンタックスハイライト機能を追加
-  - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
-- 【2024/03/29】 初期リリース
-
-## 主な機能
-
-### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
-
-- GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
-- 課題を効率的に特定し、迅速に解決策を見つけられます
-
-### [CommitCraft（開発中のコミット管理）](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)
-- 変更差分を追跡し、AIが適切なコミットメッセージを自動生成
-- コミットの内容を正確に記述でき、変更履歴を明確に管理できます
-
-### [DocuMind（リリース後のドキュメント化）](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)
-- プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化 
-- プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
-
-## 使用方法
-
-### セットアップ
-
-SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
-
-```bash
-pip install sourcesage
-```
-
-これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
-
-### クイックスタート
-
-SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
-
-1. ターミナルまたはコマンドプロンプトを開きます。
-
-2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
-   ```bash 
-   cd ~/my_project
-   ```
-   
-   Note: `cd`コマンドは "change directory" の略で、現在のディレクトリを指定したディレクトリに変更するために使用します。
-
-3. 次に、以下のコマンドを実行してSourceSageを起動します：
-   ```bash
-   sourcesage
-   ```
-
-4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
-   - `DocuMind.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
-   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
-   - `ISSUES_RESOLVE` : Issuesとプロジェクト全体がマージされたファイルを保存するディレクトリです。これらのファイルは、AIがIssueを解決するための重要な情報源となります。
-   - `COMMIT_CRAFT` : 開発中のステージされたコードのファイルを保存するディレクトリです。これらのファイルは、AIが適切なコミットメッセージを生成するために使用されます。
-   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
-   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
-
-これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
-
-### リポジトリのIssueも取得する方法
-
-デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
-
-```bash 
-sourcesage --owner Sunwood-ai-labs --repository SourceSage
-```
-
-上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
-
-Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
-
-以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
-
-### 除外ファイルの指定
-
-作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
-
-```plaintext
-# .SourceSageignoreの例
-node_modules/
-*.log
-*.tmp
-```
-
-上記の例では、`node_modules`ディレクトリと、拡張子が`.log`または`.tmp`のファイルが除外されます。
-
-`.SourceSageignore`ファイルを使用する場合は、以下のようにコマンドライン引数で指定します：
-
-```bash 
-sourcesage --owner Sunwood-ai-labs --repository SourceSage --ignore-file .SourceSageignore
-```
-
-この機能を使用することで、不要なファイルやディレクトリを処理から除外し、より効率的にSourceSageを実行できます。
-
-## 1. IssueWise：開発前の課題解決
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
-</p>
-
-IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
-
-`SourceSageAssets/ISSUE_WISE/ISSUES_RESOLVE`に生成されるマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_ISSUE_11.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_ISSUE_11.md)
-
-このマークダウンファイルをそのままAIに入力することで、AIが課題を解決するためのコードを生成します。AIは、Issueの内容とプロジェクトの概要を組み合わせて分析し、適切な修正を提案します。
-
-このマークダウンファイルは、下記のファイルのフォーマットで出力されます。
-[`docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md)
-
-IssueWiseを使用することで、開発者は手作業でIssueを確認する負担を軽減し、AIによる自動修正の恩恵を受けることができます。
-
-## 2. CommitCraft：開発中のコミット管理
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon5.png" width="50%">
-</p>
-
-CommitCraftは、開発中のステージされた変更を追跡し、AIを活用して適切なコミットメッセージを自動生成するツールです。これにより、開発者はコミットの内容を正確に記述することができ、プロジェクトの変更履歴をより明確に管理できます。
-
-`SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
-
-このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
-
-Issueとマージされたファイルの例はこちらです。
-
-例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
-
-このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
-
-CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
-
-## 3. DocuMind：リリース後のドキュメント化
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
-</p>
-
-DocuMindは、リリース後のプロジェクトの統合とドキュメント化を支援するツールです。SourceSageが生成するプロジェクトの概要と、自動生成されたGitの変更履歴を組み合わせることで、プロジェクトの全体像を明確に把握できます。これにより、開発者はプロジェクトのドキュメントを効率的に作成し、メンテナンス性を向上させることができます。
-
-`SourceSageAssets/DocuMind.md`に生成されるマークダウンファイルを使用します。 
-
-例：[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_DocuMind.md)
-
-また、`SourceSageAssets/Changelog`に生成されるコミットメッセージのマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md)
-
-この2つのマークダウンファイルをそのままAIに入力することで、AIがプロジェクトの構造と変更内容を理解し、リリースノートやドキュメントを生成することができます。AIは、プロジェクトの概要とGitの変更履歴を分析し、プロジェクトの主要な機能や変更点を要約します。
-
-DocuMindを使用することで、開発者はドキュメント作成の負担を軽減し、常に最新の状態を反映したドキュメントを自動的に生成できます。
-
-## 貢献
-
-SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
-
-## ライセンス
-
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+Metadata-Version: 2.1
+Name: sourcesage
+Version: 4.1.4
+Home-page: https://github.com/Sunwood-ai-labs/SourceSage
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: loguru
+Requires-Dist: GitPython
+Requires-Dist: requests
+Requires-Dist: art
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
+<br>
+<h1 align="center">SourceSage</h1>
+<h2 align="center">
+  ～Transforming code for AI～
+
+  <br>
+  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
+  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
+  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
+  <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
+
+  <br>
+
+</h2>
+
+
+</p>
+
+
+
+SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
+
+**このリポジトリ自体もSourceSageを活用しており、リリースノートやREADME、コミットメッセージの9割はSourceSage X クロードで生成しています。**
+
+
+## 更新内容
+
+- [【2024/04/30】 SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/v4.1.2)
+  - GitHub ActionsによるPyPIへの自動パブリッシュ設定を追加し、リリースプロセスを自動化
+
+- [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
+  - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
+  - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
+  - CLI引数の追加とコアモジュールの修正
+  - プロジェクトの構成とファイルの変更によるシンプル化
+  - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
+- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
+  - README.mdのセットアップ手順と実行手順を簡素化
+  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
+  - テスト実行方法のドキュメントを更新
+- [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
+  - コードの品質と保守性を向上させるためのリファクタリングと機能改善
+  - コミットメッセージのフォーマットとタイプの説明を追加
+  - コマンドラインからソースコードのリポジトリパスを取得するように修正
+  - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
+- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
+  - [IssueWise](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
+  - [CommitCraft](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
+  - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
+- [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
+  - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
+  - 言語ごとのシンタックスハイライト機能を追加
+  - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
+- 【2024/03/29】 初期リリース
+
+## 主な機能
+
+### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
+
+- GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
+- 課題を効率的に特定し、迅速に解決策を見つけられます
+
+### [CommitCraft（開発中のコミット管理）](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)
+- 変更差分を追跡し、AIが適切なコミットメッセージを自動生成
+- コミットの内容を正確に記述でき、変更履歴を明確に管理できます
+
+### [DocuMind（リリース後のドキュメント化）](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)
+- プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化 
+- プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
+
+## 使用方法
+
+### セットアップ
+
+SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
+
+```bash
+pip install sourcesage
+```
+
+これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
+
+### クイックスタート
+
+SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
+
+1. ターミナルまたはコマンドプロンプトを開きます。
+
+2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
+   ```bash 
+   cd ~/my_project
+   ```
+   
+   Note: `cd`コマンドは "change directory" の略で、現在のディレクトリを指定したディレクトリに変更するために使用します。
+
+3. 次に、以下のコマンドを実行してSourceSageを起動します：
+   ```bash
+   sourcesage
+   ```
+
+4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
+   - `DocuMind.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
+   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
+   - `ISSUES_RESOLVE` : Issuesとプロジェクト全体がマージされたファイルを保存するディレクトリです。これらのファイルは、AIがIssueを解決するための重要な情報源となります。
+   - `COMMIT_CRAFT` : 開発中のステージされたコードのファイルを保存するディレクトリです。これらのファイルは、AIが適切なコミットメッセージを生成するために使用されます。
+   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
+   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
+
+これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
+
+### リポジトリのIssueも取得する方法
+
+デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
+
+```bash 
+sourcesage --owner Sunwood-ai-labs --repository SourceSage
+```
+
+上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
+
+Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
+
+以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
+
+### 除外ファイルの指定
+
+作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
+
+```plaintext
+# .SourceSageignoreの例
+node_modules/
+*.log
+*.tmp
+```
+
+上記の例では、`node_modules`ディレクトリと、拡張子が`.log`または`.tmp`のファイルが除外されます。
+
+`.SourceSageignore`ファイルを使用する場合は、以下のようにコマンドライン引数で指定します：
+
+```bash 
+sourcesage --owner Sunwood-ai-labs --repository SourceSage --ignore-file .SourceSageignore
+```
+
+この機能を使用することで、不要なファイルやディレクトリを処理から除外し、より効率的にSourceSageを実行できます。
+
+## 1. IssueWise：開発前の課題解決
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
+</p>
+
+IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
+
+`SourceSageAssets/ISSUE_WISE/ISSUES_RESOLVE`に生成されるマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_ISSUE_11.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_ISSUE_11.md)
+
+このマークダウンファイルをそのままAIに入力することで、AIが課題を解決するためのコードを生成します。AIは、Issueの内容とプロジェクトの概要を組み合わせて分析し、適切な修正を提案します。
+
+このマークダウンファイルは、下記のファイルのフォーマットで出力されます。
+[`docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md)
+
+IssueWiseを使用することで、開発者は手作業でIssueを確認する負担を軽減し、AIによる自動修正の恩恵を受けることができます。
+
+## 2. CommitCraft：開発中のコミット管理
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon5.png" width="50%">
+</p>
+
+CommitCraftは、開発中のステージされた変更を追跡し、AIを活用して適切なコミットメッセージを自動生成するツールです。これにより、開発者はコミットの内容を正確に記述することができ、プロジェクトの変更履歴をより明確に管理できます。
+
+`SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
+
+このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
+
+Issueとマージされたファイルの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
+
+このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
+
+CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
+
+## 3. DocuMind：リリース後のドキュメント化
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
+</p>
+
+DocuMindは、リリース後のプロジェクトの統合とドキュメント化を支援するツールです。SourceSageが生成するプロジェクトの概要と、自動生成されたGitの変更履歴を組み合わせることで、プロジェクトの全体像を明確に把握できます。これにより、開発者はプロジェクトのドキュメントを効率的に作成し、メンテナンス性を向上させることができます。
+
+`SourceSageAssets/DocuMind.md`に生成されるマークダウンファイルを使用します。 
+
+例：[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_DocuMind.md)
+
+また、`SourceSageAssets/Changelog`に生成されるコミットメッセージのマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md)
+
+この2つのマークダウンファイルをそのままAIに入力することで、AIがプロジェクトの構造と変更内容を理解し、リリースノートやドキュメントを生成することができます。AIは、プロジェクトの概要とGitの変更履歴を分析し、プロジェクトの主要な機能や変更点を要約します。
+
+DocuMindを使用することで、開発者はドキュメント作成の負担を軽減し、常に最新の状態を反映したドキュメントを自動的に生成できます。
+
+## 貢献
+
+SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
+
+## ライセンス
+
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

#### html2text {}

```diff
@@ -1,25 +1,28 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.1.2 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.1.4 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
                        _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 **ãã®ãªãã¸ããªèªä½ãSourceSageãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯SourceSage
-X ã¯ã­ã¼ãã§çæãã¦ãã¾ãã** ## æ´æ°åå®¹ - [ã2024/04/07ã
-SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/
-undefined4.1.1) -
+X ã¯ã­ã¼ãã§çæãã¦ãã¾ãã** ## æ´æ°åå®¹ - [ã2024/04/30ã
+SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/
+v4.1.2) - GitHub
+Actionsã«ããPyPIã¸ã®èªåãããªãã·ã¥è¨­å®ãè¿½å ãããªãªã¼ã¹ãã­ã»ã¹ãèªåå
+- [ã2024/04/07ã SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/
+SourceSage/releases/tag/undefined4.1.1) -
 ãã­ã¸ã§ã¯ãå¨ä½ã®åºåãã¡ã¤ã«åã¨åã¢ã¸ã¥ã¼ã«ã®åºåãã©ã«ãåãå¤æ´
 -
 PyPIã®ãã¦ã³ã­ã¼ãããã¸ã¨Codacyã®ã¯ãªãªãã£ããã¸ãè¿½å 
 - CLIå¼æ°ã®è¿½å ã¨ã³ã¢ã¢ã¸ã¥ã¼ã«ã®ä¿®æ­£ -
 ãã­ã¸ã§ã¯ãã®æ§æã¨ãã¡ã¤ã«ã®å¤æ´ã«ããã·ã³ãã«å -
 ã»ããã¢ããæé ãå®è¡æ¹æ³ãã¯ã¤ãã¯ã¹ã¿ã¼ãã»ã¯ã·ã§ã³ããã¹ããã­ã¥ã¡ã³ãã®æ´æ°
 - [ã2024/04/05ã SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/
```

### Comparing `sourcesage-4.1.2/README.md` & `sourcesage-4.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,215 +1,218 @@
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
-<br>
-<h1 align="center">SourceSage</h1>
-<h2 align="center">
-  ～Transforming code for AI～
-
-  <br>
-  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
-  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
-  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
-  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
-  <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
-
-  <br>
-
-</h2>
-
-
-</p>
-
-
-
-SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
-
-**このリポジトリ自体もSourceSageを活用しており、リリースノートやREADME、コミットメッセージの9割はSourceSage X クロードで生成しています。**
-
-
-## 更新内容
-
-- [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
-  - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
-  - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
-  - CLI引数の追加とコアモジュールの修正
-  - プロジェクトの構成とファイルの変更によるシンプル化
-  - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
-- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
-  - README.mdのセットアップ手順と実行手順を簡素化
-  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
-  - テスト実行方法のドキュメントを更新
-- [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
-  - コードの品質と保守性を向上させるためのリファクタリングと機能改善
-  - コミットメッセージのフォーマットとタイプの説明を追加
-  - コマンドラインからソースコードのリポジトリパスを取得するように修正
-  - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
-- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
-  - [IssueWise](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
-  - [CommitCraft](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
-  - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
-- [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
-  - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
-  - 言語ごとのシンタックスハイライト機能を追加
-  - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
-- 【2024/03/29】 初期リリース
-
-## 主な機能
-
-### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
-
-- GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
-- 課題を効率的に特定し、迅速に解決策を見つけられます
-
-### [CommitCraft（開発中のコミット管理）](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)
-- 変更差分を追跡し、AIが適切なコミットメッセージを自動生成
-- コミットの内容を正確に記述でき、変更履歴を明確に管理できます
-
-### [DocuMind（リリース後のドキュメント化）](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)
-- プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化 
-- プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
-
-## 使用方法
-
-### セットアップ
-
-SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
-
-```bash
-pip install sourcesage
-```
-
-これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
-
-### クイックスタート
-
-SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
-
-1. ターミナルまたはコマンドプロンプトを開きます。
-
-2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
-   ```bash 
-   cd ~/my_project
-   ```
-   
-   Note: `cd`コマンドは "change directory" の略で、現在のディレクトリを指定したディレクトリに変更するために使用します。
-
-3. 次に、以下のコマンドを実行してSourceSageを起動します：
-   ```bash
-   sourcesage
-   ```
-
-4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
-   - `DocuMind.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
-   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
-   - `ISSUES_RESOLVE` : Issuesとプロジェクト全体がマージされたファイルを保存するディレクトリです。これらのファイルは、AIがIssueを解決するための重要な情報源となります。
-   - `COMMIT_CRAFT` : 開発中のステージされたコードのファイルを保存するディレクトリです。これらのファイルは、AIが適切なコミットメッセージを生成するために使用されます。
-   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
-   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
-
-これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
-
-### リポジトリのIssueも取得する方法
-
-デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
-
-```bash 
-sourcesage --owner Sunwood-ai-labs --repository SourceSage
-```
-
-上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
-
-Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
-
-以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
-
-### 除外ファイルの指定
-
-作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
-
-```plaintext
-# .SourceSageignoreの例
-node_modules/
-*.log
-*.tmp
-```
-
-上記の例では、`node_modules`ディレクトリと、拡張子が`.log`または`.tmp`のファイルが除外されます。
-
-`.SourceSageignore`ファイルを使用する場合は、以下のようにコマンドライン引数で指定します：
-
-```bash 
-sourcesage --owner Sunwood-ai-labs --repository SourceSage --ignore-file .SourceSageignore
-```
-
-この機能を使用することで、不要なファイルやディレクトリを処理から除外し、より効率的にSourceSageを実行できます。
-
-## 1. IssueWise：開発前の課題解決
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
-</p>
-
-IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
-
-`SourceSageAssets/ISSUE_WISE/ISSUES_RESOLVE`に生成されるマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_ISSUE_11.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_ISSUE_11.md)
-
-このマークダウンファイルをそのままAIに入力することで、AIが課題を解決するためのコードを生成します。AIは、Issueの内容とプロジェクトの概要を組み合わせて分析し、適切な修正を提案します。
-
-このマークダウンファイルは、下記のファイルのフォーマットで出力されます。
-[`docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md)
-
-IssueWiseを使用することで、開発者は手作業でIssueを確認する負担を軽減し、AIによる自動修正の恩恵を受けることができます。
-
-## 2. CommitCraft：開発中のコミット管理
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon5.png" width="50%">
-</p>
-
-CommitCraftは、開発中のステージされた変更を追跡し、AIを活用して適切なコミットメッセージを自動生成するツールです。これにより、開発者はコミットの内容を正確に記述することができ、プロジェクトの変更履歴をより明確に管理できます。
-
-`SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
-
-このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
-
-Issueとマージされたファイルの例はこちらです。
-
-例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
-
-このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
-
-CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
-
-## 3. DocuMind：リリース後のドキュメント化
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
-</p>
-
-DocuMindは、リリース後のプロジェクトの統合とドキュメント化を支援するツールです。SourceSageが生成するプロジェクトの概要と、自動生成されたGitの変更履歴を組み合わせることで、プロジェクトの全体像を明確に把握できます。これにより、開発者はプロジェクトのドキュメントを効率的に作成し、メンテナンス性を向上させることができます。
-
-`SourceSageAssets/DocuMind.md`に生成されるマークダウンファイルを使用します。 
-
-例：[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_DocuMind.md)
-
-また、`SourceSageAssets/Changelog`に生成されるコミットメッセージのマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md)
-
-この2つのマークダウンファイルをそのままAIに入力することで、AIがプロジェクトの構造と変更内容を理解し、リリースノートやドキュメントを生成することができます。AIは、プロジェクトの概要とGitの変更履歴を分析し、プロジェクトの主要な機能や変更点を要約します。
-
-DocuMindを使用することで、開発者はドキュメント作成の負担を軽減し、常に最新の状態を反映したドキュメントを自動的に生成できます。
-
-## 貢献
-
-SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
-
-## ライセンス
-
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
+<br>
+<h1 align="center">SourceSage</h1>
+<h2 align="center">
+  ～Transforming code for AI～
+
+  <br>
+  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
+  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
+  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
+  <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
+
+  <br>
+
+</h2>
+
+
+</p>
+
+
+
+SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
+
+**このリポジトリ自体もSourceSageを活用しており、リリースノートやREADME、コミットメッセージの9割はSourceSage X クロードで生成しています。**
+
+
+## 更新内容
+
+- [【2024/04/30】 SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/v4.1.2)
+  - GitHub ActionsによるPyPIへの自動パブリッシュ設定を追加し、リリースプロセスを自動化
+
+- [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
+  - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
+  - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
+  - CLI引数の追加とコアモジュールの修正
+  - プロジェクトの構成とファイルの変更によるシンプル化
+  - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
+- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
+  - README.mdのセットアップ手順と実行手順を簡素化
+  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
+  - テスト実行方法のドキュメントを更新
+- [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
+  - コードの品質と保守性を向上させるためのリファクタリングと機能改善
+  - コミットメッセージのフォーマットとタイプの説明を追加
+  - コマンドラインからソースコードのリポジトリパスを取得するように修正
+  - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
+- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
+  - [IssueWise](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
+  - [CommitCraft](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
+  - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
+- [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
+  - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
+  - 言語ごとのシンタックスハイライト機能を追加
+  - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
+- 【2024/03/29】 初期リリース
+
+## 主な機能
+
+### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
+
+- GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
+- 課題を効率的に特定し、迅速に解決策を見つけられます
+
+### [CommitCraft（開発中のコミット管理）](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)
+- 変更差分を追跡し、AIが適切なコミットメッセージを自動生成
+- コミットの内容を正確に記述でき、変更履歴を明確に管理できます
+
+### [DocuMind（リリース後のドキュメント化）](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)
+- プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化 
+- プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
+
+## 使用方法
+
+### セットアップ
+
+SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
+
+```bash
+pip install sourcesage
+```
+
+これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
+
+### クイックスタート
+
+SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
+
+1. ターミナルまたはコマンドプロンプトを開きます。
+
+2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
+   ```bash 
+   cd ~/my_project
+   ```
+   
+   Note: `cd`コマンドは "change directory" の略で、現在のディレクトリを指定したディレクトリに変更するために使用します。
+
+3. 次に、以下のコマンドを実行してSourceSageを起動します：
+   ```bash
+   sourcesage
+   ```
+
+4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
+   - `DocuMind.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
+   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
+   - `ISSUES_RESOLVE` : Issuesとプロジェクト全体がマージされたファイルを保存するディレクトリです。これらのファイルは、AIがIssueを解決するための重要な情報源となります。
+   - `COMMIT_CRAFT` : 開発中のステージされたコードのファイルを保存するディレクトリです。これらのファイルは、AIが適切なコミットメッセージを生成するために使用されます。
+   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
+   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
+
+これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
+
+### リポジトリのIssueも取得する方法
+
+デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
+
+```bash 
+sourcesage --owner Sunwood-ai-labs --repository SourceSage
+```
+
+上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
+
+Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
+
+以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
+
+### 除外ファイルの指定
+
+作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
+
+```plaintext
+# .SourceSageignoreの例
+node_modules/
+*.log
+*.tmp
+```
+
+上記の例では、`node_modules`ディレクトリと、拡張子が`.log`または`.tmp`のファイルが除外されます。
+
+`.SourceSageignore`ファイルを使用する場合は、以下のようにコマンドライン引数で指定します：
+
+```bash 
+sourcesage --owner Sunwood-ai-labs --repository SourceSage --ignore-file .SourceSageignore
+```
+
+この機能を使用することで、不要なファイルやディレクトリを処理から除外し、より効率的にSourceSageを実行できます。
+
+## 1. IssueWise：開発前の課題解決
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
+</p>
+
+IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
+
+`SourceSageAssets/ISSUE_WISE/ISSUES_RESOLVE`に生成されるマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_ISSUE_11.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_ISSUE_11.md)
+
+このマークダウンファイルをそのままAIに入力することで、AIが課題を解決するためのコードを生成します。AIは、Issueの内容とプロジェクトの概要を組み合わせて分析し、適切な修正を提案します。
+
+このマークダウンファイルは、下記のファイルのフォーマットで出力されます。
+[`docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md)
+
+IssueWiseを使用することで、開発者は手作業でIssueを確認する負担を軽減し、AIによる自動修正の恩恵を受けることができます。
+
+## 2. CommitCraft：開発中のコミット管理
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon5.png" width="50%">
+</p>
+
+CommitCraftは、開発中のステージされた変更を追跡し、AIを活用して適切なコミットメッセージを自動生成するツールです。これにより、開発者はコミットの内容を正確に記述することができ、プロジェクトの変更履歴をより明確に管理できます。
+
+`SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
+
+このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
+
+Issueとマージされたファイルの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
+
+このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
+
+CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
+
+## 3. DocuMind：リリース後のドキュメント化
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
+</p>
+
+DocuMindは、リリース後のプロジェクトの統合とドキュメント化を支援するツールです。SourceSageが生成するプロジェクトの概要と、自動生成されたGitの変更履歴を組み合わせることで、プロジェクトの全体像を明確に把握できます。これにより、開発者はプロジェクトのドキュメントを効率的に作成し、メンテナンス性を向上させることができます。
+
+`SourceSageAssets/DocuMind.md`に生成されるマークダウンファイルを使用します。 
+
+例：[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_DocuMind.md)
+
+また、`SourceSageAssets/Changelog`に生成されるコミットメッセージのマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md)
+
+この2つのマークダウンファイルをそのままAIに入力することで、AIがプロジェクトの構造と変更内容を理解し、リリースノートやドキュメントを生成することができます。AIは、プロジェクトの概要とGitの変更履歴を分析し、プロジェクトの主要な機能や変更点を要約します。
+
+DocuMindを使用することで、開発者はドキュメント作成の負担を軽減し、常に最新の状態を反映したドキュメントを自動的に生成できます。
+
+## 貢献
+
+SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
+
+## ライセンス
+
 このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

#### html2text {}

```diff
@@ -4,17 +4,20 @@
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
                        _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 **ãã®ãªãã¸ããªèªä½ãSourceSageãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯SourceSage
-X ã¯ã­ã¼ãã§çæãã¦ãã¾ãã** ## æ´æ°åå®¹ - [ã2024/04/07ã
-SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/
-undefined4.1.1) -
+X ã¯ã­ã¼ãã§çæãã¦ãã¾ãã** ## æ´æ°åå®¹ - [ã2024/04/30ã
+SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/
+v4.1.2) - GitHub
+Actionsã«ããPyPIã¸ã®èªåãããªãã·ã¥è¨­å®ãè¿½å ãããªãªã¼ã¹ãã­ã»ã¹ãèªåå
+- [ã2024/04/07ã SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/
+SourceSage/releases/tag/undefined4.1.1) -
 ãã­ã¸ã§ã¯ãå¨ä½ã®åºåãã¡ã¤ã«åã¨åã¢ã¸ã¥ã¼ã«ã®åºåãã©ã«ãåãå¤æ´
 -
 PyPIã®ãã¦ã³ã­ã¼ãããã¸ã¨Codacyã®ã¯ãªãªãã£ããã¸ãè¿½å 
 - CLIå¼æ°ã®è¿½å ã¨ã³ã¢ã¢ã¸ã¥ã¼ã«ã®ä¿®æ­£ -
 ãã­ã¸ã§ã¯ãã®æ§æã¨ãã¡ã¤ã«ã®å¤æ´ã«ããã·ã³ãã«å -
 ã»ããã¢ããæé ãå®è¡æ¹æ³ãã¯ã¤ãã¯ã¹ã¿ã¼ãã»ã¯ã·ã§ã³ããã¹ããã­ã¥ã¡ã³ãã®æ´æ°
 - [ã2024/04/05ã SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/
```

### Comparing `sourcesage-4.1.2/sourcesage/cli.py` & `sourcesage-4.1.4/sourcesage/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,48 @@
-import argparse
-from .core import SourceSage
-import os
-
-def main():
-    parser = argparse.ArgumentParser(description='SourceSage CLI')
-    parser.add_argument('--config', help='Path to the configuration file', default='sourcesage.yml')
-    parser.add_argument('--output', help='Output directory for generated files', default='./')
-    parser.add_argument('--repo', help='Path to the repository', default='./')
-    parser.add_argument('--owner', help='Owner of the repository', default='Sunwood-ai-labs')  # デフォルト値を設定
-    parser.add_argument('--repository', help='Name of the repository', default='SourceSage')  # デフォルト値を設定
-
-    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-    default_ignore_file = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
-    default_language_map = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
-
-    parser.add_argument('--ignore-file', help='Path to the ignore file', default=default_ignore_file)  # 修正
-    parser.add_argument('--language-map', help='Path to the language map file', default=default_language_map)  # 修正
-    
-    args = parser.parse_args()
-
-    sourcesage = SourceSage(args.config, args.output, args.repo, args.owner, args.repository, args.ignore_file, args.language_map)
-    sourcesage.run()
-
-if __name__ == '__main__':
+import argparse
+from .core import SourceSage
+import os
+from loguru import logger
+import sys
+# logger.add(sink=sys.stderr, format="{time:YYYY-MM-DD HH:mm:ss.SSS} | {level:<8} | {name}:{line} | {message}")
+
+# ログ出力のフォーマットを指定
+logger.configure(
+    handlers=[
+        {
+            "sink": sys.stderr,
+            "format": "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level:<6}</level> | <cyan>{name:<45}:{line:<5}</cyan> | <level>{message}</level>",
+            "colorize": True,
+        }
+    ]
+)
+
+def main():
+    parser = argparse.ArgumentParser(description='SourceSage CLI')
+    parser.add_argument('--config', help='Path to the configuration file', default='sourcesage.yml')
+    parser.add_argument('--output', help='Output directory for generated files', default='./')
+    parser.add_argument('--repo', help='Path to the repository', default='./')
+    parser.add_argument('--owner', help='Owner of the repository', default='Sunwood-ai-labs')  # デフォルト値を設定
+    parser.add_argument('--repository', help='Name of the repository', default='SourceSage')  # デフォルト値を設定
+
+    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+    default_ignore_file = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')
+    default_language_map = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')
+
+    current_dir_ignore_file = os.path.join(os.getcwd(), '.SourceSageignore')
+    if os.path.exists(current_dir_ignore_file):
+        ignore_file = current_dir_ignore_file
+        logger.info(f"Using ignore file from current directory: {ignore_file}")
+    else:
+        ignore_file = default_ignore_file
+        logger.info(f"Using default ignore file: {ignore_file}")
+
+    parser.add_argument('--ignore-file', help='Path to the ignore file', default=ignore_file)
+    parser.add_argument('--language-map', help='Path to the language map file', default=default_language_map)
+    
+    args = parser.parse_args()
+
+    sourcesage = SourceSage(args.config, args.output, args.repo, args.owner, args.repository, args.ignore_file, args.language_map)
+    sourcesage.run()
+
+if __name__ == '__main__':
     main()
```

### Comparing `sourcesage-4.1.2/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md` & `sourcesage-4.1.4/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-
-
-下記はgitはStageの情報です
-
-issueは掲載しないで
-
-見やすくコミットメッセージにして
-章やパラグラフ、箇条書きを多用して見やすくして
-
-コミットメッセージは日本語にして
-正確にstep-by-stepで処理して
-
-下記のマークダウンフォーマットで出力して
-
-## フォーマット
-
-```markdown
-
-[種類] 概要
-
-詳細な説明（必要に応じて）
-
-```
-
-## 種類
-
-種類は下記を参考にして
-
-例：
-  - feat: 新機能
-  - fix: バグ修正
-  - docs: ドキュメントのみの変更
-  - style: コードの動作に影響しない変更（空白、フォーマット、セミコロンの欠落など） 
-  - refactor: バグの修正も機能の追加も行わないコードの変更
-  - perf: パフォーマンスを向上させるコードの変更
-  - test: 欠けているテストの追加や既存のテストの修正
-  - chore: ビルドプロセスやドキュメント生成などの補助ツールやライブラリの変更
-
-
-## Stageの情報
-
-```markdown
-[STAGED_DIFF.md]
-
+
+
+下記はgitはStageの情報です
+
+issueは掲載しないで
+
+見やすくコミットメッセージにして
+章やパラグラフ、箇条書きを多用して見やすくして
+
+コミットメッセージは日本語にして
+正確にstep-by-stepで処理して
+
+下記のマークダウンフォーマットで出力して
+
+## フォーマット
+
+```markdown
+
+[種類] 概要
+
+詳細な説明（必要に応じて）
+
+```
+
+## 種類
+
+種類は下記を参考にして
+
+例：
+  - feat: 新機能
+  - fix: バグ修正
+  - docs: ドキュメントのみの変更
+  - style: コードの動作に影響しない変更（空白、フォーマット、セミコロンの欠落など） 
+  - refactor: バグの修正も機能の追加も行わないコードの変更
+  - perf: パフォーマンスを向上させるコードの変更
+  - test: 欠けているテストの追加や既存のテストの修正
+  - chore: ビルドプロセスやドキュメント生成などの補助ツールやライブラリの変更
+
+
+## Stageの情報
+
+```markdown
+[STAGED_DIFF.md]
+
 ```
```

### Comparing `sourcesage-4.1.2/sourcesage/config/constants.py` & `sourcesage-4.1.4/sourcesage/config/constants.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import os
-
-class Constants:
-    def __init__(self, output_dir, owner, repository):
-        self.OWNER = owner
-        self.REPOSITORY = repository
-        self.ISSUES_FILE_NAME = "open_issues_filtered.json"
-
-        self.BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-        self.REPO_PATH = self.BASE_DIR
-        self.CONFIG_DIR = os.path.join(self.BASE_DIR, 'config')
-        self.DOCS_DIR = os.path.join(self.BASE_DIR, "config")
-
-        self.LANGUAGE_MAP_FILE = os.path.join(self.CONFIG_DIR, 'language_map.json')
-        self.IGNORE_FILE = os.path.join(self.CONFIG_DIR, '.SourceSageignore')
-
-        self.SOURCE_SAGE_MD = "DocuMind.md"
-        self.CHANGELOG_DIR = "Changelog"
-        self.STAGED_DIFF_MD = "STAGED_DIFF.md"
-
-        self.set_output_dir(output_dir)
-
-    def set_output_dir(self, output_dir):
-        self.SOURCE_SAGE_ASSETS_DIR = os.path.join(output_dir, "SourceSageAssets")
-        self.ISSUE_LOG_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_LOG")
-        self.ISSUES_RESOLVE_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_WISE/ISSUES_RESOLVE")
-        self.STAGE_INFO_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "COMMIT_CRAFT/STAGE_INFO")
-
-        self.TEMPLATE_ISSUES_RESOLVE_DIR = os.path.join(self.DOCS_DIR, "ISSUES_RESOLVE")
-        self.ISSUES_RESOLVE_TEMPLATE_MD = "ISSUES_RESOLVE_TEMPLATE.md"
-
-        self.TEMPLATE_STAGE_INFO_DIR = os.path.join(self.DOCS_DIR, "STAGE_INFO")
-        self.STAGE_INFO_OUTPUT_MD = "STAGE_INFO_AND_ISSUES_AND_PROMT.md"
-        self.STAGE_INFO_TEMPLATE_MD = "STAGE_INFO_AND_ISSUES_TEMPLATE.md"
-
-        self.STAGE_INFO_SIMPLE_OUTPUT_MD = "STAGE_INFO_AND_PROMT.md"
+import os
+
+class Constants:
+    def __init__(self, output_dir, owner, repository):
+        self.OWNER = owner
+        self.REPOSITORY = repository
+        self.ISSUES_FILE_NAME = "open_issues_filtered.json"
+
+        self.BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+        self.REPO_PATH = self.BASE_DIR
+        self.CONFIG_DIR = os.path.join(self.BASE_DIR, 'config')
+        self.DOCS_DIR = os.path.join(self.BASE_DIR, "config")
+
+        self.LANGUAGE_MAP_FILE = os.path.join(self.CONFIG_DIR, 'language_map.json')
+        self.IGNORE_FILE = os.path.join(self.CONFIG_DIR, '.SourceSageignore')
+
+        self.SOURCE_SAGE_MD = "DocuMind.md"
+        self.CHANGELOG_DIR = "Changelog"
+        self.STAGED_DIFF_MD = "STAGED_DIFF.md"
+
+        self.set_output_dir(output_dir)
+
+    def set_output_dir(self, output_dir):
+        self.SOURCE_SAGE_ASSETS_DIR = os.path.join(output_dir, "SourceSageAssets")
+        self.ISSUE_LOG_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_LOG")
+        self.ISSUES_RESOLVE_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_WISE/ISSUES_RESOLVE")
+        self.STAGE_INFO_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "COMMIT_CRAFT/STAGE_INFO")
+
+        self.TEMPLATE_ISSUES_RESOLVE_DIR = os.path.join(self.DOCS_DIR, "ISSUES_RESOLVE")
+        self.ISSUES_RESOLVE_TEMPLATE_MD = "ISSUES_RESOLVE_TEMPLATE.md"
+
+        self.TEMPLATE_STAGE_INFO_DIR = os.path.join(self.DOCS_DIR, "STAGE_INFO")
+        self.STAGE_INFO_OUTPUT_MD = "STAGE_INFO_AND_ISSUES_AND_PROMT.md"
+        self.STAGE_INFO_TEMPLATE_MD = "STAGE_INFO_AND_ISSUES_TEMPLATE.md"
+
+        self.STAGE_INFO_SIMPLE_OUTPUT_MD = "STAGE_INFO_AND_PROMT.md"
         self.STAGE_INFO_SIMPLE_TEMPLATE_MD = "STAGE_INFO_TEMPLATE.md"
```

### Comparing `sourcesage-4.1.2/sourcesage/core.py` & `sourcesage-4.1.4/sourcesage/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,85 @@
-import os
-from .modules.EnvFileHandler import create_or_append_env_file
-from .modules.source_sage import SourceSage as SourceSageModule
-from .modules.ChangelogGenerator import ChangelogGenerator
-from .modules.StageInfoGenerator import StageInfoGenerator
-from .modules.GitHubIssueRetrieve import GitHubIssueRetriever
-from .modules.StagedDiffGenerator import StagedDiffGenerator
-from .modules.IssuesToMarkdown import IssuesToMarkdown
-
-from .config.constants import Constants
-
-from art import *
-
-class SourceSage:
-    def __init__(self, config_path, output_dir, repo_path, owner, repository, ignore_file, language_map_file):
-        self.config_path = config_path
-        self.output_dir = output_dir
-        self.repo_path = repo_path
-        self.ignore_file = ignore_file
-        self.language_map_file = language_map_file
-
-        self.constants = Constants(output_dir, owner, repository) 
-
-    def run(self):
-        tprint("SourceSage", font="rnd-medium")
-        print("Running SourceSage...")
-        
-        # Load configuration
-        config = self.load_config()
-
-        # Create necessary directories
-        os.makedirs(self.constants.ISSUE_LOG_DIR, exist_ok=True)
-        os.makedirs(self.constants.ISSUES_RESOLVE_DIR, exist_ok=True)
-        os.makedirs(self.constants.STAGE_INFO_DIR, exist_ok=True)
-        
-        # Generate SourceSage markdown
-        sourcesage_module = SourceSageModule(folders=[self.repo_path], ignore_file=self.ignore_file,
-                                             output_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
-                                             language_map_file=self.language_map_file)
-        sourcesage_module.generate_markdown()
-
-        # Generate changelog
-        changelog_generator = ChangelogGenerator(self.repo_path, os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.CHANGELOG_DIR))
-        changelog_generator.generate_changelog_for_all_branches()
-        changelog_generator.integrate_changelogs()
-
-        # Retrieve GitHub issues
-        issue_retriever = GitHubIssueRetriever(self.constants.OWNER, self.constants.REPOSITORY, self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME)
-        issue_retriever.run()
-
-        # Generate staged diff
-        diff_generator = StagedDiffGenerator(repo_path=self.repo_path, output_dir=self.constants.SOURCE_SAGE_ASSETS_DIR,
-                                             language_map_file=self.language_map_file)
-        diff_generator.run()
-
-        # Generate stage info and issues
-        stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
-                                                  stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
-                                                  template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_TEMPLATE_MD),
-                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_OUTPUT_MD))
-        stage_info_generator.run()
-
-        # Generate stage info
-        stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
-                                                  stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
-                                                  template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD),
-                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD))
-        stage_info_generator.run()
-
-        # Convert issues to markdown
-        issues_to_markdown = IssuesToMarkdown(issues_file=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
-                                              sourcesage_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
-                                              template_file=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_ISSUES_RESOLVE_DIR, self.constants.ISSUES_RESOLVE_TEMPLATE_MD),
-                                              output_folder=self.constants.ISSUES_RESOLVE_DIR)
-        issues_to_markdown.load_data()
-        issues_to_markdown.create_markdown_files()
-
-        print("SourceSage completed successfully.")
-
-    def load_config(self):
-        # Load configuration from YAML file
-        # Implement this method based on your configuration file structure
+import os
+from .modules.EnvFileHandler import create_or_append_env_file
+from .modules.source_sage import SourceSage as SourceSageModule
+from .modules.ChangelogGenerator import ChangelogGenerator
+from .modules.StageInfoGenerator import StageInfoGenerator
+from .modules.GitHubIssueRetrieve import GitHubIssueRetriever
+from .modules.StagedDiffGenerator import StagedDiffGenerator
+from .modules.IssuesToMarkdown import IssuesToMarkdown
+
+from .config.constants import Constants
+
+from art import *
+
+from loguru import logger
+
+class SourceSage:
+    def __init__(self, config_path, output_dir, repo_path, owner, repository, ignore_file, language_map_file):
+        self.config_path = config_path
+        self.output_dir = output_dir
+        self.repo_path = repo_path
+        self.ignore_file = ignore_file
+        self.language_map_file = language_map_file
+
+        self.constants = Constants(output_dir, owner, repository) 
+
+    def run(self):
+        tprint("SourceSage", font="rnd-xlarge")
+        logger.info("Running SourceSage...")
+        
+        # Load configuration
+        config = self.load_config()
+
+        # Create necessary directories
+        os.makedirs(self.constants.ISSUE_LOG_DIR, exist_ok=True)
+        os.makedirs(self.constants.ISSUES_RESOLVE_DIR, exist_ok=True)
+        os.makedirs(self.constants.STAGE_INFO_DIR, exist_ok=True)
+        
+        # Generate SourceSage markdown
+        sourcesage_module = SourceSageModule(folders=[self.repo_path], ignore_file=self.ignore_file,
+                                             output_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
+                                             language_map_file=self.language_map_file)
+        sourcesage_module.generate_markdown()
+
+        # Generate changelog
+        changelog_generator = ChangelogGenerator(self.repo_path, os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.CHANGELOG_DIR))
+        changelog_generator.generate_changelog_for_all_branches()
+        changelog_generator.integrate_changelogs()
+
+        # Retrieve GitHub issues
+        issue_retriever = GitHubIssueRetriever(self.constants.OWNER, self.constants.REPOSITORY, self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME)
+        issue_retriever.run()
+
+        # Generate staged diff
+        diff_generator = StagedDiffGenerator(repo_path=self.repo_path, output_dir=self.constants.SOURCE_SAGE_ASSETS_DIR,
+                                             language_map_file=self.language_map_file)
+        diff_generator.run()
+
+        # Generate stage info and issues
+        stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
+                                                  stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
+                                                  template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_TEMPLATE_MD),
+                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_OUTPUT_MD))
+        stage_info_generator.run()
+
+        # Generate stage info
+        stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
+                                                  stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
+                                                  template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD),
+                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD))
+        stage_info_generator.run()
+
+        # Convert issues to markdown
+        issues_to_markdown = IssuesToMarkdown(issues_file=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
+                                              sourcesage_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
+                                              template_file=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_ISSUES_RESOLVE_DIR, self.constants.ISSUES_RESOLVE_TEMPLATE_MD),
+                                              output_folder=self.constants.ISSUES_RESOLVE_DIR)
+        issues_to_markdown.load_data()
+        issues_to_markdown.create_markdown_files()
+
+        logger.info("SourceSage completed successfully.")
+        tprint("!! successfully !!", font="rnd-medium")
+    def load_config(self):
+        # Load configuration from YAML file
+        # Implement this method based on your configuration file structure
         pass
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.1.4/sourcesage/modules/ChangelogGenerator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,103 @@
-# modules/ChangelogGenerator.py (変更後)
-
-import os
-from git import Repo
-from .ChangelogUtils import ChangelogUtils
-from loguru import logger
-
-class ChangelogGenerator:
-    def __init__(self, repo_path, output_dir):
-        self.repo_path = repo_path
-        self.output_dir = output_dir
-        self.repo = self._get_repo()
-
-    def _get_repo(self):
-        return Repo(self.repo_path)
-
-    def _get_commits(self, branch):
-        return list(self.repo.iter_commits(branch))
-
-    def generate_changelog(self, branch, output_file):
-        commits = self._get_commits(branch)
-
-        # 出力ファイルのディレクトリを確認し、存在しない場合は作成
-        os.makedirs(os.path.dirname(output_file), exist_ok=True)
-
-        with open(output_file, 'w', encoding='utf-8') as f:
-            f.write(f"# Changelog\n\n")
-            f.write(f"## {branch}\n\n")
-
-            for commit in commits:
-                formatted_commit = ChangelogUtils.format_commit(commit)
-                f.write(formatted_commit + "\n")
-
-        logger.info(f"Changelog generated successfully for branch '{branch}' at {output_file}")
-
-    def generate_changelog_for_all_branches(self):
-        local_branches = [ref.name for ref in self.repo.branches]
-        remote_branches = [ref.name for ref in self.repo.remote().refs]
-
-        branches = local_branches + remote_branches
-        print(branches)
-
-        feature_branches = [branch for branch in branches if 'feature/' in branch]
-        other_branches = [branch for branch in branches if 'feature/' not in branch]
-
-        for branch in other_branches:
-            branch_name = branch.replace('origin/', '')
-            output_file = os.path.join(self.output_dir, f"CHANGELOG_{branch_name}.md").replace("release/", "release_").replace("bugfix/", "bugfix_")
-            logger.info(f"Generating changelog for branch '{branch_name}'...")
-            self.generate_changelog(branch_name, output_file)
-
-        if feature_branches:
-            output_file = os.path.join(self.output_dir, "CHANGELOG_features.md")
-            with open(output_file, 'w', encoding='utf-8') as f:
-                f.write(f"# Changelog - Features\n\n")
-                for branch in feature_branches:
-                    branch_name = branch.replace('origin/', '')
-                    f.write(f"## {branch_name}\n\n")
-                    commits = self._get_commits(branch)
-                    for commit in commits:
-                        formatted_commit = ChangelogUtils.format_commit(commit)
-                        f.write(formatted_commit + "\n")
-                    f.write("\n")
-            logger.info(f"Changelog generated successfully for feature branches at {output_file}")
-
-    def integrate_changelogs(self):
-        changelog_files = [file for file in os.listdir(self.output_dir) if file.startswith("CHANGELOG_")]
-        integrated_changelog = "# Integrated Changelog\n\n"
-
-        for file in changelog_files:
-            with open(os.path.join(self.output_dir, file), 'r', encoding='utf-8') as f:
-                content = f.read()
-                integrated_changelog += f"{content}\n\n"
-
-        output_file = os.path.join(self.output_dir, "CHANGELOG_integrated.md")
-        with open(output_file, 'w', encoding='utf-8') as f:
-            f.write(integrated_changelog)
-
-        logger.info(f"Integrated changelog generated successfully at {output_file}")
-
-
-if __name__ == "__main__":
-    repo_path = "./"
-    output_dir = "docs/Changelog"
-    os.makedirs(output_dir, exist_ok=True)  # ディレクトリが存在しない場合は作成する
-
-    logger.add("changelog_generator.log", rotation="1 MB", retention="10 days")
-
-    generator = ChangelogGenerator(repo_path, output_dir)
-    generator.generate_changelog_for_all_branches()
+# modules/ChangelogGenerator.py (変更後)
+
+import os
+from git import Repo
+from .ChangelogUtils import ChangelogUtils
+from loguru import logger
+from git.exc import GitCommandError
+
+import sys
+
+class ChangelogGenerator:
+    def __init__(self, repo_path, output_dir):
+        self.repo_path = repo_path
+        self.output_dir = output_dir
+        self.repo = self._get_repo()
+
+    def _get_repo(self):
+        return Repo(self.repo_path)
+
+    def _get_commits(self, branch):
+        return list(self.repo.iter_commits(branch))
+
+    def generate_changelog(self, branch, output_file):
+        try:
+            commits = self._get_commits(branch)
+        except GitCommandError:
+            logger.warning(f"Skipping branch '{branch}' as it does not exist.")
+            return
+
+        # 出力ファイルのディレクトリを確認し、存在しない場合は作成
+        os.makedirs(os.path.dirname(output_file), exist_ok=True)
+
+        with open(output_file, 'w', encoding='utf-8') as f:
+            f.write(f"# Changelog\n\n")
+            f.write(f"## {branch}\n\n")
+
+            for commit in commits:
+                formatted_commit = ChangelogUtils.format_commit(commit)
+                f.write(formatted_commit + "\n")
+
+        logger.info(f"Changelog generated successfully for branch '{branch}' at {output_file}")
+
+    def generate_changelog_for_all_branches(self):
+        local_branches = [ref.name for ref in self.repo.branches]
+        remote_branches = [ref.name for ref in self.repo.remote().refs]
+
+        branches = local_branches + remote_branches
+        logger.info(branches)
+
+        feature_branches = [branch for branch in branches if 'feature/' in branch]
+        other_branches = [branch for branch in branches if 'feature/' not in branch]
+
+        for branch in other_branches:
+            branch_name = branch.replace('origin/', '')
+            output_file = os.path.join(self.output_dir, f"CHANGELOG_{branch_name}.md").replace("release/", "release_").replace("bugfix/", "bugfix_")
+            logger.info(f"Generating changelog for branch '{branch_name}'...")
+            self.generate_changelog(branch_name, output_file)
+
+        if feature_branches:
+            output_file = os.path.join(self.output_dir, "CHANGELOG_features.md")
+            with open(output_file, 'w', encoding='utf-8') as f:
+                f.write(f"# Changelog - Features\n\n")
+                for branch in feature_branches:
+                    branch_name = branch.replace('origin/', '')
+                    try:
+                        commits = self._get_commits(branch)
+                    except GitCommandError:
+                        logger.warning(f"Skipping feature branch '{branch_name}' as it does not exist.")
+                        continue
+
+                    f.write(f"## {branch_name}\n\n")
+                    for commit in commits:
+                        formatted_commit = ChangelogUtils.format_commit(commit)
+                        f.write(formatted_commit + "\n")
+                    f.write("\n")
+            logger.info(f"Changelog generated successfully for feature branches at {output_file}")
+
+    def integrate_changelogs(self):
+        changelog_files = [file for file in os.listdir(self.output_dir) if file.startswith("CHANGELOG_")]
+        integrated_changelog = "# Integrated Changelog\n\n"
+
+        for file in changelog_files:
+            with open(os.path.join(self.output_dir, file), 'r', encoding='utf-8') as f:
+                content = f.read()
+                integrated_changelog += f"{content}\n\n"
+
+        output_file = os.path.join(self.output_dir, "CHANGELOG_integrated.md")
+        with open(output_file, 'w', encoding='utf-8') as f:
+            f.write(integrated_changelog)
+
+        logger.info(f"Integrated changelog generated successfully at {output_file}")
+
+
+if __name__ == "__main__":
+    repo_path = "./"
+    output_dir = "docs/Changelog"
+    os.makedirs(output_dir, exist_ok=True)  # ディレクトリが存在しない場合は作成する
+
+    logger.add("changelog_generator.log", rotation="1 MB", retention="10 days")
+
+    generator = ChangelogGenerator(repo_path, output_dir)
+    generator.generate_changelog_for_all_branches()
     generator.integrate_changelogs()
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.1.4/sourcesage/modules/ChangelogUtils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# modules/ChangelogUtils.py (新規作成)
-
-from datetime import datetime
-
-class ChangelogUtils:
-    @staticmethod
-    def format_commit(commit):
-        message = commit.message.strip()
-        sha = commit.hexsha[:7]
-        author = commit.author.name
-        date = datetime.fromtimestamp(commit.committed_date).strftime("%Y-%m-%d")
-        return f"- [{sha}] - {message} ({author}, {date})"
-
-    @staticmethod
-    def generate_git_tree(repo, branch, num_commits):
-        tree_text = "```\n"
-        tree_text += "Git Commit Log Tree:\n"
-        commits = list(repo.iter_commits(branch, max_count=num_commits))
-        for i, commit in enumerate(commits, start=1):
-            if i == len(commits):  # 最後のコミット
-                prefix = "└──"
-            else:
-                prefix = "├──"
-            tree_text += f"{prefix} {commit.hexsha[:7]} - {commit.summary}\n"
-        tree_text += "```\n"
-        return tree_text
-
-    @staticmethod
-    def write_commit_details(file, commits, index):
-        commit = commits[index]
-        formatted_message = commit.message.replace('\n', '\n    ')
-        file.write(f"### コミットハッシュ: {commit.hexsha[:5]}...\n\n")
-        file.write(f"- **作者**: {commit.author.name}\n")
-        file.write(f"- **日時**: {commit.authored_datetime}\n")
+# modules/ChangelogUtils.py (新規作成)
+
+from datetime import datetime
+
+class ChangelogUtils:
+    @staticmethod
+    def format_commit(commit):
+        message = commit.message.strip()
+        sha = commit.hexsha[:7]
+        author = commit.author.name
+        date = datetime.fromtimestamp(commit.committed_date).strftime("%Y-%m-%d")
+        return f"- [{sha}] - {message} ({author}, {date})"
+
+    @staticmethod
+    def generate_git_tree(repo, branch, num_commits):
+        tree_text = "```\n"
+        tree_text += "Git Commit Log Tree:\n"
+        commits = list(repo.iter_commits(branch, max_count=num_commits))
+        for i, commit in enumerate(commits, start=1):
+            if i == len(commits):  # 最後のコミット
+                prefix = "└──"
+            else:
+                prefix = "├──"
+            tree_text += f"{prefix} {commit.hexsha[:7]} - {commit.summary}\n"
+        tree_text += "```\n"
+        return tree_text
+
+    @staticmethod
+    def write_commit_details(file, commits, index):
+        commit = commits[index]
+        formatted_message = commit.message.replace('\n', '\n    ')
+        file.write(f"### コミットハッシュ: {commit.hexsha[:5]}...\n\n")
+        file.write(f"- **作者**: {commit.author.name}\n")
+        file.write(f"- **日時**: {commit.authored_datetime}\n")
         file.write(f"- **メッセージ**: \n\n    {formatted_message}\n\n")
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.1.4/sourcesage/modules/DiffChangelogGenerator.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# modules/DiffChangelogGenerator.py (変更後)
-
-import json
-import os
-from git import Repo
-from modules.ChangelogUtils import ChangelogUtils
-
-class RepositoryChangelogGenerator:
-    def __init__(self, repo_path, changelog_dir, language_map_file):
-        self.repo_path = repo_path
-        self.changelog_dir = changelog_dir
-        self.changelog_file = os.path.join(changelog_dir, "CHANGELOG_Diff.md")  # チェンジログのファイル名を含めたパス
-        self.language_map_file = language_map_file
-        self.repo = Repo(repo_path)
-        self.language_map = self.load_language_map()
-
-    def load_language_map(self):
-        with open(self.language_map_file, "r", encoding="utf-8") as lang_file:
-            return json.load(lang_file)
-
-    def generate_changelog(self, branch='main', num_commits=2):
-        self.ensure_directory_exists(self.changelog_dir)
-        commits = list(self.repo.iter_commits(branch, max_count=num_commits + 1))
-
-        with open(self.changelog_file, "w", encoding="utf-8") as file:
-            # Git ログのツリー表示を追加
-            git_tree = ChangelogUtils.generate_git_tree(self.repo, branch, num_commits)
-            file.write(git_tree + "\n\n")
-
-            for i in range(min(num_commits, len(commits) - 1)):
-                ChangelogUtils.write_commit_details(file, commits, i)
-                self.write_changed_files(file, commits, i)
-
-    def ensure_directory_exists(self, path):
-        os.makedirs(path, exist_ok=True)
-
-    def write_changed_files(self, file, commits, index):
-        commit = commits[index]
-        previous_commit = commits[index + 1]
-        diff = previous_commit.diff(commit, create_patch=True)
-        file.write("#### 変更されたファイル:\n\n")
-
-        for diff_item in diff:
-            self.write_file_diff(file, diff_item, commit, previous_commit)
-
-    def write_file_diff(self, file, diff_item, commit, previous_commit):
-        file_path = diff_item.a_path or diff_item.b_path
-        if file_path:
-            _, extension = os.path.splitext(file_path)
-            language = self.language_map.get(extension, "bash")
-            file.write(f"- {file_path}\n")
-
-            try:
-                self.write_diff_content(file, diff_item, commit, previous_commit, language, file_path)
-            except Exception as e:
-                file.write(f"    - 内容の取得に失敗しました: {e}\n")
-        else:
-            file.write("    - 有効なファイルパスが見つかりませんでした。\n\n")
-
-    def write_diff_content(self, file, diff_item, commit, previous_commit, language, file_path):
-        try:
-            if diff_item.new_file or diff_item.deleted_file:
-                blob = self.repo.git.show(f"{commit.hexsha if diff_item.new_file else previous_commit.hexsha}:{file_path}")
-                content = self.escape_code_block(blob, language)
-                action = '追加された内容' if diff_item.new_file else '削除された内容'
-                file.write(f"    - {action}:\n\n{content}\n\n")
-                else:
-                diff_content = diff_item.diff.decode('utf-8')
-                diff_content_escaped = self.escape_code_block(diff_content, 'diff')
-                file.write(f"    - 差分:\n\n{diff_content_escaped}\n\n")
-                except Exception as e:
-                file.write(f"    - 内容の取得に失敗しました: {e}\n")
-
-    def escape_code_block(self, content, language):
-        # マークダウンのコードブロックをエスケープする
-        if '```' in content:
-            # 入れ子のコードブロックに対処
-            fenced_code_block = f"````{language}\n{content}\n````"
-        else:
-            fenced_code_block = f"```{language}\n{content}\n```"
-        return fenced_code_block
-
-if name == "main":
-    changelog_generator = RepositoryChangelogGenerator(
-        repo_path="./",
-        changelog_dir="SourceSageAssets",
-        language_map_file="config/language_map.json"
-    )
+# modules/DiffChangelogGenerator.py (変更後)
+
+import json
+import os
+from git import Repo
+from modules.ChangelogUtils import ChangelogUtils
+
+class RepositoryChangelogGenerator:
+    def __init__(self, repo_path, changelog_dir, language_map_file):
+        self.repo_path = repo_path
+        self.changelog_dir = changelog_dir
+        self.changelog_file = os.path.join(changelog_dir, "CHANGELOG_Diff.md")  # チェンジログのファイル名を含めたパス
+        self.language_map_file = language_map_file
+        self.repo = Repo(repo_path)
+        self.language_map = self.load_language_map()
+
+    def load_language_map(self):
+        with open(self.language_map_file, "r", encoding="utf-8") as lang_file:
+            return json.load(lang_file)
+
+    def generate_changelog(self, branch='main', num_commits=2):
+        self.ensure_directory_exists(self.changelog_dir)
+        commits = list(self.repo.iter_commits(branch, max_count=num_commits + 1))
+
+        with open(self.changelog_file, "w", encoding="utf-8") as file:
+            # Git ログのツリー表示を追加
+            git_tree = ChangelogUtils.generate_git_tree(self.repo, branch, num_commits)
+            file.write(git_tree + "\n\n")
+
+            for i in range(min(num_commits, len(commits) - 1)):
+                ChangelogUtils.write_commit_details(file, commits, i)
+                self.write_changed_files(file, commits, i)
+
+    def ensure_directory_exists(self, path):
+        os.makedirs(path, exist_ok=True)
+
+    def write_changed_files(self, file, commits, index):
+        commit = commits[index]
+        previous_commit = commits[index + 1]
+        diff = previous_commit.diff(commit, create_patch=True)
+        file.write("#### 変更されたファイル:\n\n")
+
+        for diff_item in diff:
+            self.write_file_diff(file, diff_item, commit, previous_commit)
+
+    def write_file_diff(self, file, diff_item, commit, previous_commit):
+        file_path = diff_item.a_path or diff_item.b_path
+        if file_path:
+            _, extension = os.path.splitext(file_path)
+            language = self.language_map.get(extension, "bash")
+            file.write(f"- {file_path}\n")
+
+            try:
+                self.write_diff_content(file, diff_item, commit, previous_commit, language, file_path)
+            except Exception as e:
+                file.write(f"    - 内容の取得に失敗しました: {e}\n")
+        else:
+            file.write("    - 有効なファイルパスが見つかりませんでした。\n\n")
+
+    def write_diff_content(self, file, diff_item, commit, previous_commit, language, file_path):
+        try:
+            if diff_item.new_file or diff_item.deleted_file:
+                blob = self.repo.git.show(f"{commit.hexsha if diff_item.new_file else previous_commit.hexsha}:{file_path}")
+                content = self.escape_code_block(blob, language)
+                action = '追加された内容' if diff_item.new_file else '削除された内容'
+                file.write(f"    - {action}:\n\n{content}\n\n")
+                else:
+                diff_content = diff_item.diff.decode('utf-8')
+                diff_content_escaped = self.escape_code_block(diff_content, 'diff')
+                file.write(f"    - 差分:\n\n{diff_content_escaped}\n\n")
+                except Exception as e:
+                file.write(f"    - 内容の取得に失敗しました: {e}\n")
+
+    def escape_code_block(self, content, language):
+        # マークダウンのコードブロックをエスケープする
+        if '```' in content:
+            # 入れ子のコードブロックに対処
+            fenced_code_block = f"````{language}\n{content}\n````"
+        else:
+            fenced_code_block = f"```{language}\n{content}\n```"
+        return fenced_code_block
+
+if name == "main":
+    changelog_generator = RepositoryChangelogGenerator(
+        repo_path="./",
+        changelog_dir="SourceSageAssets",
+        language_map_file="config/language_map.json"
+    )
     changelog_generator.generate_changelog(branch='main', num_commits=10)
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.1.4/sourcesage/modules/GitHubUtils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-# modules/GitHubUtils.py (新規作成)
-
-import requests
-import json
-import os
-from git import Repo
-
-class GitHubUtils:
-    @staticmethod
-    def retrieve_issues(owner, repository):
-        api_url = f'https://api.github.com/repos/{owner}/{repository}/issues?state=open'
-        response = requests.get(api_url)
-        issues = response.json()
-        return issues
-
-    @staticmethod
-    def filter_issues(issues):
-        filtered_issues = [
-            {"number": issue["number"], "title": issue["title"], "body": issue["body"]}
-            for issue in issues
-            if "pull_request" not in issue
-        ]
-        return filtered_issues
-
-    @staticmethod
-    def save_issues(issues, save_path, file_name):
-        if not os.path.exists(save_path):
-            os.makedirs(save_path)
-
-        with open(os.path.join(save_path, file_name), 'w', encoding='utf-8') as f:
-            json.dump(issues, f, ensure_ascii=False, indent=4)
-
-        print(f'Filtered open issues saved to {os.path.join(save_path, file_name)}')
-
-    @staticmethod
-    def get_staged_diff(repo_path):
-        repo = Repo(repo_path)
-        previous_commit = repo.head.commit
-        staged_diff = previous_commit.diff(None, create_patch=True)
+# modules/GitHubUtils.py (新規作成)
+
+import requests
+import json
+import os
+from git import Repo
+from loguru import logger
+
+class GitHubUtils:
+    @staticmethod
+    def retrieve_issues(owner, repository):
+        api_url = f'https://api.github.com/repos/{owner}/{repository}/issues?state=open'
+        response = requests.get(api_url)
+        issues = response.json()
+        return issues
+
+    @staticmethod
+    def filter_issues(issues):
+        filtered_issues = [
+            {"number": issue["number"], "title": issue["title"], "body": issue["body"]}
+            for issue in issues
+            if "pull_request" not in issue
+        ]
+        return filtered_issues
+
+    @staticmethod
+    def save_issues(issues, save_path, file_name):
+        if not os.path.exists(save_path):
+            os.makedirs(save_path)
+
+        with open(os.path.join(save_path, file_name), 'w', encoding='utf-8') as f:
+            json.dump(issues, f, ensure_ascii=False, indent=4)
+
+        logger.info(f'Filtered open issues saved to {os.path.join(save_path, file_name)}')
+
+    @staticmethod
+    def get_staged_diff(repo_path):
+        repo = Repo(repo_path)
+        previous_commit = repo.head.commit
+        staged_diff = previous_commit.diff(None, create_patch=True)
         return staged_diff
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.1.4/sourcesage/modules/IssuesToMarkdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,57 @@
-import json
-import os
-from loguru import logger
-
-class IssuesToMarkdown:
-    def __init__(self, issues_file, sourcesage_file, template_file, output_folder):
-        self.issues_file = issues_file
-        self.sourcesage_file = sourcesage_file
-        self.template_file = template_file
-        self.output_folder = output_folder
-
-    def load_data(self):
-        logger.info("Loading data...")
-        with open(self.issues_file, "r", encoding="utf-8") as f:
-            self.issues = json.load(f)
-        logger.info(f"Loaded {len(self.issues)} issues from {self.issues_file}")
-
-        with open(self.sourcesage_file, "r", encoding="utf-8") as f:
-            self.sourcesage_md = f.read()
-        logger.info(f"Loaded SourceSage markdown from {self.sourcesage_file}")
-
-        with open(self.template_file, "r", encoding="utf-8") as f:
-            self.template = f.read()
-        logger.info(f"Loaded template from {self.template_file}")
-
-    def create_markdown_files(self):
-        logger.info("Creating markdown files for issues...")
-        for issue in self.issues:
-            number = issue["number"]
-            title = issue["title"]
-            body = issue["body"]
-
-            content = self.template.replace("{{number}}", str(number))
-            content = content.replace("{{title}}", title)
-            content = content.replace("{{body}}", body or "")
-            content = content.replace("{{sourcesage_md}}", self.sourcesage_md)
-
-            filename = os.path.join(self.output_folder, f"ISSUE_{number}.md")
-            with open(filename, "w", encoding="utf-8") as f:
-                f.write(content)
-
-            logger.info(f"Created markdown file for issue {number}")
-
-        logger.info("Created markdown files for all issues")
-
-if __name__ == "__main__":
-    issues_file = "SourceSageAssets\\open_issues_filtered.json"
-    sourcesage_file = "SourceSageAssets\\SourceSage.md"
-    template_file = "docs\\ISSUES_RESOLVE\\ISSUES_RESOLVE_TEMPLATE.md"
-    output_folder = "docs\\ISSUES_RESOLVE"
-
-    converter = IssuesToMarkdown(issues_file, sourcesage_file, template_file, output_folder)
-    converter.load_data()
+import json
+import os
+from loguru import logger
+
+import sys
+
+
+class IssuesToMarkdown:
+    def __init__(self, issues_file, sourcesage_file, template_file, output_folder):
+        self.issues_file = issues_file
+        self.sourcesage_file = sourcesage_file
+        self.template_file = template_file
+        self.output_folder = output_folder
+
+    def load_data(self):
+        logger.info("Loading data...")
+        with open(self.issues_file, "r", encoding="utf-8") as f:
+            self.issues = json.load(f)
+        logger.info(f"Loaded {len(self.issues)} issues from {self.issues_file}")
+
+        with open(self.sourcesage_file, "r", encoding="utf-8") as f:
+            self.sourcesage_md = f.read()
+        logger.info(f"Loaded SourceSage markdown from {self.sourcesage_file}")
+
+        with open(self.template_file, "r", encoding="utf-8") as f:
+            self.template = f.read()
+        logger.info(f"Loaded template from {self.template_file}")
+
+    def create_markdown_files(self):
+        logger.info("Creating markdown files for issues...")
+        for issue in self.issues:
+            number = issue["number"]
+            title = issue["title"]
+            body = issue["body"]
+
+            content = self.template.replace("{{number}}", str(number))
+            content = content.replace("{{title}}", title)
+            content = content.replace("{{body}}", body or "")
+            content = content.replace("{{sourcesage_md}}", self.sourcesage_md)
+
+            filename = os.path.join(self.output_folder, f"ISSUE_{number}.md")
+            with open(filename, "w", encoding="utf-8") as f:
+                f.write(content)
+
+            logger.info(f"Created markdown file for issue {number}")
+
+        logger.info("Created markdown files for all issues")
+
+if __name__ == "__main__":
+    issues_file = "SourceSageAssets\\open_issues_filtered.json"
+    sourcesage_file = "SourceSageAssets\\SourceSage.md"
+    template_file = "docs\\ISSUES_RESOLVE\\ISSUES_RESOLVE_TEMPLATE.md"
+    output_folder = "docs\\ISSUES_RESOLVE"
+
+    converter = IssuesToMarkdown(issues_file, sourcesage_file, template_file, output_folder)
+    converter.load_data()
     converter.create_markdown_files()
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.1.4/sourcesage/modules/StageInfoGenerator.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# modules/StageInfoGenerator.py (変更後)
-
-import json
-import os
-from .GitHubIssueRetrieve import GitHubIssueRetriever
-from .StagedDiffGenerator import StagedDiffGenerator
-
-class StageInfoGenerator:
-    def __init__(self, issue_file_path, stage_diff_file_path, template_file_path, output_file_path):
-        self.issue_file_path = issue_file_path
-        self.stage_diff_file_path = stage_diff_file_path
-        self.template_file_path = template_file_path
-        self.output_file_path = output_file_path
-
-    def load_issues(self):
-        with open(self.issue_file_path, "r", encoding="utf-8") as issue_file:
-            return json.load(issue_file)
-
-    def load_stage_diff(self):
-        with open(self.stage_diff_file_path, "r", encoding="utf-8") as diff_file:
-            return diff_file.read()
-
-    def load_template(self):
-        with open(self.template_file_path, "r", encoding="utf-8") as template_file:
-            return template_file.read()
-
-    def generate_stage_info(self):
-        issues = self.load_issues()
-        stage_diff = self.load_stage_diff()
-        template = self.load_template()
-
-        output_dir = os.path.dirname(self.output_file_path)
-        os.makedirs(output_dir, exist_ok=True)
-
-        # テンプレートの [open_issues_filtered.json] の位置に issues を挿入
-        template = template.replace("[open_issues_filtered.json]", json.dumps(issues, indent=2, ensure_ascii=False))
-
-        # テンプレートの [STAGED_DIFF.md] の位置に stage_diff を挿入
-        template = template.replace("[STAGED_DIFF.md]", stage_diff)
-
-        with open(self.output_file_path, "w", encoding="utf-8") as output_file:
-            output_file.write(template)
-
-    def run(self):
-        self.generate_stage_info()
-
-if __name__ == "__main__":
-    owner = "Sunwood-ai-labs"
-    repository = "SourceSage"
-    save_path = "SourceSageAssets"
-    file_name = "open_issues_filtered.json"
-
-    issue_retriever = GitHubIssueRetriever(owner, repository, save_path, file_name)
-    issue_retriever.run()
-
-    diff_generator = StagedDiffGenerator(
-        repo_path="./",
-        output_dir="SourceSageAssets",
-        language_map_file="config/language_map.json"
-    )
-    diff_generator.run()
-
-    stage_info_generator = StageInfoGenerator(
-        issue_file_path="SourceSageAssets/open_issues_filtered.json",
-        stage_diff_file_path="SourceSageAssets/STAGED_DIFF.md",
-        template_file_path="docs/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md",
-        output_file_path="SourceSageAssets/STAGE_INFO_AND_ISSUES_AND_PROMT.md"
-    )
-    stage_info_generator.run()
-
-    stage_info_generator = StageInfoGenerator(
-        issue_file_path="SourceSageAssets/open_issues_filtered.json",
-        stage_diff_file_path="SourceSageAssets/STAGED_DIFF.md",
-        template_file_path="docs/STAGE_INFO/STAGE_INFO_TEMPLATE.md",
-        output_file_path="SourceSageAssets/STAGE_INFO_AND_PROMT.md"
-    )
+# modules/StageInfoGenerator.py (変更後)
+
+import json
+import os
+from .GitHubIssueRetrieve import GitHubIssueRetriever
+from .StagedDiffGenerator import StagedDiffGenerator
+
+class StageInfoGenerator:
+    def __init__(self, issue_file_path, stage_diff_file_path, template_file_path, output_file_path):
+        self.issue_file_path = issue_file_path
+        self.stage_diff_file_path = stage_diff_file_path
+        self.template_file_path = template_file_path
+        self.output_file_path = output_file_path
+
+    def load_issues(self):
+        with open(self.issue_file_path, "r", encoding="utf-8") as issue_file:
+            return json.load(issue_file)
+
+    def load_stage_diff(self):
+        with open(self.stage_diff_file_path, "r", encoding="utf-8") as diff_file:
+            return diff_file.read()
+
+    def load_template(self):
+        with open(self.template_file_path, "r", encoding="utf-8") as template_file:
+            return template_file.read()
+
+    def generate_stage_info(self):
+        issues = self.load_issues()
+        stage_diff = self.load_stage_diff()
+        template = self.load_template()
+
+        output_dir = os.path.dirname(self.output_file_path)
+        os.makedirs(output_dir, exist_ok=True)
+
+        # テンプレートの [open_issues_filtered.json] の位置に issues を挿入
+        template = template.replace("[open_issues_filtered.json]", json.dumps(issues, indent=2, ensure_ascii=False))
+
+        # テンプレートの [STAGED_DIFF.md] の位置に stage_diff を挿入
+        template = template.replace("[STAGED_DIFF.md]", stage_diff)
+
+        with open(self.output_file_path, "w", encoding="utf-8") as output_file:
+            output_file.write(template)
+
+    def run(self):
+        self.generate_stage_info()
+
+if __name__ == "__main__":
+    owner = "Sunwood-ai-labs"
+    repository = "SourceSage"
+    save_path = "SourceSageAssets"
+    file_name = "open_issues_filtered.json"
+
+    issue_retriever = GitHubIssueRetriever(owner, repository, save_path, file_name)
+    issue_retriever.run()
+
+    diff_generator = StagedDiffGenerator(
+        repo_path="./",
+        output_dir="SourceSageAssets",
+        language_map_file="config/language_map.json"
+    )
+    diff_generator.run()
+
+    stage_info_generator = StageInfoGenerator(
+        issue_file_path="SourceSageAssets/open_issues_filtered.json",
+        stage_diff_file_path="SourceSageAssets/STAGED_DIFF.md",
+        template_file_path="docs/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md",
+        output_file_path="SourceSageAssets/STAGE_INFO_AND_ISSUES_AND_PROMT.md"
+    )
+    stage_info_generator.run()
+
+    stage_info_generator = StageInfoGenerator(
+        issue_file_path="SourceSageAssets/open_issues_filtered.json",
+        stage_diff_file_path="SourceSageAssets/STAGED_DIFF.md",
+        template_file_path="docs/STAGE_INFO/STAGE_INFO_TEMPLATE.md",
+        output_file_path="SourceSageAssets/STAGE_INFO_AND_PROMT.md"
+    )
     stage_info_generator.run()
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.1.4/sourcesage/modules/StagedDiffGenerator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# modules/StagedDiffGenerator.py (変更後)
-
-import json
-import os
-from .GitHubUtils import GitHubUtils
-
-class StagedDiffGenerator:
-    def __init__(self, repo_path, output_dir, language_map_file):
-        self.repo_path = repo_path
-        self.output_dir = output_dir
-        self.output_file = os.path.join(output_dir, "STAGED_DIFF.md")
-        self.language_map_file = language_map_file
-        self.language_map = self.load_language_map()
-
-    def load_language_map(self):
-        with open(self.language_map_file, "r", encoding="utf-8") as lang_file:
-            return json.load(lang_file)
-
-    def generate_staged_diff(self):
-        staged_diff = GitHubUtils.get_staged_diff(self.repo_path)
-
-        os.makedirs(self.output_dir, exist_ok=True)  # フォルダが存在しない場合は作成
-
-        with open(self.output_file, "w", encoding="utf-8") as file:
-            file.write("# Staged Files Diff\n\n")
-            for diff_item in staged_diff:
-                self.write_file_diff(file, diff_item)
-
-    def write_file_diff(self, file, diff_item):
-        file_path = diff_item.a_path or diff_item.b_path
-        if file_path:
-            _, extension = os.path.splitext(file_path)
-            language = self.language_map.get(extension, "bash")
-            file.write(f"## {file_path}\n\n")
-
-            try:
-                self.write_diff_content(file, diff_item, language, file_path)
-            except Exception as e:
-                file.write(f"- 内容の取得に失敗しました: {e}\n")
-        else:
-            file.write("- 有効なファイルパスが見つかりませんでした。\n\n")
-
-    def write_diff_content(self, file, diff_item, language, file_path):
-        try:
-            diff_content = diff_item.diff.decode('utf-8')
-            diff_content_escaped = self.escape_code_block(diff_content, 'diff')
-            file.write(f"### 差分:\n\n{diff_content_escaped}\n\n")
-        except Exception as e:
-            file.write(f"- 内容の取得に失敗しました: {e}\n")
-
-    def escape_code_block(self, content, language):
-        # マークダウンのコードブロックをエスケープする
-        if '```' in content:
-            # 入れ子のコードブロックに対処
-            fenced_code_block = f"````{language}\n{content}\n````"
-        else:
-            fenced_code_block = f"```{language}\n{content}\n```"
-        return fenced_code_block
-
-    def run(self):
-        self.generate_staged_diff()
-
-if __name__ == "__main__":
-    diff_generator = StagedDiffGenerator(
-        repo_path="./",
-        output_dir="SourceSageAssets",
-        language_map_file="config/language_map.json"
-    )
+# modules/StagedDiffGenerator.py (変更後)
+
+import json
+import os
+from .GitHubUtils import GitHubUtils
+
+class StagedDiffGenerator:
+    def __init__(self, repo_path, output_dir, language_map_file):
+        self.repo_path = repo_path
+        self.output_dir = output_dir
+        self.output_file = os.path.join(output_dir, "STAGED_DIFF.md")
+        self.language_map_file = language_map_file
+        self.language_map = self.load_language_map()
+
+    def load_language_map(self):
+        with open(self.language_map_file, "r", encoding="utf-8") as lang_file:
+            return json.load(lang_file)
+
+    def generate_staged_diff(self):
+        staged_diff = GitHubUtils.get_staged_diff(self.repo_path)
+
+        os.makedirs(self.output_dir, exist_ok=True)  # フォルダが存在しない場合は作成
+
+        with open(self.output_file, "w", encoding="utf-8") as file:
+            file.write("# Staged Files Diff\n\n")
+            for diff_item in staged_diff:
+                self.write_file_diff(file, diff_item)
+
+    def write_file_diff(self, file, diff_item):
+        file_path = diff_item.a_path or diff_item.b_path
+        if file_path:
+            _, extension = os.path.splitext(file_path)
+            language = self.language_map.get(extension, "bash")
+            file.write(f"## {file_path}\n\n")
+
+            try:
+                self.write_diff_content(file, diff_item, language, file_path)
+            except Exception as e:
+                file.write(f"- 内容の取得に失敗しました: {e}\n")
+        else:
+            file.write("- 有効なファイルパスが見つかりませんでした。\n\n")
+
+    def write_diff_content(self, file, diff_item, language, file_path):
+        try:
+            diff_content = diff_item.diff.decode('utf-8')
+            diff_content_escaped = self.escape_code_block(diff_content, 'diff')
+            file.write(f"### 差分:\n\n{diff_content_escaped}\n\n")
+        except Exception as e:
+            file.write(f"- 内容の取得に失敗しました: {e}\n")
+
+    def escape_code_block(self, content, language):
+        # マークダウンのコードブロックをエスケープする
+        if '```' in content:
+            # 入れ子のコードブロックに対処
+            fenced_code_block = f"````{language}\n{content}\n````"
+        else:
+            fenced_code_block = f"```{language}\n{content}\n```"
+        return fenced_code_block
+
+    def run(self):
+        self.generate_staged_diff()
+
+if __name__ == "__main__":
+    diff_generator = StagedDiffGenerator(
+        repo_path="./",
+        output_dir="SourceSageAssets",
+        language_map_file="config/language_map.json"
+    )
     diff_generator.generate_staged_diff()
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/file_utils.py` & `sourcesage-4.1.4/sourcesage/modules/file_utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import os
-import fnmatch
-import json
-
-def load_ignore_patterns(ignore_file):
-    if os.path.exists(ignore_file):
-        with open(ignore_file, 'r') as f:
-            return [line.strip() for line in f if line.strip() and not line.startswith('#')]
-    else:
-        return []
-
-def load_language_map(language_map_file):
-    if os.path.exists(language_map_file):
-        with open(language_map_file, 'r') as f:
-            return json.load(f)
-    else:
-        return {}
-
-def is_excluded(path, exclude_patterns):
-    for pattern in exclude_patterns:
-        if fnmatch.fnmatch(path, pattern):
-            return True
-        if fnmatch.fnmatch(os.path.basename(path), pattern):
-            return True
-    return False
-
-def is_excluded_extension(filename, exclude_patterns):
-    _, extension = os.path.splitext(filename)
+import os
+import fnmatch
+import json
+
+def load_ignore_patterns(ignore_file):
+    if os.path.exists(ignore_file):
+        with open(ignore_file, 'r') as f:
+            return [line.strip() for line in f if line.strip() and not line.startswith('#')]
+    else:
+        return []
+
+def load_language_map(language_map_file):
+    if os.path.exists(language_map_file):
+        with open(language_map_file, 'r') as f:
+            return json.load(f)
+    else:
+        return {}
+
+def is_excluded(path, exclude_patterns):
+    for pattern in exclude_patterns:
+        if fnmatch.fnmatch(path, pattern):
+            return True
+        if fnmatch.fnmatch(os.path.basename(path), pattern):
+            return True
+    return False
+
+def is_excluded_extension(filename, exclude_patterns):
+    _, extension = os.path.splitext(filename)
     return any(fnmatch.fnmatch(extension, pattern) for pattern in exclude_patterns)
```

### Comparing `sourcesage-4.1.2/sourcesage/modules/markdown_utils.py` & `sourcesage-4.1.4/sourcesage/modules/markdown_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-import os
-from .file_utils import is_excluded, is_excluded_extension
-
-def generate_markdown_for_folder(folder_path, exclude_patterns, language_map):
-    markdown_content = "```plaintext\n"
-    print(folder_path)
-    markdown_content += _display_tree(dir_path=folder_path, exclude_patterns=exclude_patterns)
-    markdown_content += "\n```\n\n"
-    base_level = folder_path.count(os.sep)
-    for root, dirs, files in os.walk(folder_path, topdown=True):
-        dirs[:] = [d for d in dirs if not is_excluded(os.path.join(root, d), exclude_patterns)]
-        files = [f for f in files if not is_excluded(os.path.join(root, f), exclude_patterns) and not is_excluded_extension(f, exclude_patterns)]
-        level = root.count(os.sep) - base_level + 1
-        header_level = '#' * (level + 1)
-        relative_path = os.path.relpath(root, folder_path)
-        markdown_content += f"{header_level} {relative_path}\n\n"
-        for f in files:
-            file_path = os.path.join(root, f)
-            relative_file_path = os.path.relpath(file_path, folder_path)
-            try:
-                with open(file_path, 'r', encoding='utf-8') as file_content:
-                    content = file_content.read().strip()
-                    language = _get_language_for_file(f, language_map)
-                    markdown_content += f"`{relative_file_path}`\n\n```{language}\n{content}\n```\n\n"
-            except Exception as e:
-                markdown_content += f"`{relative_file_path}` - Error reading file: {e}\n\n"
-    return markdown_content
-
-def _display_tree(dir_path='.', exclude_patterns=None, string_rep=True, header=True, max_depth=None, show_hidden=False):
-    tree_string = ""
-    if header:
-        tree_string += f"OS: {os.name}\nDirectory: {os.path.abspath(dir_path)}\n\n"
-    tree_string += _build_tree_string(dir_path, max_depth, show_hidden, exclude_patterns, depth=0)
-    if string_rep:
-        return tree_string.strip()
-    else:
-        print(tree_string.strip())
-
-def _build_tree_string(dir_path, max_depth, show_hidden, exclude_patterns, depth=0):
-    tree_string = ""
-    if depth == max_depth:
-        return tree_string
-    
-    print(dir_path)
-    dir_contents = [(item, os.path.join(dir_path, item)) for item in os.listdir(dir_path)]
-    dirs = [(item, path) for item, path in dir_contents if os.path.isdir(path) and not is_excluded(path, exclude_patterns)]
-    files = [(item, path) for item, path in dir_contents if os.path.isfile(path) and not is_excluded(path, exclude_patterns) and not is_excluded_extension(item, exclude_patterns)]
-    for item, path in dirs:
-        if not show_hidden and item.startswith('.'):
-            continue
-        tree_string += '│  ' * depth + '├─ ' + item + '/\n'
-        tree_string += _build_tree_string(path, max_depth, show_hidden, exclude_patterns, depth + 1)
-    for item, path in files:
-        if not show_hidden and item.startswith('.'):
-            continue
-        tree_string += '│  ' * depth + '├─ ' + item + '\n'
-    return tree_string
-
-def _get_language_for_file(filename, language_map):
-    _, extension = os.path.splitext(filename)
-    extension = extension.lower()
+import os
+from .file_utils import is_excluded, is_excluded_extension
+from loguru import logger
+
+def generate_markdown_for_folder(folder_path, exclude_patterns, language_map):
+    markdown_content = "```plaintext\n"
+    logger.info(f"folder_path is ... {folder_path}")
+    markdown_content += _display_tree(dir_path=folder_path, exclude_patterns=exclude_patterns)
+    markdown_content += "\n```\n\n"
+    base_level = folder_path.count(os.sep)
+    for root, dirs, files in os.walk(folder_path, topdown=True):
+        dirs[:] = [d for d in dirs if not is_excluded(os.path.join(root, d), exclude_patterns)]
+        files = [f for f in files if not is_excluded(os.path.join(root, f), exclude_patterns) and not is_excluded_extension(f, exclude_patterns)]
+        level = root.count(os.sep) - base_level + 1
+        header_level = '#' * (level + 1)
+        relative_path = os.path.relpath(root, folder_path)
+        markdown_content += f"{header_level} {relative_path}\n\n"
+        for f in files:
+            file_path = os.path.join(root, f)
+            relative_file_path = os.path.relpath(file_path, folder_path)
+            try:
+                with open(file_path, 'r', encoding='utf-8') as file_content:
+                    content = file_content.read().strip()
+                    language = _get_language_for_file(f, language_map)
+                    markdown_content += f"`{relative_file_path}`\n\n```{language}\n{content}\n```\n\n"
+            except Exception as e:
+                markdown_content += f"`{relative_file_path}` - Error reading file: {e}\n\n"
+    return markdown_content
+
+def _display_tree(dir_path='.', exclude_patterns=None, string_rep=True, header=True, max_depth=None, show_hidden=False):
+    tree_string = ""
+    if header:
+        tree_string += f"OS: {os.name}\nDirectory: {os.path.abspath(dir_path)}\n\n"
+    tree_string += _build_tree_string(dir_path, max_depth, show_hidden, exclude_patterns, depth=0)
+    if string_rep:
+        return tree_string.strip()
+    else:
+        logger.info(tree_string.strip())
+
+def _build_tree_string(dir_path, max_depth, show_hidden, exclude_patterns, depth=0):
+    tree_string = ""
+    if depth == max_depth:
+        return tree_string
+    
+    logger.info(f"dir_path is ... {dir_path}")
+    dir_contents = [(item, os.path.join(dir_path, item)) for item in os.listdir(dir_path)]
+    dirs = [(item, path) for item, path in dir_contents if os.path.isdir(path) and not is_excluded(path, exclude_patterns)]
+    files = [(item, path) for item, path in dir_contents if os.path.isfile(path) and not is_excluded(path, exclude_patterns) and not is_excluded_extension(item, exclude_patterns)]
+    for item, path in dirs:
+        if not show_hidden and item.startswith('.'):
+            continue
+        tree_string += '│  ' * depth + '├─ ' + item + '/\n'
+        tree_string += _build_tree_string(path, max_depth, show_hidden, exclude_patterns, depth + 1)
+    for item, path in files:
+        if not show_hidden and item.startswith('.'):
+            continue
+        tree_string += '│  ' * depth + '├─ ' + item + '\n'
+    return tree_string
+
+def _get_language_for_file(filename, language_map):
+    _, extension = os.path.splitext(filename)
+    extension = extension.lower()
     return language_map.get(extension, 'plaintext')
```

### Comparing `sourcesage-4.1.2/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.1.4/sourcesage.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,229 +1,232 @@
-Metadata-Version: 2.1
-Name: sourcesage
-Version: 4.1.2
-Home-page: https://github.com/Sunwood-ai-labs/SourceSage
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: loguru
-Requires-Dist: GitPython
-Requires-Dist: requests
-Requires-Dist: art
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
-<br>
-<h1 align="center">SourceSage</h1>
-<h2 align="center">
-  ～Transforming code for AI～
-
-  <br>
-  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
-  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
-  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
-  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
-  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
-  <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
-
-  <br>
-
-</h2>
-
-
-</p>
-
-
-
-SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
-
-**このリポジトリ自体もSourceSageを活用しており、リリースノートやREADME、コミットメッセージの9割はSourceSage X クロードで生成しています。**
-
-
-## 更新内容
-
-- [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
-  - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
-  - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
-  - CLI引数の追加とコアモジュールの修正
-  - プロジェクトの構成とファイルの変更によるシンプル化
-  - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
-- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
-  - README.mdのセットアップ手順と実行手順を簡素化
-  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
-  - テスト実行方法のドキュメントを更新
-- [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
-  - コードの品質と保守性を向上させるためのリファクタリングと機能改善
-  - コミットメッセージのフォーマットとタイプの説明を追加
-  - コマンドラインからソースコードのリポジトリパスを取得するように修正
-  - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
-- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
-  - [IssueWise](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
-  - [CommitCraft](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
-  - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
-- [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
-  - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
-  - 言語ごとのシンタックスハイライト機能を追加
-  - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
-- 【2024/03/29】 初期リリース
-
-## 主な機能
-
-### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
-
-- GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
-- 課題を効率的に特定し、迅速に解決策を見つけられます
-
-### [CommitCraft（開発中のコミット管理）](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)
-- 変更差分を追跡し、AIが適切なコミットメッセージを自動生成
-- コミットの内容を正確に記述でき、変更履歴を明確に管理できます
-
-### [DocuMind（リリース後のドキュメント化）](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)
-- プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化 
-- プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
-
-## 使用方法
-
-### セットアップ
-
-SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
-
-```bash
-pip install sourcesage
-```
-
-これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
-
-### クイックスタート
-
-SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
-
-1. ターミナルまたはコマンドプロンプトを開きます。
-
-2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
-   ```bash 
-   cd ~/my_project
-   ```
-   
-   Note: `cd`コマンドは "change directory" の略で、現在のディレクトリを指定したディレクトリに変更するために使用します。
-
-3. 次に、以下のコマンドを実行してSourceSageを起動します：
-   ```bash
-   sourcesage
-   ```
-
-4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
-   - `DocuMind.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
-   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
-   - `ISSUES_RESOLVE` : Issuesとプロジェクト全体がマージされたファイルを保存するディレクトリです。これらのファイルは、AIがIssueを解決するための重要な情報源となります。
-   - `COMMIT_CRAFT` : 開発中のステージされたコードのファイルを保存するディレクトリです。これらのファイルは、AIが適切なコミットメッセージを生成するために使用されます。
-   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
-   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
-
-これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
-
-### リポジトリのIssueも取得する方法
-
-デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
-
-```bash 
-sourcesage --owner Sunwood-ai-labs --repository SourceSage
-```
-
-上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
-
-Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
-
-以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
-
-### 除外ファイルの指定
-
-作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
-
-```plaintext
-# .SourceSageignoreの例
-node_modules/
-*.log
-*.tmp
-```
-
-上記の例では、`node_modules`ディレクトリと、拡張子が`.log`または`.tmp`のファイルが除外されます。
-
-`.SourceSageignore`ファイルを使用する場合は、以下のようにコマンドライン引数で指定します：
-
-```bash 
-sourcesage --owner Sunwood-ai-labs --repository SourceSage --ignore-file .SourceSageignore
-```
-
-この機能を使用することで、不要なファイルやディレクトリを処理から除外し、より効率的にSourceSageを実行できます。
-
-## 1. IssueWise：開発前の課題解決
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
-</p>
-
-IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
-
-`SourceSageAssets/ISSUE_WISE/ISSUES_RESOLVE`に生成されるマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_ISSUE_11.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_ISSUE_11.md)
-
-このマークダウンファイルをそのままAIに入力することで、AIが課題を解決するためのコードを生成します。AIは、Issueの内容とプロジェクトの概要を組み合わせて分析し、適切な修正を提案します。
-
-このマークダウンファイルは、下記のファイルのフォーマットで出力されます。
-[`docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md)
-
-IssueWiseを使用することで、開発者は手作業でIssueを確認する負担を軽減し、AIによる自動修正の恩恵を受けることができます。
-
-## 2. CommitCraft：開発中のコミット管理
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon5.png" width="50%">
-</p>
-
-CommitCraftは、開発中のステージされた変更を追跡し、AIを活用して適切なコミットメッセージを自動生成するツールです。これにより、開発者はコミットの内容を正確に記述することができ、プロジェクトの変更履歴をより明確に管理できます。
-
-`SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
-
-このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
-
-Issueとマージされたファイルの例はこちらです。
-
-例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
-
-このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
-
-CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
-
-## 3. DocuMind：リリース後のドキュメント化
-
-<p align="center">
-<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
-</p>
-
-DocuMindは、リリース後のプロジェクトの統合とドキュメント化を支援するツールです。SourceSageが生成するプロジェクトの概要と、自動生成されたGitの変更履歴を組み合わせることで、プロジェクトの全体像を明確に把握できます。これにより、開発者はプロジェクトのドキュメントを効率的に作成し、メンテナンス性を向上させることができます。
-
-`SourceSageAssets/DocuMind.md`に生成されるマークダウンファイルを使用します。 
-
-例：[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_DocuMind.md)
-
-また、`SourceSageAssets/Changelog`に生成されるコミットメッセージのマークダウンファイルを使用します。
-
-例：[`docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md)
-
-この2つのマークダウンファイルをそのままAIに入力することで、AIがプロジェクトの構造と変更内容を理解し、リリースノートやドキュメントを生成することができます。AIは、プロジェクトの概要とGitの変更履歴を分析し、プロジェクトの主要な機能や変更点を要約します。
-
-DocuMindを使用することで、開発者はドキュメント作成の負担を軽減し、常に最新の状態を反映したドキュメントを自動的に生成できます。
-
-## 貢献
-
-SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
-
-## ライセンス
-
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+Metadata-Version: 2.1
+Name: sourcesage
+Version: 4.1.4
+Home-page: https://github.com/Sunwood-ai-labs/SourceSage
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: loguru
+Requires-Dist: GitPython
+Requires-Dist: requests
+Requires-Dist: art
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
+<br>
+<h1 align="center">SourceSage</h1>
+<h2 align="center">
+  ～Transforming code for AI～
+
+  <br>
+  <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/sourcesage">
+  <img alt="PyPI - Format" src="https://img.shields.io/pypi/format/sourcesage">
+  <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
+  <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
+  <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
+  <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
+
+  <br>
+
+</h2>
+
+
+</p>
+
+
+
+SourceSageは、プロジェクトのソースコードとファイル構成を単一のマークダウンファイルに統合し、AIによる自動修正やドキュメント化を実現するPythonスクリプトです。開発のライフサイクル全体を通して、コードの品質向上と生産性の向上を支援します。
+
+**このリポジトリ自体もSourceSageを活用しており、リリースノートやREADME、コミットメッセージの9割はSourceSage X クロードで生成しています。**
+
+
+## 更新内容
+
+- [【2024/04/30】 SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/v4.1.2)
+  - GitHub ActionsによるPyPIへの自動パブリッシュ設定を追加し、リリースプロセスを自動化
+
+- [【2024/04/07】 SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.1.1)
+  - プロジェクト全体の出力ファイル名と各モジュールの出力フォルダ名を変更
+  - PyPIのダウンロードバッジとCodacyのクオリティバッジを追加
+  - CLI引数の追加とコアモジュールの修正
+  - プロジェクトの構成とファイルの変更によるシンプル化
+  - セットアップ手順、実行方法、クイックスタートセクション、テストドキュメントの更新
+- [【2024/04/05】 SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/undefined4.0.3)
+  - README.mdのセットアップ手順と実行手順を簡素化
+  - リポジトリのオーナーと名前をコマンドライン引数で指定可能に
+  - テスト実行方法のドキュメントを更新
+- [【2024/04/01】 SourceSage 3.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.1.0)
+  - コードの品質と保守性を向上させるためのリファクタリングと機能改善
+  - コミットメッセージのフォーマットとタイプの説明を追加
+  - コマンドラインからソースコードのリポジトリパスを取得するように修正
+  - 定数の管理方法を改善し、[`config/constants.py`](config/constants.py)ファイルで一元管理
+- [【2024/03/31】 SourceSage 3.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag3.0.0)
+  - [IssueWise](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)機能を追加し、GitHubのオープンIssueを取得してAIによる自動修正をサポート
+  - [CommitCraft](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)機能を追加し、変更差分を追跡してAIが適切なコミットメッセージを生成
+  - [DocuMind](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)機能を追加し、プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化
+- [【2024/03/30】 SourceSage 2.0.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/tag2.0.0)
+  - ChangelogGenerator classを導入し、コードの可読性と保守性を向上
+  - 言語ごとのシンタックスハイライト機能を追加
+  - .SourceSageignoreファイルを導入し、不要なファイルやフォルダを自動的に除外
+- 【2024/03/29】 初期リリース
+
+## 主な機能
+
+### [IssueWise（開発前の課題解決）](https://github.com/Sunwood-ai-labs/SourceSage/#1-issuewise開発前の課題解決)
+
+- GitHubのオープンIssueを自動取得し、AIによる課題の自動修正をサポート
+- 課題を効率的に特定し、迅速に解決策を見つけられます
+
+### [CommitCraft（開発中のコミット管理）](https://github.com/Sunwood-ai-labs/SourceSage/#2-commitcraft開発中のコミット管理)
+- 変更差分を追跡し、AIが適切なコミットメッセージを自動生成
+- コミットの内容を正確に記述でき、変更履歴を明確に管理できます
+
+### [DocuMind（リリース後のドキュメント化）](https://github.com/Sunwood-ai-labs/SourceSage/#3-documindリリース後のドキュメント化)
+- プロジェクトの概要とGitの変更履歴を組み合わせてドキュメント化 
+- プロジェクトの全体像を把握しやすく、メンテナンス性が向上します
+
+## 使用方法
+
+### セットアップ
+
+SourceSageを使用するには、まずPythonのパッケージマネージャーであるpipを使ってインストールします。以下のコマンドをターミナルまたはコマンドプロンプトで実行してください：
+
+```bash
+pip install sourcesage
+```
+
+これにより、SourceSageがシステムにインストールされ、コマンドラインから実行できるようになります。
+
+### クイックスタート
+
+SourceSageをプロジェクトで使用するには、以下の手順に従ってください：
+
+1. ターミナルまたはコマンドプロンプトを開きます。
+
+2. `cd`コマンドを使って、解析対象のプロジェクトのルートディレクトリに移動します。例えば、プロジェクトが`~/my_project`ディレクトリにある場合は、以下のコマンドを実行します：
+   ```bash 
+   cd ~/my_project
+   ```
+   
+   Note: `cd`コマンドは "change directory" の略で、現在のディレクトリを指定したディレクトリに変更するために使用します。
+
+3. 次に、以下のコマンドを実行してSourceSageを起動します：
+   ```bash
+   sourcesage
+   ```
+
+4. SourceSageが実行されると、以下のファイルが`SourceSageAssets`ディレクトリに生成されます：
+   - `DocuMind.md`：AIがプロジェクトの構造と内容を理解しやすい形式のマークダウンファイルです。
+   - `Changelog`：Gitの変更履歴を保存するディレクトリです。
+   - `ISSUES_RESOLVE` : Issuesとプロジェクト全体がマージされたファイルを保存するディレクトリです。これらのファイルは、AIがIssueを解決するための重要な情報源となります。
+   - `COMMIT_CRAFT` : 開発中のステージされたコードのファイルを保存するディレクトリです。これらのファイルは、AIが適切なコミットメッセージを生成するために使用されます。
+   - `open_issues_filtered.json`：GitHubからフェッチしたオープンなIssueのJSONファイルです。
+   - `STAGED_DIFF.md`：ステージされた変更の差分情報を含むマークダウンファイルです。
+
+これらのファイルを使って、AIによるプロジェクトの解析や自動修正、ドキュメント化などを行うことができます。
+
+### リポジトリのIssueも取得する方法
+
+デフォルトでは、SourceSageは現在のディレクトリをプロジェクトのルートとして解析します。ただし、GitHub上のリポジトリのIssueも取得したい場合は、以下のようにリポジトリのオーナー名とリポジトリ名をコマンドライン引数で指定します：
+
+```bash 
+sourcesage --owner Sunwood-ai-labs --repository SourceSage
+```
+
+上記の例では、`Sunwood-ai-labs`がリポジトリのオーナー名、`SourceSage`がリポジトリ名です。これらの引数を指定することで、SourceSageはGitHub APIを使ってリポジトリのオープンなIssueを取得し、`open_issues_filtered.json`ファイルに保存します。
+
+Note: GitHub APIを使用するには、インターネット接続が必要です。また、リポジトリがプライベートの場合は、適切なアクセストークンを設定する必要があります。
+
+以上が、SourceSageの基本的な使用方法です。ぜひ自分のプロジェクトでSourceSageを活用して、開発効率の向上を体験してみてください！
+
+### 除外ファイルの指定
+
+作業ディレクトリに`.SourceSageignore`ファイルを作成することで、任意のファイルやディレクトリを処理から除外できます。このファイルには、除外したいファイルやディレクトリのパターンを1行ずつ記述します。例えば、以下のように指定します：
+
+```plaintext
+# .SourceSageignoreの例
+node_modules/
+*.log
+*.tmp
+```
+
+上記の例では、`node_modules`ディレクトリと、拡張子が`.log`または`.tmp`のファイルが除外されます。
+
+`.SourceSageignore`ファイルを使用する場合は、以下のようにコマンドライン引数で指定します：
+
+```bash 
+sourcesage --owner Sunwood-ai-labs --repository SourceSage --ignore-file .SourceSageignore
+```
+
+この機能を使用することで、不要なファイルやディレクトリを処理から除外し、より効率的にSourceSageを実行できます。
+
+## 1. IssueWise：開発前の課題解決
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon4.png" width="50%">
+</p>
+
+IssueWiseは、GitHubのオープンなIssue(課題)を自動的に取得し、SourceSageが生成したプロジェクトの概要と組み合わせることで、AIによる課題の自動修正を可能にするツールです。これにより、開発者はプロジェクトの課題を効率的に特定し、解決策を迅速に見つけることができます。
+
+`SourceSageAssets/ISSUE_WISE/ISSUES_RESOLVE`に生成されるマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_ISSUE_11.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_ISSUE_11.md)
+
+このマークダウンファイルをそのままAIに入力することで、AIが課題を解決するためのコードを生成します。AIは、Issueの内容とプロジェクトの概要を組み合わせて分析し、適切な修正を提案します。
+
+このマークダウンファイルは、下記のファイルのフォーマットで出力されます。
+[`docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md)
+
+IssueWiseを使用することで、開発者は手作業でIssueを確認する負担を軽減し、AIによる自動修正の恩恵を受けることができます。
+
+## 2. CommitCraft：開発中のコミット管理
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon5.png" width="50%">
+</p>
+
+CommitCraftは、開発中のステージされた変更を追跡し、AIを活用して適切なコミットメッセージを自動生成するツールです。これにより、開発者はコミットの内容を正確に記述することができ、プロジェクトの変更履歴をより明確に管理できます。
+
+`SourceSageAssets/COMMIT_CRAFT/STAGED_DIFF.md`に生成されるマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_PROMT.md)
+
+このマークダウンファイルをそのままAIに入力することで、AIがコミットメッセージを生成します。AIは、ステージされた変更の差分を分析し、その内容を要約したコミットメッセージを提案します。
+
+Issueとマージされたファイルの例はこちらです。
+
+例：[`docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_STAGE_INFO_AND_ISSUES_AND_PROMT.md)
+
+このファイルには、ステージされた変更の差分とオープンなIssueの情報が含まれています。AIはこれらの情報を組み合わせて分析し、より包括的なコミットメッセージを生成します。
+
+CommitCraftを使用することで、開発者はコミットメッセージを考える負担を軽減し、一貫性のある適切なコミットメッセージを自動的に生成できます。
+
+## 3. DocuMind：リリース後のドキュメント化
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/head_icon7.png" width="100%">  
+</p>
+
+DocuMindは、リリース後のプロジェクトの統合とドキュメント化を支援するツールです。SourceSageが生成するプロジェクトの概要と、自動生成されたGitの変更履歴を組み合わせることで、プロジェクトの全体像を明確に把握できます。これにより、開発者はプロジェクトのドキュメントを効率的に作成し、メンテナンス性を向上させることができます。
+
+`SourceSageAssets/DocuMind.md`に生成されるマークダウンファイルを使用します。 
+
+例：[`docs/SAMPLE/SAMPLE_DocuMind.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_DocuMind.md)
+
+また、`SourceSageAssets/Changelog`に生成されるコミットメッセージのマークダウンファイルを使用します。
+
+例：[`docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md`](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/docs/SAMPLE/SAMPLE_CHANGELOG_release_4.1.0.md)
+
+この2つのマークダウンファイルをそのままAIに入力することで、AIがプロジェクトの構造と変更内容を理解し、リリースノートやドキュメントを生成することができます。AIは、プロジェクトの概要とGitの変更履歴を分析し、プロジェクトの主要な機能や変更点を要約します。
+
+DocuMindを使用することで、開発者はドキュメント作成の負担を軽減し、常に最新の状態を反映したドキュメントを自動的に生成できます。
+
+## 貢献
+
+SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
+
+## ライセンス
+
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

#### html2text {}

```diff
@@ -1,25 +1,28 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.1.2 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.1.4 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
                        _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 **ãã®ãªãã¸ããªèªä½ãSourceSageãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯SourceSage
-X ã¯ã­ã¼ãã§çæãã¦ãã¾ãã** ## æ´æ°åå®¹ - [ã2024/04/07ã
-SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/
-undefined4.1.1) -
+X ã¯ã­ã¼ãã§çæãã¦ãã¾ãã** ## æ´æ°åå®¹ - [ã2024/04/30ã
+SourceSage 4.1.2](https://github.com/Sunwood-ai-labs/SourceSage/releases/tag/
+v4.1.2) - GitHub
+Actionsã«ããPyPIã¸ã®èªåãããªãã·ã¥è¨­å®ãè¿½å ãããªãªã¼ã¹ãã­ã»ã¹ãèªåå
+- [ã2024/04/07ã SourceSage 4.1.0](https://github.com/Sunwood-ai-labs/
+SourceSage/releases/tag/undefined4.1.1) -
 ãã­ã¸ã§ã¯ãå¨ä½ã®åºåãã¡ã¤ã«åã¨åã¢ã¸ã¥ã¼ã«ã®åºåãã©ã«ãåãå¤æ´
 -
 PyPIã®ãã¦ã³ã­ã¼ãããã¸ã¨Codacyã®ã¯ãªãªãã£ããã¸ãè¿½å 
 - CLIå¼æ°ã®è¿½å ã¨ã³ã¢ã¢ã¸ã¥ã¼ã«ã®ä¿®æ­£ -
 ãã­ã¸ã§ã¯ãã®æ§æã¨ãã¡ã¤ã«ã®å¤æ´ã«ããã·ã³ãã«å -
 ã»ããã¢ããæé ãå®è¡æ¹æ³ãã¯ã¤ãã¯ã¹ã¿ã¼ãã»ã¯ã·ã§ã³ããã¹ããã­ã¥ã¡ã³ãã®æ´æ°
 - [ã2024/04/05ã SourceSage 4.0.3](https://github.com/Sunwood-ai-labs/
```

### Comparing `sourcesage-4.1.2/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.1.4/sourcesage.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 sourcesage.egg-info/top_level.txt
 sourcesage/config/.SourceSageignore
 sourcesage/config/constants.py
 sourcesage/config/language_map.json
 sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
-sourcesage/config/__pycache__/constants.cpython-311.pyc
 sourcesage/modules/ChangelogGenerator.py
 sourcesage/modules/ChangelogUtils.py
 sourcesage/modules/DiffChangelogGenerator.py
 sourcesage/modules/EnvFileHandler.py
 sourcesage/modules/GitHubIssueRetrieve.py
 sourcesage/modules/GitHubUtils.py
 sourcesage/modules/IssuesToMarkdown.py
```

### Comparing `sourcesage-4.1.2/tests/test_sourcesage.py` & `sourcesage-4.1.4/tests/test_sourcesage.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import os
-from sourcesage.cli import main
-from sourcesage.core import SourceSage
-import sys
-
-def ensure_temp_directory():
-    """temp フォルダが存在することを確認し、なければ作成します。"""
-    temp_path = os.path.join(os.getcwd(), 'temp')
-    os.makedirs(temp_path, exist_ok=True)
-    return temp_path
-
-def test_sourcesage_cli(capsys):
-    temp_dir = ensure_temp_directory()  # tempフォルダの確認/作成
-
-    # テスト用の設定ファイルを作成
-    config_path = os.path.join(temp_dir, 'sourcesage.yml')
-    with open(config_path, 'w') as f:
-        f.write('exclude_patterns:\n  - "*.pyc"\n  - "__pycache__"\n')
-
-    # パッケージのルートディレクトリを取得
-    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-
-    ignore_file_path = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
-    language_map_path = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
-
-    sys.argv = ['sourcesage', '--config', config_path, '--output', temp_dir, '--repo', package_root, '--owner', 'Sunwood-ai-labs', '--repository', 'SourceSage', '--ignore-file', ignore_file_path, '--language-map', language_map_path]
-    main()
-
-    # 出力を確認
-    captured = capsys.readouterr()
-    assert 'Running SourceSage...' in captured.out
-    assert 'SourceSage completed successfully.' in captured.out
-
-    # 出力ファイルが生成されたことを確認
-    output_file = os.path.join(temp_dir, 'SourceSage.md')
-    # assert os.path.exists(output_file)
-
-    # 出力ファイルの保存場所を表示
-    print(f"Output file saved at: {output_file}")
-
-def test_sourcesage_core():
-    temp_dir = ensure_temp_directory()  # tempフォルダの確認/作成
-
-    # テスト用の設定ファイルを作成
-    config_path = os.path.join(temp_dir, 'sourcesage.yml')
-    with open(config_path, 'w') as f:
-        f.write('exclude_patterns:\n  - "*.pyc"\n  - "__pycache__"\n')
-
-    # パッケージのルートディレクトリを取得
-    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-
-    ignore_file_path = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
-    language_map_path = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
-
-    # 必要なディレクトリを作成
-    necessary_dirs = ['SourceSageAssets/Changelog', 'SourceSageAssets/ISSUE_LOG', 'SourceSageAssets/ISSUES_RESOLVE', 'SourceSageAssets/STAGE_INFO']
-    for dir_path in necessary_dirs:
-        os.makedirs(os.path.join(temp_dir, dir_path), exist_ok=True)
-
-    # SourceSageクラスを直接インスタンス化して実行
-    sourcesage = SourceSage(config_path, temp_dir, package_root, 'Sunwood-ai-labs', 'SourceSage', ignore_file_path, language_map_path)
-    sourcesage.run()
-
-    # 出力ファイルが生成されたことを確認
-    output_file = os.path.join(temp_dir, 'SourceSage.md')
-    # assert os.path.exists(output_file)
-
-    # 出力ファイルの保存場所を表示
+import os
+from sourcesage.cli import main
+from sourcesage.core import SourceSage
+import sys
+
+def ensure_temp_directory():
+    """temp フォルダが存在することを確認し、なければ作成します。"""
+    temp_path = os.path.join(os.getcwd(), 'temp')
+    os.makedirs(temp_path, exist_ok=True)
+    return temp_path
+
+def test_sourcesage_cli(capsys):
+    temp_dir = ensure_temp_directory()  # tempフォルダの確認/作成
+
+    # テスト用の設定ファイルを作成
+    config_path = os.path.join(temp_dir, 'sourcesage.yml')
+    with open(config_path, 'w') as f:
+        f.write('exclude_patterns:\n  - "*.pyc"\n  - "__pycache__"\n')
+
+    # パッケージのルートディレクトリを取得
+    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+
+    ignore_file_path = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
+    language_map_path = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
+
+    sys.argv = ['sourcesage', '--config', config_path, '--output', temp_dir, '--repo', package_root, '--owner', 'Sunwood-ai-labs', '--repository', 'SourceSage', '--ignore-file', ignore_file_path, '--language-map', language_map_path]
+    main()
+
+    # 出力を確認
+    captured = capsys.readouterr()
+    assert 'Running SourceSage...' in captured.out
+    assert 'SourceSage completed successfully.' in captured.out
+
+    # 出力ファイルが生成されたことを確認
+    output_file = os.path.join(temp_dir, 'SourceSage.md')
+    # assert os.path.exists(output_file)
+
+    # 出力ファイルの保存場所を表示
+    print(f"Output file saved at: {output_file}")
+
+def test_sourcesage_core():
+    temp_dir = ensure_temp_directory()  # tempフォルダの確認/作成
+
+    # テスト用の設定ファイルを作成
+    config_path = os.path.join(temp_dir, 'sourcesage.yml')
+    with open(config_path, 'w') as f:
+        f.write('exclude_patterns:\n  - "*.pyc"\n  - "__pycache__"\n')
+
+    # パッケージのルートディレクトリを取得
+    package_root = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
+
+    ignore_file_path = os.path.join(package_root, 'sourcesage', 'config', '.SourceSageignore')  # 修正
+    language_map_path = os.path.join(package_root, 'sourcesage', 'config', 'language_map.json')  # 修正
+
+    # 必要なディレクトリを作成
+    necessary_dirs = ['SourceSageAssets/Changelog', 'SourceSageAssets/ISSUE_LOG', 'SourceSageAssets/ISSUES_RESOLVE', 'SourceSageAssets/STAGE_INFO']
+    for dir_path in necessary_dirs:
+        os.makedirs(os.path.join(temp_dir, dir_path), exist_ok=True)
+
+    # SourceSageクラスを直接インスタンス化して実行
+    sourcesage = SourceSage(config_path, temp_dir, package_root, 'Sunwood-ai-labs', 'SourceSage', ignore_file_path, language_map_path)
+    sourcesage.run()
+
+    # 出力ファイルが生成されたことを確認
+    output_file = os.path.join(temp_dir, 'SourceSage.md')
+    # assert os.path.exists(output_file)
+
+    # 出力ファイルの保存場所を表示
     print(f"Output file saved at: {output_file}")
```

