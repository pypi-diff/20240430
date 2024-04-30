# Comparing `tmp/djsciops-1.5.5.tar.gz` & `tmp/djsciops-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djsciops-1.5.5.tar", last modified: Mon Aug 21 15:54:10 2023, max compression
+gzip compressed data, was "djsciops-1.5.7.tar", last modified: Tue Apr 30 18:46:49 2024, max compression
```

## Comparing `djsciops-1.5.5.tar` & `djsciops-1.5.7.tar`

### file list

```diff
@@ -1,306 +1,306 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.725177 djsciops-1.5.5/
--rw-r--r--   0 root         (0) root         (0)     1438 2023-08-21 15:54:10.725177 djsciops-1.5.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-08-21 15:53:57.000000 djsciops-1.5.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.665176 djsciops-1.5.5/djsciops/
--rw-r--r--   0 root         (0) root         (0)       60 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15141 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/authentication.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.665176 djsciops-1.5.5/djsciops/axon/
--rw-r--r--   0 root         (0) root         (0)    14174 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5129 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon/speed_audit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.669176 djsciops-1.5.5/djsciops/axon_gui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/__init__.py
--rw-r--r--   0 root         (0) root         (0)   255038 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/icon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.661176 djsciops-1.5.5/djsciops/axon_gui/images/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.721177 djsciops-1.5.5/djsciops/axon_gui/images/icons/
--rw-r--r--   0 root         (0) root         (0)     1953 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-3d.png
--rw-r--r--   0 root         (0) root         (0)     1948 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-4k.png
--rw-r--r--   0 root         (0) root         (0)     1865 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-account-logout.png
--rw-r--r--   0 root         (0) root         (0)     1870 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-action-redo.png
--rw-r--r--   0 root         (0) root         (0)     1882 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-action-undo.png
--rw-r--r--   0 root         (0) root         (0)     1987 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-airplane-mode-off.png
--rw-r--r--   0 root         (0) root         (0)     1950 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-airplane-mode.png
--rw-r--r--   0 root         (0) root         (0)     1974 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-alarm.png
--rw-r--r--   0 root         (0) root         (0)     1839 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-align-center.png
--rw-r--r--   0 root         (0) root         (0)     1838 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-align-left.png
--rw-r--r--   0 root         (0) root         (0)     1825 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-align-right.png
--rw-r--r--   0 root         (0) root         (0)     1797 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-bottom-2.png
--rw-r--r--   0 root         (0) root         (0)     1821 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-bottom.png
--rw-r--r--   0 root         (0) root         (0)     1970 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-bottom.png
--rw-r--r--   0 root         (0) root         (0)     1967 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-left.png
--rw-r--r--   0 root         (0) root         (0)     1969 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-right.png
--rw-r--r--   0 root         (0) root         (0)     1971 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-top.png
--rw-r--r--   0 root         (0) root         (0)     1790 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-left.png
--rw-r--r--   0 root         (0) root         (0)     1794 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-right.png
--rw-r--r--   0 root         (0) root         (0)     1824 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-top.png
--rw-r--r--   0 root         (0) root         (0)     1975 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-at.png
--rw-r--r--   0 root         (0) root         (0)     1949 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-av-timer.png
--rw-r--r--   0 root         (0) root         (0)     1933 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-ban.png
--rw-r--r--   0 root         (0) root         (0)     1830 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-0.png
--rw-r--r--   0 root         (0) root         (0)     1913 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-3.png
--rw-r--r--   0 root         (0) root         (0)     1879 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-5.png
--rw-r--r--   0 root         (0) root         (0)     1897 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-alert.png
--rw-r--r--   0 root         (0) root         (0)     1914 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-slash.png
--rw-r--r--   0 root         (0) root         (0)     1903 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-bell.png
--rw-r--r--   0 root         (0) root         (0)     1882 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-bluetooth.png
--rw-r--r--   0 root         (0) root         (0)     1940 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-briefcase.png
--rw-r--r--   0 root         (0) root         (0)     1851 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-browser.png
--rw-r--r--   0 root         (0) root         (0)     1914 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-calendar-check.png
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-camera-roll.png
--rw-r--r--   0 root         (0) root         (0)     1936 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-camera.png
--rw-r--r--   0 root         (0) root         (0)     1868 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-bottom.png
--rw-r--r--   0 root         (0) root         (0)     1853 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-left.png
--rw-r--r--   0 root         (0) root         (0)     1863 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-right.png
--rw-r--r--   0 root         (0) root         (0)     1842 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-top.png
--rw-r--r--   0 root         (0) root         (0)     1924 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cart.png
--rw-r--r--   0 root         (0) root         (0)     1886 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cast.png
--rw-r--r--   0 root         (0) root         (0)     1881 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chart-line.png
--rw-r--r--   0 root         (0) root         (0)     1948 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chart-pie.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chart.png
--rw-r--r--   0 root         (0) root         (0)     1954 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chat-bubble.png
--rw-r--r--   0 root         (0) root         (0)     1773 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-check-alt.png
--rw-r--r--   0 root         (0) root         (0)     1965 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-check-circle.png
--rw-r--r--   0 root         (0) root         (0)     1861 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-check.png
--rw-r--r--   0 root         (0) root         (0)     1884 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-bottom.png
--rw-r--r--   0 root         (0) root         (0)     1956 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-down-alt.png
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-left-alt.png
--rw-r--r--   0 root         (0) root         (0)     1953 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-right-alt.png
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-up-alt.png
--rw-r--r--   0 root         (0) root         (0)     1956 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-down.png
--rw-r--r--   0 root         (0) root         (0)     1941 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-left.png
--rw-r--r--   0 root         (0) root         (0)     1949 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-right.png
--rw-r--r--   0 root         (0) root         (0)     1840 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-up-alt.png
--rw-r--r--   0 root         (0) root         (0)     1934 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-up.png
--rw-r--r--   0 root         (0) root         (0)     1872 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-left.png
--rw-r--r--   0 root         (0) root         (0)     1877 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-right.png
--rw-r--r--   0 root         (0) root         (0)     1874 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-top.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-circle.png
--rw-r--r--   0 root         (0) root         (0)     1865 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-clipboard.png
--rw-r--r--   0 root         (0) root         (0)     1952 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-clock.png
--rw-r--r--   0 root         (0) root         (0)     1895 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-clone.png
--rw-r--r--   0 root         (0) root         (0)     1919 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-closed-captioning.png
--rw-r--r--   0 root         (0) root         (0)     1939 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cloud-download.png
--rw-r--r--   0 root         (0) root         (0)     1947 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cloud-upload.png
--rw-r--r--   0 root         (0) root         (0)     1927 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cloudy.png
--rw-r--r--   0 root         (0) root         (0)     1906 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-code.png
--rw-r--r--   0 root         (0) root         (0)     1897 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-coffee.png
--rw-r--r--   0 root         (0) root         (0)     1933 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-comment-bubble.png
--rw-r--r--   0 root         (0) root         (0)     1824 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-comment-square.png
--rw-r--r--   0 root         (0) root         (0)     1858 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-credit-card.png
--rw-r--r--   0 root         (0) root         (0)     1924 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cursor-move.png
--rw-r--r--   0 root         (0) root         (0)     1898 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cursor.png
--rw-r--r--   0 root         (0) root         (0)     1928 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cut.png
--rw-r--r--   0 root         (0) root         (0)     1827 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-data-transfer-down.png
--rw-r--r--   0 root         (0) root         (0)     1833 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-data-transfer-up.png
--rw-r--r--   0 root         (0) root         (0)     1932 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-deaf.png
--rw-r--r--   0 root         (0) root         (0)     1922 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-description.png
--rw-r--r--   0 root         (0) root         (0)     1916 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-devices.png
--rw-r--r--   0 root         (0) root         (0)     1820 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-dialpad.png
--rw-r--r--   0 root         (0) root         (0)     1946 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-dog.png
--rw-r--r--   0 root         (0) root         (0)     1856 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-door.png
--rw-r--r--   0 root         (0) root         (0)     1929 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-double-quote-sans-left.png
--rw-r--r--   0 root         (0) root         (0)     1931 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-double-quote-sans-right.png
--rw-r--r--   0 root         (0) root         (0)     1895 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-drop.png
--rw-r--r--   0 root         (0) root         (0)     1916 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-envelope-closed.png
--rw-r--r--   0 root         (0) root         (0)     1967 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-envelope-letter.png
--rw-r--r--   0 root         (0) root         (0)     1969 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-envelope-open.png
--rw-r--r--   0 root         (0) root         (0)     1952 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-equalizer.png
--rw-r--r--   0 root         (0) root         (0)     1851 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-ethernet.png
--rw-r--r--   0 root         (0) root         (0)     1914 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-exit-to-app.png
--rw-r--r--   0 root         (0) root         (0)     1896 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-down.png
--rw-r--r--   0 root         (0) root         (0)     1911 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-left.png
--rw-r--r--   0 root         (0) root         (0)     1904 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-right.png
--rw-r--r--   0 root         (0) root         (0)     1902 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-up.png
--rw-r--r--   0 root         (0) root         (0)     1925 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-exposure.png
--rw-r--r--   0 root         (0) root         (0)     1902 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-external-link.png
--rw-r--r--   0 root         (0) root         (0)     1973 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-face-dead.png
--rw-r--r--   0 root         (0) root         (0)     1915 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-featured-playlist.png
--rw-r--r--   0 root         (0) root         (0)     1870 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-file.png
--rw-r--r--   0 root         (0) root         (0)     1924 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-find-in-page.png
--rw-r--r--   0 root         (0) root         (0)     1997 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-fingerprint.png
--rw-r--r--   0 root         (0) root         (0)     1949 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-fire.png
--rw-r--r--   0 root         (0) root         (0)     1910 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-flip-to-back.png
--rw-r--r--   0 root         (0) root         (0)     1921 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-folder-open.png
--rw-r--r--   0 root         (0) root         (0)     1834 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-folder.png
--rw-r--r--   0 root         (0) root         (0)     1961 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-frown.png
--rw-r--r--   0 root         (0) root         (0)     1977 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-gamepad.png
--rw-r--r--   0 root         (0) root         (0)     1925 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-down.png
--rw-r--r--   0 root         (0) root         (0)     1912 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-left.png
--rw-r--r--   0 root         (0) root         (0)     1909 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-right.png
--rw-r--r--   0 root         (0) root         (0)     1922 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-up.png
--rw-r--r--   0 root         (0) root         (0)     1925 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hd.png
--rw-r--r--   0 root         (0) root         (0)     1939 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hdr.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-headphones.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-heart.png
--rw-r--r--   0 root         (0) root         (0)     1903 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-highligt.png
--rw-r--r--   0 root         (0) root         (0)     1966 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-history.png
--rw-r--r--   0 root         (0) root         (0)     1910 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-home.png
--rw-r--r--   0 root         (0) root         (0)     1948 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-house.png
--rw-r--r--   0 root         (0) root         (0)     1963 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-image-plus.png
--rw-r--r--   0 root         (0) root         (0)     1951 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-image1.png
--rw-r--r--   0 root         (0) root         (0)     1875 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-infinity.png
--rw-r--r--   0 root         (0) root         (0)     1912 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-input-power.png
--rw-r--r--   0 root         (0) root         (0)     1875 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-input.png
--rw-r--r--   0 root         (0) root         (0)     1818 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-justify-center.png
--rw-r--r--   0 root         (0) root         (0)     1814 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-justify-left.png
--rw-r--r--   0 root         (0) root         (0)     1807 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-justify-right.png
--rw-r--r--   0 root         (0) root         (0)     1890 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-keyboard.png
--rw-r--r--   0 root         (0) root         (0)     1818 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-laptop.png
--rw-r--r--   0 root         (0) root         (0)     1982 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-layers.png
--rw-r--r--   0 root         (0) root         (0)     1827 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-level-down.png
--rw-r--r--   0 root         (0) root         (0)     1826 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-level-up.png
--rw-r--r--   0 root         (0) root         (0)     1946 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-library-add.png
--rw-r--r--   0 root         (0) root         (0)     1875 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-library.png
--rw-r--r--   0 root         (0) root         (0)     1929 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-lightbulb.png
--rw-r--r--   0 root         (0) root         (0)     1869 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-link-alt.png
--rw-r--r--   0 root         (0) root         (0)     1938 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-link-broken.png
--rw-r--r--   0 root         (0) root         (0)     1904 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-link.png
--rw-r--r--   0 root         (0) root         (0)     1923 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-location-pin.png
--rw-r--r--   0 root         (0) root         (0)     1921 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-lock-locked.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-lock-unlocked.png
--rw-r--r--   0 root         (0) root         (0)     1948 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-loop-1.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-loop-circular.png
--rw-r--r--   0 root         (0) root         (0)     1892 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-loop.png
--rw-r--r--   0 root         (0) root         (0)     1984 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-low-vision.png
--rw-r--r--   0 root         (0) root         (0)     1910 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-magnifying-glass.png
--rw-r--r--   0 root         (0) root         (0)     1908 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-map.png
--rw-r--r--   0 root         (0) root         (0)     1886 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-eject.png
--rw-r--r--   0 root         (0) root         (0)     1847 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-pause.png
--rw-r--r--   0 root         (0) root         (0)     1856 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-play.png
--rw-r--r--   0 root         (0) root         (0)     1918 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-skip-backward.png
--rw-r--r--   0 root         (0) root         (0)     1919 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-skip-forward.png
--rw-r--r--   0 root         (0) root         (0)     1864 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-step-backward.png
--rw-r--r--   0 root         (0) root         (0)     1869 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-step-forward.png
--rw-r--r--   0 root         (0) root         (0)     1800 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-stop.png
--rw-r--r--   0 root         (0) root         (0)     1908 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-medical-cross.png
--rw-r--r--   0 root         (0) root         (0)     1959 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-meh.png
--rw-r--r--   0 root         (0) root         (0)     1775 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-menu.png
--rw-r--r--   0 root         (0) root         (0)     1923 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-microphone.png
--rw-r--r--   0 root         (0) root         (0)     1697 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-minus.png
--rw-r--r--   0 root         (0) root         (0)     1858 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mobile-landscape.png
--rw-r--r--   0 root         (0) root         (0)     1906 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mobile.png
--rw-r--r--   0 root         (0) root         (0)     1968 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-bad.png
--rw-r--r--   0 root         (0) root         (0)     1962 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-good.png
--rw-r--r--   0 root         (0) root         (0)     1978 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-very-bad.png
--rw-r--r--   0 root         (0) root         (0)     1969 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-very-good.png
--rw-r--r--   0 root         (0) root         (0)     1918 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-moon.png
--rw-r--r--   0 root         (0) root         (0)     1924 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mouse.png
--rw-r--r--   0 root         (0) root         (0)     1914 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-move.png
--rw-r--r--   0 root         (0) root         (0)     2000 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-movie.png
--rw-r--r--   0 root         (0) root         (0)     1974 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mug-tea.png
--rw-r--r--   0 root         (0) root         (0)     1911 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mug.png
--rw-r--r--   0 root         (0) root         (0)     1883 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-notes.png
--rw-r--r--   0 root         (0) root         (0)     1827 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-options-horizontal.png
--rw-r--r--   0 root         (0) root         (0)     1819 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-options.png
--rw-r--r--   0 root         (0) root         (0)     1953 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paint-bucket.png
--rw-r--r--   0 root         (0) root         (0)     1928 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paper-plane.png
--rw-r--r--   0 root         (0) root         (0)     1905 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paperclip.png
--rw-r--r--   0 root         (0) root         (0)     1881 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paragraph.png
--rw-r--r--   0 root         (0) root         (0)     1917 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-pen-alt.png
--rw-r--r--   0 root         (0) root         (0)     1875 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-pencil.png
--rw-r--r--   0 root         (0) root         (0)     1974 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-people.png
--rw-r--r--   0 root         (0) root         (0)     1889 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-phone.png
--rw-r--r--   0 root         (0) root         (0)     1933 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-pin.png
--rw-r--r--   0 root         (0) root         (0)     1791 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-plus.png
--rw-r--r--   0 root         (0) root         (0)     1927 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-power-standby.png
--rw-r--r--   0 root         (0) root         (0)     1970 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-print.png
--rw-r--r--   0 root         (0) root         (0)     1784 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-rectangle.png
--rw-r--r--   0 root         (0) root         (0)     1917 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-reload.png
--rw-r--r--   0 root         (0) root         (0)     1924 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-remove.png
--rw-r--r--   0 root         (0) root         (0)     1956 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-rss.png
--rw-r--r--   0 root         (0) root         (0)     1944 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-satelite.png
--rw-r--r--   0 root         (0) root         (0)     1935 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-save.png
--rw-r--r--   0 root         (0) root         (0)     1851 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-screen-desktop.png
--rw-r--r--   0 root         (0) root         (0)     1854 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-screen-smartphone.png
--rw-r--r--   0 root         (0) root         (0)     1970 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-settings.png
--rw-r--r--   0 root         (0) root         (0)     1973 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-share-boxed.png
--rw-r--r--   0 root         (0) root         (0)     1921 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-share.png
--rw-r--r--   0 root         (0) root         (0)     1790 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-signal-cellular-0.png
--rw-r--r--   0 root         (0) root         (0)     1872 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-signal-cellular-3.png
--rw-r--r--   0 root         (0) root         (0)     1989 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-size-grip.png
--rw-r--r--   0 root         (0) root         (0)     1967 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-smile.png
--rw-r--r--   0 root         (0) root         (0)     1942 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-speaker.png
--rw-r--r--   0 root         (0) root         (0)     1886 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-speech.png
--rw-r--r--   0 root         (0) root         (0)     1963 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-speedometer.png
--rw-r--r--   0 root         (0) root         (0)     1934 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-star.png
--rw-r--r--   0 root         (0) root         (0)      417 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-sun.png
--rw-r--r--   0 root         (0) root         (0)     1942 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-tags.png
--rw-r--r--   0 root         (0) root         (0)     1952 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-task.png
--rw-r--r--   0 root         (0) root         (0)     1889 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-terminal.png
--rw-r--r--   0 root         (0) root         (0)     1910 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-text-size.png
--rw-r--r--   0 root         (0) root         (0)     1896 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-text-square.png
--rw-r--r--   0 root         (0) root         (0)     1850 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-text.png
--rw-r--r--   0 root         (0) root         (0)     1942 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-thumb-down.png
--rw-r--r--   0 root         (0) root         (0)     1943 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-thumb-up.png
--rw-r--r--   0 root         (0) root         (0)     1869 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-transfer.png
--rw-r--r--   0 root         (0) root         (0)     1862 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-triangle.png
--rw-r--r--   0 root         (0) root         (0)     1977 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-truck.png
--rw-r--r--   0 root         (0) root         (0)     1925 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user-female.png
--rw-r--r--   0 root         (0) root         (0)     1916 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user-follow.png
--rw-r--r--   0 root         (0) root         (0)     1942 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user-unfollow.png
--rw-r--r--   0 root         (0) root         (0)     1888 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user.png
--rw-r--r--   0 root         (0) root         (0)     1799 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-vertical-align-bottom.png
--rw-r--r--   0 root         (0) root         (0)     1863 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-column.png
--rw-r--r--   0 root         (0) root         (0)     1942 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-module.png
--rw-r--r--   0 root         (0) root         (0)     1899 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-quilt.png
--rw-r--r--   0 root         (0) root         (0)     1820 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-stream.png
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-voice-over-record.png
--rw-r--r--   0 root         (0) root         (0)     1986 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-volume-high.png
--rw-r--r--   0 root         (0) root         (0)     1936 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-volume-low.png
--rw-r--r--   0 root         (0) root         (0)     1945 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-volume-off.png
--rw-r--r--   0 root         (0) root         (0)     1865 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wallet.png
--rw-r--r--   0 root         (0) root         (0)     1915 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-watch.png
--rw-r--r--   0 root         (0) root         (0)     1903 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-0.png
--rw-r--r--   0 root         (0) root         (0)     1921 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-1.png
--rw-r--r--   0 root         (0) root         (0)     1944 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-2.png
--rw-r--r--   0 root         (0) root         (0)     1973 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-4.png
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-off.png
--rw-r--r--   0 root         (0) root         (0)     1817 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-window-maximize.png
--rw-r--r--   0 root         (0) root         (0)     1689 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-window-minimize.png
--rw-r--r--   0 root         (0) root         (0)     1915 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-window-restore.png
--rw-r--r--   0 root         (0) root         (0)     1876 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wrap-text.png
--rw-r--r--   0 root         (0) root         (0)     1970 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-x-circle.png
--rw-r--r--   0 root         (0) root         (0)     1844 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-x.png
--rw-r--r--   0 root         (0) root         (0)     1945 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-zoom-in.png
--rw-r--r--   0 root         (0) root         (0)     1938 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-zoom-out.png
--rw-r--r--   0 root         (0) root         (0)      210 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/icon_close.png
--rw-r--r--   0 root         (0) root         (0)      248 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/icon_maximize.png
--rw-r--r--   0 root         (0) root         (0)      248 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/icon_menu.png
--rw-r--r--   0 root         (0) root         (0)      172 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/icon_minimize.png
--rw-r--r--   0 root         (0) root         (0)      322 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/icon_restore.png
--rw-r--r--   0 root         (0) root         (0)      386 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/icons/icon_settings.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.721177 djsciops-1.5.5/djsciops/axon_gui/images/images/
--rw-r--r--   0 root         (0) root         (0)     1349 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/images/symbol-black.png
--rw-r--r--   0 root         (0) root         (0)     1380 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/images/symbol-white.png
--rw-r--r--   0 root         (0) root         (0)     2399 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/images/images/symbol.png
--rw-r--r--   0 root         (0) root         (0)    17152 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/main.py
--rw-r--r--   0 root         (0) root         (0)   116139 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/main.ui
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.725177 djsciops-1.5.5/djsciops/axon_gui/modules/
--rw-r--r--   0 root         (0) root         (0)      906 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/modules/app_functions.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/modules/app_settings.py
--rw-r--r--   0 root         (0) root         (0)   850907 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/modules/resources_rc.py
--rw-r--r--   0 root         (0) root         (0)    14376 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/modules/ui_functions.py
--rw-r--r--   0 root         (0) root         (0)    70229 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/modules/ui_main.py
--rw-r--r--   0 root         (0) root         (0)    12751 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/resources.qrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.725177 djsciops-1.5.5/djsciops/axon_gui/themes/
--rw-r--r--   0 root         (0) root         (0)    14159 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/themes/py_dracula_dark.qss
--rw-r--r--   0 root         (0) root         (0)    13864 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/themes/py_dracula_light.qss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.725177 djsciops-1.5.5/djsciops/axon_gui/widgets/
--rw-r--r--   0 root         (0) root         (0)      660 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.725177 djsciops-1.5.5/djsciops/axon_gui/widgets/custom_grips/
--rw-r--r--   0 root         (0) root         (0)      660 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/widgets/custom_grips/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10293 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/axon_gui/widgets/custom_grips/custom_grips.py
--rw-r--r--   0 root         (0) root         (0)    11931 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/command_line.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/log.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/settings.py
--rw-r--r--   0 root         (0) root         (0)      761 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-08-21 15:53:57.000000 djsciops-1.5.5/djsciops/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 15:54:10.665176 djsciops-1.5.5/djsciops.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1438 2023-08-21 15:54:10.000000 djsciops-1.5.5/djsciops.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13943 2023-08-21 15:54:10.000000 djsciops-1.5.5/djsciops.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 15:54:10.000000 djsciops-1.5.5/djsciops.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-08-21 15:54:10.000000 djsciops-1.5.5/djsciops.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       93 2023-08-21 15:54:10.000000 djsciops-1.5.5/djsciops.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-08-21 15:54:10.000000 djsciops-1.5.5/djsciops.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-21 15:54:10.725177 djsciops-1.5.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1560 2023-08-21 15:53:57.000000 djsciops-1.5.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.072226 djsciops-1.5.7/
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-30 18:46:49.072226 djsciops-1.5.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-01-06 07:07:55.000000 djsciops-1.5.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.012226 djsciops-1.5.7/djsciops/
+-rw-r--r--   0 root         (0) root         (0)       60 2022-03-23 14:46:07.000000 djsciops-1.5.7/djsciops/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16463 2024-04-29 21:38:26.000000 djsciops-1.5.7/djsciops/authentication.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.012226 djsciops-1.5.7/djsciops/axon/
+-rw-rw-r--   0 root         (0) root         (0)    14174 2024-04-29 21:38:26.000000 djsciops-1.5.7/djsciops/axon/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5129 2023-07-17 20:50:47.000000 djsciops-1.5.7/djsciops/axon/speed_audit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.012226 djsciops-1.5.7/djsciops/axon_gui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   255038 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/icon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.008226 djsciops-1.5.7/djsciops/axon_gui/images/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.068226 djsciops-1.5.7/djsciops/axon_gui/images/icons/
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-3d.png
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-4k.png
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-account-logout.png
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-action-redo.png
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-action-undo.png
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-airplane-mode-off.png
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-airplane-mode.png
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-alarm.png
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-align-center.png
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-align-left.png
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-align-right.png
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-bottom-2.png
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-bottom.png
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-bottom.png
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-left.png
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-right.png
+-rw-r--r--   0 root         (0) root         (0)     1971 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-top.png
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-left.png
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-right.png
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-top.png
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-at.png
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-av-timer.png
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-ban.png
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-0.png
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-3.png
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-5.png
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-alert.png
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-slash.png
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-bell.png
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-bluetooth.png
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-briefcase.png
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-browser.png
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-calendar-check.png
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-camera-roll.png
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-camera.png
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-bottom.png
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-left.png
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-right.png
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-top.png
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cart.png
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cast.png
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chart-line.png
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chart-pie.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chart.png
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chat-bubble.png
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-check-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-check-circle.png
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-check.png
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-bottom.png
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-down-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-left-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-right-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-up-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-down.png
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-left.png
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-right.png
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-up-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-up.png
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-left.png
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-right.png
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-top.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-circle.png
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-clipboard.png
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-clock.png
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-clone.png
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-closed-captioning.png
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cloud-download.png
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cloud-upload.png
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cloudy.png
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-code.png
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-coffee.png
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-comment-bubble.png
+-rw-r--r--   0 root         (0) root         (0)     1824 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-comment-square.png
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-credit-card.png
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cursor-move.png
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cursor.png
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cut.png
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-data-transfer-down.png
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-data-transfer-up.png
+-rw-r--r--   0 root         (0) root         (0)     1932 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-deaf.png
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-description.png
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-devices.png
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-dialpad.png
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-dog.png
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-door.png
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-double-quote-sans-left.png
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-double-quote-sans-right.png
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-drop.png
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-envelope-closed.png
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-envelope-letter.png
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-envelope-open.png
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-equalizer.png
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-ethernet.png
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-exit-to-app.png
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-down.png
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-left.png
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-right.png
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-up.png
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-exposure.png
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-external-link.png
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-face-dead.png
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-featured-playlist.png
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-file.png
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-find-in-page.png
+-rw-r--r--   0 root         (0) root         (0)     1997 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-fingerprint.png
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-fire.png
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-flip-to-back.png
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-folder-open.png
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-folder.png
+-rw-r--r--   0 root         (0) root         (0)     1961 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-frown.png
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-gamepad.png
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-down.png
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-left.png
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-right.png
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-up.png
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hd.png
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hdr.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-headphones.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-heart.png
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-highligt.png
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-history.png
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-home.png
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-house.png
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-image-plus.png
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-image1.png
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-infinity.png
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-input-power.png
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-input.png
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-justify-center.png
+-rw-r--r--   0 root         (0) root         (0)     1814 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-justify-left.png
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-justify-right.png
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-keyboard.png
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-laptop.png
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-layers.png
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-level-down.png
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-level-up.png
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-library-add.png
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-library.png
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-lightbulb.png
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-link-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-link-broken.png
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-link.png
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-location-pin.png
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-lock-locked.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-lock-unlocked.png
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-loop-1.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-loop-circular.png
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-loop.png
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-low-vision.png
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-magnifying-glass.png
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-map.png
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-eject.png
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-pause.png
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-play.png
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-skip-backward.png
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-skip-forward.png
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-step-backward.png
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-step-forward.png
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-stop.png
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-medical-cross.png
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-meh.png
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-menu.png
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-microphone.png
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-minus.png
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mobile-landscape.png
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mobile.png
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-bad.png
+-rw-r--r--   0 root         (0) root         (0)     1962 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-good.png
+-rw-r--r--   0 root         (0) root         (0)     1978 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-very-bad.png
+-rw-r--r--   0 root         (0) root         (0)     1969 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-very-good.png
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-moon.png
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mouse.png
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-move.png
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-movie.png
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mug-tea.png
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mug.png
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-notes.png
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-options-horizontal.png
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-options.png
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paint-bucket.png
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paper-plane.png
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paperclip.png
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paragraph.png
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-pen-alt.png
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-pencil.png
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-people.png
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-phone.png
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-pin.png
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-plus.png
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-power-standby.png
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-print.png
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-rectangle.png
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-reload.png
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-remove.png
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-rss.png
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-satelite.png
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-save.png
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-screen-desktop.png
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-screen-smartphone.png
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-settings.png
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-share-boxed.png
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-share.png
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-signal-cellular-0.png
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-signal-cellular-3.png
+-rw-r--r--   0 root         (0) root         (0)     1989 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-size-grip.png
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-smile.png
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-speaker.png
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-speech.png
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-speedometer.png
+-rw-r--r--   0 root         (0) root         (0)     1934 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-star.png
+-rw-r--r--   0 root         (0) root         (0)      417 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-sun.png
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-tags.png
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-task.png
+-rw-r--r--   0 root         (0) root         (0)     1889 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-terminal.png
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-text-size.png
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-text-square.png
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-text.png
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-thumb-down.png
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-thumb-up.png
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-transfer.png
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-triangle.png
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-truck.png
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user-female.png
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user-follow.png
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user-unfollow.png
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user.png
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-vertical-align-bottom.png
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-column.png
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-module.png
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-quilt.png
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-stream.png
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-voice-over-record.png
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-volume-high.png
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-volume-low.png
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-volume-off.png
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wallet.png
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-watch.png
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-0.png
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-1.png
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-2.png
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-4.png
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-off.png
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-window-maximize.png
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-window-minimize.png
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-window-restore.png
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wrap-text.png
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-x-circle.png
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-x.png
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-zoom-in.png
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-zoom-out.png
+-rw-r--r--   0 root         (0) root         (0)      210 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/icon_close.png
+-rw-r--r--   0 root         (0) root         (0)      248 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/icon_maximize.png
+-rw-r--r--   0 root         (0) root         (0)      248 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/icon_menu.png
+-rw-r--r--   0 root         (0) root         (0)      172 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/icon_minimize.png
+-rw-r--r--   0 root         (0) root         (0)      322 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/icon_restore.png
+-rw-r--r--   0 root         (0) root         (0)      386 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/icons/icon_settings.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.068226 djsciops-1.5.7/djsciops/axon_gui/images/images/
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/images/symbol-black.png
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/images/symbol-white.png
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/images/images/symbol.png
+-rw-rw-r--   0 root         (0) root         (0)    17297 2024-04-29 21:38:26.000000 djsciops-1.5.7/djsciops/axon_gui/main.py
+-rw-r--r--   0 root         (0) root         (0)   116139 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/main.ui
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.072226 djsciops-1.5.7/djsciops/axon_gui/modules/
+-rw-r--r--   0 root         (0) root         (0)      906 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/modules/app_functions.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/modules/app_settings.py
+-rw-r--r--   0 root         (0) root         (0)   850907 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/modules/resources_rc.py
+-rw-r--r--   0 root         (0) root         (0)    14376 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/modules/ui_functions.py
+-rw-r--r--   0 root         (0) root         (0)    70229 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/modules/ui_main.py
+-rw-r--r--   0 root         (0) root         (0)    12751 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/resources.qrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.072226 djsciops-1.5.7/djsciops/axon_gui/themes/
+-rw-r--r--   0 root         (0) root         (0)    14159 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/themes/py_dracula_dark.qss
+-rw-r--r--   0 root         (0) root         (0)    13864 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/themes/py_dracula_light.qss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.072226 djsciops-1.5.7/djsciops/axon_gui/widgets/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.072226 djsciops-1.5.7/djsciops/axon_gui/widgets/custom_grips/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/widgets/custom_grips/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10293 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/axon_gui/widgets/custom_grips/custom_grips.py
+-rw-rw-r--   0 root         (0) root         (0)    11995 2024-04-29 21:38:26.000000 djsciops-1.5.7/djsciops/command_line.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/log.py
+-rw-rw-r--   0 root         (0) root         (0)     4626 2024-04-29 21:38:26.000000 djsciops-1.5.7/djsciops/settings.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-01-06 07:07:55.000000 djsciops-1.5.7/djsciops/utils.py
+-rw-rw-r--   0 root         (0) root         (0)       22 2024-04-29 21:38:26.000000 djsciops-1.5.7/djsciops/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 18:46:49.012226 djsciops-1.5.7/djsciops.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-04-30 18:46:48.000000 djsciops-1.5.7/djsciops.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13943 2024-04-30 18:46:48.000000 djsciops-1.5.7/djsciops.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 18:46:48.000000 djsciops-1.5.7/djsciops.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-30 18:46:48.000000 djsciops-1.5.7/djsciops.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-30 18:46:48.000000 djsciops-1.5.7/djsciops.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-30 18:46:48.000000 djsciops-1.5.7/djsciops.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 18:46:49.072226 djsciops-1.5.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1560 2023-01-06 07:07:55.000000 djsciops-1.5.7/setup.py
```

### Comparing `djsciops-1.5.5/PKG-INFO` & `djsciops-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsciops
-Version: 1.5.5
+Version: 1.5.7
 Summary: A suite of customer CLI tools for DataJoint SciOps.
 Home-page: https://github.com/dj-sciops/djsciops-python
 Author: DataJoint
 Author-email: djbot@datajoint.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `djsciops-1.5.5/README.md` & `djsciops-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/authentication.py` & `djsciops-1.5.7/djsciops/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 import base64
 from datetime import datetime, timezone
 import json
 import logging
+import os
+import sys
 import flask
 import webbrowser
 import urllib
 import http.client
 import botocore
 import botocore.config
 from .log import log
 from time import time
 import multiprocessing
 
 import boto3
 from botocore.credentials import RefreshableCredentials
 from botocore.session import get_session
 from djsciops import settings as djsciops_settings
+try:
+    # Python 3.4+
+    if sys.platform.startswith('win'):
+        import multiprocessing.popen_spawn_win32 as forking
+    else:
+        import multiprocessing.popen_fork as forking
+except ImportError:
+    import multiprocessing.forking as forking
 
 LOOKUP_SERVICE_ALLOWED_ORIGIN = "https://ops.datajoint.io"
 LOOKUP_SERVICE_DOMAIN = "ops.datajoint.io"
 LOOKUP_SERVICE_ROUTE = "/social-login/api/user"
 # Everything LOOKUP_SERVICE_AUTH is changed, need to change:
 # https://github.com/datajoint-company/dj-gitops/blob/main/applications/k8s/deployments/ops.datajoint.io/social_login_interceptor/client_store_secrets.yaml
 LOOKUP_SERVICE_AUTH = {
@@ -237,14 +247,39 @@
     jwt_data = json.loads(
         base64.b64decode((bearer_token.split(".")[1] + "==").encode()).decode()
     )
     log.debug(f"jwt_data: {jwt_data}")
     return jwt_data
 
 
+if sys.platform.startswith('win'):
+    # First define a modified version of Popen.
+    class _Popen(forking.Popen):
+        def __init__(self, *args, **kw):
+            if hasattr(sys, 'frozen'):
+                # We have to set original _MEIPASS2 value from sys._MEIPASS
+                # to get --onefile mode working.
+                os.putenv('_MEIPASS2', sys._MEIPASS)
+            try:
+                super(_Popen, self).__init__(*args, **kw)
+            finally:
+                if hasattr(sys, 'frozen'):
+                    # On some platforms (e.g. AIX) 'os.unsetenv()' is not
+                    # available. In those cases we cannot delete the variable
+                    # but only set it to the empty string. The bootloader
+                    # can handle this case.
+                    if hasattr(os, 'unsetenv'):
+                        os.unsetenv('_MEIPASS2')
+                    else:
+                        os.putenv('_MEIPASS2', '')
+
+    # Second override 'Popen' class with our modified version.
+    forking.Popen = _Popen
+
+
 class Session:
     def __init__(
         self,
         aws_account_id: str,
         s3_role: str,
         auth_client_id: str,
         auth_client_secret: str = None,
```

