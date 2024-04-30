# Comparing `tmp/picomet-0.0.8.tar.gz` & `tmp/picomet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picomet-0.0.8.tar", last modified: Tue Mar 26 11:04:49 2024, max compression
+gzip compressed data, was "picomet-0.0.9.tar", last modified: Tue Mar 26 20:22:04 2024, max compression
```

## Comparing `picomet-0.0.8.tar` & `picomet-0.0.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.429283 picomet-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-26 11:04:31.000000 picomet-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 11:04:31.000000 picomet-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-26 11:04:49.429283 picomet-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-26 11:04:31.000000 picomet-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-26 11:04:31.000000 picomet-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 11:04:49.429283 picomet-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-26 11:04:31.000000 picomet-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.413282 picomet-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.417282 picomet-0.0.8/src/picomet/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.413282 picomet-0.0.8/src/picomet/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.421282 picomet-0.0.8/src/picomet/assets/picomet/
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-03-26 11:04:41.000000 picomet-0.0.8/src/picomet/assets/picomet/comet.js
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/assets/picomet/comet.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-26 11:04:40.000000 picomet-0.0.8/src/picomet/assets/picomet/hmr.js
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/assets/picomet/hmr.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.421282 picomet-0.0.8/src/picomet/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/backends/picomet.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/copier.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.413282 picomet-0.0.8/src/picomet/management/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.421282 picomet-0.0.8/src/picomet/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/management/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/management/commands/newapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/management/commands/recompile.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.421282 picomet-0.0.8/src/picomet/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29170 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/sockets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.421282 picomet-0.0.8/src/picomet/template/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/.env.example.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/.env.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.421282 picomet-0.0.8/src/picomet/template/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.425282 picomet-0.0.8/src/picomet/template/apps/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.425282 picomet-0.0.8/src/picomet/template/apps/core/comets/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/comets/Index.css
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/comets/Index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.425282 picomet-0.0.8/src/picomet/template/apps/core/comets/components/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/comets/components/Arrow.html
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/apps/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.425282 picomet-0.0.8/src/picomet/template/comets/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/comets/Base.html.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/comets/{% if Tailwind %}base.postcss.js{% endif %}.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/comets/{% if Tailwind %}base.tailwind.css{% endif %}.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/comets/{% if Tailwind %}base.tailwind.js{% endif %}.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/copier.yml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.425282 picomet-0.0.8/src/picomet/template/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.425282 picomet-0.0.8/src/picomet/template/project/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/settings/base.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/settings/dev.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/settings/pro.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/project/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.429283 picomet-0.0.8/src/picomet/template/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/requirements/base.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/requirements/dev.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/{% if Precommit %}.pre-commit-config.yaml{% endif %}.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/{% if Ruff %}pyproject.toml{% endif %}.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/{% if Tailwind or Prettier %}package.json{% endif %}.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.429283 picomet-0.0.8/src/picomet/template/{% if VSCode %}.vscode{% endif %}/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/{% if VSCode %}.vscode{% endif %}/extensions.json.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/{% if VSCode %}.vscode{% endif %}/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/template/{% if VSCode %}.vscode{% endif %}/settings.json.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    23020 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-26 11:04:31.000000 picomet-0.0.8/src/picomet/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:04:49.429283 picomet-0.0.8/src/picomet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-26 11:04:49.000000 picomet-0.0.8/src/picomet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-26 11:04:49.000000 picomet-0.0.8/src/picomet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:04:49.000000 picomet-0.0.8/src/picomet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 11:04:49.000000 picomet-0.0.8/src/picomet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 11:04:49.000000 picomet-0.0.8/src/picomet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.843758 picomet-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-26 20:21:32.000000 picomet-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 20:21:32.000000 picomet-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-26 20:22:04.843758 picomet-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-26 20:21:32.000000 picomet-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-26 20:21:32.000000 picomet-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 20:22:04.843758 picomet-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-26 20:21:32.000000 picomet-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.827758 picomet-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.831758 picomet-0.0.9/src/picomet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.827758 picomet-0.0.9/src/picomet/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.835758 picomet-0.0.9/src/picomet/assets/picomet/
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-03-26 20:21:49.000000 picomet-0.0.9/src/picomet/assets/picomet/comet.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/assets/picomet/comet.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-26 20:21:49.000000 picomet-0.0.9/src/picomet/assets/picomet/hmr.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/assets/picomet/hmr.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.835758 picomet-0.0.9/src/picomet/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/backends/picomet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/copier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.827758 picomet-0.0.9/src/picomet/management/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.835758 picomet-0.0.9/src/picomet/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/management/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/management/commands/newapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/management/commands/recompile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.835758 picomet-0.0.9/src/picomet/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29170 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/sockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.835758 picomet-0.0.9/src/picomet/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/.env.example.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/.env.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.835758 picomet-0.0.9/src/picomet/template/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.839758 picomet-0.0.9/src/picomet/template/apps/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.839758 picomet-0.0.9/src/picomet/template/apps/core/comets/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/comets/Index.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/comets/Index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.839758 picomet-0.0.9/src/picomet/template/apps/core/comets/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/comets/components/Arrow.html
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/apps/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.839758 picomet-0.0.9/src/picomet/template/comets/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/comets/Base.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/comets/{% if Tailwind %}base.postcss.js{% endif %}.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/comets/{% if Tailwind %}base.tailwind.css{% endif %}.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/comets/{% if Tailwind %}base.tailwind.js{% endif %}.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/copier.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.839758 picomet-0.0.9/src/picomet/template/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.843758 picomet-0.0.9/src/picomet/template/project/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/settings/base.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/settings/dev.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/settings/pro.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/project/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.843758 picomet-0.0.9/src/picomet/template/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/requirements/base.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/requirements/dev.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/{% if Precommit %}.pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/{% if Ruff %}pyproject.toml{% endif %}.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/{% if Tailwind or Prettier %}package.json{% endif %}.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.843758 picomet-0.0.9/src/picomet/template/{% if VSCode %}.vscode{% endif %}/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/{% if VSCode %}.vscode{% endif %}/extensions.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/{% if VSCode %}.vscode{% endif %}/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/template/{% if VSCode %}.vscode{% endif %}/settings.json.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23020 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-26 20:21:32.000000 picomet-0.0.9/src/picomet/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:22:04.843758 picomet-0.0.9/src/picomet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-26 20:22:04.000000 picomet-0.0.9/src/picomet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-03-26 20:22:04.000000 picomet-0.0.9/src/picomet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:22:04.000000 picomet-0.0.9/src/picomet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-26 20:22:04.000000 picomet-0.0.9/src/picomet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 20:22:04.000000 picomet-0.0.9/src/picomet.egg-info/top_level.txt
```

### Comparing `picomet-0.0.8/LICENSE` & `picomet-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/PKG-INFO` & `picomet-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picomet
-Version: 0.0.8
+Version: 0.0.9
 Summary: The nextjs of django
 Author-email: Al Mahdi <picometproject@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Al Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `picomet-0.0.8/README.md` & `picomet-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/pyproject.toml` & `picomet-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "picomet"
-version = "0.0.8"
+version = "0.0.9"
 authors = [{ name = "Al Mahdi", email = "picometproject@gmail.com" }]
 license = { file = "LICENSE" }
 description = "The nextjs of django"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = []
 classifiers = [
```

