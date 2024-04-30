# Comparing `tmp/nautobot_show_tech-2.0.1.tar.gz` & `tmp/nautobot_show_tech-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_show_tech-2.0.1.tar", max compression
+gzip compressed data, was "nautobot_show_tech-2.0.2.tar", max compression
```

## Comparing `nautobot_show_tech-2.0.1.tar` & `nautobot_show_tech-2.0.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      591 2024-04-29 22:10:42.144477 nautobot_show_tech-2.0.1/LICENSE
--rw-r--r--   0        0        0     3012 2024-04-29 22:10:42.144477 nautobot_show_tech-2.0.1/README.md
--rw-r--r--   0        0        0      973 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/__init__.py
--rw-r--r--   0        0        0       44 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/api/__init__.py
--rw-r--r--   0        0        0     2826 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/helpers.py
--rw-r--r--   0        0        0     4676 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/jobs.py
--rw-r--r--   0        0        0     1152 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_apps.py
--rw-r--r--   0        0        0     2190 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_counts.py
--rw-r--r--   0        0        0     1242 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_django_settings.py
--rw-r--r--   0        0        0     2466 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_jobs.py
--rw-r--r--   0        0        0        0 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/migrations/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/run_check.py
--rw-r--r--   0        0        0     4438 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/README.md
--rw-r--r--   0        0        0       75 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/__init__.py
--rw-r--r--   0        0        0      632 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/alias.yaml
--rw-r--r--   0        0        0      447 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/ansible_version.yaml
--rw-r--r--   0        0        0      467 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/available_commands.yaml
--rw-r--r--   0        0        0      305 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/date.yaml
--rw-r--r--   0        0        0      517 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/disk_space.yaml
--rw-r--r--   0        0        0      424 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/dns.yaml
--rw-r--r--   0        0        0      491 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/host_uptime.yaml
--rw-r--r--   0        0        0      372 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/hostname.yaml
--rw-r--r--   0        0        0      449 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/lscpu.yaml
--rw-r--r--   0        0        0      415 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/meminfo.yaml
--rw-r--r--   0        0        0      700 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml
--rw-r--r--   0        0        0      697 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml
--rw-r--r--   0        0        0      730 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml
--rw-r--r--   0        0        0      713 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml
--rw-r--r--   0        0        0      703 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml
--rw-r--r--   0        0        0      535 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml
--rw-r--r--   0        0        0      395 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/os-release.yaml
--rw-r--r--   0        0        0      565 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pip_freeze.yaml
--rw-r--r--   0        0        0      383 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pip_version.yaml
--rw-r--r--   0        0        0      422 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pwd.yaml
--rw-r--r--   0        0        0      395 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/python_version.yaml
--rw-r--r--   0        0        0     4280 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/subprocess_run.py
--rw-r--r--   0        0        0      449 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/uname_a.yaml
--rw-r--r--   0        0        0      371 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/which_pip.yaml
--rw-r--r--   0        0        0      383 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/which_python.yaml
--rw-r--r--   0        0        0      366 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/whoami.yaml
--rw-r--r--   0        0        0    30314 2024-04-29 22:11:05.940513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/404.html
--rw-r--r--   0        0        0    33918 2024-04-29 22:11:05.960513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html
--rw-r--r--   0        0        0    40791 2024-04-29 22:11:05.964513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html
--rw-r--r--   0        0        0    33401 2024-04-29 22:11:05.972513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html
--rw-r--r--   0        0        0    39294 2024-04-29 22:11:05.972513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html
--rw-r--r--   0        0        0    34846 2024-04-29 22:11:05.964513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html
--rw-r--r--   0        0        0    34763 2024-04-29 22:11:05.968513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html
--rw-r--r--   0        0        0     1000 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     4805 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css
--rw-r--r--   0        0        0    15086 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico
--rw-r--r--   0        0        0     1870 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   113489 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js
--rw-r--r--   0        0        0   954781 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map
--rw-r--r--   0        0        0    17074 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0     1264 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js
--rw-r--r--   0        0        0    11232 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     3494 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js
--rw-r--r--   0        0        0     7972 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     4901 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js
--rw-r--r--   0        0        0     3647 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     2330 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js
--rw-r--r--   0        0        0     1031 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2158 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677463 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0     9204 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png
--rw-r--r--   0        0        0    13318 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg
--rw-r--r--   0        0        0     7562 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png
--rw-r--r--   0        0        0      846 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html
--rw-r--r--   0        0        0   113505 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css
--rw-r--r--   0        0        0    38975 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map
--rw-r--r--   0        0        0    12245 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css
--rw-r--r--   0        0        0     3639 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map
--rw-r--r--   0        0        0    33963 2024-04-29 22:11:06.008513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html
--rw-r--r--   0        0        0    33682 2024-04-29 22:11:06.004513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html
--rw-r--r--   0        0        0    40314 2024-04-29 22:11:06.012513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html
--rw-r--r--   0        0        0    38617 2024-04-29 22:11:05.976513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html
--rw-r--r--   0        0        0    94815 2024-04-29 22:11:05.996513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html
--rw-r--r--   0        0        0    35509 2024-04-29 22:11:06.000513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html
--rw-r--r--   0        0        0    45941 2024-04-29 22:11:06.004513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html
--rw-r--r--   0        0        0    40260 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-nautobot-show-tech.png
--rw-r--r--   0        0        0    40260 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.png
--rw-r--r--   0        0        0    10398 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.svg
--rw-r--r--   0        0        0  1150397 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_example.webm
--rw-r--r--   0        0        0   217106 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_meminfo.png
--rw-r--r--   0        0        0   814242 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_example.webm
--rw-r--r--   0        0        0   347891 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_result.png
--rw-r--r--   0        0        0   301965 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_run.png
--rw-r--r--   0        0        0    39833 2024-04-29 22:11:05.956513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/index.html
--rw-r--r--   0        0        0      259 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/objects.inv
--rw-r--r--   0        0        0      120 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/requirements.txt
--rw-r--r--   0        0        0    49323 2024-04-29 22:11:06.024513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json
--rw-r--r--   0        0        0     3245 2024-04-29 22:11:05.832514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml
--rw-r--r--   0        0        0      388 2024-04-29 22:11:05.832514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    36675 2024-04-29 22:11:06.016513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html
--rw-r--r--   0        0        0    36378 2024-04-29 22:11:06.020513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html
--rw-r--r--   0        0        0    34678 2024-04-29 22:11:06.020513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html
--rw-r--r--   0        0        0    34448 2024-04-29 22:11:06.024513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html
--rw-r--r--   0        0        0       45 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/tests/__init__.py
--rw-r--r--   0        0        0      992 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_api.py
--rw-r--r--   0        0        0     1042 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_basic.py
--rwxr-xr-x   0        0        0     1942 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/update_readme.py
--rw-r--r--   0        0        0     5543 2024-04-29 22:10:50.288492 nautobot_show_tech-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 nautobot_show_tech-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-30 14:30:43.217617 nautobot_show_tech-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3402 2024-04-30 14:30:43.217617 nautobot_show_tech-2.0.2/README.md
+-rw-r--r--   0        0        0      973 2024-04-30 14:30:43.229617 nautobot_show_tech-2.0.2/nautobot_show_tech/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/api/__init__.py
+-rw-r--r--   0        0        0     2826 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/helpers.py
+-rw-r--r--   0        0        0     4676 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/jobs.py
+-rw-r--r--   0        0        0     1152 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_apps.py
+-rw-r--r--   0        0        0     2190 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_counts.py
+-rw-r--r--   0        0        0     1242 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_django_settings.py
+-rw-r--r--   0        0        0     2466 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_jobs.py
+-rw-r--r--   0        0        0        0 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/migrations/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/run_check.py
+-rw-r--r--   0        0        0     4438 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/README.md
+-rw-r--r--   0        0        0       75 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/alias.yaml
+-rw-r--r--   0        0        0      447 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/ansible_version.yaml
+-rw-r--r--   0        0        0      467 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/available_commands.yaml
+-rw-r--r--   0        0        0      305 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/date.yaml
+-rw-r--r--   0        0        0      517 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/disk_space.yaml
+-rw-r--r--   0        0        0      424 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/dns.yaml
+-rw-r--r--   0        0        0      491 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/host_uptime.yaml
+-rw-r--r--   0        0        0      372 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/hostname.yaml
+-rw-r--r--   0        0        0      449 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/lscpu.yaml
+-rw-r--r--   0        0        0      415 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/meminfo.yaml
+-rw-r--r--   0        0        0      700 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml
+-rw-r--r--   0        0        0      697 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml
+-rw-r--r--   0        0        0      730 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml
+-rw-r--r--   0        0        0      713 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml
+-rw-r--r--   0        0        0      703 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml
+-rw-r--r--   0        0        0      535 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml
+-rw-r--r--   0        0        0      395 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/os-release.yaml
+-rw-r--r--   0        0        0      565 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/pip_freeze.yaml
+-rw-r--r--   0        0        0      383 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/pip_version.yaml
+-rw-r--r--   0        0        0      422 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/pwd.yaml
+-rw-r--r--   0        0        0      395 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/python_version.yaml
+-rw-r--r--   0        0        0     4280 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/subprocess_run.py
+-rw-r--r--   0        0        0      449 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/uname_a.yaml
+-rw-r--r--   0        0        0      371 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/which_pip.yaml
+-rw-r--r--   0        0        0      383 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/which_python.yaml
+-rw-r--r--   0        0        0      366 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/whoami.yaml
+-rw-r--r--   0        0        0    30314 2024-04-30 14:31:08.693420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/404.html
+-rw-r--r--   0        0        0    33918 2024-04-30 14:31:08.713420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    40791 2024-04-30 14:31:08.717420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html
+-rw-r--r--   0        0        0    33401 2024-04-30 14:31:08.721420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    39294 2024-04-30 14:31:08.725420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    34846 2024-04-30 14:31:08.717420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    34763 2024-04-30 14:31:08.721420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     4805 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2024-04-30 14:31:08.577421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0     9204 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   113505 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css
+-rw-r--r--   0        0        0    38975 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map
+-rw-r--r--   0        0        0    12245 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css
+-rw-r--r--   0        0        0     3639 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map
+-rw-r--r--   0        0        0    33963 2024-04-30 14:31:08.761420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    33682 2024-04-30 14:31:08.757420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0    40314 2024-04-30 14:31:08.765420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    38617 2024-04-30 14:31:08.729420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html
+-rw-r--r--   0        0        0    94815 2024-04-30 14:31:08.749420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    35509 2024-04-30 14:31:08.753420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html
+-rw-r--r--   0        0        0    45941 2024-04-30 14:31:08.757420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html
+-rw-r--r--   0        0        0    40260 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-nautobot-show-tech.png
+-rw-r--r--   0        0        0    40260 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.png
+-rw-r--r--   0        0        0    10398 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.svg
+-rw-r--r--   0        0        0  1150397 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_example.webm
+-rw-r--r--   0        0        0   217106 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_meminfo.png
+-rw-r--r--   0        0        0   814242 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_example.webm
+-rw-r--r--   0        0        0   347891 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_result.png
+-rw-r--r--   0        0        0   301965 2024-04-30 14:31:08.573421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_run.png
+-rw-r--r--   0        0        0    40223 2024-04-30 14:31:08.709420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/index.html
+-rw-r--r--   0        0        0      259 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/objects.inv
+-rw-r--r--   0        0        0      120 2024-04-30 14:31:08.569421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/requirements.txt
+-rw-r--r--   0        0        0    49323 2024-04-30 14:31:08.777419 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json
+-rw-r--r--   0        0        0     3245 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml
+-rw-r--r--   0        0        0      388 2024-04-30 14:31:08.581421 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    36675 2024-04-30 14:31:08.769420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    36378 2024-04-30 14:31:08.769420 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html
+-rw-r--r--   0        0        0    34678 2024-04-30 14:31:08.773419 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    34448 2024-04-30 14:31:08.777419 nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html
+-rw-r--r--   0        0        0       45 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/tests/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/tests/test_api.py
+-rw-r--r--   0        0        0     1042 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/tests/test_basic.py
+-rwxr-xr-x   0        0        0     1942 2024-04-30 14:30:43.233617 nautobot_show_tech-2.0.2/nautobot_show_tech/update_readme.py
+-rw-r--r--   0        0        0     5543 2024-04-30 14:30:52.881542 nautobot_show_tech-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4504 1970-01-01 00:00:00.000000 nautobot_show_tech-2.0.2/PKG-INFO
```

### Comparing `nautobot_show_tech-2.0.1/LICENSE` & `nautobot_show_tech-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/README.md` & `nautobot_show_tech-2.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Nautobot Show Tech
 
 <p align="center">
