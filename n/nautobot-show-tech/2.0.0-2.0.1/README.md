# Comparing `tmp/nautobot_show_tech-2.0.0.tar.gz` & `tmp/nautobot_show_tech-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_show_tech-2.0.0.tar", max compression
+gzip compressed data, was "nautobot_show_tech-2.0.1.tar", max compression
```

## Comparing `nautobot_show_tech-2.0.0.tar` & `nautobot_show_tech-2.0.1.tar`

### file list

```diff
@@ -1,120 +1,126 @@
--rw-r--r--   0        0        0      591 2024-04-10 22:57:11.852040 nautobot_show_tech-2.0.0/LICENSE
--rw-r--r--   0        0        0     5121 2024-04-10 22:57:11.852040 nautobot_show_tech-2.0.0/README.md
--rw-r--r--   0        0        0      973 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/__init__.py
--rw-r--r--   0        0        0       44 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/api/__init__.py
--rw-r--r--   0        0        0     2826 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/helpers.py
--rw-r--r--   0        0        0     4676 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/jobs.py
--rw-r--r--   0        0        0     1152 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_apps.py
--rw-r--r--   0        0        0     2190 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_counts.py
--rw-r--r--   0        0        0     1242 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_django_settings.py
--rw-r--r--   0        0        0     2466 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_jobs.py
--rw-r--r--   0        0        0        0 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/migrations/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/run_check.py
--rw-r--r--   0        0        0     4438 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/README.md
--rw-r--r--   0        0        0       75 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/__init__.py
--rw-r--r--   0        0        0      632 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/alias.yaml
--rw-r--r--   0        0        0      447 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/ansible_version.yaml
--rw-r--r--   0        0        0      467 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/available_commands.yaml
--rw-r--r--   0        0        0      305 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/date.yaml
--rw-r--r--   0        0        0      517 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/disk_space.yaml
--rw-r--r--   0        0        0      424 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/dns.yaml
--rw-r--r--   0        0        0      491 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/host_uptime.yaml
--rw-r--r--   0        0        0      372 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/hostname.yaml
--rw-r--r--   0        0        0      449 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/lscpu.yaml
--rw-r--r--   0        0        0      415 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/meminfo.yaml
--rw-r--r--   0        0        0      700 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml
--rw-r--r--   0        0        0      697 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml
--rw-r--r--   0        0        0      730 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml
--rw-r--r--   0        0        0      713 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml
--rw-r--r--   0        0        0      703 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml
--rw-r--r--   0        0        0      535 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml
--rw-r--r--   0        0        0      395 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/os-release.yaml
--rw-r--r--   0        0        0      565 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/pip_freeze.yaml
--rw-r--r--   0        0        0      383 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/pip_version.yaml
--rw-r--r--   0        0        0      422 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/pwd.yaml
--rw-r--r--   0        0        0      395 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/python_version.yaml
--rw-r--r--   0        0        0     4280 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/subprocess_run.py
--rw-r--r--   0        0        0      449 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/uname_a.yaml
--rw-r--r--   0        0        0      371 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/which_pip.yaml
--rw-r--r--   0        0        0      383 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/which_python.yaml
--rw-r--r--   0        0        0      366 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/whoami.yaml
--rw-r--r--   0        0        0    30302 2024-04-10 22:57:39.467998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/404.html
--rw-r--r--   0        0        0    33898 2024-04-10 22:57:39.487998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html
--rw-r--r--   0        0        0    40771 2024-04-10 22:57:39.491998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html
--rw-r--r--   0        0        0    33381 2024-04-10 22:57:39.495998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html
--rw-r--r--   0        0        0    39270 2024-04-10 22:57:39.499997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html
--rw-r--r--   0        0        0    34826 2024-04-10 22:57:39.491998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html
--rw-r--r--   0        0        0    34743 2024-04-10 22:57:39.495998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html
--rw-r--r--   0        0        0     1000 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     4805 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css
--rw-r--r--   0        0        0    15086 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico
--rw-r--r--   0        0        0     1870 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png
--rw-r--r--   0        0        0   113489 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js
--rw-r--r--   0        0        0   954781 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map
--rw-r--r--   0        0        0    17074 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0     1264 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js
--rw-r--r--   0        0        0    11232 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     3494 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js
--rw-r--r--   0        0        0     7972 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     4901 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js
--rw-r--r--   0        0        0     3647 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     2330 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js
--rw-r--r--   0        0        0     1031 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2158 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677463 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2024-04-10 22:57:39.351998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2024-04-10 22:57:39.355998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0     9204 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png
--rw-r--r--   0        0        0    13318 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg
--rw-r--r--   0        0        0     7562 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png
--rw-r--r--   0        0        0      846 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html
--rw-r--r--   0        0        0   113505 2024-04-10 22:57:39.355998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css
--rw-r--r--   0        0        0    38975 2024-04-10 22:57:39.355998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map
--rw-r--r--   0        0        0    12245 2024-04-10 22:57:39.355998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css
--rw-r--r--   0        0        0     3639 2024-04-10 22:57:39.355998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map
--rw-r--r--   0        0        0    33943 2024-04-10 22:57:39.535997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html
--rw-r--r--   0        0        0    33662 2024-04-10 22:57:39.531998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html
--rw-r--r--   0        0        0    40294 2024-04-10 22:57:39.539997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html
--rw-r--r--   0        0        0    38597 2024-04-10 22:57:39.503998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html
--rw-r--r--   0        0        0    94795 2024-04-10 22:57:39.523997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html
--rw-r--r--   0        0        0    35489 2024-04-10 22:57:39.523997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html
--rw-r--r--   0        0        0    45921 2024-04-10 22:57:39.527998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html
--rw-r--r--   0        0        0    74601 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-ratchet.png
--rw-r--r--   0        0        0    74601 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-show-tech.png
--rw-r--r--   0        0        0    41953 2024-04-10 22:57:39.483998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/index.html
--rw-r--r--   0        0        0      259 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/objects.inv
--rw-r--r--   0        0        0      120 2024-04-10 22:57:39.347998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/requirements.txt
--rw-r--r--   0        0        0    50186 2024-04-10 22:57:39.547998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json
--rw-r--r--   0        0        0     3245 2024-04-10 22:57:39.359998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml
--rw-r--r--   0        0        0      388 2024-04-10 22:57:39.359998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    36655 2024-04-10 22:57:39.539997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html
--rw-r--r--   0        0        0    36822 2024-04-10 22:57:39.543997 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html
--rw-r--r--   0        0        0    34658 2024-04-10 22:57:39.547998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html
--rw-r--r--   0        0        0    34428 2024-04-10 22:57:39.547998 nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html
--rw-r--r--   0        0        0       45 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/tests/__init__.py
--rw-r--r--   0        0        0      992 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/tests/test_api.py
--rw-r--r--   0        0        0     1042 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/tests/test_basic.py
--rwxr-xr-x   0        0        0     1942 2024-04-10 22:57:11.856040 nautobot_show_tech-2.0.0/nautobot_show_tech/update_readme.py
--rw-r--r--   0        0        0     5531 2024-04-10 22:57:23.300035 nautobot_show_tech-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6215 1970-01-01 00:00:00.000000 nautobot_show_tech-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-29 22:10:42.144477 nautobot_show_tech-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3012 2024-04-29 22:10:42.144477 nautobot_show_tech-2.0.1/README.md
+-rw-r--r--   0        0        0      973 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/api/__init__.py
+-rw-r--r--   0        0        0     2826 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/helpers.py
+-rw-r--r--   0        0        0     4676 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/jobs.py
+-rw-r--r--   0        0        0     1152 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_apps.py
+-rw-r--r--   0        0        0     2190 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_counts.py
+-rw-r--r--   0        0        0     1242 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_django_settings.py
+-rw-r--r--   0        0        0     2466 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_jobs.py
+-rw-r--r--   0        0        0        0 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/migrations/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/run_check.py
+-rw-r--r--   0        0        0     4438 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/README.md
+-rw-r--r--   0        0        0       75 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/alias.yaml
+-rw-r--r--   0        0        0      447 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/ansible_version.yaml
+-rw-r--r--   0        0        0      467 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/available_commands.yaml
+-rw-r--r--   0        0        0      305 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/date.yaml
+-rw-r--r--   0        0        0      517 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/disk_space.yaml
+-rw-r--r--   0        0        0      424 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/dns.yaml
+-rw-r--r--   0        0        0      491 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/host_uptime.yaml
+-rw-r--r--   0        0        0      372 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/hostname.yaml
+-rw-r--r--   0        0        0      449 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/lscpu.yaml
+-rw-r--r--   0        0        0      415 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/meminfo.yaml
+-rw-r--r--   0        0        0      700 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml
+-rw-r--r--   0        0        0      697 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml
+-rw-r--r--   0        0        0      730 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml
+-rw-r--r--   0        0        0      713 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml
+-rw-r--r--   0        0        0      703 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml
+-rw-r--r--   0        0        0      535 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml
+-rw-r--r--   0        0        0      395 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/os-release.yaml
+-rw-r--r--   0        0        0      565 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pip_freeze.yaml
+-rw-r--r--   0        0        0      383 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pip_version.yaml
+-rw-r--r--   0        0        0      422 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pwd.yaml
+-rw-r--r--   0        0        0      395 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/python_version.yaml
+-rw-r--r--   0        0        0     4280 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/subprocess_run.py
+-rw-r--r--   0        0        0      449 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/uname_a.yaml
+-rw-r--r--   0        0        0      371 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/which_pip.yaml
+-rw-r--r--   0        0        0      383 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/which_python.yaml
+-rw-r--r--   0        0        0      366 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/whoami.yaml
+-rw-r--r--   0        0        0    30314 2024-04-29 22:11:05.940513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/404.html
+-rw-r--r--   0        0        0    33918 2024-04-29 22:11:05.960513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    40791 2024-04-29 22:11:05.964513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html
+-rw-r--r--   0        0        0    33401 2024-04-29 22:11:05.972513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    39294 2024-04-29 22:11:05.972513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    34846 2024-04-29 22:11:05.964513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    34763 2024-04-29 22:11:05.968513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     4805 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-04-29 22:11:05.824514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0     9204 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   113505 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css
+-rw-r--r--   0        0        0    38975 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map
+-rw-r--r--   0        0        0    12245 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css
+-rw-r--r--   0        0        0     3639 2024-04-29 22:11:05.828514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map
+-rw-r--r--   0        0        0    33963 2024-04-29 22:11:06.008513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    33682 2024-04-29 22:11:06.004513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0    40314 2024-04-29 22:11:06.012513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    38617 2024-04-29 22:11:05.976513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html
+-rw-r--r--   0        0        0    94815 2024-04-29 22:11:05.996513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    35509 2024-04-29 22:11:06.000513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html
+-rw-r--r--   0        0        0    45941 2024-04-29 22:11:06.004513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html
+-rw-r--r--   0        0        0    40260 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/icon-nautobot-show-tech.png
+-rw-r--r--   0        0        0    40260 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.png
+-rw-r--r--   0        0        0    10398 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/nautobot_show_tech_logo_202404.svg
+-rw-r--r--   0        0        0  1150397 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_example.webm
+-rw-r--r--   0        0        0   217106 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_cli_meminfo.png
+-rw-r--r--   0        0        0   814242 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_example.webm
+-rw-r--r--   0        0        0   347891 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_result.png
+-rw-r--r--   0        0        0   301965 2024-04-29 22:11:05.820514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/images/show_tech_gui_job_run.png
+-rw-r--r--   0        0        0    39833 2024-04-29 22:11:05.956513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/index.html
+-rw-r--r--   0        0        0      259 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/objects.inv
+-rw-r--r--   0        0        0      120 2024-04-29 22:11:05.816514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/requirements.txt
+-rw-r--r--   0        0        0    49323 2024-04-29 22:11:06.024513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json
+-rw-r--r--   0        0        0     3245 2024-04-29 22:11:05.832514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml
+-rw-r--r--   0        0        0      388 2024-04-29 22:11:05.832514 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    36675 2024-04-29 22:11:06.016513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    36378 2024-04-29 22:11:06.020513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html
+-rw-r--r--   0        0        0    34678 2024-04-29 22:11:06.020513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    34448 2024-04-29 22:11:06.024513 nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html
+-rw-r--r--   0        0        0       45 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/tests/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_api.py
+-rw-r--r--   0        0        0     1042 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_basic.py
+-rwxr-xr-x   0        0        0     1942 2024-04-29 22:10:42.160477 nautobot_show_tech-2.0.1/nautobot_show_tech/update_readme.py
+-rw-r--r--   0        0        0     5543 2024-04-29 22:10:50.288492 nautobot_show_tech-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 nautobot_show_tech-2.0.1/PKG-INFO
```

### Comparing `nautobot_show_tech-2.0.0/LICENSE` & `nautobot_show_tech-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/__init__.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/helpers.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/jobs.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_apps.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_apps.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_counts.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_counts.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_django_settings.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_django_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/management/commands/show_tech_check_jobs.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/management/commands/show_tech_check_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/run_check.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/run_check.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/README.md` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/alias.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/alias.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/disk_space.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/disk_space.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_apps.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_counts.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_django_settings.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_health_check.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_jobs.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/nautobot_server_version.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/pip_freeze.yaml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/pip_freeze.yaml`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/show_tech_checks/subprocess_run.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/show_tech_checks/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/404.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/404.html`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -299,15 +299,15 @@
   <img src="/en/latest/assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -843,15 +843,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/compatibility_matrix.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -851,24 +851,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/compatibility_matrix.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/compatibility_matrix.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/compatibility_matrix.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/compatibility_matrix.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="compatibility-matrix">Compatibility Matrix<a class="headerlink" href="#compatibility-matrix" title="Permanent link">&para;</a></h1>
@@ -938,15 +938,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/install.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -937,24 +937,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/install.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/install.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/install.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/install.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="installing-the-app-in-nautobot">Installing the App in Nautobot<a class="headerlink" href="#installing-the-app-in-nautobot" title="Permanent link">&para;</a></h1>
@@ -1083,15 +1083,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -843,24 +843,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/release_notes/index.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/release_notes/index.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/release_notes/index.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/release_notes/index.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="release-notes">Release Notes<a class="headerlink" href="#release-notes" title="Permanent link">&para;</a></h1>
@@ -923,15 +923,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/release_notes/version_1.0.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -1035,24 +1035,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/release_notes/version_1.0.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/release_notes/version_1.0.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/release_notes/version_1.0.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/release_notes/version_1.0.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="v10-release-notes">v1.0 Release Notes<a class="headerlink" href="#v10-release-notes" title="Permanent link">&para;</a></h1>
@@ -1086,15 +1086,15 @@
 <li>Changes to compatibility with Nautobot and/or other plugins, libraries etc.</li>
 </ul>
 <h2 id="v101-2021-09-08">[v1.0.1] - 2021-09-08<a class="headerlink" href="#v101-2021-09-08" title="Permanent link">&para;</a></h2>
 <h3 id="added">Added<a class="headerlink" href="#added" title="Permanent link">&para;</a></h3>
 <h3 id="changed">Changed<a class="headerlink" href="#changed" title="Permanent link">&para;</a></h3>
 <h3 id="fixed">Fixed<a class="headerlink" href="#fixed" title="Permanent link">&para;</a></h3>
 <ul>
-<li><a href="https://github.com/networktocode/nautobot-app-show-tech/issues/123">#123</a> Fixed Tag filtering not working in job launch form</li>
+<li><a href="https://github.com/networktocode-llc/nautobot-app-show-tech/issues/123">#123</a> Fixed Tag filtering not working in job launch form</li>
 </ul>
 <h2 id="v100-2021-08-03">[v1.0.0] - 2021-08-03<a class="headerlink" href="#v100-2021-08-03" title="Permanent link">&para;</a></h2>
 <h3 id="added_1">Added<a class="headerlink" href="#added_1" title="Permanent link">&para;</a></h3>
 <h3 id="changed_1">Changed<a class="headerlink" href="#changed_1" title="Permanent link">&para;</a></h3>
 <h3 id="fixed_1">Fixed<a class="headerlink" href="#fixed_1" title="Permanent link">&para;</a></h3>
 
 
@@ -1154,15 +1154,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/uninstall.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -897,24 +897,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/uninstall.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/uninstall.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/uninstall.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/uninstall.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="uninstall-the-app-from-nautobot">Uninstall the App from Nautobot<a class="headerlink" href="#uninstall-the-app-from-nautobot" title="Permanent link">&para;</a></h1>
@@ -983,15 +983,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/admin/upgrade.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -897,24 +897,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/upgrade.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/admin/upgrade.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/upgrade.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/admin/upgrade.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="upgrading-the-app">Upgrading the App<a class="headerlink" href="#upgrading-the-app" title="Permanent link">&para;</a></h1>
@@ -979,15 +979,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/extra.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/bundle.b4d07000.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.hy.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.kn.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sa.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.te.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/nautobot_logo.svg`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/networktocode_bw.png`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/overrides/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/main.26e3688c.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/assets/stylesheets/palette.ecc896b0.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -310,15 +310,15 @@
   <img src="../../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -897,24 +897,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/code_reference/api.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/code_reference/api.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/code_reference/api.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/code_reference/api.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="show-tech-api-package">Show Tech API Package<a class="headerlink" href="#show-tech-api-package" title="Permanent link">&para;</a></h1>
@@ -981,15 +981,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -843,24 +843,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/code_reference/index.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/code_reference/index.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/code_reference/index.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/code_reference/index.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="code-reference">Code Reference<a class="headerlink" href="#code-reference" title="Permanent link">&para;</a></h1>
@@ -927,15 +927,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/code_reference/package.html`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -919,24 +919,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/code_reference/package.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/code_reference/package.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/code_reference/package.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/code_reference/package.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
   <h1>Package</h1>