### Comparing `picomet-0.0.8/src/picomet/__init__.py` & `picomet-0.0.9/src/picomet/__init__.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/assets/picomet/comet.js` & `picomet-0.0.9/src/picomet/assets/picomet/comet.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -296,15 +296,15 @@
                             linkElement.rel = "stylesheet";
                             linkElement.href = partial.css[id];
                             linkElement.setAttribute("data-style-id", id);
                             document.head.appendChild(linkElement);
                         }
                     }
                     for (const id in partial.js) {
-                        if (!window[`${id}_cleanup`]) {
+                        if (!document.querySelector(`[data-script-id="${id}"]`)) {
                             import(partial.js[id]).then((module) => {
                                 Object.keys(module).forEach((key) => {
                                     if (key == "cleanup") {
                                         window[`${id}_cleanup`] = module[key];
                                     } else {
                                         window[key] = module[key];
                                     }
```

### Comparing `picomet-0.0.8/src/picomet/assets/picomet/comet.ts` & `picomet-0.0.9/src/picomet/assets/picomet/comet.ts`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
             linkElement.rel = "stylesheet";
             linkElement.href = partial.css[id];
             linkElement.setAttribute("data-style-id", id);
             document.head.appendChild(linkElement);
           }
         }
         for (const id in partial.js) {
-          if (!window[`${id}_cleanup`]) {
+          if (!document.querySelector(`[data-script-id="${id}"]`)) {
             import(partial.js[id])
               .then((module: object) => {
                 Object.keys(module).forEach((key) => {
                   if (key == "cleanup") {
                     window[`${id}_cleanup`] = module[key] as unknown;
                   } else {
                     window[key] = module[key] as unknown;
```

### Comparing `picomet-0.0.8/src/picomet/assets/picomet/hmr.js` & `picomet-0.0.9/src/picomet/assets/picomet/hmr.js`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/assets/picomet/hmr.ts` & `picomet-0.0.9/src/picomet/assets/picomet/hmr.ts`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/backends/picomet.py` & `picomet-0.0.9/src/picomet/backends/picomet.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/compiler.py` & `picomet-0.0.9/src/picomet/compiler.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/consumers.py` & `picomet-0.0.9/src/picomet/consumers.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/decorators.py` & `picomet-0.0.9/src/picomet/decorators.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/loaders.py` & `picomet-0.0.9/src/picomet/loaders.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/management/commands/build.py` & `picomet-0.0.9/src/picomet/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/management/commands/newapp.py` & `picomet-0.0.9/src/picomet/management/commands/newapp.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/management/commands/recompile.py` & `picomet-0.0.9/src/picomet/management/commands/recompile.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/middleware.py` & `picomet-0.0.9/src/picomet/middleware.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/parser.py` & `picomet-0.0.9/src/picomet/parser.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/apps/core/comets/Index.css` & `picomet-0.0.9/src/picomet/template/apps/core/comets/Index.css`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/apps/core/comets/Index.html` & `picomet-0.0.9/src/picomet/template/apps/core/comets/Index.html`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/comets/Base.html.jinja` & `picomet-0.0.9/src/picomet/template/comets/Base.html.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <!doctype html>
 <html lang="en">
 
 <head>
   <meta charset="UTF-8" />
   <meta http-equiv="X-UA-Compatible" content="IE=edge" />
-  <meta name="viewport" content="width=device-width, initial-scale=1.0" />{% if Tailwind %}
+  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
+  <Group name="styles" />{% if Tailwind %}
   <Tailwind @="base" />{% endif %}
   <Js @="picomet/comet.js" defer />
   <script
     src="https://cdnjs.cloudflare.com/ajax/libs/alpinejs/3.13.7/cdn.min.js"
     integrity="sha512-kJ22SdASORIix8XIrKdqHU4+nBMOg5qAWigToRMshSGut+Nn6axu6cfecNay5piPo/v9QZYI38ZIGQw2tlCaYQ=="
     crossorigin="anonymous"
     defer
```

### Comparing `picomet-0.0.8/src/picomet/template/manage.py` & `picomet-0.0.9/src/picomet/template/manage.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/project/asgi.py` & `picomet-0.0.9/src/picomet/template/project/asgi.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/project/settings/base.py.jinja` & `picomet-0.0.9/src/picomet/template/project/settings/base.py.jinja`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/project/settings/pro.py.jinja` & `picomet-0.0.9/src/picomet/template/project/settings/pro.py.jinja`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/project/urls.py` & `picomet-0.0.9/src/picomet/template/project/urls.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/template/{% if Precommit %}.pre-commit-config.yaml{% endif %}.jinja` & `picomet-0.0.9/src/picomet/template/{% if Precommit %}.pre-commit-config.yaml{% endif %}.jinja`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 repos:{% if Ruff %}
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: v0.3.4
     hooks:
       - id: ruff
-      - id: ruff-format{% endif %}
+      - id: ruff-format{% endif %}{% if Prettier %}
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v3.1.0
+    hooks:
+      - id: prettier{% endif %}
   - repo: local
     hooks:
       - id: check-absent-migrations
         name: Check absent migrations
         entry: python manage.py makemigrations --check
         pass_filenames: false
         language: system
```

### Comparing `picomet-0.0.8/src/picomet/template/{% if VSCode %}.vscode{% endif %}/settings.json.jinja` & `picomet-0.0.9/src/picomet/template/{% if VSCode %}.vscode{% endif %}/settings.json.jinja`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/transformer.py` & `picomet-0.0.9/src/picomet/transformer.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/utils.py` & `picomet-0.0.9/src/picomet/utils.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet/views.py` & `picomet-0.0.9/src/picomet/views.py`

 * *Files identical despite different names*

### Comparing `picomet-0.0.8/src/picomet.egg-info/PKG-INFO` & `picomet-0.0.9/src/picomet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picomet
-Version: 0.0.8
+Version: 0.0.9
 Summary: The nextjs of django
 Author-email: Al Mahdi <picometproject@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Al Mahdi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `picomet-0.0.8/src/picomet.egg-info/SOURCES.txt` & `picomet-0.0.9/src/picomet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

