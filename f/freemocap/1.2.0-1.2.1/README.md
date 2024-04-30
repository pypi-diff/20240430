# Comparing `tmp/freemocap-1.2.0.tar.gz` & `tmp/freemocap-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freemocap-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "freemocap-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `freemocap-1.2.0.tar` & `freemocap-1.2.1.tar`

### file list

```diff
@@ -1,275 +1,275 @@
--rw-r--r--   0        0        0     1649 2024-04-29 19:29:24.857720 freemocap-1.2.0/.flake8
--rwxr-xr-x   0        0        0      492 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      423 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      730 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/coverage-testing.yml
--rw-r--r--   0        0        0     1138 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/flit_publish_to_pypi.yml
--rwxr-xr-x   0        0        0      385 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/linting-flake8.yml
--rw-r--r--   0        0        0     2049 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/linux_installer.yml
--rw-r--r--   0        0        0     2613 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/mac_installer.yml
--rw-r--r--   0        0        0     1246 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/publish_to_pypi.yml
--rwxr-xr-x   0        0        0     1018 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/python-testing.yml
--rwxr-xr-x   0        0        0      733 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/version-testing.yml
--rw-r--r--   0        0        0     2312 2024-04-29 19:29:24.857720 freemocap-1.2.0/.github/workflows/windows_installer.yml
--rw-r--r--   0        0        0     2043 2024-04-29 19:29:24.857720 freemocap-1.2.0/.gitignore
--rw-r--r--   0        0        0      229 2024-04-29 19:29:24.857720 freemocap-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      657 2024-04-29 19:29:24.857720 freemocap-1.2.0/CITATION.cff
--rw-r--r--   0        0        0      327 2024-04-29 19:29:24.857720 freemocap-1.2.0/CODEOWNERS
--rw-r--r--   0        0        0     1513 2024-04-29 19:29:24.857720 freemocap-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3552 2024-04-29 19:29:24.857720 freemocap-1.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2024-04-29 19:29:24.857720 freemocap-1.2.0/LICENSE
--rw-r--r--   0        0        0      234 2024-04-29 19:29:24.857720 freemocap-1.2.0/MANIFEST.in
--rw-r--r--   0        0        0     4112 2024-04-29 19:29:24.857720 freemocap-1.2.0/README.md
--rwxr-xr-x   0        0        0      607 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/builds/install_packages
--rwxr-xr-x   0        0        0       66 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/installer.sh
--rwxr-xr-x   0        0        0      278 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/build.sh
--rwxr-xr-x   0        0        0      161 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/run_uvicorn_server.sh
--rwxr-xr-x   0        0        0      381 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/run_web_server.sh
--rwxr-xr-x   0        0        0      118 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/shell.sh
--rwxr-xr-x   0        0        0      104 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/test.sh
--rwxr-xr-x   0        0        0       71 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/linux/up.sh
--rw-r--r--   0        0        0      410 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/windows/installChocolatey.cmd
--rw-r--r--   0        0        0      112 2024-04-29 19:29:24.857720 freemocap-1.2.0/bin/windows/run_web_server.cmd
--rw-r--r--   0        0        0     4783 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/batch_process/batch_process.py
--rw-r--r--   0        0        0     1415 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/batch_process/headless_calibration.py
--rw-r--r--   0        0        0     3495 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/directory_view.py
--rw-r--r--   0        0        0      331 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/freemocap-ui/.gitignore
--rw-r--r--   0        0        0     2358 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/freemocap-ui/README.md
--rw-r--r--   0        0        0      804 2024-04-29 19:29:24.857720 freemocap-1.2.0/experimental/freemocap-ui/config-overrides.js
--rw-r--r--   0        0        0   725486 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/package-lock.json
--rw-r--r--   0        0        0     2548 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/package.json
--rw-r--r--   0        0        0     3585 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/favicon.ico
--rw-r--r--   0        0        0     1919 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/index.html
--rw-r--r--   0        0        0     4153 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/logo192.png
--rw-r--r--   0        0        0    12066 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/logo512.png
--rw-r--r--   0        0        0      492 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/manifest.json
--rw-r--r--   0        0        0       67 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/public/robots.txt
--rw-r--r--   0        0        0       33 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/scripts/cert.sh
--rw-r--r--   0        0        0      634 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/App.css
--rw-r--r--   0        0        0      383 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/App.test.tsx
--rw-r--r--   0        0        0      210 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/App.tsx
--rw-r--r--   0        0        0      346 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/app/hooks.ts
--rw-r--r--   0        0        0      461 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/app/store.ts
--rw-r--r--   0        0        0     1057 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/start-stop-process.tsx
--rw-r--r--   0        0        0      512 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
--rw-r--r--   0        0        0     1159 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
--rw-r--r--   0        0        0      105 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/webcam.tsx
--rw-r--r--   0        0        0      642 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
--rw-r--r--   0        0        0     1383 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.module.css
--rw-r--r--   0        0        0     2156 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.tsx
--rw-r--r--   0        0        0      220 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterAPI.ts
--rw-r--r--   0        0        0      912 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
--rw-r--r--   0        0        0     3161 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.ts
--rw-r--r--   0        0        0      325 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/hooks/use-device-stream.ts
--rw-r--r--   0        0        0      857 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
--rw-r--r--   0        0        0      376 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/index.css
--rw-r--r--   0        0        0      642 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/index.tsx
--rw-r--r--   0        0        0      461 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Copyright.tsx
--rw-r--r--   0        0        0     2033 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Header.tsx
--rw-r--r--   0        0        0     2823 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Navigator.tsx
--rw-r--r--   0        0        0     5588 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/Paperbase.tsx
--rw-r--r--   0        0        0      440 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
--rw-r--r--   0        0        0      290 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
--rw-r--r--   0        0        0     2398 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/Content.tsx
--rw-r--r--   0        0        0      769 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/layout/routing/router.tsx
--rw-r--r--   0        0        0     1160 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/logo.svg
--rw-r--r--   0        0        0       40 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/react-app-env.d.ts
--rw-r--r--   0        0        0     6114 2024-04-29 19:29:24.861720 freemocap-1.2.0/experimental/freemocap-ui/src/serviceWorker.ts
--rw-r--r--   0        0        0      697 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/Capture.tsx
--rw-r--r--   0        0        0      442 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/Record.ts
--rw-r--r--   0        0        0      208 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/cam.ts
--rw-r--r--   0        0        0      341 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/download.ts
--rw-r--r--   0        0        0     1879 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/frame-capture.tsx
--rw-r--r--   0        0        0      519 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/image_send_worker.ts
--rw-r--r--   0        0        0     2252 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/recorder.ts
--rw-r--r--   0        0        0     1563 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/services/supported_recorder.ts
--rw-r--r--   0        0        0      254 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/setupTests.ts
--rw-r--r--   0        0        0     1682 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/Capture.tsx
--rw-r--r--   0        0        0      835 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/Config.tsx
--rw-r--r--   0        0        0     1298 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
--rw-r--r--   0        0        0      121 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/ShowCameras.tsx
--rw-r--r--   0        0        0      129 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/UserConfig.tsx
--rw-r--r--   0        0        0     1090 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
--rw-r--r--   0        0        0      851 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
--rw-r--r--   0        0        0     1090 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
--rw-r--r--   0        0        0     2118 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
--rw-r--r--   0        0        0      599 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/freemocap-ui/tsconfig.json
--rw-r--r--   0        0        0      790 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/python_scratch/qt_drag_and_drop.py
--rw-r--r--   0        0        0        2 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/__init__.py
--rw-r--r--   0        0        0      423 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/app_factory.py
--rw-r--r--   0        0        0       89 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/globals.py
--rw-r--r--   0        0        0      241 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/middleware/cors.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/models/__init__.py
--rw-r--r--   0        0        0      534 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/__init__.py
--rw-r--r--   0        0        0     1034 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/cam_data_ws.py
--rw-r--r--   0        0        0     3135 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/camera_route.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/health/__init__.py
--rw-r--r--   0        0        0      305 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/health/health_check_route.py
--rw-r--r--   0        0        0      209 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/home/home.py
--rw-r--r--   0        0        0     7413 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/session/session_router.py
--rw-r--r--   0        0        0      221 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/routes/startup/startup.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/__init__.py
--rw-r--r--   0        0        0      138 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/board_detect_service.py
--rw-r--r--   0        0        0       50 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/mediapipe_detect_service.py
--rw-r--r--   0        0        0     2021 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/react_fastapi/api/services/user_config.py
--rw-r--r--   0        0        0      315 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/rerun_playground.py
--rw-r--r--   0        0        0     1637 2024-04-29 19:29:24.865721 freemocap-1.2.0/experimental/tool_bar.py
--rw-r--r--   0        0        0   661822 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap-ui/package-lock.json
--rw-r--r--   0        0        0     2776 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/.idea/workspace.xml
--rw-r--r--   0        0        0      693 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/__init__.py
--rw-r--r--   0        0        0      945 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/__main__.py
--rw-r--r--   0        0        0    44734 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.png
--rw-r--r--   0        0        0     2948 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.svg
--rw-r--r--   0        0        0   332173 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image_highRes.png
--rw-r--r--   0        0        0    26593 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap-logo-black-border.svg
--rw-r--r--   0        0        0   126495 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png
--rw-r--r--   0        0        0   124841 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
--rw-r--r--   0        0        0    99678 2024-04-29 19:29:24.869721 freemocap-1.2.0/freemocap/assets/logo/freemocap_skelly_logo.ico
--rw-r--r--   0        0        0   259115 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/assets/mac_app_files/freemocap.icns
--rw-r--r--   0        0        0     1148 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/assets/mac_app_files/info.plist
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
--rw-r--r--   0        0        0     7091 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
--rw-r--r--   0        0        0    71193 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
--rw-r--r--   0        0        0     2712 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
--rw-r--r--   0        0        0    13416 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
--rw-r--r--   0        0        0      820 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
--rw-r--r--   0        0        0     1163 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
--rw-r--r--   0        0        0     2842 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py
--rw-r--r--   0        0        0     5621 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
--rw-r--r--   0        0        0    14583 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/__init__.py
--rw-r--r--   0        0        0     2251 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py
--rw-r--r--   0        0        0     3368 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py
--rw-r--r--   0        0        0    23381 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/__init__.py
--rw-r--r--   0        0        0     1270 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/export_to_blender.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/__init__.py
--rw-r--r--   0        0        0      151 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/get_numpy_path.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/__init__.py
--rw-r--r--   0        0        0     3024 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py
--rw-r--r--   0        0        0     1709 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py
--rw-r--r--   0        0        0     6781 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_ajc_addon_main.py
--rw-r--r--   0        0        0      791 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py
--rw-r--r--   0        0        0     3076 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/__init__.py
--rw-r--r--   0        0        0    10465 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb
--rw-r--r--   0        0        0     1089 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/__init__.py
--rw-r--r--   0        0        0    13879 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py
--rw-r--r--   0        0        0     4240 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py
--rw-r--r--   0        0        0     1654 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/__init__.py
--rw-r--r--   0        0        0     5952 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
--rw-r--r--   0        0        0     4207 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py
--rw-r--r--   0        0        0     1674 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py
--rw-r--r--   0        0        0     2617 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py
--rw-r--r--   0        0        0     3482 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py
--rw-r--r--   0        0        0     2041 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py
--rw-r--r--   0        0        0     5670 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/__init__.py
--rw-r--r--   0        0        0     9173 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/data_loader.py
--rw-r--r--   0        0        0     4854 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/data_models.py
--rw-r--r--   0        0        0     4195 2024-04-29 19:29:24.873721 freemocap-1.2.0/freemocap/data_layer/data_saver/data_saver.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/__init__.py
--rw-r--r--   0        0        0    10465 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb
--rw-r--r--   0        0        0     1089 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/recording_models/__init__.py
--rw-r--r--   0        0        0     1473 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/recording_models/post_processing_parameter_models.py
--rw-r--r--   0        0        0    10940 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/data_layer/recording_models/recording_info_model.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/__init__.py
--rw-r--r--   0        0        0     5822 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/actions.py
--rw-r--r--   0        0        0     2777 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/menu_bar.py
--rw-r--r--   0        0        0     2129 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/freemocap_main.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/main_window/__init__.py
--rw-r--r--   0        0        0    25937 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/main_window/freemocap_main_window.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/__init__.py
--rw-r--r--   0        0        0      362 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
--rw-r--r--   0        0        0     1325 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/css_file_watcher.py
--rw-r--r--   0        0        0     3905 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.css
--rw-r--r--   0        0        0     5105 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
--rw-r--r--   0        0        0     1500 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/scss_file_watcher.py
--rw-r--r--   0        0        0      305 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/__init__.py
--rw-r--r--   0        0        0     1850 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/colors.py
--rw-r--r--   0        0        0     1127 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/copy_timestamps_folder.py
--rw-r--r--   0        0        0      194 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/get_qt_app.py
--rw-r--r--   0        0        0     1105 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/save_and_load_gui_state.py
--rw-r--r--   0        0        0      864 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0     7141 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/active_recording_widget.py
--rw-r--r--   0        0        0    11878 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/camera_controller_group_box.py
--rw-r--r--   0        0        0     3728 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/central_tab_widget.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/__init__.py
--rw-r--r--   0        0        0    14844 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
--rw-r--r--   0        0        0     1924 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
--rw-r--r--   0        0        0     3636 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/export_data_control_panel.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
--rw-r--r--   0        0        0    13078 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
--rw-r--r--   0        0        0    12727 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
--rw-r--r--   0        0        0     2316 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel_dock_widget.py
--rw-r--r--   0        0        0     6771 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/directory_view_widget.py
--rw-r--r--   0        0        0     7903 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/home_widget.py
--rw-r--r--   0        0        0    10889 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/import_videos_wizard.py
--rw-r--r--   0        0        0     3089 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/jupyter_console_widget.py
--rw-r--r--   0        0        0     7817 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/log_view_widget.py
--rw-r--r--   0        0        0      415 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/logo_svg_widget.py
--rw-r--r--   0        0        0     3864 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/opencv_conflict_dialog.py
--rw-r--r--   0        0        0     2701 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/set_data_folder_dialog.py
--rw-r--r--   0        0        0     3989 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/widgets/welcome_screen_dialog.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/__init__.py
--rw-r--r--   0        0        0     2380 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
--rw-r--r--   0        0        0     1269 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/download_sample_data_thread_worker.py
--rw-r--r--   0        0        0     1654 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/export_to_blender_thread_worker.py
--rw-r--r--   0        0        0     2793 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
--rw-r--r--   0        0        0     2791 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/logging/__init__.py
--rw-r--r--   0        0        0     7505 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/logging/configure_logging.py
--rw-r--r--   0        0        0      256 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/logging/queue_logger.py
--rw-r--r--   0        0        0      259 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/open_file.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/paths_and_filenames/__init__.py
--rw-r--r--   0        0        0     3347 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/paths_and_filenames/file_and_folder_names.py
--rw-r--r--   0        0        0    12662 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/paths_and_filenames/path_getters.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/user_data/__init__.py
--rw-r--r--   0        0        0      957 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/system/user_data/pipedream_pings.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/conftest.py
--rw-r--r--   0        0        0     3685 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_by_camera_reprojection_filtering.py
--rw-r--r--   0        0        0     3151 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_geometry_utilities.py
--rw-r--r--   0        0        0     2145 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_image_tracking_data_shape.py
--rw-r--r--   0        0        0     2415 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_mediapipe_skeleton_data_shape.py
--rw-r--r--   0        0        0      943 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_synchronized_video_frame_counts.py
--rw-r--r--   0        0        0     1378 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/tests/test_total_body_center_of_mass_data_shape.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/__init__.py
--rw-r--r--   0        0        0     1268 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/create_nested_dict_from_pydantic.py
--rw-r--r--   0        0        0     2450 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/download_sample_data.py
--rw-r--r--   0        0        0     1022 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/fix_opencv_conflict.py
--rw-r--r--   0        0        0        0 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/geometry/__init__.py
--rw-r--r--   0        0        0      446 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/geometry/project_3d_data_to_z_plane.py
--rw-r--r--   0        0        0      631 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py
--rw-r--r--   0        0        0      813 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0      691 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/get_video_paths.py
--rw-r--r--   0        0        0      111 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/kill_event_exception.py
--rw-r--r--   0        0        0      708 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/remove_empty_directories.py
--rw-r--r--   0        0        0      486 2024-04-29 19:29:24.877720 freemocap-1.2.0/freemocap/utilities/save_dictionary_to_json.py
--rw-r--r--   0        0        0    25394 2024-04-29 19:29:24.877720 freemocap-1.2.0/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb
--rw-r--r--   0        0        0     5252 2024-04-29 19:29:24.881720 freemocap-1.2.0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
--rw-r--r--   0        0        0    21821 2024-04-29 19:29:24.881720 freemocap-1.2.0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
--rw-r--r--   0        0        0    13464 2024-04-29 19:29:24.881720 freemocap-1.2.0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
--rw-r--r--   0        0        0      690 2024-04-29 19:29:24.881720 freemocap-1.2.0/noxfile.py
--rw-r--r--   0        0        0     1748 2024-04-29 19:29:24.881720 freemocap-1.2.0/poetry_pyproject.toml
--rw-r--r--   0        0        0     3930 2024-04-29 19:29:24.881720 freemocap-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       50 2024-04-29 19:29:24.881720 freemocap-1.2.0/setup.py
--rw-r--r--   0        0        0     7307 1970-01-01 00:00:00.000000 freemocap-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1649 2024-04-30 21:53:47.949915 freemocap-1.2.1/.flake8
+-rwxr-xr-x   0        0        0      492 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      423 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      730 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/coverage-testing.yml
+-rw-r--r--   0        0        0     1138 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/flit_publish_to_pypi.yml
+-rwxr-xr-x   0        0        0      385 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/linting-flake8.yml
+-rw-r--r--   0        0        0     2049 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/linux_installer.yml
+-rw-r--r--   0        0        0     2613 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/mac_installer.yml
+-rw-r--r--   0        0        0     1246 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/publish_to_pypi.yml
+-rwxr-xr-x   0        0        0     1018 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/python-testing.yml
+-rwxr-xr-x   0        0        0      733 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/version-testing.yml
+-rw-r--r--   0        0        0     2312 2024-04-30 21:53:47.949915 freemocap-1.2.1/.github/workflows/windows_installer.yml
+-rw-r--r--   0        0        0     2043 2024-04-30 21:53:47.949915 freemocap-1.2.1/.gitignore
+-rw-r--r--   0        0        0      229 2024-04-30 21:53:47.949915 freemocap-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      657 2024-04-30 21:53:47.949915 freemocap-1.2.1/CITATION.cff
+-rw-r--r--   0        0        0      327 2024-04-30 21:53:47.949915 freemocap-1.2.1/CODEOWNERS
+-rw-r--r--   0        0        0     1513 2024-04-30 21:53:47.949915 freemocap-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3552 2024-04-30 21:53:47.949915 freemocap-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2024-04-30 21:53:47.953915 freemocap-1.2.1/LICENSE
+-rw-r--r--   0        0        0      234 2024-04-30 21:53:47.953915 freemocap-1.2.1/MANIFEST.in
+-rw-r--r--   0        0        0     4112 2024-04-30 21:53:47.953915 freemocap-1.2.1/README.md
+-rwxr-xr-x   0        0        0      607 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/builds/install_packages
+-rwxr-xr-x   0        0        0       66 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/installer.sh
+-rwxr-xr-x   0        0        0      278 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/linux/build.sh
+-rwxr-xr-x   0        0        0      161 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/linux/run_uvicorn_server.sh
+-rwxr-xr-x   0        0        0      381 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/linux/run_web_server.sh
+-rwxr-xr-x   0        0        0      118 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/linux/shell.sh
+-rwxr-xr-x   0        0        0      104 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/linux/test.sh
+-rwxr-xr-x   0        0        0       71 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/linux/up.sh
+-rw-r--r--   0        0        0      410 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/windows/installChocolatey.cmd
+-rw-r--r--   0        0        0      112 2024-04-30 21:53:47.953915 freemocap-1.2.1/bin/windows/run_web_server.cmd
+-rw-r--r--   0        0        0     4783 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/batch_process/batch_process.py
+-rw-r--r--   0        0        0     1415 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/batch_process/headless_calibration.py
+-rw-r--r--   0        0        0     3495 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/directory_view.py
+-rw-r--r--   0        0        0      331 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/.gitignore
+-rw-r--r--   0        0        0     2358 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/README.md
+-rw-r--r--   0        0        0      804 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/config-overrides.js
+-rw-r--r--   0        0        0   725486 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/package-lock.json
+-rw-r--r--   0        0        0     2548 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/package.json
+-rw-r--r--   0        0        0     3585 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/public/favicon.ico
+-rw-r--r--   0        0        0     1919 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/public/index.html
+-rw-r--r--   0        0        0     4153 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/public/logo192.png
+-rw-r--r--   0        0        0    12066 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/public/logo512.png
+-rw-r--r--   0        0        0      492 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/public/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-30 21:53:47.953915 freemocap-1.2.1/experimental/freemocap-ui/public/robots.txt
+-rw-r--r--   0        0        0       33 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/scripts/cert.sh
+-rw-r--r--   0        0        0      634 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/App.css
+-rw-r--r--   0        0        0      383 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/App.test.tsx
+-rw-r--r--   0        0        0      210 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/App.tsx
+-rw-r--r--   0        0        0      346 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/app/hooks.ts
+-rw-r--r--   0        0        0      461 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/app/store.ts
+-rw-r--r--   0        0        0     1057 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/components/start-stop-process.tsx
+-rw-r--r--   0        0        0      512 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx
+-rw-r--r--   0        0        0     1159 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx
+-rw-r--r--   0        0        0      105 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/components/webcam/webcam.tsx
+-rw-r--r--   0        0        0      642 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx
+-rw-r--r--   0        0        0     1383 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/Counter.module.css
+-rw-r--r--   0        0        0     2156 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/Counter.tsx
+-rw-r--r--   0        0        0      220 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/counterAPI.ts
+-rw-r--r--   0        0        0      912 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts
+-rw-r--r--   0        0        0     3161 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/counterSlice.ts
+-rw-r--r--   0        0        0      325 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/hooks/use-device-stream.ts
+-rw-r--r--   0        0        0      857 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx
+-rw-r--r--   0        0        0      376 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/index.css
+-rw-r--r--   0        0        0      642 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/index.tsx
+-rw-r--r--   0        0        0      461 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/Copyright.tsx
+-rw-r--r--   0        0        0     2033 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/Header.tsx
+-rw-r--r--   0        0        0     2823 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/Navigator.tsx
+-rw-r--r--   0        0        0     5588 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/Paperbase.tsx
+-rw-r--r--   0        0        0      440 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/content/BaseContent.tsx
+-rw-r--r--   0        0        0      290 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/content/BasePaper.tsx
+-rw-r--r--   0        0        0     2398 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/content/Content.tsx
+-rw-r--r--   0        0        0      769 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/layout/routing/router.tsx
+-rw-r--r--   0        0        0     1160 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/logo.svg
+-rw-r--r--   0        0        0       40 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/react-app-env.d.ts
+-rw-r--r--   0        0        0     6114 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/serviceWorker.ts
+-rw-r--r--   0        0        0      697 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/Capture.tsx
+-rw-r--r--   0        0        0      442 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/Record.ts
+-rw-r--r--   0        0        0      208 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/cam.ts
+-rw-r--r--   0        0        0      341 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/download.ts
+-rw-r--r--   0        0        0     1879 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/frame-capture.tsx
+-rw-r--r--   0        0        0      519 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/image_send_worker.ts
+-rw-r--r--   0        0        0     2252 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/recorder.ts
+-rw-r--r--   0        0        0     1563 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/services/supported_recorder.ts
+-rw-r--r--   0        0        0      254 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/setupTests.ts
+-rw-r--r--   0        0        0     1682 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/Capture.tsx
+-rw-r--r--   0        0        0      835 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/Config.tsx
+-rw-r--r--   0        0        0     1298 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/SessionWorkflow.tsx
+-rw-r--r--   0        0        0      121 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/ShowCameras.tsx
+-rw-r--r--   0        0        0      129 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/UserConfig.tsx
+-rw-r--r--   0        0        0     1090 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx
+-rw-r--r--   0        0        0      851 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx
+-rw-r--r--   0        0        0     1090 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx
+-rw-r--r--   0        0        0     2118 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx
+-rw-r--r--   0        0        0      599 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/freemocap-ui/tsconfig.json
+-rw-r--r--   0        0        0      790 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/python_scratch/qt_drag_and_drop.py
+-rw-r--r--   0        0        0        2 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/__init__.py
+-rw-r--r--   0        0        0      423 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/app_factory.py
+-rw-r--r--   0        0        0       89 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/globals.py
+-rw-r--r--   0        0        0      241 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/middleware/cors.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/models/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/camera/__init__.py
+-rw-r--r--   0        0        0     1034 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/camera/cam_data_ws.py
+-rw-r--r--   0        0        0     3135 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/camera/camera_route.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/health/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/health/health_check_route.py
+-rw-r--r--   0        0        0      209 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/home/home.py
+-rw-r--r--   0        0        0     7413 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/session/session_router.py
+-rw-r--r--   0        0        0      221 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/routes/startup/startup.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/services/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/services/board_detect_service.py
+-rw-r--r--   0        0        0       50 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/services/mediapipe_detect_service.py
+-rw-r--r--   0        0        0     2021 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/react_fastapi/api/services/user_config.py
+-rw-r--r--   0        0        0      315 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/rerun_playground.py
+-rw-r--r--   0        0        0     1637 2024-04-30 21:53:47.957915 freemocap-1.2.1/experimental/tool_bar.py
+-rw-r--r--   0        0        0   661822 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap-ui/package-lock.json
+-rw-r--r--   0        0        0     2776 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/.idea/workspace.xml
+-rw-r--r--   0        0        0      693 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/__init__.py
+-rw-r--r--   0        0        0      945 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/__main__.py
+-rw-r--r--   0        0        0    44734 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/assets/charuco/charuco_board_image.png
+-rw-r--r--   0        0        0     2948 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/assets/charuco/charuco_board_image.svg
+-rw-r--r--   0        0        0   332173 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/assets/charuco/charuco_board_image_highRes.png
+-rw-r--r--   0        0        0    26593 2024-04-30 21:53:47.961915 freemocap-1.2.1/freemocap/assets/logo/freemocap-logo-black-border.svg
+-rw-r--r--   0        0        0   126495 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png
+-rw-r--r--   0        0        0   124841 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png
+-rw-r--r--   0        0        0    99678 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/assets/logo/freemocap_skelly_logo.ico
+-rw-r--r--   0        0        0   259115 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/assets/mac_app_files/freemocap.icns
+-rw-r--r--   0        0        0     1148 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/assets/mac_app_files/info.plist
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/__init__.py
+-rw-r--r--   0        0        0     7091 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py
+-rw-r--r--   0        0        0    71193 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py
+-rw-r--r--   0        0        0     2712 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py
+-rw-r--r--   0        0        0    13416 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/charuco_stuff/__init__.py
+-rw-r--r--   0        0        0      820 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py
+-rw-r--r--   0        0        0     1163 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py
+-rw-r--r--   0        0        0     2842 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py
+-rw-r--r--   0        0        0     5621 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/__init__.py
+-rw-r--r--   0        0        0    14583 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/__init__.py
+-rw-r--r--   0        0        0     2251 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py
+-rw-r--r--   0        0        0     3368 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py
+-rw-r--r--   0        0        0    23381 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/__init__.py
+-rw-r--r--   0        0        0     1270 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/export_to_blender.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.965915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/get_numpy_path.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/__init__.py
+-rw-r--r--   0        0        0     3024 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py
+-rw-r--r--   0        0        0     1709 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py
+-rw-r--r--   0        0        0     6781 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_ajc_addon_main.py
+-rw-r--r--   0        0        0      791 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py
+-rw-r--r--   0        0        0     3076 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/generate_jupyter_notebook/__init__.py
+-rw-r--r--   0        0        0    10465 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb
+-rw-r--r--   0        0        0     1089 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/__init__.py
+-rw-r--r--   0        0        0    13879 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py
+-rw-r--r--   0        0        0     4240 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py
+-rw-r--r--   0        0        0     1654 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/__init__.py
+-rw-r--r--   0        0        0     5952 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py
+-rw-r--r--   0        0        0     4207 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py
+-rw-r--r--   0        0        0     1674 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py
+-rw-r--r--   0        0        0     2617 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py
+-rw-r--r--   0        0        0     3482 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py
+-rw-r--r--   0        0        0     2041 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py
+-rw-r--r--   0        0        0     5670 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/data_saver/__init__.py
+-rw-r--r--   0        0        0     9173 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/data_saver/data_loader.py
+-rw-r--r--   0        0        0     4854 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/data_saver/data_models.py
+-rw-r--r--   0        0        0     4195 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/data_saver/data_saver.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/generate_jupyter_notebook/__init__.py
+-rw-r--r--   0        0        0    10465 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb
+-rw-r--r--   0        0        0     1089 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/recording_models/__init__.py
+-rw-r--r--   0        0        0     1473 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/recording_models/post_processing_parameter_models.py
+-rw-r--r--   0        0        0    10940 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/data_layer/recording_models/recording_info_model.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/actions_and_menus/__init__.py
+-rw-r--r--   0        0        0     5822 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/actions_and_menus/actions.py
+-rw-r--r--   0        0        0     2777 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/actions_and_menus/menu_bar.py
+-rw-r--r--   0        0        0     2129 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/freemocap_main.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/main_window/__init__.py
+-rw-r--r--   0        0        0    25937 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/main_window/freemocap_main_window.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/compile_scss_to_css.py
+-rw-r--r--   0        0        0     1325 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/css_file_watcher.py
+-rw-r--r--   0        0        0     3905 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/qt_style_sheet.css
+-rw-r--r--   0        0        0     5105 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/qt_style_sheet.scss
+-rw-r--r--   0        0        0     1500 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/scss_file_watcher.py
+-rw-r--r--   0        0        0      305 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/style_sheet/set_css_style_sheet.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/utilities/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/utilities/colors.py
+-rw-r--r--   0        0        0     1127 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/utilities/copy_timestamps_folder.py
+-rw-r--r--   0        0        0      194 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/utilities/get_qt_app.py
+-rw-r--r--   0        0        0     1105 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/utilities/save_and_load_gui_state.py
+-rw-r--r--   0        0        0      864 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0     7141 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/active_recording_widget.py
+-rw-r--r--   0        0        0    11878 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/camera_controller_group_box.py
+-rw-r--r--   0        0        0     3728 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/central_tab_widget.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/__init__.py
+-rw-r--r--   0        0        0    14844 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py
+-rw-r--r--   0        0        0     1924 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py
+-rw-r--r--   0        0        0     3636 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/export_data_control_panel.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_3d_triangulation_parameter_group.py
+-rw-r--r--   0        0        0    13078 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py
+-rw-r--r--   0        0        0    12727 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py
+-rw-r--r--   0        0        0     2316 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel_dock_widget.py
+-rw-r--r--   0        0        0     6771 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/directory_view_widget.py
+-rw-r--r--   0        0        0     7903 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/home_widget.py
+-rw-r--r--   0        0        0    10889 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/import_videos_wizard.py
+-rw-r--r--   0        0        0     3089 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/jupyter_console_widget.py
+-rw-r--r--   0        0        0     7817 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/log_view_widget.py
+-rw-r--r--   0        0        0      415 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/logo_svg_widget.py
+-rw-r--r--   0        0        0     3864 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/opencv_conflict_dialog.py
+-rw-r--r--   0        0        0     2701 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/set_data_folder_dialog.py
+-rw-r--r--   0        0        0     3989 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/widgets/welcome_screen_dialog.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/workers/__init__.py
+-rw-r--r--   0        0        0     2380 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py
+-rw-r--r--   0        0        0     1269 2024-04-30 21:53:47.969915 freemocap-1.2.1/freemocap/gui/qt/workers/download_sample_data_thread_worker.py
+-rw-r--r--   0        0        0     1654 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/gui/qt/workers/export_to_blender_thread_worker.py
+-rw-r--r--   0        0        0     2793 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py
+-rw-r--r--   0        0        0     2791 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/logging/__init__.py
+-rw-r--r--   0        0        0     7505 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/logging/configure_logging.py
+-rw-r--r--   0        0        0      256 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/logging/queue_logger.py
+-rw-r--r--   0        0        0      259 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/open_file.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/paths_and_filenames/__init__.py
+-rw-r--r--   0        0        0     3347 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/paths_and_filenames/file_and_folder_names.py
+-rw-r--r--   0        0        0    12662 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/paths_and_filenames/path_getters.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/user_data/__init__.py
+-rw-r--r--   0        0        0      957 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/system/user_data/pipedream_pings.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/conftest.py
+-rw-r--r--   0        0        0     3685 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/test_by_camera_reprojection_filtering.py
+-rw-r--r--   0        0        0     3151 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/test_geometry_utilities.py
+-rw-r--r--   0        0        0     2145 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/test_image_tracking_data_shape.py
+-rw-r--r--   0        0        0     2415 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/test_mediapipe_skeleton_data_shape.py
+-rw-r--r--   0        0        0      943 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/test_synchronized_video_frame_counts.py
+-rw-r--r--   0        0        0     1378 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/tests/test_total_body_center_of_mass_data_shape.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/__init__.py
+-rw-r--r--   0        0        0     1268 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/create_nested_dict_from_pydantic.py
+-rw-r--r--   0        0        0     2450 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/download_sample_data.py
+-rw-r--r--   0        0        0     1022 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/fix_opencv_conflict.py
+-rw-r--r--   0        0        0        0 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/geometry/__init__.py
+-rw-r--r--   0        0        0      446 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/geometry/project_3d_data_to_z_plane.py
+-rw-r--r--   0        0        0      631 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py
+-rw-r--r--   0        0        0      813 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0      691 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/get_video_paths.py
+-rw-r--r--   0        0        0      111 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/kill_event_exception.py
+-rw-r--r--   0        0        0      708 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/remove_empty_directories.py
+-rw-r--r--   0        0        0      486 2024-04-30 21:53:47.973915 freemocap-1.2.1/freemocap/utilities/save_dictionary_to_json.py
+-rw-r--r--   0        0        0    25394 2024-04-30 21:53:47.973915 freemocap-1.2.1/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb
+-rw-r--r--   0        0        0     5252 2024-04-30 21:53:47.973915 freemocap-1.2.1/ipython_jupyter_notebooks/batch_process_session_folders.ipynb
+-rw-r--r--   0        0        0    21821 2024-04-30 21:53:47.973915 freemocap-1.2.1/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb
+-rw-r--r--   0        0        0    13464 2024-04-30 21:53:47.973915 freemocap-1.2.1/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb
+-rw-r--r--   0        0        0      690 2024-04-30 21:53:47.973915 freemocap-1.2.1/noxfile.py
+-rw-r--r--   0        0        0     1748 2024-04-30 21:53:47.973915 freemocap-1.2.1/poetry_pyproject.toml
+-rw-r--r--   0        0        0     3930 2024-04-30 21:53:47.973915 freemocap-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-04-30 21:53:47.973915 freemocap-1.2.1/setup.py
+-rw-r--r--   0        0        0     7307 1970-01-01 00:00:00.000000 freemocap-1.2.1/PKG-INFO
```