@@ -1112,15 +1112,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/contributing.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -911,24 +911,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/contributing.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/contributing.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/contributing.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/contributing.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="contributing-to-the-app">Contributing to the App<a class="headerlink" href="#contributing-to-the-app" title="Permanent link">&para;</a></h1>
@@ -1035,15 +1035,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/dev_environment.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -1349,24 +1349,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/dev_environment.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/dev_environment.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/dev_environment.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/dev_environment.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="building-your-development-environment">Building Your Development Environment<a class="headerlink" href="#building-your-development-environment" title="Permanent link">&para;</a></h1>
@@ -1776,15 +1776,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/extending.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -897,24 +897,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/extending.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/extending.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/extending.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/extending.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="extending-the-app">Extending the App<a class="headerlink" href="#extending-the-app" title="Permanent link">&para;</a></h1>
@@ -984,15 +984,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/dev/framework.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -951,24 +951,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/framework.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/dev/framework.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/framework.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/dev/framework.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="show-techs-design-and-code-intent">Show Tech's Design and Code Intent<a class="headerlink" href="#show-techs-design-and-code-intent" title="Permanent link">&para;</a></h1>
@@ -1094,15 +1094,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/index.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html`

 * *Files 15% similar despite different names*

```diff
@@ -4,33 +4,35 @@
   <head>
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
-        <link rel="canonical" href="https://doshow-tech/en/latest/index.html">
+        <link rel="canonical" href="https://doshow-tech/en/latest/user/faq.html">
       
       
+        <link rel="prev" href="app_use_cases.html">
       
-        <link rel="next" href="user/app_overview.html">
       
-      <link rel="icon" href="assets/favicon.ico">
+        <link rel="next" href="../admin/install.html">
+      
+      <link rel="icon" href="../assets/favicon.ico">
       <meta name="generator" content="mkdocs-1.5.2, mkdocs-material-9.1.15">
     
     
       
-        <title>Nautobot Show Tech Documentation</title>
+        <title>Frequently Asked Questions - Nautobot Show Tech Documentation</title>
       
     
     
-      <link rel="stylesheet" href="assets/stylesheets/main.26e3688c.min.css">
+      <link rel="stylesheet" href="../assets/stylesheets/main.26e3688c.min.css">
       
         
-        <link rel="stylesheet" href="assets/stylesheets/palette.ecc896b0.min.css">
+        <link rel="stylesheet" href="../assets/stylesheets/palette.ecc896b0.min.css">
       
       
 
     
     
     
       
@@ -38,19 +40,19 @@
         
         <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
         <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,300i,400,400i,700,700i%7CRoboto+Mono:400,400i,700,700i&display=fallback">
         <style>:root{--md-text-font:"Roboto";--md-code-font:"Roboto Mono"}</style>
       
     
     
-      <link rel="stylesheet" href="assets/_mkdocstrings.css">
+      <link rel="stylesheet" href="../assets/_mkdocstrings.css">
     
-      <link rel="stylesheet" href="assets/extra.css">
+      <link rel="stylesheet" href="../assets/extra.css">
     
-    <script>__md_scope=new URL(".",location),__md_hash=e=>[...e].reduce((e,_)=>(e<<5)-e+_.charCodeAt(0),0),__md_get=(e,_=localStorage,t=__md_scope)=>JSON.parse(_.getItem(t.pathname+"."+e)),__md_set=(e,_,t=localStorage,a=__md_scope)=>{try{t.setItem(a.pathname+"."+e,JSON.stringify(_))}catch(e){}}</script>
+    <script>__md_scope=new URL("..",location),__md_hash=e=>[...e].reduce((e,_)=>(e<<5)-e+_.charCodeAt(0),0),__md_get=(e,_=localStorage,t=__md_scope)=>JSON.parse(_.getItem(t.pathname+"."+e)),__md_set=(e,_,t=localStorage,a=__md_scope)=>{try{t.setItem(a.pathname+"."+e,JSON.stringify(_))}catch(e){}}</script>
     
       
 
     
     
     
   </head>
@@ -71,15 +73,15 @@
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#nautobot-show-tech" class="md-skip">
+        <a href="#frequently-asked-questions" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
@@ -87,17 +89,17 @@
     
       
 
   
 
 <header class="md-header md-header--shadow md-header--lifted" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href="index.html" title="Nautobot Show Tech Documentation" class="md-header__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
+    <a href="../index.html" title="Nautobot Show Tech Documentation" class="md-header__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
       
-  <img src="assets/nautobot_logo.svg" alt="logo">
+  <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2Z"/></svg>
     </label>
     <div class="md-header__title" data-md-component="header-title">
       <div class="md-header__ellipsis">
@@ -105,15 +107,15 @@
           <span class="md-ellipsis">
             Nautobot Show Tech Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Overview
+              Frequently Asked Questions
             
           </span>
         </div>
       </div>
     </div>
     
       
@@ -181,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -203,35 +205,35 @@
 <nav class="md-tabs" aria-label="Tabs" data-md-component="tabs">
   <div class="md-grid">
     <ul class="md-tabs__list">
       
         
   
   
-    
-  
 
 
   <li class="md-tabs__item">
-    <a href="index.html" class="md-tabs__link md-tabs__link--active">
+    <a href="../index.html" class="md-tabs__link">
       Overview
     </a>
   </li>
 
       
         
   
   
+    
+  
 
 
   
   
   
     <li class="md-tabs__item">
-      <a href="user/app_overview.html" class="md-tabs__link">
+      <a href="app_overview.html" class="md-tabs__link md-tabs__link--active">
         User Guide
       </a>
     </li>
   
 
       
         
@@ -239,15 +241,15 @@
   
 
 
   
   
   
     <li class="md-tabs__item">
-      <a href="admin/install.html" class="md-tabs__link">
+      <a href="../admin/install.html" class="md-tabs__link">
         Administrator Guide
       </a>
     </li>
   
 
       
         
@@ -255,15 +257,15 @@
   
 
 
   
   
   
     <li class="md-tabs__item">
-      <a href="dev/extending.html" class="md-tabs__link">
+      <a href="../dev/extending.html" class="md-tabs__link">
         Developer Guide
       </a>
     </li>
   
 
       
         
@@ -291,36 +293,34 @@
         
       
       <main class="md-main" data-md-component="main">
         <div class="md-main__inner md-grid">
           
             
               
-                
-              
-              <div class="md-sidebar md-sidebar--primary" data-md-component="sidebar" data-md-type="navigation" hidden>
+              <div class="md-sidebar md-sidebar--primary" data-md-component="sidebar" data-md-type="navigation" >
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
   
 
 
 <nav class="md-nav md-nav--primary md-nav--lifted" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href="index.html" title="Nautobot Show Tech Documentation" class="md-nav__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
+    <a href="../index.html" title="Nautobot Show Tech Documentation" class="md-nav__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
       