### Comparing `djsciops-1.5.5/djsciops/axon/__init__.py` & `djsciops-1.5.7/djsciops/axon/__init__.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon/speed_audit.py` & `djsciops-1.5.7/djsciops/axon/speed_audit.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/icon.ico` & `djsciops-1.5.7/djsciops/axon_gui/icon.ico`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-3d.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-3d.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-4k.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-4k.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-account-logout.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-account-logout.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-action-redo.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-action-redo.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-action-undo.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-action-undo.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-airplane-mode-off.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-airplane-mode-off.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-airplane-mode.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-airplane-mode.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-alarm.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-alarm.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-align-center.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-align-center.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-align-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-align-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-align-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-align-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-bottom-2.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-bottom-2.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-bottom.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-bottom.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-bottom.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-bottom.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-circle-top.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-circle-top.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-arrow-top.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-arrow-top.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-at.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-at.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-av-timer.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-av-timer.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-ban.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-ban.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-0.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-0.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-3.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-3.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-5.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-5.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-alert.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-alert.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-battery-slash.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-battery-slash.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-bell.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-bell.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-bluetooth.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-bluetooth.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-briefcase.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-briefcase.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-browser.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-browser.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-calendar-check.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-calendar-check.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-camera-roll.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-camera-roll.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-camera.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-camera.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-bottom.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-bottom.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-caret-top.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-caret-top.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cart.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cart.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cast.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cast.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chart-line.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chart-line.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chart-pie.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chart-pie.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chart.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chart.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chat-bubble.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chat-bubble.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-check-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-check-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-check-circle.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-check-circle.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-check.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-check.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-bottom.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-bottom.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-down-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-down-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-left-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-left-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-right-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-right-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-circle-up-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-circle-up-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-down.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-down.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-up-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-up-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-double-up.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-double-up.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-chevron-top.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-chevron-top.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-circle.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-circle.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-clipboard.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-clipboard.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-clock.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-clock.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-clone.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-clone.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-closed-captioning.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-closed-captioning.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cloud-download.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cloud-download.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cloud-upload.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cloud-upload.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cloudy.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cloudy.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-code.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-code.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-coffee.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-coffee.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-comment-bubble.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-comment-bubble.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-comment-square.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-comment-square.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-credit-card.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-credit-card.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cursor-move.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cursor-move.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cursor.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cursor.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-cut.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-cut.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-data-transfer-down.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-data-transfer-down.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-data-transfer-up.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-data-transfer-up.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-deaf.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-deaf.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-description.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-description.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-devices.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-devices.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-dialpad.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-dialpad.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-dog.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-dog.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-door.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-door.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-double-quote-sans-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-double-quote-sans-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-double-quote-sans-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-double-quote-sans-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-drop.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-drop.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-envelope-closed.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-envelope-closed.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-envelope-letter.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-envelope-letter.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-envelope-open.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-envelope-open.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-equalizer.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-equalizer.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-ethernet.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-ethernet.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-exit-to-app.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-exit-to-app.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-down.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-down.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-expand-up.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-expand-up.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-exposure.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-exposure.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-external-link.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-external-link.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-face-dead.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-face-dead.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-featured-playlist.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-featured-playlist.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-file.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-file.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-find-in-page.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-find-in-page.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-fingerprint.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-fingerprint.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-fire.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-fire.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-flip-to-back.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-flip-to-back.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-folder-open.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-folder-open.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-folder.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-folder.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-frown.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-frown.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-gamepad.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-gamepad.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-down.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-down.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hand-point-up.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hand-point-up.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hd.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hd.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-hdr.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-hdr.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-headphones.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-headphones.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-heart.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-heart.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-highligt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-highligt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-history.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-history.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-home.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-home.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-house.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-house.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-image-plus.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-image-plus.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-image1.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-image1.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-infinity.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-infinity.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-input-power.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-input-power.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-input.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-input.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-justify-center.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-justify-center.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-justify-left.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-justify-left.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-justify-right.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-justify-right.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-keyboard.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-keyboard.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-laptop.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-laptop.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-layers.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-layers.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-level-down.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-level-down.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-level-up.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-level-up.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-library-add.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-library-add.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-library.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-library.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-lightbulb.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-lightbulb.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-link-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-link-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-link-broken.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-link-broken.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-link.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-link.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-location-pin.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-location-pin.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-lock-locked.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-lock-locked.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-lock-unlocked.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-lock-unlocked.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-loop-1.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-loop-1.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-loop-circular.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-loop-circular.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-loop.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-loop.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-low-vision.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-low-vision.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-magnifying-glass.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-magnifying-glass.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-map.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-map.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-eject.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-eject.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-pause.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-pause.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-play.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-play.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-skip-backward.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-skip-backward.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-skip-forward.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-skip-forward.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-step-backward.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-step-backward.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-step-forward.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-step-forward.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-media-stop.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-media-stop.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-medical-cross.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-medical-cross.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-meh.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-meh.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-menu.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-menu.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-microphone.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-microphone.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-minus.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-minus.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mobile-landscape.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mobile-landscape.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mobile.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mobile.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-bad.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-bad.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-good.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-good.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-very-bad.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-very-bad.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mood-very-good.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mood-very-good.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-moon.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-moon.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mouse.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mouse.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-move.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-move.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-movie.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-movie.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mug-tea.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mug-tea.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-mug.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-mug.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-notes.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-notes.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-options-horizontal.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-options-horizontal.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-options.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-options.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paint-bucket.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paint-bucket.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paper-plane.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paper-plane.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paperclip.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paperclip.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-paragraph.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-paragraph.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-pen-alt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-pen-alt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-pencil.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-pencil.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-people.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-people.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-phone.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-phone.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-pin.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-pin.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-plus.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-plus.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-power-standby.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-power-standby.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-print.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-print.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-rectangle.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-rectangle.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-reload.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-reload.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-remove.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-remove.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-rss.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-rss.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-satelite.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-satelite.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-save.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-save.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-screen-desktop.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-screen-desktop.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-screen-smartphone.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-screen-smartphone.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-settings.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-settings.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-share-boxed.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-share-boxed.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-share.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-share.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-signal-cellular-0.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-signal-cellular-0.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-signal-cellular-3.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-signal-cellular-3.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-size-grip.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-size-grip.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-smile.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-smile.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-speaker.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-speaker.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-speech.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-speech.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-speedometer.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-speedometer.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-star.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-star.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-tags.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-tags.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-task.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-task.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-terminal.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-terminal.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-text-size.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-text-size.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-text-square.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-text-square.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-text.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-text.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-thumb-down.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-thumb-down.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-thumb-up.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-thumb-up.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-transfer.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-transfer.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-triangle.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-triangle.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-truck.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-truck.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user-female.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user-female.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user-follow.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user-follow.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user-unfollow.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user-unfollow.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-user.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-user.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-vertical-align-bottom.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-vertical-align-bottom.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-column.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-column.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-module.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-module.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-quilt.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-quilt.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-view-stream.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-view-stream.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-voice-over-record.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-voice-over-record.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-volume-high.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-volume-high.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-volume-low.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-volume-low.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-volume-off.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-volume-off.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wallet.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wallet.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-watch.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-watch.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-0.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-0.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-1.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-1.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-2.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-2.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-4.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-4.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wifi-signal-off.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wifi-signal-off.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-window-maximize.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-window-maximize.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-window-minimize.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-window-minimize.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-window-restore.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-window-restore.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-wrap-text.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-wrap-text.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-x-circle.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-x-circle.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-x.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-x.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-zoom-in.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-zoom-in.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/icons/cil-zoom-out.png` & `djsciops-1.5.7/djsciops/axon_gui/images/icons/cil-zoom-out.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/images/symbol-black.png` & `djsciops-1.5.7/djsciops/axon_gui/images/images/symbol-black.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/images/symbol-white.png` & `djsciops-1.5.7/djsciops/axon_gui/images/images/symbol-white.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/images/images/symbol.png` & `djsciops-1.5.7/djsciops/axon_gui/images/images/symbol.png`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/main.py` & `djsciops-1.5.7/djsciops/axon_gui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #
 # There are limitations on Qt licenses if you want to use your products
 # commercially, I recommend reading them on the official website:
 # https://doc.qt.io/qtforpython/licenses.html
 #
 # ///////////////////////////////////////////////////////////////
 