-  <img src="./docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
   <br>
   <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-show-tech/badge/"></a>
   <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/v/nautobot-show-tech"></a>
   <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/dm/nautobot-show-tech"></a>
   <br>
   An App for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
@@ -20,25 +20,25 @@
 
 Nautobot Show Tech is versioned in coordination with the Major Release version of Nautobot.  Please be sure to use the appropriate version for best diagnostic return results.
 - Nautobot Show Tech 2.X will support Nautobot 2.X environments.
 - Nautobot Show Tech 1.X will support Nautobot 1.X environments.
 
 ### Screenshots
 
-![Show Tech GUI Job Run Mem Info](./docs/images/show_tech_gui_job_run.png)
+![Show Tech GUI Job Run Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_job_run.png)
 
-![Show Tech GUI Job Result Mem Info](./docs/images/show_tech_gui_job_result.png)
+![Show Tech GUI Job Result Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_job_result.png)
 
-![Show Tech CLI Mem Info](./docs/images/show_tech_cli_meminfo.png)
+![Show Tech CLI Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_cli_meminfo.png)
 
 #### Recorded Examples
 
-![Show_Tech_GUI](./docs/images/show_tech_gui_example.webm)
+![Show_Tech_GUI](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_example.webm)
 
-![Show_Tech_CLI](./docs/images/show_tech_cli_example.webm)
+![Show_Tech_CLI](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_cli_example.webm)
 
 
 ## Current Release
 
 This App is available is not currently open sourced.  Instead it is currently available via [pypi.org](https://pypi.org/) and the maintainers are not accepting feature requests, bugs, or pull requests at this time.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 # Nautobot Show Tech
-             [./docs/images/icon-nautobot-show-tech.png?raw=true]
+   [https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/
+                 images/icon-nautobot-show-tech.png?raw=true]
    _[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_a_p_p_-_s_h_o_w_-_t_e_c_h_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
                               _n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]
                              An App for _N_a_u_t_o_b_o_t.
 ## Overview ### Purpose: Providing diagnostics in a Nautobot environment When
 troubleshooting an environment, it is best to be able to answer questions about
 the environment quickly. This process is challenging to perform with a back-
@@ -12,27 +13,31 @@
 time ask. The goal is to aid in troubleshooting managed service customer
 environments, but it can be extended to do more or be used to meet stakeholder
 requirements. ### Versions: Nautobot 2.X or 1.X compatible Nautobot Show Tech
 is versioned in coordination with the Major Release version of Nautobot. Please
 be sure to use the appropriate version for best diagnostic return results. -
 Nautobot Show Tech 2.X will support Nautobot 2.X environments. - Nautobot Show
 Tech 1.X will support Nautobot 1.X environments. ### Screenshots ![Show Tech
-GUI Job Run Mem Info](./docs/images/show_tech_gui_job_run.png) ![Show Tech GUI
-Job Result Mem Info](./docs/images/show_tech_gui_job_result.png) ![Show Tech
-CLI Mem Info](./docs/images/show_tech_cli_meminfo.png) #### Recorded Examples !
-[Show_Tech_GUI](./docs/images/show_tech_gui_example.webm) ![Show_Tech_CLI](./
-docs/images/show_tech_cli_example.webm) ## Current Release This App is
-available is not currently open sourced. Instead it is currently available via
-[pypi.org](https://pypi.org/) and the maintainers are not accepting feature
-requests, bugs, or pull requests at this time. ## Documentation Coming Soon.
-Until then, use this readme and the [`docs`](https://github.com/networktocode-
-llc/nautobot-app-show-tech/tree/main/docs) folder in this repository. - [User
-Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/
-app_overview/) - Overview, Using the App, Getting Started. - [Administrator
-Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/
-install/) - How to Install, Configure, Upgrade, or Uninstall the App. -
-[Developer Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/
-latest/dev/contributing/) - Extending the App, Code Reference, Contribution
-Guide. - [Release Notes / Changelog](https://docs.nautobot.com/projects/
-nautobot-show-tech/en/latest/admin/release_notes/). - [Frequently Asked
-Questions](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/
-user/faq/).
+GUI Job Run Mem Info](https://raw.githubusercontent.com/mattmiller87/
+ratchet_images/main/docs/images/show_tech_gui_job_run.png) ![Show Tech GUI Job
+Result Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/
+main/docs/images/show_tech_gui_job_result.png) ![Show Tech CLI Mem Info](https:
+//raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/
+show_tech_cli_meminfo.png) #### Recorded Examples ![Show_Tech_GUI](https://
+raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/
+show_tech_gui_example.webm) ![Show_Tech_CLI](https://raw.githubusercontent.com/
+mattmiller87/ratchet_images/main/docs/images/show_tech_cli_example.webm) ##
+Current Release This App is available is not currently open sourced. Instead it
+is currently available via [pypi.org](https://pypi.org/) and the maintainers
+are not accepting feature requests, bugs, or pull requests at this time. ##
+Documentation Coming Soon. Until then, use this readme and the [`docs`](https:/
+/github.com/networktocode-llc/nautobot-app-show-tech/tree/main/docs) folder in
+this repository. - [User Guide](https://docs.nautobot.com/projects/nautobot-
+show-tech/en/latest/user/app_overview/) - Overview, Using the App, Getting
+Started. - [Administrator Guide](https://docs.nautobot.com/projects/nautobot-
+show-tech/en/latest/admin/install/) - How to Install, Configure, Upgrade, or
+Uninstall the App. - [Developer Guide](https://docs.nautobot.com/projects/
+nautobot-show-tech/en/latest/dev/contributing/) - Extending the App, Code
+Reference, Contribution Guide. - [Release Notes / Changelog](https://
+docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/release_notes/).
+- [Frequently Asked Questions](https://docs.nautobot.com/projects/nautobot-
+show-tech/en/latest/user/faq/).
```

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/__init__.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/helpers.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/jobs.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_apps.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_apps.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_counts.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_counts.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_django_settings.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_django_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_jobs.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/management/commands/show_tech_check_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/run_check.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/run_check.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/README.md` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/alias.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/alias.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/disk_space.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/disk_space.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pip_freeze.yaml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/pip_freeze.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/subprocess_run.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/show_tech_checks/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/404.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/404.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-nautobot-show-tech.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-nautobot-show-tech.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.svg` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.svg`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_example.webm` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_example.webm`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_meminfo.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_meminfo.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_example.webm` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_example.webm`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_result.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_result.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_run.png` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_run.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/index.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1023,15 +1023,15 @@
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="nautobot-show-tech">Nautobot Show Tech<a class="headerlink" href="#nautobot-show-tech" title="Permanent link">&para;</a></h1>
 <p align="center">
-  <img src="./docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
   <br>
   <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-show-tech/badge/"></a>
   <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/v/nautobot-show-tech"></a>
   <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/dm/nautobot-show-tech"></a>
   <br>
   An App for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
@@ -1040,20 +1040,20 @@
 <h3 id="purpose-providing-diagnostics-in-a-nautobot-environment">Purpose: Providing diagnostics in a Nautobot environment<a class="headerlink" href="#purpose-providing-diagnostics-in-a-nautobot-environment" title="Permanent link">&para;</a></h3>
 <p>When troubleshooting an environment, it is best to be able to answer questions about the environment quickly. This process is challenging to perform with a back-and-forth with a customer. Therefore, Nautobot Show Tech is designed to aggregate and provide that information in an easy-to-consume format as a one-time ask. The goal is to aid in troubleshooting managed service customer environments, but it can be extended to do more or be used to meet stakeholder requirements.</p>
 <h3 id="versions-nautobot-2x-or-1x-compatible">Versions: Nautobot 2.X or 1.X compatible<a class="headerlink" href="#versions-nautobot-2x-or-1x-compatible" title="Permanent link">&para;</a></h3>
 <p>Nautobot Show Tech is versioned in coordination with the Major Release version of Nautobot.  Please be sure to use the appropriate version for best diagnostic return results.
 - Nautobot Show Tech 2.X will support Nautobot 2.X environments.
 - Nautobot Show Tech 1.X will support Nautobot 1.X environments.</p>
 <h3 id="screenshots">Screenshots<a class="headerlink" href="#screenshots" title="Permanent link">&para;</a></h3>
-<p><img alt="Show Tech GUI Job Run Mem Info" src="./docs/images/show_tech_gui_job_run.png" /></p>
-<p><img alt="Show Tech GUI Job Result Mem Info" src="./docs/images/show_tech_gui_job_result.png" /></p>
-<p><img alt="Show Tech CLI Mem Info" src="./docs/images/show_tech_cli_meminfo.png" /></p>
+<p><img alt="Show Tech GUI Job Run Mem Info" src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_job_run.png" /></p>
+<p><img alt="Show Tech GUI Job Result Mem Info" src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_job_result.png" /></p>
+<p><img alt="Show Tech CLI Mem Info" src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_cli_meminfo.png" /></p>
 <h4 id="recorded-examples">Recorded Examples<a class="headerlink" href="#recorded-examples" title="Permanent link">&para;</a></h4>
-<p><img alt="Show_Tech_GUI" src="./docs/images/show_tech_gui_example.webm" /></p>
-<p><img alt="Show_Tech_CLI" src="./docs/images/show_tech_cli_example.webm" /></p>
+<p><img alt="Show_Tech_GUI" src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_example.webm" /></p>
+<p><img alt="Show_Tech_CLI" src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_cli_example.webm" /></p>
 <h2 id="current-release">Current Release<a class="headerlink" href="#current-release" title="Permanent link">&para;</a></h2>
 <p>This App is available is not currently open sourced.  Instead it is currently available via <a href="https://pypi.org/">pypi.org</a> and the maintainers are not accepting feature requests, bugs, or pull requests at this time.</p>
 <h2 id="documentation">Documentation<a class="headerlink" href="#documentation" title="Permanent link">&para;</a></h2>
 <p>Coming Soon. Until then, use this readme and the <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/tree/main/docs"><code>docs</code></a> folder in this repository.</p>
 <ul>
 <li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/app_overview/">User Guide</a> - Overview, Using the App, Getting Started.</li>
 <li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/install/">Administrator Guide</a> - How to Install, Configure, Upgrade, or Uninstall the App.</li>
```

#### html2text {}

```diff
@@ -52,15 +52,16 @@
           o _P_u_r_p_o_s_e_:_ _P_r_o_v_i_d_i_n_g_ _d_i_a_g_n_o_s_t_i_c_s_ _i_n_ _a_ _N_a_u_t_o_b_o_t_ _e_n_v_i_r_o_n_m_e_n_t
           o _V_e_r_s_i_o_n_s_:_ _N_a_u_t_o_b_o_t_ _2_._X_ _o_r_ _1_._X_ _c_o_m_p_a_t_i_b_l_e
           o _S_c_r_e_e_n_s_h_o_t_s
                 # _R_e_c_o_r_d_e_d_ _E_x_a_m_p_l_e_s
     * _C_u_r_r_e_n_t_ _R_e_l_e_a_s_e
     * _D_o_c_u_m_e_n_t_a_t_i_o_n
 ************ NNaauuttoobboott SShhooww TTeecchh_?¶ ************
-             [./docs/images/icon-nautobot-show-tech.png?raw=true]
+   [https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/
+                 images/icon-nautobot-show-tech.png?raw=true]
    _[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_a_p_p_-_s_h_o_w_-_t_e_c_h_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
                               _n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]
                              An App for _N_a_u_t_o_b_o_t.
 ********** OOvveerrvviieeww_?¶ **********
 ******** PPuurrppoossee:: PPrroovviiddiinngg ddiiaaggnnoossttiiccss iinn aa NNaauuttoobboott eennvviirroonnmmeenntt_?¶ ********
 When troubleshooting an environment, it is best to be able to answer questions
```

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml`

 * *Files 6% similar despite different names*

#### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml`

```diff
@@ -1,93 +1,93 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://doshow-tech/en/latest/index.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/compatibility_matrix.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/install.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/uninstall.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/upgrade.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/release_notes/index.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/release_notes/version_1.0.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/contributing.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/dev_environment.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/extending.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/framework.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/code_reference/index.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/code_reference/api.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/code_reference/package.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/app_getting_started.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/app_overview.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/app_use_cases.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/faq.html</loc>
-    <lastmod>2024-04-29</lastmod>
+    <lastmod>2024-04-30</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html` & `nautobot_show_tech-2.0.2/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_api.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_basic.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/nautobot_show_tech/update_readme.py` & `nautobot_show_tech-2.0.2/nautobot_show_tech/update_readme.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.1/pyproject.toml` & `nautobot_show_tech-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-show-tech"
-version = "v2.0.1"
+version = "v2.0.2"
 description = "An app to aid in troubleshooting a Nautobot environment."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode-llc/nautobot-app-show-tech"
 repository = "https://github.com/networktocode-llc/nautobot-app-show-tech"
 documentation = "https://doshow-tech/en/latest/"
```

### Comparing `nautobot_show_tech-2.0.1/PKG-INFO` & `nautobot_show_tech-2.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-show-tech
-Version: 2.0.1
+Version: 2.0.2
 Summary: An app to aid in troubleshooting a Nautobot environment.
 Home-page: https://github.com/networktocode-llc/nautobot-app-show-tech
 License: Apache-2.0
 Keywords: nautobot,nautobot-app,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.8,<3.12
@@ -23,15 +23,15 @@
 Project-URL: Documentation, https://doshow-tech/en/latest/
 Project-URL: Repository, https://github.com/networktocode-llc/nautobot-app-show-tech
 Description-Content-Type: text/markdown
 
 # Nautobot Show Tech
 
 <p align="center">
-  <img src="./docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
   <br>
   <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-show-tech/badge/"></a>
   <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/v/nautobot-show-tech"></a>
   <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/dm/nautobot-show-tech"></a>
   <br>
   An App for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
@@ -46,25 +46,25 @@
 
 Nautobot Show Tech is versioned in coordination with the Major Release version of Nautobot.  Please be sure to use the appropriate version for best diagnostic return results.
 - Nautobot Show Tech 2.X will support Nautobot 2.X environments.
 - Nautobot Show Tech 1.X will support Nautobot 1.X environments.
 
 ### Screenshots
 
-![Show Tech GUI Job Run Mem Info](./docs/images/show_tech_gui_job_run.png)
+![Show Tech GUI Job Run Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_job_run.png)
 
-![Show Tech GUI Job Result Mem Info](./docs/images/show_tech_gui_job_result.png)
+![Show Tech GUI Job Result Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_job_result.png)
 
-![Show Tech CLI Mem Info](./docs/images/show_tech_cli_meminfo.png)
+![Show Tech CLI Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_cli_meminfo.png)
 
 #### Recorded Examples
 
-![Show_Tech_GUI](./docs/images/show_tech_gui_example.webm)
+![Show_Tech_GUI](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_gui_example.webm)
 
-![Show_Tech_CLI](./docs/images/show_tech_cli_example.webm)
+![Show_Tech_CLI](https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/show_tech_cli_example.webm)
 
 
 ## Current Release
 
 This App is available is not currently open sourced.  Instead it is currently available via [pypi.org](https://pypi.org/) and the maintainers are not accepting feature requests, bugs, or pull requests at this time.
 
 ## Documentation
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: nautobot-show-tech Version: 2.0.1 Summary: An app
+Metadata-Version: 2.1 Name: nautobot-show-tech Version: 2.0.2 Summary: An app
 to aid in troubleshooting a Nautobot environment. Home-page: https://
 github.com/networktocode-llc/nautobot-app-show-tech License: Apache-2.0
 Keywords: nautobot,nautobot-app,nautobot-plugin Author: Network to Code, LLC
 Author-email: info@networktocode.com Requires-Python: >=3.8,<3.12 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Requires-Dist: click
 (>=8.1.0,<9.0.0) Requires-Dist: nautobot (>=2.0.0,<3.0.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Project-URL: Documentation, https://doshow-tech/en/
 latest/ Project-URL: Repository, https://github.com/networktocode-llc/nautobot-
 app-show-tech Description-Content-Type: text/markdown # Nautobot Show Tech
-             [./docs/images/icon-nautobot-show-tech.png?raw=true]
+   [https://raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/
+                 images/icon-nautobot-show-tech.png?raw=true]
    _[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_a_p_p_-_s_h_o_w_-_t_e_c_h_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/
    _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
                               _n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]
                              An App for _N_a_u_t_o_b_o_t.
 ## Overview ### Purpose: Providing diagnostics in a Nautobot environment When
 troubleshooting an environment, it is best to be able to answer questions about
 the environment quickly. This process is challenging to perform with a back-
@@ -26,27 +27,31 @@
 time ask. The goal is to aid in troubleshooting managed service customer
 environments, but it can be extended to do more or be used to meet stakeholder
 requirements. ### Versions: Nautobot 2.X or 1.X compatible Nautobot Show Tech
 is versioned in coordination with the Major Release version of Nautobot. Please
 be sure to use the appropriate version for best diagnostic return results. -
 Nautobot Show Tech 2.X will support Nautobot 2.X environments. - Nautobot Show
 Tech 1.X will support Nautobot 1.X environments. ### Screenshots ![Show Tech
-GUI Job Run Mem Info](./docs/images/show_tech_gui_job_run.png) ![Show Tech GUI
-Job Result Mem Info](./docs/images/show_tech_gui_job_result.png) ![Show Tech
-CLI Mem Info](./docs/images/show_tech_cli_meminfo.png) #### Recorded Examples !
-[Show_Tech_GUI](./docs/images/show_tech_gui_example.webm) ![Show_Tech_CLI](./
-docs/images/show_tech_cli_example.webm) ## Current Release This App is
-available is not currently open sourced. Instead it is currently available via
-[pypi.org](https://pypi.org/) and the maintainers are not accepting feature
-requests, bugs, or pull requests at this time. ## Documentation Coming Soon.
-Until then, use this readme and the [`docs`](https://github.com/networktocode-
-llc/nautobot-app-show-tech/tree/main/docs) folder in this repository. - [User
-Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/
-app_overview/) - Overview, Using the App, Getting Started. - [Administrator
-Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/
-install/) - How to Install, Configure, Upgrade, or Uninstall the App. -
-[Developer Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/
-latest/dev/contributing/) - Extending the App, Code Reference, Contribution
-Guide. - [Release Notes / Changelog](https://docs.nautobot.com/projects/
-nautobot-show-tech/en/latest/admin/release_notes/). - [Frequently Asked
-Questions](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/
-user/faq/).
+GUI Job Run Mem Info](https://raw.githubusercontent.com/mattmiller87/
+ratchet_images/main/docs/images/show_tech_gui_job_run.png) ![Show Tech GUI Job
+Result Mem Info](https://raw.githubusercontent.com/mattmiller87/ratchet_images/
+main/docs/images/show_tech_gui_job_result.png) ![Show Tech CLI Mem Info](https:
+//raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/
+show_tech_cli_meminfo.png) #### Recorded Examples ![Show_Tech_GUI](https://
+raw.githubusercontent.com/mattmiller87/ratchet_images/main/docs/images/
+show_tech_gui_example.webm) ![Show_Tech_CLI](https://raw.githubusercontent.com/
+mattmiller87/ratchet_images/main/docs/images/show_tech_cli_example.webm) ##
+Current Release This App is available is not currently open sourced. Instead it
+is currently available via [pypi.org](https://pypi.org/) and the maintainers
+are not accepting feature requests, bugs, or pull requests at this time. ##
+Documentation Coming Soon. Until then, use this readme and the [`docs`](https:/
+/github.com/networktocode-llc/nautobot-app-show-tech/tree/main/docs) folder in
+this repository. - [User Guide](https://docs.nautobot.com/projects/nautobot-
+show-tech/en/latest/user/app_overview/) - Overview, Using the App, Getting
+Started. - [Administrator Guide](https://docs.nautobot.com/projects/nautobot-
+show-tech/en/latest/admin/install/) - How to Install, Configure, Upgrade, or
+Uninstall the App. - [Developer Guide](https://docs.nautobot.com/projects/
+nautobot-show-tech/en/latest/dev/contributing/) - Extending the App, Code
+Reference, Contribution Guide. - [Release Notes / Changelog](https://
+docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/release_notes/).
+- [Frequently Asked Questions](https://docs.nautobot.com/projects/nautobot-
+show-tech/en/latest/user/faq/).
```