-  <img src="assets/nautobot_logo.svg" alt="logo">
+  <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -331,132 +331,39 @@
     
       
       
       
 
   
   
-    
-  
   
-    <li class="md-nav__item md-nav__item--active">
-      
-      <input class="md-nav__toggle md-toggle" type="checkbox" id="__toc">
-      
-      
-        
-      
-      
-        <label class="md-nav__link md-nav__link--active" for="__toc">
-          Overview
-          <span class="md-nav__icon md-icon"></span>
-        </label>
-      
-      <a href="index.html" class="md-nav__link md-nav__link--active">
+    <li class="md-nav__item">
+      <a href="../index.html" class="md-nav__link">
         Overview
       </a>
-      
-        
-
-<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
-  
-  
-  
-    
-  
-  
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#overview" class="md-nav__link">
-    Overview
-  </a>
-  
-    <nav class="md-nav" aria-label="Overview">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#purpose-providing-diagnostics-in-a-nautobot-environment" class="md-nav__link">
-    Purpose: Providing diagnostics in a Nautobot environment
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#versions-nautobot-2x-or-1x-compatible" class="md-nav__link">
-    Versions: Nautobot 2.X or 1.X compatible
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#screenshots" class="md-nav__link">
-    Screenshots
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#documentation" class="md-nav__link">
-    Documentation
-  </a>
-  
-    <nav class="md-nav" aria-label="Documentation">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#contributing-to-the-documentation" class="md-nav__link">
-    Contributing to the Documentation
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#questions" class="md-nav__link">
-    Questions
-  </a>
-  
-</li>
-      
-    </ul>
-  
-</nav>
-      
     </li>
   
 
     
       
       
       
 
   
   
+    
+  
   
     
-    <li class="md-nav__item md-nav__item--nested">
+    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
       
       
       
       
-      <input class="md-nav__toggle md-toggle " type="checkbox" id="__nav_2" >
+      <input class="md-nav__toggle md-toggle " type="checkbox" id="__nav_2" checked>
       
       
         
           
         
           
         
@@ -467,72 +374,82 @@
       
       
         <label class="md-nav__link" for="__nav_2" id="__nav_2_label" tabindex="0">
           User Guide
           <span class="md-nav__icon md-icon"></span>
         </label>
       
-      <nav class="md-nav" data-md-level="1" aria-labelledby="__nav_2_label" aria-expanded="false">
+      <nav class="md-nav" data-md-level="1" aria-labelledby="__nav_2_label" aria-expanded="true">
         <label class="md-nav__title" for="__nav_2">
           <span class="md-nav__icon md-icon"></span>
           User Guide
         </label>
         <ul class="md-nav__list" data-md-scrollfix>
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="user/app_overview.html" class="md-nav__link">
+      <a href="app_overview.html" class="md-nav__link">
         App Overview
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="user/app_getting_started.html" class="md-nav__link">
+      <a href="app_getting_started.html" class="md-nav__link">
         Getting Started
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="user/app_use_cases.html" class="md-nav__link">
+      <a href="app_use_cases.html" class="md-nav__link">
         Using the App
       </a>
     </li>
   
 
             
           
             
               
   
   
+    
   
-    <li class="md-nav__item">
-      <a href="user/faq.html" class="md-nav__link">
+  
+    <li class="md-nav__item md-nav__item--active">
+      
+      <input class="md-nav__toggle md-toggle" type="checkbox" id="__toc">
+      
+      
+        
+      
+      
+      <a href="faq.html" class="md-nav__link md-nav__link--active">
         Frequently Asked Questions
       </a>
+      
     </li>
   
 
             
           
         </ul>
       </nav>
@@ -583,57 +500,57 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="admin/install.html" class="md-nav__link">
+      <a href="../admin/install.html" class="md-nav__link">
         Install and Configure
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="admin/upgrade.html" class="md-nav__link">
+      <a href="../admin/upgrade.html" class="md-nav__link">
         Upgrade
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="admin/uninstall.html" class="md-nav__link">
+      <a href="../admin/uninstall.html" class="md-nav__link">
         Uninstall
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="admin/compatibility_matrix.html" class="md-nav__link">
+      <a href="../admin/compatibility_matrix.html" class="md-nav__link">
         Compatibility Matrix
       </a>
     </li>
   
 
             
           
@@ -659,15 +576,15 @@
           
         
       
       
         
         
         <div class="md-nav__link md-nav__link--index ">
-          <a href="admin/release_notes/index.html">Release Notes</a>
+          <a href="../admin/release_notes/index.html">Release Notes</a>
           
             <label for="__nav_3_5">
               <span class="md-nav__icon md-icon"></span>
             </label>
           
         </div>
       
@@ -682,15 +599,15 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="admin/release_notes/version_1.0.html" class="md-nav__link">
+      <a href="../admin/release_notes/version_1.0.html" class="md-nav__link">
         v1.0
       </a>
     </li>
   
 
             
           
@@ -750,57 +667,57 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="dev/extending.html" class="md-nav__link">
+      <a href="../dev/extending.html" class="md-nav__link">
         Extending the App
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="dev/contributing.html" class="md-nav__link">
+      <a href="../dev/contributing.html" class="md-nav__link">
         Contributing to the App
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="dev/dev_environment.html" class="md-nav__link">
+      <a href="../dev/dev_environment.html" class="md-nav__link">
         Development Environment
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="dev/framework.html" class="md-nav__link">
+      <a href="../dev/framework.html" class="md-nav__link">
         Framework for the App
       </a>
     </li>
   
 
             
           
@@ -828,15 +745,15 @@
           
         
       
       
         
         
         <div class="md-nav__link md-nav__link--index ">
-          <a href="dev/code_reference/index.html">Code Reference</a>
+          <a href="../dev/code_reference/index.html">Code Reference</a>
           
             <label for="__nav_4_5">
               <span class="md-nav__icon md-icon"></span>
             </label>
           
         </div>
       
@@ -851,29 +768,29 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="dev/code_reference/package.html" class="md-nav__link">
+      <a href="../dev/code_reference/package.html" class="md-nav__link">
         Package
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="dev/code_reference/api.html" class="md-nav__link">
+      <a href="../dev/code_reference/api.html" class="md-nav__link">
         API
       </a>
     </li>
   
 
             
           
@@ -909,173 +826,67 @@
 </nav>
                   </div>
                 </div>
               </div>
             
             
               