### Comparing `freemocap-1.2.0/.flake8` & `freemocap-1.2.1/.flake8`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/.github/workflows/coverage-testing.yml` & `freemocap-1.2.1/.github/workflows/coverage-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/.github/workflows/flit_publish_to_pypi.yml` & `freemocap-1.2.1/.github/workflows/flit_publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/.github/workflows/linux_installer.yml` & `freemocap-1.2.1/.github/workflows/linux_installer.yml`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       - name: Unzip PyApp
         run: |
           unzip pyapp.zip
       - name: Create Linux Installer
         run: |
           cd ${{ github.workspace }}/pyapp-v0.12.0
           export PYAPP_PROJECT_NAME=freemocap
-          export PYAPP_PROJECT_VERSION=v1.2.0
+          export PYAPP_PROJECT_VERSION=v1.2.1
           export PYAPP_PROJECT_DEPENDENCY_FILE=${{ github.workspace }}/requirements.txt
           export PYAPP_EXEC_SCRIPT=${{ github.workspace }}/freemocap/__main__.py
           export PYAPP_PIP_EXTRA_ARGS=--no-deps
           cargo build --release
           cargo install pyapp --force --root ${{ github.workspace }}
           cd ${{ github.workspace }}
           mv ${{ github.workspace }}/bin/pyapp freemocap_app && chmod +x freemocap_app