+from multiprocessing import freeze_support
 import sys
 import os
 import platform
 import traceback
 import logging
 import yaml
 from datetime import datetime
@@ -361,14 +362,15 @@
     def generate_auth_token(self):
         widgets.refreshTokenBtn.setEnabled(False)
         worker = Worker(
             djsciops_authentication.Session,
             aws_account_id=self.config["aws"]["account_id"],
             s3_role=self.config["s3"]["role"],
             auth_client_id=self.config["djauth"]["client_id"],
+            auth_client_secret=self.config["djauth"].get("client_secret", None),
         )
         worker.signals.result.connect(self.auth_result)
         worker.signals.finished.connect(self.auth_finished)
         self.threadpool.start(worker)
 
     def load_bucket_dir(self):
         if self.check_auth_token():
@@ -463,11 +465,12 @@
         if event.buttons() == Qt.LeftButton:
             print("Mouse click: LEFT CLICK")
         if event.buttons() == Qt.RightButton:
             print("Mouse click: RIGHT CLICK")
 
 
 if __name__ == "__main__":
+    freeze_support()
     app = QApplication(sys.argv)
     app.setWindowIcon(QIcon(os.path.join(basedir, "icon.ico")))
     window = MainWindow()
     sys.exit(app.exec())
```

### Comparing `djsciops-1.5.5/djsciops/axon_gui/main.ui` & `djsciops-1.5.7/djsciops/axon_gui/main.ui`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/modules/__init__.py` & `djsciops-1.5.7/djsciops/axon_gui/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/modules/app_functions.py` & `djsciops-1.5.7/djsciops/axon_gui/modules/app_functions.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/modules/app_settings.py` & `djsciops-1.5.7/djsciops/axon_gui/modules/app_settings.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/modules/resources_rc.py` & `djsciops-1.5.7/djsciops/axon_gui/modules/resources_rc.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/modules/ui_functions.py` & `djsciops-1.5.7/djsciops/axon_gui/modules/ui_functions.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/modules/ui_main.py` & `djsciops-1.5.7/djsciops/axon_gui/modules/ui_main.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/resources.qrc` & `djsciops-1.5.7/djsciops/axon_gui/resources.qrc`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/themes/py_dracula_dark.qss` & `djsciops-1.5.7/djsciops/axon_gui/themes/py_dracula_dark.qss`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/themes/py_dracula_light.qss` & `djsciops-1.5.7/djsciops/axon_gui/themes/py_dracula_light.qss`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/widgets/__init__.py` & `djsciops-1.5.7/djsciops/axon_gui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/widgets/custom_grips/__init__.py` & `djsciops-1.5.7/djsciops/axon_gui/widgets/custom_grips/__init__.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/axon_gui/widgets/custom_grips/custom_grips.py` & `djsciops-1.5.7/djsciops/axon_gui/widgets/custom_grips/custom_grips.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/command_line.py` & `djsciops-1.5.7/djsciops/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+from multiprocessing import freeze_support
 import sys
 import yaml
 from djsciops import __version__ as version
 from djsciops import authentication as djsciops_authentication
 from djsciops import axon as djsciops_axon
 from djsciops import settings as djsciops_settings
 from djsciops.axon import speed_audit as djsciops_speed_audit
@@ -312,8 +313,9 @@
 
         else:
             log.info(yaml.dump(djsciops_config), extra={"disable_format": True})
     raise SystemExit
 
 
 if __name__ == "__main__":
+    freeze_support()
     djsciops()
```

### Comparing `djsciops-1.5.5/djsciops/log.py` & `djsciops-1.5.7/djsciops/log.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/settings.py` & `djsciops-1.5.7/djsciops/settings.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops/utils.py` & `djsciops-1.5.7/djsciops/utils.py`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/djsciops.egg-info/PKG-INFO` & `djsciops-1.5.7/djsciops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djsciops
-Version: 1.5.5
+Version: 1.5.7
 Summary: A suite of customer CLI tools for DataJoint SciOps.
 Home-page: https://github.com/dj-sciops/djsciops-python
 Author: DataJoint
 Author-email: djbot@datajoint.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `djsciops-1.5.5/djsciops.egg-info/SOURCES.txt` & `djsciops-1.5.7/djsciops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djsciops-1.5.5/setup.py` & `djsciops-1.5.7/setup.py`

 * *Files identical despite different names*

