# Comparing `tmp/akita_ai-0.1.102.tar.gz` & `tmp/akita_ai-0.1.200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akita_ai-0.1.102.tar", max compression
+gzip compressed data, was "akita_ai-0.1.200.tar", max compression
```

## Comparing `akita_ai-0.1.102.tar` & `akita_ai-0.1.200.tar`

### file list

```diff
@@ -1,110 +1,119 @@
--rw-r--r--   0        0        0    11337 2024-03-06 14:39:51.045954 akita_ai-0.1.102/LICENSE
--rw-r--r--   0        0        0     3699 2024-03-06 14:39:51.045954 akita_ai-0.1.102/README.md
--rw-r--r--   0        0        0    10244 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/__init__.py
--rw-r--r--   0        0        0       70 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/__main__.py
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/api/__init__.py
--rw-r--r--   0        0        0     1273 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/api/openai_client.py
--rw-r--r--   0        0        0     8196 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/.DS_Store
--rw-r--r--   0        0        0     2431 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/.chainlit/config.toml
--rw-r--r--   0        0        0     5594 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/.chainlit/translations/en-US.json
--rw-r--r--   0        0        0     5974 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/.chainlit/translations/pt-BR.json
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/__init__.py
--rw-r--r--   0        0        0     1930 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/app.py
--rw-r--r--   0        0        0     5273 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/app_terminal.py
--rw-r--r--   0        0        0     2761 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/chainlit.md
--rw-r--r--   0        0        0     1358 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/config.py
--rw-r--r--   0        0        0      254 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/database.py
--rw-r--r--   0        0        0      752 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/document_loader.py
--rw-r--r--   0        0        0     6148 2024-03-06 14:39:51.045954 akita_ai-0.1.102/akita/assistant/public/.DS_Store
--rw-r--r--   0        0        0    21277 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/assistant/public/favicon.png
--rw-r--r--   0        0        0    30151 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/assistant/public/logo_dark.png
--rw-r--r--   0        0        0    32611 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/assistant/public/logo_light.png
--rw-r--r--   0        0        0     1702 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/assistant/run.py
--rw-r--r--   0        0        0      543 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/assistant/text_splitter.py
--rw-r--r--   0        0        0     8196 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/__init__.py
--rw-r--r--   0        0        0     2313 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/cli.py
--rw-r--r--   0        0        0     2232 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/command_factory.py
--rw-r--r--   0        0        0     6148 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__init__.py
--rw-r--r--   0        0        0      177 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      925 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/add_command.cpython-311.pyc
--rw-r--r--   0        0        0      941 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/assistant_command.cpython-311.pyc
--rw-r--r--   0        0        0      980 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/base_command.cpython-311.pyc
--rw-r--r--   0        0        0     2775 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/describe_command.cpython-311.pyc
--rw-r--r--   0        0        0      907 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/init_command.cpython-311.pyc
--rw-r--r--   0        0        0     3074 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/readme_command.cpython-311.pyc
--rw-r--r--   0        0        0      984 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/remove_command.cpython-311.pyc
--rw-r--r--   0        0        0     3078 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/review_command.cpython-311.pyc
--rw-r--r--   0        0        0     1513 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/__pycache__/show_command.cpython-311.pyc
--rw-r--r--   0        0        0      246 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/add_command.py
--rw-r--r--   0        0        0      321 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/assistant_command.py
--rw-r--r--   0        0        0      432 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/base_command.py
--rw-r--r--   0        0        0     2157 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/describe_command.py
--rw-r--r--   0        0        0      238 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/init_command.py
--rw-r--r--   0        0        0     2417 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/readme_command.py
--rw-r--r--   0        0        0      276 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/remove_command.py
--rw-r--r--   0        0        0     2419 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/review_command.py
--rw-r--r--   0        0        0      627 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/commands/show_command.py
--rw-r--r--   0        0        0      304 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/config.py
--rw-r--r--   0        0        0     5970 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/main_parser.py
--rw-r--r--   0        0        0     2718 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/cli/plugin_manager.py
--rw-r--r--   0        0        0     8196 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/__init__.py
--rw-r--r--   0        0        0     2028 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/base_plugin.py
--rw-r--r--   0        0        0     6148 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__init__.py
--rw-r--r--   0        0        0      176 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      145 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     2298 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__pycache__/file_handler.cpython-37.pyc
--rw-r--r--   0        0        0     2460 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__pycache__/git_integration.cpython-37.pyc
--rw-r--r--   0        0        0     3156 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__pycache__/git_plugin.cpython-311.pyc
--rw-r--r--   0        0        0      549 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/commands/__init__.py
--rw-r--r--   0        0        0      185 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2443 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/commands/__pycache__/git_add_command.cpython-311.pyc
--rw-r--r--   0        0        0     3531 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/commands/__pycache__/git_commit_command.cpython-311.pyc
--rw-r--r--   0        0        0     1714 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/commands/git_add_command.py
--rw-r--r--   0        0        0     3232 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/commands/git_commit_command.py
--rw-r--r--   0        0        0     1586 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/git_plugin.py
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/utils/__init__.py
--rw-r--r--   0        0        0      182 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1853 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/utils/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     1165 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/git/utils/utils.py
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/__init__.py
--rw-r--r--   0        0        0      181 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1196 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/__pycache__/template_plugin.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/commands/__init__.py
--rw-r--r--   0        0        0      190 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      874 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/commands/__pycache__/template_dummy_command.cpython-311.pyc
--rw-r--r--   0        0        0      277 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/commands/template_dummy_command.py
--rw-r--r--   0        0        0      390 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/plugins/template/template_plugin.py
--rw-r--r--   0        0        0     6148 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/__init__.py
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__init__.py
--rw-r--r--   0        0        0      194 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5193 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__pycache__/file_handler.cpython-311.pyc
--rw-r--r--   0        0        0     4660 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__pycache__/prompt_builder.cpython-311.pyc
--rw-r--r--   0        0        0      664 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     9256 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__pycache__/text_generator.cpython-311.pyc
--rw-r--r--   0        0        0     1088 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     2856 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/file_handler.py
--rw-r--r--   0        0        0       33 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/models.json
--rw-r--r--   0        0        0     3058 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompt_builder.py
--rw-r--r--   0        0        0      732 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/commit_message_prompt.txt
--rw-r--r--   0        0        0      649 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/describe_code_diff_prompt.txt
--rw-r--r--   0        0        0      351 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/describe_files_prompt.txt
--rw-r--r--   0        0        0     1311 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/docstring_prompt.txt
--rw-r--r--   0        0        0     1916 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/inline_comments_prompt.txt
--rw-r--r--   0        0        0      749 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/readme_prompt.txt
--rw-r--r--   0        0        0     1556 2024-03-06 14:39:51.049954 akita_ai-0.1.102/akita/services/text_generation/prompts/review_prompt.txt
--rw-r--r--   0        0        0     2062 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/services/text_generation/prompts/tests_prompt.txt
--rw-r--r--   0        0        0      295 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/services/text_generation/settings.py
--rw-r--r--   0        0        0     6544 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/services/text_generation/text_generator.py
--rw-r--r--   0        0        0      390 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/services/text_generation/utils.py
--rw-r--r--   0        0        0        0 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/utils/__init__.py
--rw-r--r--   0        0        0      655 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/utils/console.py
--rw-r--r--   0        0        0    18446 2024-03-06 14:39:51.053954 akita_ai-0.1.102/akita/utils/file_handler.py
--rw-r--r--   0        0        0     1590 2024-03-06 14:39:51.053954 akita_ai-0.1.102/pyproject.toml
--rw-r--r--   0        0        0     5091 1970-01-01 00:00:00.000000 akita_ai-0.1.102/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-04-30 13:04:03.361675 akita_ai-0.1.200/LICENSE
+-rw-r--r--   0        0        0     4480 2024-04-30 13:04:03.361675 akita_ai-0.1.200/README.md
+-rw-r--r--   0        0        0    10244 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/__init__.py
+-rw-r--r--   0        0        0       70 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/api/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/api/base_ai_provider.py
+-rw-r--r--   0        0        0      221 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/api/config.toml
+-rw-r--r--   0        0        0     2323 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/api/google_genai_provider.py
+-rw-r--r--   0        0        0     1940 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/api/openai_provider.py
+-rw-r--r--   0        0        0     1453 2024-04-30 13:04:03.361675 akita_ai-0.1.200/akita/api/provider_factory.py
+-rw-r--r--   0        0        0     1543 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/api/utils/__pycache__/config_loader.cpython-311.pyc
+-rw-r--r--   0        0        0     1677 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/api/utils/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      540 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/api/utils/config_loader.py
+-rw-r--r--   0        0        0      422 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/api/utils/utils.py
+-rw-r--r--   0        0        0     8196 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/.DS_Store
+-rw-r--r--   0        0        0     2431 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/.chainlit/config.toml
+-rw-r--r--   0        0        0     5594 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/.chainlit/translations/en-US.json
+-rw-r--r--   0        0        0     5974 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/.chainlit/translations/pt-BR.json
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/app.py
+-rw-r--r--   0        0        0     3975 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/app_terminal.py
+-rw-r--r--   0        0        0     2761 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/chainlit.md
+-rw-r--r--   0        0        0     1358 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/config.py
+-rw-r--r--   0        0        0      249 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/database.py
+-rw-r--r--   0        0        0      752 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/document_loader.py
+-rw-r--r--   0        0        0     6148 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/public/.DS_Store
+-rw-r--r--   0        0        0    11009 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/public/favicon.png
+-rw-r--r--   0        0        0    44631 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/public/logo_dark.png
+-rw-r--r--   0        0        0    41138 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/public/logo_light.png
+-rw-r--r--   0        0        0     5102 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/rag_chain.py
+-rw-r--r--   0        0        0     1702 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/run.py
+-rw-r--r--   0        0        0      543 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/assistant/text_splitter.py
+-rw-r--r--   0        0        0     8196 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/__init__.py
+-rw-r--r--   0        0        0     2313 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/cli.py
+-rw-r--r--   0        0        0     2232 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/command_factory.py
+-rw-r--r--   0        0        0     6148 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__init__.py
+-rw-r--r--   0        0        0      177 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      925 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/add_command.cpython-311.pyc
+-rw-r--r--   0        0        0      941 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/assistant_command.cpython-311.pyc
+-rw-r--r--   0        0        0      980 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/base_command.cpython-311.pyc
+-rw-r--r--   0        0        0     2775 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/describe_command.cpython-311.pyc
+-rw-r--r--   0        0        0      907 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/init_command.cpython-311.pyc
+-rw-r--r--   0        0        0     3074 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/readme_command.cpython-311.pyc
+-rw-r--r--   0        0        0      984 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/remove_command.cpython-311.pyc
+-rw-r--r--   0        0        0     3078 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/review_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1513 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/__pycache__/show_command.cpython-311.pyc
+-rw-r--r--   0        0        0      246 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/add_command.py
+-rw-r--r--   0        0        0      321 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/assistant_command.py
+-rw-r--r--   0        0        0      432 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/base_command.py
+-rw-r--r--   0        0        0     2157 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/describe_command.py
+-rw-r--r--   0        0        0      238 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/init_command.py
+-rw-r--r--   0        0        0     2417 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/readme_command.py
+-rw-r--r--   0        0        0      276 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/remove_command.py
+-rw-r--r--   0        0        0     2419 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/review_command.py
+-rw-r--r--   0        0        0      627 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/commands/show_command.py
+-rw-r--r--   0        0        0      304 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/config.py
+-rw-r--r--   0        0        0     5970 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/main_parser.py
+-rw-r--r--   0        0        0     2718 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/cli/plugin_manager.py
+-rw-r--r--   0        0        0     8196 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/__init__.py
+-rw-r--r--   0        0        0     2028 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/base_plugin.py
+-rw-r--r--   0        0        0     6148 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      145 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0        0        0     2298 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__pycache__/file_handler.cpython-37.pyc
+-rw-r--r--   0        0        0     2460 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__pycache__/git_integration.cpython-37.pyc
+-rw-r--r--   0        0        0     3156 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__pycache__/git_plugin.cpython-311.pyc
+-rw-r--r--   0        0        0      549 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/commands/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2443 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/commands/__pycache__/git_add_command.cpython-311.pyc
+-rw-r--r--   0        0        0     3531 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/commands/__pycache__/git_commit_command.cpython-311.pyc
+-rw-r--r--   0        0        0     1714 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/commands/git_add_command.py
+-rw-r--r--   0        0        0     3232 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/commands/git_commit_command.py
+-rw-r--r--   0        0        0     1586 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/git_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/utils/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1853 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/utils/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     1165 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/git/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/template/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/template/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1196 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/template/__pycache__/template_plugin.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/template/commands/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/template/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      874 2024-04-30 13:04:03.365675 akita_ai-0.1.200/akita/plugins/template/commands/__pycache__/template_dummy_command.cpython-311.pyc
+-rw-r--r--   0        0        0      277 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/plugins/template/commands/template_dummy_command.py
+-rw-r--r--   0        0        0      390 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/plugins/template/template_plugin.py
+-rw-r--r--   0        0        0     6148 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5193 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__pycache__/file_handler.cpython-311.pyc
+-rw-r--r--   0        0        0     4660 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__pycache__/prompt_builder.cpython-311.pyc
+-rw-r--r--   0        0        0      664 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     9256 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__pycache__/text_generator.cpython-311.pyc
+-rw-r--r--   0        0        0     1088 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     2856 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/file_handler.py
+-rw-r--r--   0        0        0       33 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/models.json
+-rw-r--r--   0        0        0     3058 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompt_builder.py
+-rw-r--r--   0        0        0      732 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/commit_message_prompt.txt
+-rw-r--r--   0        0        0      649 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/describe_code_diff_prompt.txt
+-rw-r--r--   0        0        0      351 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/describe_files_prompt.txt
+-rw-r--r--   0        0        0     1311 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/docstring_prompt.txt
+-rw-r--r--   0        0        0     1916 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/inline_comments_prompt.txt
+-rw-r--r--   0        0        0      749 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/readme_prompt.txt
+-rw-r--r--   0        0        0     1556 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/review_prompt.txt
+-rw-r--r--   0        0        0     2062 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/prompts/tests_prompt.txt
+-rw-r--r--   0        0        0      295 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/settings.py
+-rw-r--r--   0        0        0     5599 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/text_generator.py
+-rw-r--r--   0        0        0      390 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/services/text_generation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/utils/__init__.py
+-rw-r--r--   0        0        0      655 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/utils/console.py
+-rw-r--r--   0        0        0    18446 2024-04-30 13:04:03.369675 akita_ai-0.1.200/akita/utils/file_handler.py
+-rw-r--r--   0        0        0     1655 2024-04-30 13:04:03.369675 akita_ai-0.1.200/pyproject.toml
+-rw-r--r--   0        0        0     5979 1970-01-01 00:00:00.000000 akita_ai-0.1.200/PKG-INFO
```

### Comparing `akita_ai-0.1.102/LICENSE` & `akita_ai-0.1.200/LICENSE`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/.DS_Store` & `akita_ai-0.1.200/akita/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/.DS_Store` & `akita_ai-0.1.200/akita/assistant/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/.chainlit/config.toml` & `akita_ai-0.1.200/akita/assistant/.chainlit/config.toml`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/.chainlit/translations/en-US.json` & `akita_ai-0.1.200/akita/assistant/.chainlit/translations/en-US.json`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/.chainlit/translations/pt-BR.json` & `akita_ai-0.1.200/akita/assistant/.chainlit/translations/pt-BR.json`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/app_terminal.py` & `akita_ai-0.1.200/akita/assistant/app_terminal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import asyncio
 from rich.console import Console
 from prompt_toolkit import PromptSession
 from rich.panel import Panel
 from prompt_toolkit.styles import Style
 from prompt_toolkit.history import InMemoryHistory