```

### Comparing `freemocap-1.2.0/.github/workflows/mac_installer.yml` & `freemocap-1.2.1/.github/workflows/mac_installer.yml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
       - name: Unzip PyApp
         run: |
           unzip pyapp.zip
       - name: Create Mac Installer
         run: |
           cd ${{ github.workspace }}/pyapp-v0.12.0
           export PYAPP_PROJECT_NAME=freemocap
-          export PYAPP_PROJECT_VERSION=v1.2.0
+          export PYAPP_PROJECT_VERSION=v1.2.1
           export PYAPP_PROJECT_DEPENDENCY_FILE=${{ github.workspace }}/requirements.txt
           export PYAPP_EXEC_SCRIPT=${{ github.workspace }}/freemocap/__main__.py
           export PYAPP_PIP_EXTRA_ARGS=--no-deps
           cargo build --release
           cargo install pyapp --force --root ${{ github.workspace }}
           cd ${{ github.workspace }}
           mv ${{ github.workspace }}/bin/pyapp freemocap_app
```

### Comparing `freemocap-1.2.0/.github/workflows/publish_to_pypi.yml` & `freemocap-1.2.1/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/.github/workflows/python-testing.yml` & `freemocap-1.2.1/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/.github/workflows/version-testing.yml` & `freemocap-1.2.1/.github/workflows/version-testing.yml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/.github/workflows/windows_installer.yml` & `freemocap-1.2.1/.github/workflows/windows_installer.yml`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           ls -la
         shell: bash
       - name: Create Windows Installer
         run: |
           WORKSPACE=$(cygpath -u "${{ github.workspace}}")
           cd $WORKSPACE/pyapp-v0.12.0
           export PYAPP_PROJECT_NAME=freemocap
-          export PYAPP_PROJECT_VERSION=v1.2.0
+          export PYAPP_PROJECT_VERSION=v1.2.1
           export PYAPP_PROJECT_DEPENDENCY_FILE=$WORKSPACE/requirements.txt
           export PYAPP_EXEC_SCRIPT=$WORKSPACE/freemocap/__main__.py
           export PYAPP_PIP_EXTRA_ARGS=--no-deps
           cargo build --release
           cargo install pyapp --force --root $WORKSPACE
           cd $WORKSPACE
           mv $WORKSPACE/bin/pyapp freemocap_app.exe
```