-                
-              
               <div class="md-sidebar md-sidebar--secondary" data-md-component="sidebar" data-md-type="toc" >
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
   
     
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#overview" class="md-nav__link">
-    Overview
-  </a>
-  
-    <nav class="md-nav" aria-label="Overview">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#purpose-providing-diagnostics-in-a-nautobot-environment" class="md-nav__link">
-    Purpose: Providing diagnostics in a Nautobot environment
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#versions-nautobot-2x-or-1x-compatible" class="md-nav__link">
-    Versions: Nautobot 2.X or 1.X compatible
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#screenshots" class="md-nav__link">
-    Screenshots
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#documentation" class="md-nav__link">
-    Documentation
-  </a>
-  
-    <nav class="md-nav" aria-label="Documentation">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#contributing-to-the-documentation" class="md-nav__link">
-    Contributing to the Documentation
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#questions" class="md-nav__link">
-    Questions
-  </a>
-  
-</li>
-      
-    </ul>
-  
 </nav>
                   </div>
                 </div>
               </div>
             
           
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/index.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/faq.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/index.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/faq.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
-<h1 id="nautobot-show-tech">Nautobot Show Tech<a class="headerlink" href="#nautobot-show-tech" title="Permanent link">&para;</a></h1>
-<p align="center">
-  <img src="https://raw.githubusercontent.com/networktocode/nautobot-app-show-tech/main/docs/images/icon-nautobot-show-tech.png" class="logo" height="200px">
-  <br>
-  <a href="https://github.com/networktocode/nautobot-app-show-tech/actions"><img src="https://github.com/networktocode/nautobot-app-show-tech/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-show-tech/badge/"></a>
-  <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/v/nautobot-show-tech"></a>
-  <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/dm/nautobot-show-tech"></a>
-  <br>
-  A diagnostics app for <a href="https://nautobot.com/">Nautobot</a>.
-</p>
-
-<h2 id="overview">Overview<a class="headerlink" href="#overview" title="Permanent link">&para;</a></h2>
-<h3 id="purpose-providing-diagnostics-in-a-nautobot-environment">Purpose: Providing diagnostics in a Nautobot environment<a class="headerlink" href="#purpose-providing-diagnostics-in-a-nautobot-environment" title="Permanent link">&para;</a></h3>
-<p>When troubleshooting an environment, it is best to be able to answer questions about the environment quickly. This process is challenging to perform with a back-and-forth with a customer. Therefore, Nautobot Show Tech is designed to aggregate and provide that information in an easy-to-consume format as a one-time ask. The goal is to aid in troubleshooting managed service customer environments, but it can be extended to do more or be used to meet stakeholder requirements.</p>
-<h3 id="versions-nautobot-2x-or-1x-compatible">Versions: Nautobot 2.X or 1.X compatible<a class="headerlink" href="#versions-nautobot-2x-or-1x-compatible" title="Permanent link">&para;</a></h3>
-<p>With the addition of commands using Nautobot ORM and Jobs, there is a requirement to have two versions of this plugin.  Nautobot Show Tech is therefore versioned in coordination with the Major Release version of Nautobot.  Nautobot Show Tech 2.X will support Nautobot 2.X environments. Nautobot Show Tech 1.X will support Nautobot 1.X environments.  Please be sure to use the appropriate version for best diagnostic return results.</p>
-<h3 id="screenshots">Screenshots<a class="headerlink" href="#screenshots" title="Permanent link">&para;</a></h3>
-<blockquote>
-<p>Developer Note: Add any representative screenshots of the App in action. These images should also be added to the <code>docs/user/app_use_cases.md</code> section.</p>
-<p>Developer Note: Place the files in the <code>docs/images/</code> folder and link them using only full URLs from GitHub, for example: <code>![Overview](https://raw.githubusercontent.com/networktocode/nautobot-app-show-tech/main/docs/images/plugin-overview.png)</code>. This absolute static linking is required to ensure the README renders properly in GitHub, the docs site, and any other external sites like PyPI.</p>
-</blockquote>
-<p>More screenshots can be found in the <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/app_use_cases/">Using the App</a> page in the documentation. Here's a quick overview of some of the plugin's added functionality:</p>
-<p><img alt="" src="https://raw.githubusercontent.com/networktocode/nautobot-app-show-tech/main/docs/images/placeholder.png" /></p>
-<h2 id="documentation">Documentation<a class="headerlink" href="#documentation" title="Permanent link">&para;</a></h2>
-<p>Coming Soon. Until then, use this readme and the <a href="https://github.com/networktocode/nautobot-app-show-tech/tree/main/docs"><code>docs</code></a> folder in this repository.</p>
-<!--
-Full documentation for this App can be found over on the [Nautobot Docs](https://docs.nautobot.com) website:
-
-- [User Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/app_overview/) - Overview, Using the App, Getting Started.
-- [Administrator Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the App.
-- [Developer Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution Guide.
-- [Release Notes / Changelog](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/release_notes/).
-- [Frequently Asked Questions](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/faq/).
--->
-<h3 id="contributing-to-the-documentation">Contributing to the Documentation<a class="headerlink" href="#contributing-to-the-documentation" title="Permanent link">&para;</a></h3>
-<p>You can find all the Markdown source for the App documentation under the <a href="https://github.com/networktocode/nautobot-app-show-tech/tree/main/docs"><code>docs</code></a> folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.</p>
-<!--
-If you need to view the fully-generated documentation site, you can build it with [MkDocs](https://www.mkdocs.org/). A container hosting the documentation can be started using the `invoke` commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). Using this container, as your changes to the documentation are saved, they will be automatically rebuilt and any pages currently being viewed will be reloaded in your browser.
--->
-<p>Any PRs with fixes or improvements are very welcome!</p>
-<h2 id="questions">Questions<a class="headerlink" href="#questions" title="Permanent link">&para;</a></h2>
-<p>For any questions or comments, please check the <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/faq/">FAQ</a> first. Feel free to also swing by the <a href="https://networktocode.slack.com/">Network to Code Slack</a> (channel <code>#nautobot</code>), sign up <a href="http://slack.networktocode.com/">here</a> if you don't have an account.</p>
-
+<h1 id="frequently-asked-questions">Frequently Asked Questions<a class="headerlink" href="#frequently-asked-questions" title="Permanent link">&para;</a></h1>
+<p><strong>Is Show Tech a standalone program or a Nautobot App?</strong>
+- Show Tech is primarily intended a standalone program, however it can be registered as a Nautobot App. The reason being is that if Nautobot is down, Show Tech needs to be able to continue to function.</p>
+<p><strong>Do you recommend installing Show Tech as a Nautobot App?</strong>
+- Yes. The diagnostics functionality is the same however as a Nautobot App we can leverage Nautobot Jobs and Nautobot views for quality-of-life.</p>
+<p><strong>Who is the target audience of Show Tech?</strong>
+- Initially the target audience is anyone looking for assistance in troubleshooting an Nautobot Environment.  Show Tech performs several checks which help provide information about what could be going wrong.
+- Additionally, there are features of Show Tech which may be important to other audiences. We hope to include those people as we iterate Show Tech.</p>
+<p><strong>Why is the name of the App Show Tech?</strong>
+- The name Show Tech was chosen to because it is recognizable to known industry naming patterns for the intended use-case.</p>
 
 
-  
 
 
 
                 
               </article>
             </div>
           
@@ -1084,27 +895,40 @@
         
       </main>
       
         <footer class="md-footer">
   
     
       
-        
-      
       <nav class="md-footer__inner md-grid" aria-label="Footer" >
         
+          
+          <a href="app_use_cases.html" class="md-footer__link md-footer__link--prev" aria-label="Previous: Using the App" rel="prev">
+            <div class="md-footer__button md-icon">
+              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12Z"/></svg>
+            </div>
+            <div class="md-footer__title">
+              <span class="md-footer__direction">
+                Previous
+              </span>
+              <div class="md-ellipsis">
+                Using the App
+              </div>
+            </div>
+          </a>
+        
         
           
-          <a href="user/app_overview.html" class="md-footer__link md-footer__link--next" aria-label="Next: App Overview" rel="next">
+          <a href="../admin/install.html" class="md-footer__link md-footer__link--next" aria-label="Next: Install and Configure" rel="next">
             <div class="md-footer__title">
               <span class="md-footer__direction">
                 Next
               </span>
               <div class="md-ellipsis">
-                App Overview
+                Install and Configure
               </div>
             </div>
             <div class="md-footer__button md-icon">
               <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4Z"/></svg>
             </div>
           </a>
         
@@ -1115,24 +939,24 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
     
     | <a href="https://networktocode.com" target="_blank" rel="noopener">Sponsored by <img
-            src=assets/networktocode_bw.png class="copyright-logo"></a>
+            src=../assets/networktocode_bw.png class="copyright-logo"></a>
     
 </div>
 
 <!-- RTD version flyout injected on live site -->
 <div id="readthedocs-embed-flyout"></div>
 
       
@@ -1185,17 +1009,17 @@
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
     
-    <script id="__config" type="application/json">{"base": ".", "features": ["content.action.edit", "content.action.view", "content.code.copy", "navigation.footer", "navigation.indexes", "navigation.tabs", "navigation.tabs.sticky", "navigation.tracking", "search.highlight", "search.share", "search.suggest"], "search": "assets/javascripts/workers/search.208ed371.min.js", "translations": {"clipboard.copied": "Copied to clipboard", "clipboard.copy": "Copy to clipboard", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.placeholder": "Type to start searching", "search.result.term.missing": "Missing", "select.version": "Select version"}}</script>
+    <script id="__config" type="application/json">{"base": "..", "features": ["content.action.edit", "content.action.view", "content.code.copy", "navigation.footer", "navigation.indexes", "navigation.tabs", "navigation.tabs.sticky", "navigation.tracking", "search.highlight", "search.share", "search.suggest"], "search": "../assets/javascripts/workers/search.208ed371.min.js", "translations": {"clipboard.copied": "Copied to clipboard", "clipboard.copy": "Copy to clipboard", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.placeholder": "Type to start searching", "search.result.term.missing": "Missing", "select.version": "Select version"}}</script>
     
     
-      <script src="assets/javascripts/bundle.b4d07000.min.js"></script>
+      <script src="../assets/javascripts/bundle.b4d07000.min.js"></script>
       
         <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,36 +1,29 @@
 ????
 _S_k_i_p_ _t_o_ _c_o_n_t_e_n_t
 _[_l_o_g_o_]
 Nautobot Show Tech Documentation
-Overview
+Frequently Asked Questions
 oo
 [query               ]
 Initializing search
 _G_i_t_H_u_b
     * _O_v_e_r_v_i_e_w
     * _U_s_e_r_ _G_u_i_d_e
     * _A_d_m_i_n_i_s_t_r_a_t_o_r_ _G_u_i_d_e
     * _D_e_v_e_l_o_p_e_r_ _G_u_i_d_e
     * _N_a_u_t_o_b_o_t_ _D_o_c_s_ _H_o_m_e_ _↗_︎
 _[_l_o_g_o_]Nautobot Show Tech Documentation
 _G_i_t_H_u_b
-    * ??Overview _O_v_e_r_v_i_e_w_ Table of contents
-          o _O_v_e_r_v_i_e_w
-                # _P_u_r_p_o_s_e_:_ _P_r_o_v_i_d_i_n_g_ _d_i_a_g_n_o_s_t_i_c_s_ _i_n_ _a_ _N_a_u_t_o_b_o_t_ _e_n_v_i_r_o_n_m_e_n_t
-                # _V_e_r_s_i_o_n_s_:_ _N_a_u_t_o_b_o_t_ _2_._X_ _o_r_ _1_._X_ _c_o_m_p_a_t_i_b_l_e
-                # _S_c_r_e_e_n_s_h_o_t_s
-          o _D_o_c_u_m_e_n_t_a_t_i_o_n
-                # _C_o_n_t_r_i_b_u_t_i_n_g_ _t_o_ _t_h_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n
-          o _Q_u_e_s_t_i_o_n_s
-    * ??User Guide User Guide
+    * _O_v_e_r_v_i_e_w
+    * User Guide User Guide
           o _A_p_p_ _O_v_e_r_v_i_e_w
           o _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _U_s_i_n_g_ _t_h_e_ _A_p_p
-          o _F_r_e_q_u_e_n_t_l_y_ _A_s_k_e_d_ _Q_u_e_s_t_i_o_n_s
+          o ??_F_r_e_q_u_e_n_t_l_y_ _A_s_k_e_d_ _Q_u_e_s_t_i_o_n_s
     * ??Administrator Guide Administrator Guide
           o _I_n_s_t_a_l_l_ _a_n_d_ _C_o_n_f_i_g_u_r_e
           o _U_p_g_r_a_d_e
           o _U_n_i_n_s_t_a_l_l
           o _C_o_m_p_a_t_i_b_i_l_i_t_y_ _M_a_t_r_i_x
           o ??
             _R_e_l_e_a_s_e_ _N_o_t_e_s
@@ -43,69 +36,32 @@
           o _F_r_a_m_e_w_o_r_k_ _f_o_r_ _t_h_e_ _A_p_p
           o ??
             _C_o_d_e_ _R_e_f_e_r_e_n_c_e
             Code Reference
                 # _P_a_c_k_a_g_e
                 # _A_P_I
     * _N_a_u_t_o_b_o_t_ _D_o_c_s_ _H_o_m_e_ _↗_︎
-Table of contents
-    * _O_v_e_r_v_i_e_w
-          o _P_u_r_p_o_s_e_:_ _P_r_o_v_i_d_i_n_g_ _d_i_a_g_n_o_s_t_i_c_s_ _i_n_ _a_ _N_a_u_t_o_b_o_t_ _e_n_v_i_r_o_n_m_e_n_t
-          o _V_e_r_s_i_o_n_s_:_ _N_a_u_t_o_b_o_t_ _2_._X_ _o_r_ _1_._X_ _c_o_m_p_a_t_i_b_l_e
-          o _S_c_r_e_e_n_s_h_o_t_s
-    * _D_o_c_u_m_e_n_t_a_t_i_o_n
-          o _C_o_n_t_r_i_b_u_t_i_n_g_ _t_o_ _t_h_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n
-    * _Q_u_e_s_t_i_o_n_s
-************ NNaauuttoobboott SShhooww TTeecchh_?¶ ************
- [https://raw.githubusercontent.com/networktocode/nautobot-app-show-tech/main/
-                   docs/images/icon-nautobot-show-tech.png]
-  _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_e_t_w_o_r_k_t_o_c_o_d_e_/_n_a_u_t_o_b_o_t_-_a_p_p_-_s_h_o_w_-_t_e_c_h_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
- _c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_a_p_p_-
- _s_h_o_w_-_t_e_c_h_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]_[_h_t_t_p_s_:_/_/
-                  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]
-                        A diagnostics app for _N_a_u_t_o_b_o_t.
-********** OOvveerrvviieeww_?¶ **********
-******** PPuurrppoossee:: PPrroovviiddiinngg ddiiaaggnnoossttiiccss iinn aa NNaauuttoobboott eennvviirroonnmmeenntt_?¶ ********
-When troubleshooting an environment, it is best to be able to answer questions
-about the environment quickly. This process is challenging to perform with a
-back-and-forth with a customer. Therefore, Nautobot Show Tech is designed to
-aggregate and provide that information in an easy-to-consume format as a one-
-time ask. The goal is to aid in troubleshooting managed service customer
-environments, but it can be extended to do more or be used to meet stakeholder
-requirements.
-******** VVeerrssiioonnss:: NNaauuttoobboott 22..XX oorr 11..XX ccoommppaattiibbllee_?¶ ********
-With the addition of commands using Nautobot ORM and Jobs, there is a
-requirement to have two versions of this plugin. Nautobot Show Tech is
-therefore versioned in coordination with the Major Release version of Nautobot.
-Nautobot Show Tech 2.X will support Nautobot 2.X environments. Nautobot Show
-Tech 1.X will support Nautobot 1.X environments. Please be sure to use the
-appropriate version for best diagnostic return results.
-******** SSccrreeeennsshhoottss_?¶ ********
-     Developer Note: Add any representative screenshots of the App in
-     action. These images should also be added to the docs/user/
-     app_use_cases.md section.
-     Developer Note: Place the files in the docs/images/ folder and link
-     them using only full URLs from GitHub, for example: ![Overview]
-     (https://raw.githubusercontent.com/networktocode/nautobot-app-show-
-     tech/main/docs/images/plugin-overview.png). This absolute static
-     linking is required to ensure the README renders properly in GitHub,
-     the docs site, and any other external sites like PyPI.
-More screenshots can be found in the _U_s_i_n_g_ _t_h_e_ _A_p_p page in the documentation.
-Here's a quick overview of some of the plugin's added functionality:
-********** DDooccuummeennttaattiioonn_?¶ **********
-Coming Soon. Until then, use this readme and the _d_o_c_s folder in this
-repository.
-******** CCoonnttrriibbuuttiinngg ttoo tthhee DDooccuummeennttaattiioonn_?¶ ********
-You can find all the Markdown source for the App documentation under the _d_o_c_s
-folder in this repository. For simple edits, a Markdown capable editor is
-sufficient: clone the repository and edit away.
-Any PRs with fixes or improvements are very welcome!
-********** QQuueessttiioonnss_?¶ **********
-For any questions or comments, please check the _F_A_Q first. Feel free to also
-swing by the _N_e_t_w_o_r_k_ _t_o_ _C_o_d_e_ _S_l_a_c_k (channel #nautobot), sign up _h_e_r_e if you
-don't have an account.
+************ FFrreeqquueennttllyy AAsskkeedd QQuueessttiioonnss_?¶ ************
+IIss SShhooww TTeecchh aa ssttaannddaalloonnee pprrooggrraamm oorr aa NNaauuttoobboott AApppp?? - Show Tech is primarily
+intended a standalone program, however it can be registered as a Nautobot App.
+The reason being is that if Nautobot is down, Show Tech needs to be able to
+continue to function.
+DDoo yyoouu rreeccoommmmeenndd iinnssttaalllliinngg SShhooww TTeecchh aass aa NNaauuttoobboott AApppp?? - Yes. The diagnostics
+functionality is the same however as a Nautobot App we can leverage Nautobot
+Jobs and Nautobot views for quality-of-life.
+WWhhoo iiss tthhee ttaarrggeett aauuddiieennccee ooff SShhooww TTeecchh?? - Initially the target audience is
+anyone looking for assistance in troubleshooting an Nautobot Environment. Show
+Tech performs several checks which help provide information about what could be
+going wrong. - Additionally, there are features of Show Tech which may be
+important to other audiences. We hope to include those people as we iterate
+Show Tech.
+WWhhyy iiss tthhee nnaammee ooff tthhee AApppp SShhooww TTeecchh?? - The name Show Tech was chosen to
+because it is recognizable to known industry naming patterns for the intended
+use-case.
+_P_r_e_v_i_o_u_s
+_U_s_i_n_g_ _t_h_e_ _A_p_p
 _N_e_x_t
-_A_p_p_ _O_v_e_r_v_i_e_w
+_I_n_s_t_a_l_l_ _a_n_d_ _C_o_n_f_i_g_u_r_e
 Copyright © The Authors
 _A_p_a_c_h_e_-_2_._0_ _L_I_C_E_N_S_E
-_M_a_d_e_ _w_i_t_h_ _M_a_t_e_r_i_a_l_ _f_o_r_ _M_k_D_o_c_s | _J_o_i_n_ _N_a_u_t_o_b_o_t_ _S_l_a_c_k | _S_p_o_n_s_o_r_e_d_ _b_y_[_a_s_s_e_t_s_/
+_M_a_d_e_ _w_i_t_h_ _M_a_t_e_r_i_a_l_ _f_o_r_ _M_k_D_o_c_s | _J_o_i_n_ _N_a_u_t_o_b_o_t_ _S_l_a_c_k | _S_p_o_n_s_o_r_e_d_ _b_y_[_._._/_a_s_s_e_t_s_/
 _n_e_t_w_o_r_k_t_o_c_o_d_e___b_w_._p_n_g_]
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/search/search_index.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9939814814814815%*

 * *Differences: {"'docs'": "{0: {'text': '<p>    An App for Nautobot. </p>'}, 3: {'text': '<p>Nautobot Show Tech "*

 * *           'is versioned in coordination with the Major Release version of Nautobot.  Please be '*

 * *           'sure to use the appropriate version for best diagnostic return results. - Nautobot '*

 * *           'Show Tech 2.X will support Nautobot 2.X environments. - Nautobot Show Tech 1.X will '*

 * *           "support Nautobot 1.X environments.</p>'}, 4: {'text': ''}, 5: {'location': "*

 * *           "'index.html#recorde […]*

```diff
@@ -7,51 +7,51 @@
             "stopWordFilter"
         ],
         "separator": "[\\s\\-]+"
     },
     "docs": [
         {
             "location": "index.html",
-            "text": "<p>    A diagnostics app for Nautobot. </p>",
+            "text": "<p>    An App for Nautobot. </p>",
             "title": "Nautobot Show Tech"
         },
         {
             "location": "index.html#overview",
             "text": "",
             "title": "Overview"
         },
         {
             "location": "index.html#purpose-providing-diagnostics-in-a-nautobot-environment",
             "text": "<p>When troubleshooting an environment, it is best to be able to answer questions about the environment quickly. This process is challenging to perform with a back-and-forth with a customer. Therefore, Nautobot Show Tech is designed to aggregate and provide that information in an easy-to-consume format as a one-time ask. The goal is to aid in troubleshooting managed service customer environments, but it can be extended to do more or be used to meet stakeholder requirements.</p>",
             "title": "Purpose: Providing diagnostics in a Nautobot environment"
         },
         {
             "location": "index.html#versions-nautobot-2x-or-1x-compatible",
-            "text": "<p>With the addition of commands using Nautobot ORM and Jobs, there is a requirement to have two versions of this plugin.  Nautobot Show Tech is therefore versioned in coordination with the Major Release version of Nautobot.  Nautobot Show Tech 2.X will support Nautobot 2.X environments. Nautobot Show Tech 1.X will support Nautobot 1.X environments.  Please be sure to use the appropriate version for best diagnostic return results.</p>",
+            "text": "<p>Nautobot Show Tech is versioned in coordination with the Major Release version of Nautobot.  Please be sure to use the appropriate version for best diagnostic return results. - Nautobot Show Tech 2.X will support Nautobot 2.X environments. - Nautobot Show Tech 1.X will support Nautobot 1.X environments.</p>",
             "title": "Versions: Nautobot 2.X or 1.X compatible"
         },
         {
             "location": "index.html#screenshots",
-            "text": "<p>Developer Note: Add any representative screenshots of the App in action. These images should also be added to the <code>docs/user/app_use_cases.md</code> section.</p> <p>Developer Note: Place the files in the <code>docs/images/</code> folder and link them using only full URLs from GitHub, for example: <code>![Overview](https://raw.githubusercontent.com/networktocode/nautobot-app-show-tech/main/docs/images/plugin-overview.png)</code>. This absolute static linking is required to ensure the README renders properly in GitHub, the docs site, and any other external sites like PyPI.</p> <p>More screenshots can be found in the Using the App page in the documentation. Here's a quick overview of some of the plugin's added functionality:</p> <p></p>",
+            "text": "",
             "title": "Screenshots"
         },
         {
-            "location": "index.html#documentation",
-            "text": "<p>Coming Soon. Until then, use this readme and the <code>docs</code> folder in this repository.</p>",
-            "title": "Documentation"
+            "location": "index.html#recorded-examples",
+            "text": "",
+            "title": "Recorded Examples"
         },
         {
-            "location": "index.html#contributing-to-the-documentation",
-            "text": "<p>You can find all the Markdown source for the App documentation under the <code>docs</code> folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.</p> <p>Any PRs with fixes or improvements are very welcome!</p>",
-            "title": "Contributing to the Documentation"
+            "location": "index.html#current-release",
+            "text": "<p>This App is available is not currently open sourced.  Instead it is currently available via pypi.org and the maintainers are not accepting feature requests, bugs, or pull requests at this time.</p>",
+            "title": "Current Release"
         },
         {
-            "location": "index.html#questions",
-            "text": "<p>For any questions or comments, please check the FAQ first. Feel free to also swing by the Network to Code Slack (channel <code>#nautobot</code>), sign up here if you don't have an account.</p>",
-            "title": "Questions"
+            "location": "index.html#documentation",
+            "text": "<p>Coming Soon. Until then, use this readme and the <code>docs</code> folder in this repository.</p> <ul> <li>User Guide - Overview, Using the App, Getting Started.</li> <li>Administrator Guide - How to Install, Configure, Upgrade, or Uninstall the App.</li> <li>Developer Guide - Extending the App, Code Reference, Contribution Guide.</li> <li>Release Notes / Changelog.</li> <li>Frequently Asked Questions.</li> </ul>",
+            "title": "Documentation"
         },
         {
             "location": "admin/compatibility_matrix.html",
             "text": "<p>Show Tech has been designed to work primarily as a standalone python package.  Show Tech can be installed and registered with Nautobot as an Nautobot App.  This enables Show Tech Checks to be ran as as Nautobot Jobs.</p>",
             "title": "Compatibility Matrix"
         },
         {
@@ -437,15 +437,15 @@
         {
             "location": "user/app_overview.html#audience-user-personas-who-should-use-this-app",
             "text": "<p>All users of Nautobot are encouraged to use Show Tech any time there is the need for troubleshooting the Nautobot environment.</p>",
             "title": "Audience (User Personas) - Who should use this App?"
         },
         {
             "location": "user/app_overview.html#authors-and-maintainers",
-            "text": "<p>Matt Miller Nikko Hayde</p>",
+            "text": "<p>Matt Miller Nikko Hayden</p>",
             "title": "Authors and Maintainers"
         },
         {
             "location": "user/app_use_cases.html",
             "text": "<p>This document describes common use-cases and scenarios for this App.</p>",
             "title": "Using the App"
         },
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml`

 * *Files 8% similar despite different names*

#### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/sitemap.xml`

```diff
@@ -1,93 +1,93 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://doshow-tech/en/latest/index.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/compatibility_matrix.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/install.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/uninstall.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/upgrade.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/release_notes/index.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/admin/release_notes/version_1.0.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/contributing.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/dev_environment.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/extending.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/framework.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/code_reference/index.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/code_reference/api.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/dev/code_reference/package.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/app_getting_started.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/app_overview.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/app_use_cases.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://doshow-tech/en/latest/user/faq.html</loc>
-    <lastmod>2024-04-10</lastmod>
+    <lastmod>2024-04-29</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_getting_started.html`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -939,24 +939,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/app_getting_started.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/app_getting_started.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/app_getting_started.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/app_getting_started.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="getting-started-with-the-app">Getting Started with the App<a class="headerlink" href="#getting-started-with-the-app" title="Permanent link">&para;</a></h1>
@@ -1030,15 +1030,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_overview.html`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -925,24 +925,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/app_overview.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/app_overview.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/app_overview.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/app_overview.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="app-overview">App Overview<a class="headerlink" href="#app-overview" title="Permanent link">&para;</a></h1>
@@ -953,27 +953,15 @@
 </div>
 <h2 id="description">Description<a class="headerlink" href="#description" title="Permanent link">&para;</a></h2>
 <p>Purpose: When troubleshooting an environment, it is best to be able to answer questions about the environment quickly. This process is difficult to perform with a back and forth with a customer. Therefore, Show Tech is designed to aggregate that information together and provide it in a easy to consume format as a one-time ask. The goal is to aid in troubleshooting managed service customer environments, but can absolutely be extended to do more or be used to stakeholder requirements.</p>
 <h2 id="audience-user-personas-who-should-use-this-app">Audience (User Personas) - Who should use this App?<a class="headerlink" href="#audience-user-personas-who-should-use-this-app" title="Permanent link">&para;</a></h2>
 <p>All users of Nautobot are encouraged to use Show Tech any time there is the need for troubleshooting the Nautobot environment.</p>
 <h2 id="authors-and-maintainers">Authors and Maintainers<a class="headerlink" href="#authors-and-maintainers" title="Permanent link">&para;</a></h2>
 <p>Matt Miller
-Nikko Hayde</p>
-<!--- To be added once Show Tech is a more defined plugin to Nautobot
-## Nautobot Features Used
-
-!!! warning "Developer Note - Remove Me!"
-    What is shown today in the Installed Plugins page in Nautobot. What parts of Nautobot does it interact with, what does it add etc. ?
-
-### Extras
-
-!!! warning "Developer Note - Remove Me!"
-    Custom Fields - things like which CFs are created by this app?
-    Jobs - are jobs, if so, which ones, installed by this app?
--->
+Nikko Hayden</p>
 
 
 
 
 
                 
               </article>
@@ -1028,15 +1016,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

#### html2text {}

```diff
@@ -61,15 +61,15 @@
 as a one-time ask. The goal is to aid in troubleshooting managed service
 customer environments, but can absolutely be extended to do more or be used to
 stakeholder requirements.
 ********** AAuuddiieennccee ((UUsseerr PPeerrssoonnaass)) -- WWhhoo sshhoouulldd uussee tthhiiss AApppp??_?¶ **********
 All users of Nautobot are encouraged to use Show Tech any time there is the
 need for troubleshooting the Nautobot environment.
 ********** AAuutthhoorrss aanndd MMaaiinnttaaiinneerrss_?¶ **********
-Matt Miller Nikko Hayde
+Matt Miller Nikko Hayden
 _P_r_e_v_i_o_u_s
 _O_v_e_r_v_i_e_w
 _N_e_x_t
 _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
 Copyright © The Authors
 _A_p_a_c_h_e_-_2_._0_ _L_I_C_E_N_S_E
 _M_a_d_e_ _w_i_t_h_ _M_a_t_e_r_i_a_l_ _f_o_r_ _M_k_D_o_c_s | _J_o_i_n_ _N_a_u_t_o_b_o_t_ _S_l_a_c_k | _S_p_o_n_s_o_r_e_d_ _b_y_[_._._/_a_s_s_e_t_s_/
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/user/app_use_cases.html`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -312,15 +312,15 @@
   <img src="../assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -897,24 +897,24 @@
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/app_use_cases.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/app_use_cases.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/app_use_cases.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/app_use_cases.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
 <h1 id="using-the-app">Using the App<a class="headerlink" href="#using-the-app" title="Permanent link">&para;</a></h1>
@@ -980,15 +980,15 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/static/nautobot_show_tech/docs/user/faq.html` & `nautobot_show_tech-2.0.1/nautobot_show_tech/static/nautobot_show_tech/docs/index.html`

 * *Files 23% similar despite different names*

```diff
@@ -4,35 +4,33 @@
   <head>
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
-        <link rel="canonical" href="https://doshow-tech/en/latest/user/faq.html">
+        <link rel="canonical" href="https://doshow-tech/en/latest/index.html">
       
       
-        <link rel="prev" href="app_use_cases.html">
       
+        <link rel="next" href="user/app_overview.html">
       
-        <link rel="next" href="../admin/install.html">
-      
-      <link rel="icon" href="../assets/favicon.ico">
+      <link rel="icon" href="assets/favicon.ico">
       <meta name="generator" content="mkdocs-1.5.2, mkdocs-material-9.1.15">
     
     
       
-        <title>Frequently Asked Questions - Nautobot Show Tech Documentation</title>
+        <title>Nautobot Show Tech Documentation</title>
       
     
     
-      <link rel="stylesheet" href="../assets/stylesheets/main.26e3688c.min.css">
+      <link rel="stylesheet" href="assets/stylesheets/main.26e3688c.min.css">
       
         
-        <link rel="stylesheet" href="../assets/stylesheets/palette.ecc896b0.min.css">
+        <link rel="stylesheet" href="assets/stylesheets/palette.ecc896b0.min.css">
       
       
 
     
     
     
       
@@ -40,19 +38,19 @@
         
         <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
         <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,300i,400,400i,700,700i%7CRoboto+Mono:400,400i,700,700i&display=fallback">
         <style>:root{--md-text-font:"Roboto";--md-code-font:"Roboto Mono"}</style>
       
     
     
-      <link rel="stylesheet" href="../assets/_mkdocstrings.css">
+      <link rel="stylesheet" href="assets/_mkdocstrings.css">
     
-      <link rel="stylesheet" href="../assets/extra.css">
+      <link rel="stylesheet" href="assets/extra.css">
     
-    <script>__md_scope=new URL("..",location),__md_hash=e=>[...e].reduce((e,_)=>(e<<5)-e+_.charCodeAt(0),0),__md_get=(e,_=localStorage,t=__md_scope)=>JSON.parse(_.getItem(t.pathname+"."+e)),__md_set=(e,_,t=localStorage,a=__md_scope)=>{try{t.setItem(a.pathname+"."+e,JSON.stringify(_))}catch(e){}}</script>
+    <script>__md_scope=new URL(".",location),__md_hash=e=>[...e].reduce((e,_)=>(e<<5)-e+_.charCodeAt(0),0),__md_get=(e,_=localStorage,t=__md_scope)=>JSON.parse(_.getItem(t.pathname+"."+e)),__md_set=(e,_,t=localStorage,a=__md_scope)=>{try{t.setItem(a.pathname+"."+e,JSON.stringify(_))}catch(e){}}</script>
     
       
 
     
     
     
   </head>
@@ -73,15 +71,15 @@
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#frequently-asked-questions" class="md-skip">
+        <a href="#nautobot-show-tech" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
@@ -89,17 +87,17 @@
     
       
 
   
 
 <header class="md-header md-header--shadow md-header--lifted" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href="../index.html" title="Nautobot Show Tech Documentation" class="md-header__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
+    <a href="index.html" title="Nautobot Show Tech Documentation" class="md-header__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
       
-  <img src="../assets/nautobot_logo.svg" alt="logo">
+  <img src="assets/nautobot_logo.svg" alt="logo">
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2Z"/></svg>
     </label>
     <div class="md-header__title" data-md-component="header-title">
       <div class="md-header__ellipsis">
@@ -107,15 +105,15 @@
           <span class="md-ellipsis">
             Nautobot Show Tech Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Frequently Asked Questions
+              Overview
             
           </span>
         </div>
       </div>
     </div>
     
       
@@ -183,15 +181,15 @@
       </div>
     </div>
   </div>
 </div>
     
     
       <div class="md-header__source">
-        <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+        <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -205,35 +203,35 @@
 <nav class="md-tabs" aria-label="Tabs" data-md-component="tabs">
   <div class="md-grid">
     <ul class="md-tabs__list">
       
         
   
   
+    
+  
 
 
   <li class="md-tabs__item">
-    <a href="../index.html" class="md-tabs__link">
+    <a href="index.html" class="md-tabs__link md-tabs__link--active">
       Overview
     </a>
   </li>
 
       
         
   
   
-    
-  
 
 
   
   
   
     <li class="md-tabs__item">
-      <a href="app_overview.html" class="md-tabs__link md-tabs__link--active">
+      <a href="user/app_overview.html" class="md-tabs__link">
         User Guide
       </a>
     </li>
   
 
       
         
@@ -241,15 +239,15 @@
   
 
 
   
   
   
     <li class="md-tabs__item">
-      <a href="../admin/install.html" class="md-tabs__link">
+      <a href="admin/install.html" class="md-tabs__link">
         Administrator Guide
       </a>
     </li>
   
 
       
         
@@ -257,15 +255,15 @@
   
 
 
   
   
   
     <li class="md-tabs__item">
-      <a href="../dev/extending.html" class="md-tabs__link">
+      <a href="dev/extending.html" class="md-tabs__link">
         Developer Guide
       </a>
     </li>
   
 
       
         
@@ -293,34 +291,36 @@
         
       
       <main class="md-main" data-md-component="main">
         <div class="md-main__inner md-grid">
           
             
               
-              <div class="md-sidebar md-sidebar--primary" data-md-component="sidebar" data-md-type="navigation" >
+                
+              
+              <div class="md-sidebar md-sidebar--primary" data-md-component="sidebar" data-md-type="navigation" hidden>
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
   
 
 
 <nav class="md-nav md-nav--primary md-nav--lifted" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href="../index.html" title="Nautobot Show Tech Documentation" class="md-nav__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
+    <a href="index.html" title="Nautobot Show Tech Documentation" class="md-nav__button md-logo" aria-label="Nautobot Show Tech Documentation" data-md-component="logo">
       
-  <img src="../assets/nautobot_logo.svg" alt="logo">
+  <img src="assets/nautobot_logo.svg" alt="logo">
 
     </a>
     Nautobot Show Tech Documentation
   </label>
   
     <div class="md-nav__source">
-      <a href="https://github.com/networktocode/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
+      <a href="https://github.com/networktocode-llc/nautobot-app-show-tech" title="Go to repository" class="md-source" data-md-component="source">
   <div class="md-source__icon md-icon">
     
     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512"><!--! Font Awesome Free 6.4.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license/free (Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT License) Copyright 2023 Fonticons, Inc.--><path d="M439.55 236.05 244 40.45a28.87 28.87 0 0 0-40.81 0l-40.66 40.63 51.52 51.52c27.06-9.14 52.68 16.77 43.39 43.68l49.66 49.66c34.23-11.8 61.18 31 35.47 56.69-26.49 26.49-70.21-2.87-56-37.34L240.22 199v121.85c25.3 12.54 22.26 41.85 9.08 55a34.34 34.34 0 0 1-48.55 0c-17.57-17.6-11.07-46.91 11.25-56v-123c-20.8-8.51-24.6-30.74-18.64-45L142.57 101 8.45 235.14a28.86 28.86 0 0 0 0 40.81l195.61 195.6a28.86 28.86 0 0 0 40.8 0l194.69-194.69a28.86 28.86 0 0 0 0-40.81z"/></svg>
   </div>
   <div class="md-source__repository">
     GitHub
   </div>
@@ -331,39 +331,132 @@
     
       
       
       
 
   
   
+    
   
-    <li class="md-nav__item">
-      <a href="../index.html" class="md-nav__link">
+  
+    <li class="md-nav__item md-nav__item--active">
+      
+      <input class="md-nav__toggle md-toggle" type="checkbox" id="__toc">
+      
+      
+        
+      
+      
+        <label class="md-nav__link md-nav__link--active" for="__toc">
+          Overview
+          <span class="md-nav__icon md-icon"></span>
+        </label>
+      
+      <a href="index.html" class="md-nav__link md-nav__link--active">
         Overview
       </a>
+      
+        
+
+<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
+  
+  
+  
+    
+  
+  
+    <label class="md-nav__title" for="__toc">
+      <span class="md-nav__icon md-icon"></span>
+      Table of contents
+    </label>
+    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
+      
+        <li class="md-nav__item">
+  <a href="#overview" class="md-nav__link">
+    Overview
+  </a>
+  
+    <nav class="md-nav" aria-label="Overview">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#purpose-providing-diagnostics-in-a-nautobot-environment" class="md-nav__link">
+    Purpose: Providing diagnostics in a Nautobot environment
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#versions-nautobot-2x-or-1x-compatible" class="md-nav__link">
+    Versions: Nautobot 2.X or 1.X compatible
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#screenshots" class="md-nav__link">
+    Screenshots
+  </a>
+  
+    <nav class="md-nav" aria-label="Screenshots">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#recorded-examples" class="md-nav__link">
+    Recorded Examples
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#current-release" class="md-nav__link">
+    Current Release
+  </a>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#documentation" class="md-nav__link">
+    Documentation
+  </a>
+  
+</li>
+      
+    </ul>
+  
+</nav>
+      
     </li>
   
 
     
       
       
       
 
   
   
-    
-  
   
     
-    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
+    <li class="md-nav__item md-nav__item--nested">
       
       
       
       
-      <input class="md-nav__toggle md-toggle " type="checkbox" id="__nav_2" checked>
+      <input class="md-nav__toggle md-toggle " type="checkbox" id="__nav_2" >
       
       
         
           
         
           
         
@@ -374,82 +467,72 @@
       
       
         <label class="md-nav__link" for="__nav_2" id="__nav_2_label" tabindex="0">
           User Guide
           <span class="md-nav__icon md-icon"></span>
         </label>
       
-      <nav class="md-nav" data-md-level="1" aria-labelledby="__nav_2_label" aria-expanded="true">
+      <nav class="md-nav" data-md-level="1" aria-labelledby="__nav_2_label" aria-expanded="false">
         <label class="md-nav__title" for="__nav_2">
           <span class="md-nav__icon md-icon"></span>
           User Guide
         </label>
         <ul class="md-nav__list" data-md-scrollfix>
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="app_overview.html" class="md-nav__link">
+      <a href="user/app_overview.html" class="md-nav__link">
         App Overview
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="app_getting_started.html" class="md-nav__link">
+      <a href="user/app_getting_started.html" class="md-nav__link">
         Getting Started
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="app_use_cases.html" class="md-nav__link">
+      <a href="user/app_use_cases.html" class="md-nav__link">
         Using the App
       </a>
     </li>
   
 
             
           
             
               
   
   
-    
   
-  
-    <li class="md-nav__item md-nav__item--active">
-      
-      <input class="md-nav__toggle md-toggle" type="checkbox" id="__toc">
-      
-      
-        
-      
-      
-      <a href="faq.html" class="md-nav__link md-nav__link--active">
+    <li class="md-nav__item">
+      <a href="user/faq.html" class="md-nav__link">
         Frequently Asked Questions
       </a>
-      
     </li>
   
 
             
           
         </ul>
       </nav>
@@ -500,57 +583,57 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../admin/install.html" class="md-nav__link">
+      <a href="admin/install.html" class="md-nav__link">
         Install and Configure
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../admin/upgrade.html" class="md-nav__link">
+      <a href="admin/upgrade.html" class="md-nav__link">
         Upgrade
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../admin/uninstall.html" class="md-nav__link">
+      <a href="admin/uninstall.html" class="md-nav__link">
         Uninstall
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../admin/compatibility_matrix.html" class="md-nav__link">
+      <a href="admin/compatibility_matrix.html" class="md-nav__link">
         Compatibility Matrix
       </a>
     </li>
   
 
             
           
@@ -576,15 +659,15 @@
           
         
       
       
         
         
         <div class="md-nav__link md-nav__link--index ">
-          <a href="../admin/release_notes/index.html">Release Notes</a>
+          <a href="admin/release_notes/index.html">Release Notes</a>
           
             <label for="__nav_3_5">
               <span class="md-nav__icon md-icon"></span>
             </label>
           
         </div>
       
@@ -599,15 +682,15 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../admin/release_notes/version_1.0.html" class="md-nav__link">
+      <a href="admin/release_notes/version_1.0.html" class="md-nav__link">
         v1.0
       </a>
     </li>
   
 
             
           
@@ -667,57 +750,57 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../dev/extending.html" class="md-nav__link">
+      <a href="dev/extending.html" class="md-nav__link">
         Extending the App
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../dev/contributing.html" class="md-nav__link">
+      <a href="dev/contributing.html" class="md-nav__link">
         Contributing to the App
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../dev/dev_environment.html" class="md-nav__link">
+      <a href="dev/dev_environment.html" class="md-nav__link">
         Development Environment
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../dev/framework.html" class="md-nav__link">
+      <a href="dev/framework.html" class="md-nav__link">
         Framework for the App
       </a>
     </li>
   
 
             
           
@@ -745,15 +828,15 @@
           
         
       
       
         
         
         <div class="md-nav__link md-nav__link--index ">
-          <a href="../dev/code_reference/index.html">Code Reference</a>
+          <a href="dev/code_reference/index.html">Code Reference</a>
           
             <label for="__nav_4_5">
               <span class="md-nav__icon md-icon"></span>
             </label>
           
         </div>
       
@@ -768,29 +851,29 @@
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../dev/code_reference/package.html" class="md-nav__link">
+      <a href="dev/code_reference/package.html" class="md-nav__link">
         Package
       </a>
     </li>
   
 
             
           
             
               
   
   
   
     <li class="md-nav__item">
-      <a href="../dev/code_reference/api.html" class="md-nav__link">
+      <a href="dev/code_reference/api.html" class="md-nav__link">
         API
       </a>
     </li>
   
 
             
           
@@ -826,67 +909,166 @@
 </nav>
                   </div>
                 </div>
               </div>
             
             
               
+                
+              
               <div class="md-sidebar md-sidebar--secondary" data-md-component="sidebar" data-md-type="toc" >
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
   
     
   
   
+    <label class="md-nav__title" for="__toc">
+      <span class="md-nav__icon md-icon"></span>
+      Table of contents
+    </label>
+    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
+      
+        <li class="md-nav__item">
+  <a href="#overview" class="md-nav__link">
+    Overview
+  </a>
+  
+    <nav class="md-nav" aria-label="Overview">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#purpose-providing-diagnostics-in-a-nautobot-environment" class="md-nav__link">
+    Purpose: Providing diagnostics in a Nautobot environment
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#versions-nautobot-2x-or-1x-compatible" class="md-nav__link">
+    Versions: Nautobot 2.X or 1.X compatible
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#screenshots" class="md-nav__link">
+    Screenshots
+  </a>
+  
+    <nav class="md-nav" aria-label="Screenshots">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#recorded-examples" class="md-nav__link">
+    Recorded Examples
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#current-release" class="md-nav__link">
+    Current Release
+  </a>
+  
+</li>
+      
+        <li class="md-nav__item">
+  <a href="#documentation" class="md-nav__link">
+    Documentation
+  </a>
+  
+</li>
+      
+    </ul>
+  
 </nav>
                   </div>
                 </div>
               </div>
             
           
           
             <div class="md-content" data-md-component="content">
               <article class="md-content__inner md-typeset">
                 
                   
 
   
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/user/faq.md" title="Edit this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/edit/main/nautobot-app-show-tech/docs/index.md" title="Edit this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 20H6V4h7v5h5v3.1l2-2V8l-6-6H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h4v-2m10.2-7c.1 0 .3.1.4.2l1.3 1.3c.2.2.2.6 0 .8l-1 1-2.1-2.1 1-1c.1-.1.2-.2.4-.2m0 3.9L14.1 23H12v-2.1l6.1-6.1 2.1 2.1Z"/></svg>
     </a>
   
   
     
       
     
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/user/faq.md" title="View source of this page" class="md-content__button md-icon">
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/raw/main/nautobot-app-show-tech/docs/index.md" title="View source of this page" class="md-content__button md-icon">
       
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17 18c.56 0 1 .44 1 1s-.44 1-1 1-1-.44-1-1 .44-1 1-1m0-3c-2.73 0-5.06 1.66-6 4 .94 2.34 3.27 4 6 4s5.06-1.66 6-4c-.94-2.34-3.27-4-6-4m0 6.5a2.5 2.5 0 0 1-2.5-2.5 2.5 2.5 0 0 1 2.5-2.5 2.5 2.5 0 0 1 2.5 2.5 2.5 2.5 0 0 1-2.5 2.5M9.27 20H6V4h7v5h5v4.07c.7.08 1.36.25 2 .49V8l-6-6H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h4.5a8.15 8.15 0 0 1-1.23-2Z"/></svg>
     </a>
   
 
 
-<h1 id="frequently-asked-questions">Frequently Asked Questions<a class="headerlink" href="#frequently-asked-questions" title="Permanent link">&para;</a></h1>
-<p><strong>Is Show Tech a standalone program or a Nautobot App?</strong>
-- Show Tech is primarily intended a standalone program, however it can be registered as a Nautobot App. The reason being is that if Nautobot is down, Show Tech needs to be able to continue to function.</p>
-<p><strong>Do you recommend installing Show Tech as a Nautobot App?</strong>
-- Yes. The diagnostics functionality is the same however as a Nautobot App we can leverage Nautobot Jobs and Nautobot views for quality-of-life.</p>
-<p><strong>Who is the target audience of Show Tech?</strong>
-- Initially the target audience is anyone looking for assistance in troubleshooting an Nautobot Environment.  Show Tech performs several checks which help provide information about what could be going wrong.
-- Additionally, there are features of Show Tech which may be important to other audiences. We hope to include those people as we iterate Show Tech.</p>
-<p><strong>Why is the name of the App Show Tech?</strong>
-- The name Show Tech was chosen to because it is recognizable to known industry naming patterns for the intended use-case.</p>
+<h1 id="nautobot-show-tech">Nautobot Show Tech<a class="headerlink" href="#nautobot-show-tech" title="Permanent link">&para;</a></h1>
+<p align="center">
+  <img src="./docs/images/icon-nautobot-show-tech.png?raw=true" class="logo" height="200px">
+  <br>
+  <a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest"><img src="https://readthedocs.org/projects/nautobot-app-show-tech/badge/"></a>
+  <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/v/nautobot-show-tech"></a>
+  <a href="https://pypi.org/project/nautobot-show-tech/"><img src="https://img.shields.io/pypi/dm/nautobot-show-tech"></a>
+  <br>
+  An App for <a href="https://nautobot.com/">Nautobot</a>.
+</p>
+
+<h2 id="overview">Overview<a class="headerlink" href="#overview" title="Permanent link">&para;</a></h2>
+<h3 id="purpose-providing-diagnostics-in-a-nautobot-environment">Purpose: Providing diagnostics in a Nautobot environment<a class="headerlink" href="#purpose-providing-diagnostics-in-a-nautobot-environment" title="Permanent link">&para;</a></h3>
+<p>When troubleshooting an environment, it is best to be able to answer questions about the environment quickly. This process is challenging to perform with a back-and-forth with a customer. Therefore, Nautobot Show Tech is designed to aggregate and provide that information in an easy-to-consume format as a one-time ask. The goal is to aid in troubleshooting managed service customer environments, but it can be extended to do more or be used to meet stakeholder requirements.</p>
+<h3 id="versions-nautobot-2x-or-1x-compatible">Versions: Nautobot 2.X or 1.X compatible<a class="headerlink" href="#versions-nautobot-2x-or-1x-compatible" title="Permanent link">&para;</a></h3>
+<p>Nautobot Show Tech is versioned in coordination with the Major Release version of Nautobot.  Please be sure to use the appropriate version for best diagnostic return results.
+- Nautobot Show Tech 2.X will support Nautobot 2.X environments.
+- Nautobot Show Tech 1.X will support Nautobot 1.X environments.</p>
+<h3 id="screenshots">Screenshots<a class="headerlink" href="#screenshots" title="Permanent link">&para;</a></h3>
+<p><img alt="Show Tech GUI Job Run Mem Info" src="./docs/images/show_tech_gui_job_run.png" /></p>
+<p><img alt="Show Tech GUI Job Result Mem Info" src="./docs/images/show_tech_gui_job_result.png" /></p>
+<p><img alt="Show Tech CLI Mem Info" src="./docs/images/show_tech_cli_meminfo.png" /></p>
+<h4 id="recorded-examples">Recorded Examples<a class="headerlink" href="#recorded-examples" title="Permanent link">&para;</a></h4>
+<p><img alt="Show_Tech_GUI" src="./docs/images/show_tech_gui_example.webm" /></p>
+<p><img alt="Show_Tech_CLI" src="./docs/images/show_tech_cli_example.webm" /></p>
+<h2 id="current-release">Current Release<a class="headerlink" href="#current-release" title="Permanent link">&para;</a></h2>
+<p>This App is available is not currently open sourced.  Instead it is currently available via <a href="https://pypi.org/">pypi.org</a> and the maintainers are not accepting feature requests, bugs, or pull requests at this time.</p>
+<h2 id="documentation">Documentation<a class="headerlink" href="#documentation" title="Permanent link">&para;</a></h2>
+<p>Coming Soon. Until then, use this readme and the <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/tree/main/docs"><code>docs</code></a> folder in this repository.</p>
+<ul>
+<li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/app_overview/">User Guide</a> - Overview, Using the App, Getting Started.</li>
+<li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/install/">Administrator Guide</a> - How to Install, Configure, Upgrade, or Uninstall the App.</li>
+<li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/dev/contributing/">Developer Guide</a> - Extending the App, Code Reference, Contribution Guide.</li>
+<li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/admin/release_notes/">Release Notes / Changelog</a>.</li>
+<li><a href="https://docs.nautobot.com/projects/nautobot-show-tech/en/latest/user/faq/">Frequently Asked Questions</a>.</li>
+</ul>
+
 
 
+  
 
 
 
                 
               </article>
             </div>
           
@@ -895,40 +1077,27 @@
         
       </main>
       
         <footer class="md-footer">
   
     
       
-      <nav class="md-footer__inner md-grid" aria-label="Footer" >
         
-          
-          <a href="app_use_cases.html" class="md-footer__link md-footer__link--prev" aria-label="Previous: Using the App" rel="prev">
-            <div class="md-footer__button md-icon">
-              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12Z"/></svg>
-            </div>
-            <div class="md-footer__title">
-              <span class="md-footer__direction">
-                Previous
-              </span>
-              <div class="md-ellipsis">
-                Using the App
-              </div>
-            </div>
-          </a>
+      
+      <nav class="md-footer__inner md-grid" aria-label="Footer" >
         
         
           
-          <a href="../admin/install.html" class="md-footer__link md-footer__link--next" aria-label="Next: Install and Configure" rel="next">
+          <a href="user/app_overview.html" class="md-footer__link md-footer__link--next" aria-label="Next: App Overview" rel="next">
             <div class="md-footer__title">
               <span class="md-footer__direction">
                 Next
               </span>
               <div class="md-ellipsis">
-                Install and Configure
+                App Overview
               </div>
             </div>
             <div class="md-footer__button md-icon">
               <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4Z"/></svg>
             </div>
           </a>
         
@@ -939,24 +1108,24 @@
     <div class="md-footer-meta__inner md-grid">
       
 <div class="md-copyright">
     
     <div class="md-copyright__highlight">
         Copyright &copy; The Authors
     </div>
-    <a href="https://github.com/networktocode/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
+    <a href="https://github.com/networktocode-llc/nautobot-app-show-tech/blob/main/LICENSE">Apache-2.0 LICENSE</a>
     
 </div>
 
 <div class="md-copyright">
     <a href="https://squidfunk.github.io/mkdocs-material/" target="_blank" rel="noopener">Made with Material for MkDocs</a>
     | <a href="https://www.networktocode.com/community/" target="_blank" rel="noopener">Join Nautobot Slack</a>
     
     | <a href="https://networktocode.com" target="_blank" rel="noopener">Sponsored by <img
-            src=../assets/networktocode_bw.png class="copyright-logo"></a>
+            src=assets/networktocode_bw.png class="copyright-logo"></a>
     
 </div>
 
 <!-- RTD version flyout injected on live site -->
 <div id="readthedocs-embed-flyout"></div>
 
       
@@ -1009,17 +1178,17 @@
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
     
-    <script id="__config" type="application/json">{"base": "..", "features": ["content.action.edit", "content.action.view", "content.code.copy", "navigation.footer", "navigation.indexes", "navigation.tabs", "navigation.tabs.sticky", "navigation.tracking", "search.highlight", "search.share", "search.suggest"], "search": "../assets/javascripts/workers/search.208ed371.min.js", "translations": {"clipboard.copied": "Copied to clipboard", "clipboard.copy": "Copy to clipboard", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.placeholder": "Type to start searching", "search.result.term.missing": "Missing", "select.version": "Select version"}}</script>
+    <script id="__config" type="application/json">{"base": ".", "features": ["content.action.edit", "content.action.view", "content.code.copy", "navigation.footer", "navigation.indexes", "navigation.tabs", "navigation.tabs.sticky", "navigation.tracking", "search.highlight", "search.share", "search.suggest"], "search": "assets/javascripts/workers/search.208ed371.min.js", "translations": {"clipboard.copied": "Copied to clipboard", "clipboard.copy": "Copy to clipboard", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.placeholder": "Type to start searching", "search.result.term.missing": "Missing", "select.version": "Select version"}}</script>
     
     
-      <script src="../assets/javascripts/bundle.b4d07000.min.js"></script>
+      <script src="assets/javascripts/bundle.b4d07000.min.js"></script>
       
         <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,29 +1,36 @@
 ????
 _S_k_i_p_ _t_o_ _c_o_n_t_e_n_t
 _[_l_o_g_o_]
 Nautobot Show Tech Documentation
-Frequently Asked Questions
+Overview
 oo
 [query               ]
 Initializing search
 _G_i_t_H_u_b
     * _O_v_e_r_v_i_e_w
     * _U_s_e_r_ _G_u_i_d_e
     * _A_d_m_i_n_i_s_t_r_a_t_o_r_ _G_u_i_d_e
     * _D_e_v_e_l_o_p_e_r_ _G_u_i_d_e
     * _N_a_u_t_o_b_o_t_ _D_o_c_s_ _H_o_m_e_ _↗_︎
 _[_l_o_g_o_]Nautobot Show Tech Documentation
 _G_i_t_H_u_b
-    * _O_v_e_r_v_i_e_w
-    * User Guide User Guide
+    * ??Overview _O_v_e_r_v_i_e_w_ Table of contents
+          o _O_v_e_r_v_i_e_w
+                # _P_u_r_p_o_s_e_:_ _P_r_o_v_i_d_i_n_g_ _d_i_a_g_n_o_s_t_i_c_s_ _i_n_ _a_ _N_a_u_t_o_b_o_t_ _e_n_v_i_r_o_n_m_e_n_t
+                # _V_e_r_s_i_o_n_s_:_ _N_a_u_t_o_b_o_t_ _2_._X_ _o_r_ _1_._X_ _c_o_m_p_a_t_i_b_l_e
+                # _S_c_r_e_e_n_s_h_o_t_s
+                      # _R_e_c_o_r_d_e_d_ _E_x_a_m_p_l_e_s
+          o _C_u_r_r_e_n_t_ _R_e_l_e_a_s_e
+          o _D_o_c_u_m_e_n_t_a_t_i_o_n
+    * ??User Guide User Guide
           o _A_p_p_ _O_v_e_r_v_i_e_w
           o _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _U_s_i_n_g_ _t_h_e_ _A_p_p
-          o ??_F_r_e_q_u_e_n_t_l_y_ _A_s_k_e_d_ _Q_u_e_s_t_i_o_n_s
+          o _F_r_e_q_u_e_n_t_l_y_ _A_s_k_e_d_ _Q_u_e_s_t_i_o_n_s
     * ??Administrator Guide Administrator Guide
           o _I_n_s_t_a_l_l_ _a_n_d_ _C_o_n_f_i_g_u_r_e
           o _U_p_g_r_a_d_e
           o _U_n_i_n_s_t_a_l_l
           o _C_o_m_p_a_t_i_b_i_l_i_t_y_ _M_a_t_r_i_x
           o ??
             _R_e_l_e_a_s_e_ _N_o_t_e_s
@@ -36,32 +43,61 @@
           o _F_r_a_m_e_w_o_r_k_ _f_o_r_ _t_h_e_ _A_p_p
           o ??
             _C_o_d_e_ _R_e_f_e_r_e_n_c_e
             Code Reference
                 # _P_a_c_k_a_g_e
                 # _A_P_I
     * _N_a_u_t_o_b_o_t_ _D_o_c_s_ _H_o_m_e_ _↗_︎
-************ FFrreeqquueennttllyy AAsskkeedd QQuueessttiioonnss_?¶ ************
-IIss SShhooww TTeecchh aa ssttaannddaalloonnee pprrooggrraamm oorr aa NNaauuttoobboott AApppp?? - Show Tech is primarily
-intended a standalone program, however it can be registered as a Nautobot App.
-The reason being is that if Nautobot is down, Show Tech needs to be able to
-continue to function.
-DDoo yyoouu rreeccoommmmeenndd iinnssttaalllliinngg SShhooww TTeecchh aass aa NNaauuttoobboott AApppp?? - Yes. The diagnostics
-functionality is the same however as a Nautobot App we can leverage Nautobot
-Jobs and Nautobot views for quality-of-life.
-WWhhoo iiss tthhee ttaarrggeett aauuddiieennccee ooff SShhooww TTeecchh?? - Initially the target audience is
-anyone looking for assistance in troubleshooting an Nautobot Environment. Show
-Tech performs several checks which help provide information about what could be
-going wrong. - Additionally, there are features of Show Tech which may be
-important to other audiences. We hope to include those people as we iterate
-Show Tech.
-WWhhyy iiss tthhee nnaammee ooff tthhee AApppp SShhooww TTeecchh?? - The name Show Tech was chosen to
-because it is recognizable to known industry naming patterns for the intended
-use-case.
-_P_r_e_v_i_o_u_s
-_U_s_i_n_g_ _t_h_e_ _A_p_p
+Table of contents
+    * _O_v_e_r_v_i_e_w
+          o _P_u_r_p_o_s_e_:_ _P_r_o_v_i_d_i_n_g_ _d_i_a_g_n_o_s_t_i_c_s_ _i_n_ _a_ _N_a_u_t_o_b_o_t_ _e_n_v_i_r_o_n_m_e_n_t
+          o _V_e_r_s_i_o_n_s_:_ _N_a_u_t_o_b_o_t_ _2_._X_ _o_r_ _1_._X_ _c_o_m_p_a_t_i_b_l_e
+          o _S_c_r_e_e_n_s_h_o_t_s
+                # _R_e_c_o_r_d_e_d_ _E_x_a_m_p_l_e_s
+    * _C_u_r_r_e_n_t_ _R_e_l_e_a_s_e
+    * _D_o_c_u_m_e_n_t_a_t_i_o_n
+************ NNaauuttoobboott SShhooww TTeecchh_?¶ ************
+             [./docs/images/icon-nautobot-show-tech.png?raw=true]
+   _[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_a_p_p_-_s_h_o_w_-_t_e_c_h_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/
+   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
+                              _n_a_u_t_o_b_o_t_-_s_h_o_w_-_t_e_c_h_]
+                             An App for _N_a_u_t_o_b_o_t.
+********** OOvveerrvviieeww_?¶ **********
+******** PPuurrppoossee:: PPrroovviiddiinngg ddiiaaggnnoossttiiccss iinn aa NNaauuttoobboott eennvviirroonnmmeenntt_?¶ ********
+When troubleshooting an environment, it is best to be able to answer questions
+about the environment quickly. This process is challenging to perform with a
+back-and-forth with a customer. Therefore, Nautobot Show Tech is designed to
+aggregate and provide that information in an easy-to-consume format as a one-
+time ask. The goal is to aid in troubleshooting managed service customer
+environments, but it can be extended to do more or be used to meet stakeholder
+requirements.
+******** VVeerrssiioonnss:: NNaauuttoobboott 22..XX oorr 11..XX ccoommppaattiibbllee_?¶ ********
+Nautobot Show Tech is versioned in coordination with the Major Release version
+of Nautobot. Please be sure to use the appropriate version for best diagnostic
+return results. - Nautobot Show Tech 2.X will support Nautobot 2.X
+environments. - Nautobot Show Tech 1.X will support Nautobot 1.X environments.
+******** SSccrreeeennsshhoottss_?¶ ********
+[Show Tech GUI Job Run Mem Info]
+[Show Tech GUI Job Result Mem Info]
+[Show Tech CLI Mem Info]
+****** RReeccoorrddeedd EExxaammpplleess_?¶ ******
+[Show_Tech_GUI]
+[Show_Tech_CLI]
+********** CCuurrrreenntt RReelleeaassee_?¶ **********
+This App is available is not currently open sourced. Instead it is currently
+available via _p_y_p_i_._o_r_g and the maintainers are not accepting feature requests,
+bugs, or pull requests at this time.
+********** DDooccuummeennttaattiioonn_?¶ **********
+Coming Soon. Until then, use this readme and the _d_o_c_s folder in this
+repository.
+    * _U_s_e_r_ _G_u_i_d_e - Overview, Using the App, Getting Started.
+    * _A_d_m_i_n_i_s_t_r_a_t_o_r_ _G_u_i_d_e - How to Install, Configure, Upgrade, or Uninstall
+      the App.
+    * _D_e_v_e_l_o_p_e_r_ _G_u_i_d_e - Extending the App, Code Reference, Contribution Guide.
+    * _R_e_l_e_a_s_e_ _N_o_t_e_s_ _/_ _C_h_a_n_g_e_l_o_g.
+    * _F_r_e_q_u_e_n_t_l_y_ _A_s_k_e_d_ _Q_u_e_s_t_i_o_n_s.
 _N_e_x_t
-_I_n_s_t_a_l_l_ _a_n_d_ _C_o_n_f_i_g_u_r_e
+_A_p_p_ _O_v_e_r_v_i_e_w
 Copyright © The Authors
 _A_p_a_c_h_e_-_2_._0_ _L_I_C_E_N_S_E
-_M_a_d_e_ _w_i_t_h_ _M_a_t_e_r_i_a_l_ _f_o_r_ _M_k_D_o_c_s | _J_o_i_n_ _N_a_u_t_o_b_o_t_ _S_l_a_c_k | _S_p_o_n_s_o_r_e_d_ _b_y_[_._._/_a_s_s_e_t_s_/
+_M_a_d_e_ _w_i_t_h_ _M_a_t_e_r_i_a_l_ _f_o_r_ _M_k_D_o_c_s | _J_o_i_n_ _N_a_u_t_o_b_o_t_ _S_l_a_c_k | _S_p_o_n_s_o_r_e_d_ _b_y_[_a_s_s_e_t_s_/
 _n_e_t_w_o_r_k_t_o_c_o_d_e___b_w_._p_n_g_]
```

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/tests/test_api.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/tests/test_basic.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/nautobot_show_tech/update_readme.py` & `nautobot_show_tech-2.0.1/nautobot_show_tech/update_readme.py`

 * *Files identical despite different names*

### Comparing `nautobot_show_tech-2.0.0/pyproject.toml` & `nautobot_show_tech-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "nautobot-show-tech"
-version = "v2.0.0"
+version = "v2.0.1"
 description = "An app to aid in troubleshooting a Nautobot environment."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/networktocode/nautobot-app-show-tech"
-repository = "https://github.com/networktocode/nautobot-app-show-tech"
+homepage = "https://github.com/networktocode-llc/nautobot-app-show-tech"
+repository = "https://github.com/networktocode-llc/nautobot-app-show-tech"
 documentation = "https://doshow-tech/en/latest/"
 keywords = ["nautobot", "nautobot-app", "nautobot-plugin"]
 classifiers = [
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
@@ -162,15 +162,15 @@
 
 [tool.towncrier]
 package = "nautobot_show_tech"
 directory = "changes"
 filename = "docs/admin/release_notes/version_X.Y.md"
 template = "development/towncrier_template.j2"
 start_string = "<!-- towncrier release notes start -->"
-issue_format = "[#{issue}](https://github.com/networktocode/nautobot-app-show-tech/issues/{issue})"
+issue_format = "[#{issue}](https://github.com/networktocode-llc/nautobot-app-show-tech/issues/{issue})"
 
 [[tool.towncrier.type]]
 directory = "security"
 name = "Security"
 showcontent = true
 
 [[tool.towncrier.type]]
```