-from akita.assistant.config import MODEL_NAME, SEARCH_TYPE, SEARCH_K, HELP_MESSAGE
-from akita.assistant.document_loader import load_documents
-from akita.assistant.text_splitter import split_texts
-from akita.assistant.database import create_database
-from langchain.memory import ConversationBufferMemory
-from langchain_openai import ChatOpenAI
-from langchain.chains import ConversationalRetrievalChain
-from typing import Dict, Any, List, NoReturn
+from akita.assistant.config import SEARCH_TYPE, SEARCH_K, HELP_MESSAGE
+from akita.assistant.rag_chain import RAGChain
+from akita.api.provider_factory import ProviderFactory
+from typing import NoReturn
+from langchain.schema.runnable import RunnablePassthrough
 
 
 console = Console()
 
 # Define a custom style for the prompt
 custom_style = Style.from_dict({"prompt": "#248542"})
 
@@ -24,15 +21,15 @@
     """A terminal-based chat interface for interacting with the Akita Assistant.
 
     This class provides an interactive command-line interface for users to interact
     with the Akita Assistant.
 
     Attributes:
         session (PromptSession): A prompt session for capturing user input.
-        qa (ConversationalRetrievalChain): The conversational retrieval chain
+        rag_chain (RAGChain): The conversational retrieval chain
             responsible for processing user queries and generating responses.
     """
 
     def __init__(self) -> None:
         """Initializes the TerminalChat with a custom prompt session
         and setups up the assistant."""
         self.session: PromptSession = PromptSession(
@@ -42,69 +39,44 @@
 
     def setup(self) -> None:
         """Sets up the conversational components and the QA chain for the assistant.
 
         Loads documents, splits texts, creates the database, and initializes the
         conversational retrieval chain.
         """
-        documents: List[Dict[str, Any]] = load_documents()
-        texts: List[str] = split_texts(documents)
-        db = create_database(texts)
-        retriever = db.as_retriever(
-            search_type=SEARCH_TYPE, search_kwargs={"k": SEARCH_K}
-        )
-        llm: ChatOpenAI = ChatOpenAI(model_name=MODEL_NAME)
-        memory: ConversationBufferMemory = ConversationBufferMemory(
-            llm=llm,
-            memory_key="chat_history",
-            return_messages=True,
-            output_key="answer",
-        )
-        self.qa: ConversationalRetrievalChain = ConversationalRetrievalChain.from_llm(
-            llm,
-            retriever=retriever,
-            memory=memory,
-            chain_type="stuff",
-            return_source_documents=True,
-        )
+        ai_provider = ProviderFactory.get_provider()
+        self.rag_chain: RunnablePassthrough = RAGChain(
+            ai_provider, SEARCH_TYPE, SEARCH_K
+        ).create_runnable()
 
-    def process_answer(self, response: Dict[str, Any]) -> str:
+    def process_answer(self, response: str) -> str:
         """Processes the response from the QA chain to generate a human-readable answer.
 
         Args:
-            response (Dict[str, Any]): The response from the QA chain.
+            response (str): The response from the QA chain.
 
         Returns:
             str: The processed answer ready to be displayed to the user.
         """
-        answer: str = response["answer"]
-        source_documents: List[Dict[str, Any]] = response.get("source_documents", [])
-        if source_documents:
-            source_info: List[str] = [
-                doc.metadata.get("source", "Unknown Filename")
-                for doc in source_documents
-            ]
-            source_info = list(set(source_info))
-            # answer += f"\n\nSources: {', '.join(source_info)}"
-            # if source_info else "\n\nNo sources found"
+        answer: str = response
         return answer
 
     async def handle_user_input(self, user_input: str) -> NoReturn:
         """Asynchronously handles user input, processing it
            through the QA chain and displaying the response.
 
         Args:
             user_input (str): The user's input string to be processed.
 
         Raises:
             NoReturn: This function is designed to run indefinitely,
             handling user input.
         """
         with console.status("Thinking...", spinner="dots"):
-            response = await self.qa.ainvoke(user_input)
+            response = self.rag_chain.invoke(user_input)
 
         answer = self.process_answer(response)
         chat_response = f"[blue]Akita:[/blue] {answer}"
         console.print(chat_response)
 
     def display_help(self) -> None:
         """Displays help information about using the Akita Assistant."""
@@ -116,15 +88,15 @@
 
         This method sets up the event loop, captures user inputs, and handles clean-up
         and exit procedures.
         """
         console.print("Welcome to the Akita Assistant!", style="blue")
         self.display_help()
 
-        loop = asyncio.get_event_loop()  # Get the existing event loop
+        loop = asyncio.get_event_loop()
 
         while True:
             try:
                 user_input: str = self.session.prompt("You: ")
                 if user_input.lower() in ["exit", "quit"]:
                     console.print("Exiting...", style="red")
                     break
```

### Comparing `akita_ai-0.1.102/akita/assistant/chainlit.md` & `akita_ai-0.1.200/akita/assistant/chainlit.md`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/config.py` & `akita_ai-0.1.200/akita/assistant/config.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/document_loader.py` & `akita_ai-0.1.200/akita/assistant/document_loader.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/public/.DS_Store` & `akita_ai-0.1.200/akita/assistant/public/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/run.py` & `akita_ai-0.1.200/akita/assistant/run.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/assistant/text_splitter.py` & `akita_ai-0.1.200/akita/assistant/text_splitter.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/.DS_Store` & `akita_ai-0.1.200/akita/cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/cli.py` & `akita_ai-0.1.200/akita/cli/cli.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/command_factory.py` & `akita_ai-0.1.200/akita/cli/command_factory.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/.DS_Store` & `akita_ai-0.1.200/akita/cli/commands/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/add_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/add_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/assistant_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/assistant_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/base_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/base_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/describe_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/describe_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/init_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/init_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/readme_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/readme_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/remove_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/remove_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/review_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/review_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/__pycache__/show_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/cli/commands/__pycache__/show_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/describe_command.py` & `akita_ai-0.1.200/akita/cli/commands/describe_command.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/readme_command.py` & `akita_ai-0.1.200/akita/cli/commands/readme_command.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/review_command.py` & `akita_ai-0.1.200/akita/cli/commands/review_command.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/commands/show_command.py` & `akita_ai-0.1.200/akita/cli/commands/show_command.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/main_parser.py` & `akita_ai-0.1.200/akita/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/cli/plugin_manager.py` & `akita_ai-0.1.200/akita/cli/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/.DS_Store` & `akita_ai-0.1.200/akita/plugins/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/base_plugin.py` & `akita_ai-0.1.200/akita/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/.DS_Store` & `akita_ai-0.1.200/akita/plugins/git/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/__pycache__/file_handler.cpython-37.pyc` & `akita_ai-0.1.200/akita/plugins/git/__pycache__/file_handler.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/__pycache__/git_integration.cpython-37.pyc` & `akita_ai-0.1.200/akita/plugins/git/__pycache__/git_integration.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/__pycache__/git_plugin.cpython-311.pyc` & `akita_ai-0.1.200/akita/plugins/git/__pycache__/git_plugin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/__pycache__/utils.cpython-37.pyc` & `akita_ai-0.1.200/akita/plugins/git/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/commands/__pycache__/git_add_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/plugins/git/commands/__pycache__/git_add_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/commands/__pycache__/git_commit_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/plugins/git/commands/__pycache__/git_commit_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/commands/git_add_command.py` & `akita_ai-0.1.200/akita/plugins/git/commands/git_add_command.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/commands/git_commit_command.py` & `akita_ai-0.1.200/akita/plugins/git/commands/git_commit_command.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/git_plugin.py` & `akita_ai-0.1.200/akita/plugins/git/git_plugin.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/utils/__pycache__/utils.cpython-311.pyc` & `akita_ai-0.1.200/akita/plugins/git/utils/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/git/utils/utils.py` & `akita_ai-0.1.200/akita/plugins/git/utils/utils.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/template/__pycache__/template_plugin.cpython-311.pyc` & `akita_ai-0.1.200/akita/plugins/template/__pycache__/template_plugin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/plugins/template/commands/__pycache__/template_dummy_command.cpython-311.pyc` & `akita_ai-0.1.200/akita/plugins/template/commands/__pycache__/template_dummy_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/.DS_Store` & `akita_ai-0.1.200/akita/services/.DS_Store`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/__pycache__/file_handler.cpython-311.pyc` & `akita_ai-0.1.200/akita/services/text_generation/__pycache__/file_handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/__pycache__/prompt_builder.cpython-311.pyc` & `akita_ai-0.1.200/akita/services/text_generation/__pycache__/prompt_builder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/__pycache__/settings.cpython-311.pyc` & `akita_ai-0.1.200/akita/services/text_generation/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/__pycache__/text_generator.cpython-311.pyc` & `akita_ai-0.1.200/akita/services/text_generation/__pycache__/text_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/__pycache__/utils.cpython-311.pyc` & `akita_ai-0.1.200/akita/services/text_generation/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/file_handler.py` & `akita_ai-0.1.200/akita/services/text_generation/file_handler.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompt_builder.py` & `akita_ai-0.1.200/akita/services/text_generation/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/commit_message_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/commit_message_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/describe_code_diff_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/describe_code_diff_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/docstring_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/docstring_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/inline_comments_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/inline_comments_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/readme_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/readme_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/review_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/review_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/prompts/tests_prompt.txt` & `akita_ai-0.1.200/akita/services/text_generation/prompts/tests_prompt.txt`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/services/text_generation/text_generator.py` & `akita_ai-0.1.200/akita/services/text_generation/text_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,123 @@
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, List, Optional, Union
+import os
 from akita.services.text_generation.prompt_builder import PromptBuilder
 from akita.services.text_generation.file_handler import FileHandler
-from akita.api.openai_client import OpenAIClient
+from akita.api.base_ai_provider import AIProvider
+from akita.api.provider_factory import ProviderFactory
 from .settings import Settings
-from .utils import load_model_config
-import os
 
 
 class TextGenerator:
     """
-    Generates various types of text content using OpenAI's GPT models,
+    Generates various types of text content using AI models,
     based on the provided code content.
 
     Attributes:
-        model_config (Dict[str, Any]): Configuration for the models
-                                       used in generating text.
         file_handler (FileHandler): Handles file operations,
                                     like reading files to get their content.
-        chatgpt_client (OpenAIClient): Client for calling OpenAI's API to generate text.
+        ai_provider (AIProvider): An AI provider conforming to the AIProvider interface,
+                              used to generate text.
         prompt_builder (PromptBuilder): Builds prompts for the AI based on templates.
     """
 
     def __init__(self) -> None:
-        self.model_config: Dict[str, Any] = load_model_config(
-            Settings.MODEL_CONFIG_FILE
-        )
         self.file_handler: FileHandler = FileHandler()
-        self.chatgpt_client: OpenAIClient = OpenAIClient()
+        self.ai_provider: AIProvider = ProviderFactory.get_provider()
         self.prompt_builder: PromptBuilder = PromptBuilder(
             prompts_dir=Settings.DEFAULT_PROMPT_DIR
         )
 
     def generate_docstring(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("docstring", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=3000, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=3000)
 
     def generate_inline_comments(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("inline_comments", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=4000, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=4000)
 
     def generate_description_files(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("describe_files", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=4000, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=4000)
 
     def generate_description_code_diff(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("describe_code_diff", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=500, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=500)
 
     def generate_commit_message(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("commit_message", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=60, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=60)
 
     def generate_readme(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("readme", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=3000, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=3000)
 
     def generate_review(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("review", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=3000, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=3000)
 
     def generate_tests(
         self,
         input_data: Union[str, List[str]],
-        model: str = "default",
         verbosity: Optional[str] = None,
         language: Optional[str] = None,
     ) -> Any:
         self._prepare_prompt_builder(verbosity, language)
         code_content: str = self._process_input(input_data)
         prompt: str = self.prompt_builder.get_prompt("tests", code_content)
-        return self.chatgpt_client.call_openai_api(
-            prompt, max_tokens=3000, model=self.model_config[model]
-        )
+        return self.ai_provider.call_api(prompt, max_tokens=3000)
 
     def _prepare_prompt_builder(
         self, verbosity: Optional[str], language: Optional[str]
     ) -> None:
         self.prompt_builder.verbosity = (
             verbosity if verbosity else Settings.DEFAULT_VERBOSITY
         )
```

### Comparing `akita_ai-0.1.102/akita/utils/console.py` & `akita_ai-0.1.200/akita/utils/console.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/akita/utils/file_handler.py` & `akita_ai-0.1.200/akita/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `akita_ai-0.1.102/pyproject.toml` & `akita_ai-0.1.200/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "akita-ai"
-version = "0.1.102"
+version = "0.1.200"
 description = "AI-enhanced development tool."
 authors = ["Gauthier Piarrette <gauthier@akita.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://akita.ai"
 repository = "https://github.com/gauthierpiarrette/akita-ai"
 documentation = "https://github.com/gauthierpiarrette/akita-ai"
@@ -18,24 +18,26 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 openai = "1.10.0"
 rich = "12.6.0"
 langchain = "0.1.9"
 langchain-community = "0.0.24"
-langchain-core = "0.1.26"
+langchain-core = "0.1.45"
 langchain-openai = "0.0.7"
 tiktoken = "0.6.0"
 tree-sitter = "0.20.4"
 tree-sitter-languages = "1.10.2"
 chromadb = "0.4.23"
 onnxruntime = "1.16.0"
 chardet = "5.1.0"
 prompt-toolkit = "3.0.43"
 chainlit = "1.0.0"
+google-generativeai = "^0.5.2"
+langchain-google-genai = "^1.0.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-mock = "^3.6.1"
 black = {version = "^22.3", allow-prereleases = true}
 flake8 = "^3.9.2"
```