### Comparing `freemocap-1.2.0/.gitignore` & `freemocap-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/CITATION.cff` & `freemocap-1.2.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/CODE_OF_CONDUCT.md` & `freemocap-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/CONTRIBUTING.md` & `freemocap-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/LICENSE` & `freemocap-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/README.md` & `freemocap-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/bin/builds/install_packages` & `freemocap-1.2.1/bin/builds/install_packages`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/batch_process/batch_process.py` & `freemocap-1.2.1/experimental/batch_process/batch_process.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/batch_process/headless_calibration.py` & `freemocap-1.2.1/experimental/batch_process/headless_calibration.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/directory_view.py` & `freemocap-1.2.1/experimental/directory_view.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/README.md` & `freemocap-1.2.1/experimental/freemocap-ui/README.md`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/config-overrides.js` & `freemocap-1.2.1/experimental/freemocap-ui/config-overrides.js`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/package-lock.json` & `freemocap-1.2.1/experimental/freemocap-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/package.json` & `freemocap-1.2.1/experimental/freemocap-ui/package.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/public/favicon.ico` & `freemocap-1.2.1/experimental/freemocap-ui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/public/index.html` & `freemocap-1.2.1/experimental/freemocap-ui/public/index.html`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/public/logo192.png` & `freemocap-1.2.1/experimental/freemocap-ui/public/logo192.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/public/logo512.png` & `freemocap-1.2.1/experimental/freemocap-ui/public/logo512.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/App.css` & `freemocap-1.2.1/experimental/freemocap-ui/src/App.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/components/start-stop-process.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/components/start-stop-process.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/components/webcam/LivePreview.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/components/webcam/webcam-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/features/camera/cameraSlice.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.module.css` & `freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/Counter.module.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/Counter.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/Counter.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts` & `freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/counterSlice.spec.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/features/counter/counterSlice.ts` & `freemocap-1.2.1/experimental/freemocap-ui/src/features/counter/counterSlice.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/hooks/use-frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/index.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/layout/Header.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/layout/Header.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/layout/Navigator.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/layout/Navigator.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/layout/Paperbase.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/layout/Paperbase.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/layout/content/Content.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/layout/content/Content.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/layout/routing/router.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/layout/routing/router.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/logo.svg` & `freemocap-1.2.1/experimental/freemocap-ui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/serviceWorker.ts` & `freemocap-1.2.1/experimental/freemocap-ui/src/serviceWorker.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/services/Capture.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/services/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/services/frame-capture.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/services/frame-capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/services/image_send_worker.ts` & `freemocap-1.2.1/experimental/freemocap-ui/src/services/image_send_worker.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/services/recorder.ts` & `freemocap-1.2.1/experimental/freemocap-ui/src/services/recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/services/supported_recorder.ts` & `freemocap-1.2.1/experimental/freemocap-ui/src/services/supported_recorder.ts`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/Capture.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/Capture.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/Config.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/Config.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/SessionWorkflow.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/SessionWorkflow.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/prod/ConfigForm.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewCamera.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/prod/SetupAndPreviewView.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx` & `freemocap-1.2.1/experimental/freemocap-ui/src/views/sessionWizard/SessionWizard.tsx`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/freemocap-ui/tsconfig.json` & `freemocap-1.2.1/experimental/freemocap-ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/python_scratch/qt_drag_and_drop.py` & `freemocap-1.2.1/experimental/python_scratch/qt_drag_and_drop.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/react_fastapi/api/routes/__init__.py` & `freemocap-1.2.1/experimental/react_fastapi/api/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/cam_data_ws.py` & `freemocap-1.2.1/experimental/react_fastapi/api/routes/camera/cam_data_ws.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/react_fastapi/api/routes/camera/camera_route.py` & `freemocap-1.2.1/experimental/react_fastapi/api/routes/camera/camera_route.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/react_fastapi/api/routes/session/session_router.py` & `freemocap-1.2.1/experimental/react_fastapi/api/routes/session/session_router.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/react_fastapi/api/services/user_config.py` & `freemocap-1.2.1/experimental/react_fastapi/api/services/user_config.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/experimental/tool_bar.py` & `freemocap-1.2.1/experimental/tool_bar.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap-ui/package-lock.json` & `freemocap-1.2.1/freemocap-ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/.idea/workspace.xml` & `freemocap-1.2.1/freemocap/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/__init__.py` & `freemocap-1.2.1/freemocap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A free and open source markerless motion capture system for everyone 💀✨"""
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v1.2.0"
+__version__ = "v1.2.1"
 __description__ = "A free and open source markerless motion capture system for everyone 💀✨"
 
 __package_name__ = "freemocap"
 __repo_url__ = f"https://github.com/freemocap/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
 
 from freemocap.system.logging.configure_logging import configure_logging, LogLevel
```

### Comparing `freemocap-1.2.0/freemocap/__main__.py` & `freemocap-1.2.1/freemocap/__main__.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.png` & `freemocap-1.2.1/freemocap/assets/charuco/charuco_board_image.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image.svg` & `freemocap-1.2.1/freemocap/assets/charuco/charuco_board_image.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/charuco/charuco_board_image_highRes.png` & `freemocap-1.2.1/freemocap/assets/charuco/charuco_board_image_highRes.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/logo/freemocap-logo-black-border.svg` & `freemocap-1.2.1/freemocap/assets/logo/freemocap-logo-black-border.svg`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png` & `freemocap-1.2.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-transparent-bkgd.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png` & `freemocap-1.2.1/freemocap/assets/logo/freemocap-skelly-logo-black-border-white-bkgd.png`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/logo/freemocap_skelly_logo.ico` & `freemocap-1.2.1/freemocap/assets/logo/freemocap_skelly_logo.ico`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/mac_app_files/freemocap.icns` & `freemocap-1.2.1/freemocap/assets/mac_app_files/freemocap.icns`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/assets/mac_app_files/info.plist` & `freemocap-1.2.1/freemocap/assets/mac_app_files/info.plist`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/anipose_camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/freemocap_anipose.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/anipose_camera_calibration/get_anipose_calibration_object.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/by_camera_reprojection_filtering.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/charuco_stuff/charuco_board_definition.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/run_anipose_capture_volume_calibration.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/save_mediapipe_3d_data_to_npy.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py` & `freemocap-1.2.1/freemocap/core_processes/capture_volume_calibration/triangulate_3d_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py` & `freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/convert_mediapipe_npy_to_csv.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py` & `freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_dataclasses.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py` & `freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/data_models/mediapipe_skeleton_names_and_connections.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py` & `freemocap-1.2.1/freemocap/core_processes/detecting_things_in_2d_images/mediapipe_stuff/mediapipe_skeleton_detector.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/export_to_blender.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/export_to_blender.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/bpy_install_addon.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/install/install_ajc_addon.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_ajc_addon_main.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_ajc_addon_main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/export_to_blender/methods/ajc_addon/run_simple.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/blender_stuff/get_best_guess_of_blender_path.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb` & `freemocap-1.2.1/freemocap/core_processes/export_data/generate_jupyter_notebook/freemocap_template.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py` & `freemocap-1.2.1/freemocap/core_processes/export_data/generate_jupyter_notebook/generate_jupyter_notebook.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py` & `freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/calculate_center_of_mass.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py` & `freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/post_process_skeleton.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py` & `freemocap-1.2.1/freemocap/core_processes/post_process_skeleton_data/process_single_camera_skeleton_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/process_recording_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/process_recording_headless.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/anatomical_data_pipeline_functions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/data_saving_pipeline_functions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/image_tracking_pipeline_functions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/pipeline_check.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py` & `freemocap-1.2.1/freemocap/core_processes/process_motion_capture_videos/processing_pipeline_functions/triangulation_pipeline_functions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/data_saver/data_loader.py` & `freemocap-1.2.1/freemocap/data_layer/data_saver/data_loader.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/data_saver/data_models.py` & `freemocap-1.2.1/freemocap/data_layer/data_saver/data_models.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/data_saver/data_saver.py` & `freemocap-1.2.1/freemocap/data_layer/data_saver/data_saver.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb` & `freemocap-1.2.1/freemocap/data_layer/generate_jupyter_notebook/freemocap_template.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py` & `freemocap-1.2.1/freemocap/data_layer/generate_jupyter_notebook/generate_jupyter_notebook.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/recording_models/post_processing_parameter_models.py` & `freemocap-1.2.1/freemocap/data_layer/recording_models/post_processing_parameter_models.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/data_layer/recording_models/recording_info_model.py` & `freemocap-1.2.1/freemocap/data_layer/recording_models/recording_info_model.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/actions.py` & `freemocap-1.2.1/freemocap/gui/qt/actions_and_menus/actions.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/actions_and_menus/menu_bar.py` & `freemocap-1.2.1/freemocap/gui/qt/actions_and_menus/menu_bar.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/freemocap_main.py` & `freemocap-1.2.1/freemocap/gui/qt/freemocap_main.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/main_window/freemocap_main_window.py` & `freemocap-1.2.1/freemocap/gui/qt/main_window/freemocap_main_window.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/style_sheet/css_file_watcher.py` & `freemocap-1.2.1/freemocap/gui/qt/style_sheet/css_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.css` & `freemocap-1.2.1/freemocap/gui/qt/style_sheet/qt_style_sheet.css`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/style_sheet/qt_style_sheet.scss` & `freemocap-1.2.1/freemocap/gui/qt/style_sheet/qt_style_sheet.scss`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/style_sheet/scss_file_watcher.py` & `freemocap-1.2.1/freemocap/gui/qt/style_sheet/scss_file_watcher.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/utilities/colors.py` & `freemocap-1.2.1/freemocap/gui/qt/utilities/colors.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/utilities/copy_timestamps_folder.py` & `freemocap-1.2.1/freemocap/gui/qt/utilities/copy_timestamps_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/utilities/save_and_load_gui_state.py` & `freemocap-1.2.1/freemocap/gui/qt/utilities/save_and_load_gui_state.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py` & `freemocap-1.2.1/freemocap/gui/qt/utilities/update_most_recent_recording_toml.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/active_recording_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/active_recording_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/camera_controller_group_box.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/camera_controller_group_box.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/central_tab_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/central_tab_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/calibration_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/export_data_control_panel.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/export_data_control_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/parameter_groups/create_parameter_groups.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel/process_mocap_data_panel/process_motion_capture_data_panel.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/control_panel_dock_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/control_panel_dock_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/directory_view_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/directory_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/home_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/home_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/import_videos_wizard.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/import_videos_wizard.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/jupyter_console_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/jupyter_console_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/log_view_widget.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/log_view_widget.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/opencv_conflict_dialog.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/opencv_conflict_dialog.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/set_data_folder_dialog.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/set_data_folder_dialog.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/widgets/welcome_screen_dialog.py` & `freemocap-1.2.1/freemocap/gui/qt/widgets/welcome_screen_dialog.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py` & `freemocap-1.2.1/freemocap/gui/qt/workers/anipose_calibration_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/workers/download_sample_data_thread_worker.py` & `freemocap-1.2.1/freemocap/gui/qt/workers/download_sample_data_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/workers/export_to_blender_thread_worker.py` & `freemocap-1.2.1/freemocap/gui/qt/workers/export_to_blender_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py` & `freemocap-1.2.1/freemocap/gui/qt/workers/process_motion_capture_data_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py` & `freemocap-1.2.1/freemocap/gui/qt/workers/synchronize_videos_thread_worker.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/system/logging/configure_logging.py` & `freemocap-1.2.1/freemocap/system/logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/system/paths_and_filenames/file_and_folder_names.py` & `freemocap-1.2.1/freemocap/system/paths_and_filenames/file_and_folder_names.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/system/paths_and_filenames/path_getters.py` & `freemocap-1.2.1/freemocap/system/paths_and_filenames/path_getters.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/system/user_data/pipedream_pings.py` & `freemocap-1.2.1/freemocap/system/user_data/pipedream_pings.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/conftest.py` & `freemocap-1.2.1/freemocap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/test_by_camera_reprojection_filtering.py` & `freemocap-1.2.1/freemocap/tests/test_by_camera_reprojection_filtering.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/test_geometry_utilities.py` & `freemocap-1.2.1/freemocap/tests/test_geometry_utilities.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/test_image_tracking_data_shape.py` & `freemocap-1.2.1/freemocap/tests/test_image_tracking_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/test_mediapipe_skeleton_data_shape.py` & `freemocap-1.2.1/freemocap/tests/test_mediapipe_skeleton_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/test_synchronized_video_frame_counts.py` & `freemocap-1.2.1/freemocap/tests/test_synchronized_video_frame_counts.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/tests/test_total_body_center_of_mass_data_shape.py` & `freemocap-1.2.1/freemocap/tests/test_total_body_center_of_mass_data_shape.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/create_nested_dict_from_pydantic.py` & `freemocap-1.2.1/freemocap/utilities/create_nested_dict_from_pydantic.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/download_sample_data.py` & `freemocap-1.2.1/freemocap/utilities/download_sample_data.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/fix_opencv_conflict.py` & `freemocap-1.2.1/freemocap/utilities/fix_opencv_conflict.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py` & `freemocap-1.2.1/freemocap/utilities/geometry/rotate_by_90_degrees_around_x_axis.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `freemocap-1.2.1/freemocap/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/get_video_paths.py` & `freemocap-1.2.1/freemocap/utilities/get_video_paths.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/freemocap/utilities/remove_empty_directories.py` & `freemocap-1.2.1/freemocap/utilities/remove_empty_directories.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb` & `freemocap-1.2.1/ipython_jupyter_notebooks/COM_Jumping_Analysis.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/ipython_jupyter_notebooks/batch_process_session_folders.ipynb` & `freemocap-1.2.1/ipython_jupyter_notebooks/batch_process_session_folders.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb` & `freemocap-1.2.1/ipython_jupyter_notebooks/export_freemocap_npy_as_pandas_data_frame_csv.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb` & `freemocap-1.2.1/ipython_jupyter_notebooks/rotate_translate_skeleton.ipynb`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/noxfile.py` & `freemocap-1.2.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/poetry_pyproject.toml` & `freemocap-1.2.1/poetry_pyproject.toml`

 * *Files identical despite different names*

### Comparing `freemocap-1.2.0/pyproject.toml` & `freemocap-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 [project.urls]
 Homepage = "https://freemocap.org"
 Documentation = "https://freemocap.github.io/documentation/"
 Github = "https://github.com/freemocap/freemocap"
 
 [tool.bumpver]
-current_version = "v1.2.0"
+current_version = "v1.2.1"
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `freemocap-1.2.0/PKG-INFO` & `freemocap-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freemocap
-Version: 1.2.0
+Version: 1.2.1
 Summary: A free and open source markerless motion capture system for everyone 💀✨
 Keywords: camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d animation,Blender,Blender3d,synchronization,computer vision
 Author: Endurance Idehen, Aaron Cherian, Jonathan Samir Matthis
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.9,<3.12
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope__ugw5xvc_/tmp4q94qyrf_TarContainer/0/274", line 75, column 87: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: freemocap Version: 1.2.0 Summary: A free and open
+Metadata-Version: 2.1 Name: freemocap Version: 1.2.1 Summary: A free and open
 source markerless motion capture system for everyone ðâ¨ Keywords:
 camera,stream,video,image,opencv,skelly,freemocap,motion capture,markerless
 motion capture,mocap,markerless mocap,markerless,kinematic,animation,3d
 animation,Blender,Blender3d,synchronization,computer vision Author: Endurance
 Idehen, Aaron Cherian, Jonathan Samir Matthis Author-email: Skelly FreeMoCap
 freemocap.org> Requires-Python: >=3.9,<3.12 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI
```

