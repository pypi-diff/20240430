# Comparing `tmp/wagtail_resume-2.7.2.tar.gz` & `tmp/wagtail_resume-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_resume-2.7.2.tar", max compression
+gzip compressed data, was "wagtail_resume-2.8.0.tar", max compression
```

## Comparing `wagtail_resume-2.7.2.tar` & `wagtail_resume-2.8.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1069 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/LICENSE
--rw-r--r--   0        0        0     3496 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/README.md
--rw-r--r--   0        0        0     3729 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/__init__.py
--rw-r--r--   0        0        0      138 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/apps.py
--rw-r--r--   0        0        0     7326 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/blocks.py
--rw-r--r--   0        0        0     1085 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3477 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0001_initial.py
--rw-r--r--   0        0        0     1955 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0002_auto_20191227_0916.py
--rw-r--r--   0        0        0     3655 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0003_auto_20200110_1525.py
--rw-r--r--   0        0        0      467 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0004_auto_20200110_1656.py
--rw-r--r--   0        0        0     3843 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0005_auto_20200227_1224.py
--rw-r--r--   0        0        0      694 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
--rw-r--r--   0        0        0      792 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0     4472 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0008_auto_20220211_1557.py
--rw-r--r--   0        0        0      953 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0    18241 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
--rw-r--r--   0        0        0    17599 2024-04-17 21:41:46.363672 wagtail_resume-2.7.2/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
--rw-r--r--   0        0        0    17734 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0    18655 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0      535 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
--rw-r--r--   0        0        0        0 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/migrations/__init__.py
--rw-r--r--   0        0        0     4037 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/models.py
--rw-r--r--   0        0        0        0 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/static/wagtail_resume/css/.gitkeep
--rw-r--r--   0        0        0     2024 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/static/wagtail_resume/css/resume_page.css
--rw-r--r--   0        0        0        0 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/static/wagtail_resume/images/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/static/wagtail_resume/js/.gitkeep
--rw-r--r--   0        0        0      406 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
--rw-r--r--   0        0        0     1516 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
--rw-r--r--   0        0        0      951 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
--rw-r--r--   0        0        0      691 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
--rw-r--r--   0        0        0      653 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
--rw-r--r--   0        0        0      107 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/resume_page.html
--rw-r--r--   0        0        0     2556 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/resume_page_body.html
--rw-r--r--   0        0        0      564 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/resume_page_head.html
--rw-r--r--   0        0        0        0 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templatetags/__init__.py
--rw-r--r--   0        0        0      139 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/templatetags/wagtail_resume_extras.py
--rw-r--r--   0        0        0      142 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/urls.py
--rw-r--r--   0        0        0     2075 2024-04-17 21:41:46.367672 wagtail_resume-2.7.2/wagtail_resume/views.py
--rw-r--r--   0        0        0     4955 1970-01-01 00:00:00.000000 wagtail_resume-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-30 11:10:18.101386 wagtail_resume-2.8.0/LICENSE
+-rw-r--r--   0        0        0     3496 2024-04-30 11:10:18.101386 wagtail_resume-2.8.0/README.md
+-rw-r--r--   0        0        0     3813 2024-04-30 11:10:18.101386 wagtail_resume-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/apps.py
+-rw-r--r--   0        0        0     7326 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/blocks.py
+-rw-r--r--   0        0        0     1085 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3477 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1955 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
+-rw-r--r--   0        0        0     3655 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
+-rw-r--r--   0        0        0      467 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
+-rw-r--r--   0        0        0     3843 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
+-rw-r--r--   0        0        0      694 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
+-rw-r--r--   0        0        0      792 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0     4472 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
+-rw-r--r--   0        0        0      953 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0    18241 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
+-rw-r--r--   0        0        0    17599 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
+-rw-r--r--   0        0        0    17734 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0    18655 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0      535 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
+-rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/migrations/__init__.py
+-rw-r--r--   0        0        0     4037 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/models.py
+-rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
+-rw-r--r--   0        0        0     2058 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
+-rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
+-rw-r--r--   0        0        0      401 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
+-rw-r--r--   0        0        0     1516 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
+-rw-r--r--   0        0        0      951 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
+-rw-r--r--   0        0        0      710 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
+-rw-r--r--   0        0        0      653 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
+-rw-r--r--   0        0        0      107 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page.html
+-rw-r--r--   0        0        0     2556 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
+-rw-r--r--   0        0        0      688 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
+-rw-r--r--   0        0        0        0 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templatetags/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/templatetags/wagtail_resume_extras.py
+-rw-r--r--   0        0        0      142 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/urls.py
+-rw-r--r--   0        0        0     2453 2024-04-30 11:10:18.105386 wagtail_resume-2.8.0/wagtail_resume/views.py
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 wagtail_resume-2.8.0/PKG-INFO
```

### Comparing `wagtail_resume-2.7.2/LICENSE` & `wagtail_resume-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/README.md` & `wagtail_resume-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/pyproject.toml` & `wagtail_resume-2.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail-resume"
 authors = ["Adin Hodovic <hodovicadin@gmail.com>"]
 license = "MIT"
-version = "2.7.2"
+version = "2.8.0"
 readme = "README.md"
 homepage = "https://github.com/adinhodovic/wagtail-resume"
 repository = "https://github.com/adinhodovic/wagtail-resume"
 documentation = "https://github.com/adinhodovic/wagtail-resume"
 description = "A Wagtail project made to simplify creation of resumes for developers."
 keywords = ["Resume", "Django", "Wagtail", "CMS"]
 classifiers = [
@@ -27,23 +27,24 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10 || ^3.11"
+python = "^3.10 || ^3.11 || 3.12"
 Django = "^3.2.0 || ^4.0.0 || ^5.0.0"
 wagtail = "^4.0.0 || ^5.0.0 || ^6.0.0"
-wagtail-markdown = "^0.10 || ^0.11"
+wagtail-markdown = "^0.10 || ^0.11 || ^0.12 || ^0.13"
 wagtail-metadata = "^4.0.0 || ^5.0.0"
-weasyprint = "^52"
+weasyprint = "^59 || ^60 || ^61"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "5.5.2"
 pylint-plugin-utils = "0.7"
 tox = "^3.14.3"
 coverage = "^5.0.2"
```

### Comparing `wagtail_resume-2.7.2/wagtail_resume/blocks.py` & `wagtail_resume-2.8.0/wagtail_resume/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/locale/sv/LC_MESSAGES/django.po` & `wagtail_resume-2.8.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0001_initial.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0002_auto_20191227_0916.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0002_auto_20191227_0916.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0003_auto_20200110_1525.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0003_auto_20200110_1525.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0005_auto_20200227_1224.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0005_auto_20200227_1224.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0008_auto_20220211_1557.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0008_auto_20220211_1557.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py` & `wagtail_resume-2.8.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/models.py` & `wagtail_resume-2.8.0/wagtail_resume/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/static/wagtail_resume/css/resume_page.css` & `wagtail_resume-2.8.0/wagtail_resume/static/wagtail_resume/css/resume_page.css`

 * *Files 2% similar despite different names*

```diff
@@ -131,21 +131,21 @@
   font-size: 1.5rem;
 }
 
 .pdf {
   display: None;
 }
 
-@media (min-width: 768px) {
-  .personal-info {
-    align-items: center;
-    display: flex;
-    justify-content: space-between;
-  }
+.personal-info {
+  align-items: center;
+  display: flex;
+  justify-content: space-between;
+}
 
+@media (min-width: 768px) {
   .resume {
     padding: 4rem 3rem;
     width: 80%;
   }
 
   .pdf {
     color: white;
@@ -169,11 +169,15 @@
 }
 
 @media (max-width: 768px) {
   .resume {
     padding: 1.5rem;
   }
 
+  .personal-info {
+    display: block;
+  }
+
   .photo {
     width: 45%;
   }
 }
```

### Comparing `wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/education_block.html` & `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html` & `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html` & `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% load wagtailcore_tags %}
 
 <h2 class="mt-4 mb-0">
-  {% if value.fa_icon %}<i class="{{ value.fa_icon }}"></i>{% endif %}
+  {% if value.fa_icon %}<i class="{{ value.fa_icon }} mr-2"></i>{% endif %}
   <span>{{ value.heading }}</span>
 </h2>
 <hr />
-{% for post in value.posts %}
-  <ul>
+<ul>
+  {% for post in value.posts %}
     <li>
       {% if post.block_type == "external_post" %}
-        <a href="{{ post.value.url }}">{{ post.value.title }}</a>
+        <a href="{{ post.value.url }}"><b>{{ post.value.title }}</b></a>
         <p class="date mt-1">{{ post.value.date }}</p>
       {% else %}
         {% with post.value.post as internal_post %}
-          <a href="{{ internal_post.url }}">{{ internal_post.title }}</a>
+          <a href="{{ internal_post.url }}"><b>{{ internal_post.title }}</b></a>
           <p class="date mt-1">{{ internal_post.first_published_at|date:"M. d, Y" }}</p>
         {% endwith %}
       {% endif %}
     </li>
-  </ul>
-{% endfor %}
+  {% endfor %}
+</ul>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load wagtailcore_tags %}
 {{%% iiff vvaalluuee..ffaa__iiccoonn %%}}{{%% eennddiiff %%}} {{{{ vvaalluuee..hheeaaddiinngg }}}}
 ===============================================================================
-{% for post in value.posts %}
-    * {% if post.block_type == "external_post" %} _{_{_ _p_o_s_t_._v_a_l_u_e_._t_i_t_l_e_ _}_}
+    * {% for post in value.posts %}
+    * {% if post.block_type == "external_post" %} _{{_{{_ _pp_oo_ss_tt_.._vv_aa_ll_uu_ee_.._tt_ii_tt_ll_ee_ _}}_}}
       {{ post.value.date }}
-      {% else %} {% with post.value.post as internal_post %} _{
-      _{_ _i_n_t_e_r_n_a_l___p_o_s_t_._t_i_t_l_e_ _}_}
+      {% else %} {% with post.value.post as internal_post %} _{{
+      _{{_ _ii_nn_tt_ee_rr_nn_aa_ll____pp_oo_ss_tt_.._tt_ii_tt_ll_ee_ _}}_}}
       {{ internal_post.first_published_at|date:"M. d, Y" }}
       {% endwith %} {% endif %}
-{% endfor %}
+    * {% endfor %}
```

### Comparing `wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/localization_dropdown.html` & `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/resume_page_body.html` & `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.2/wagtail_resume/templates/wagtail_resume/resume_page_head.html` & `wagtail_resume-2.8.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 {% load static %}
 {% load wagtailmetadata_tags %}
 {% load wagtail_resume_extras %}
 
 <head>
-  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.css" />
-  <link href="https://fonts.googleapis.com/css?family={% if page.font %}{{ page.font|title|space_to_plus }}|{% endif %}Roboto+Condensed&display=swap" rel="stylesheet">
-  <link rel="stylesheet" type="text/css" href="{% static 'wagtail_resume/css/resume_page.css' %}" />
-  <meta name="viewport" content="width=device-width, initial-scale=1">
-
+  <link rel="stylesheet"
+        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.css" />
+  <link href="https://fonts.googleapis.com/css?family={% if page.font %}{{ page.font|title|space_to_plus }}|{{ page.font|title|space_to_plus }}:bold,bolditalic:italic|{% endif %}Roboto|Roboto+Condensed:bold,bolditalic,italic&display=swap"
+        rel="stylesheet" />
+  <link rel="stylesheet"
+        type="text/css"
+        href="{% static 'wagtail_resume/css/resume_page.css' %}" />
+  <meta name="viewport" content="width=device-width, initial-scale=1" />
   {% meta_tags %}
 </head>
```

### Comparing `wagtail_resume-2.7.2/wagtail_resume/views.py` & `wagtail_resume-2.8.0/wagtail_resume/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,23 +45,32 @@
     if not authenticated and specific.pdf_generation_visibility == "authenticated":
         return HttpResponseForbidden(
             "<h1>You need to be authenticated to generate a resume PDF file.</h1>"
         )
 
     resume_url = specific.full_url
     name = slugify(specific.full_name)
-    date = datetime.datetime.now().strftime("%Y-%m-%d")
+    if resume.latest_revision_created_at:
+        resume_date = resume.latest_revision_created_at
+    else:
+        resume_date = datetime.datetime.now()
+    date = resume_date.strftime("%Y-%m-%d")
     font = specific.font
 
     response["Content-Disposition"] = f"inline; filename={name}-resume-{date}.pdf"
     if font:
         font = space_to_plus(font).title()
-        HTML(url=resume_url).write_pdf(
-            response,
-            stylesheets=[
-                # pylint: disable=line-too-long
-                f"https://fonts.googleapis.com/css2?family={font}&display=swap"
-            ],
-        )
+        full_font = f"{font}:bold|{font}:bold,bolditalic,italic"
     else:
-        HTML(url=resume_url).write_pdf(response)
+        full_font = "Roboto+Condensed|Roboto+Condensed:bold,bolditalic,italic"
+
+    print(full_font)
+    HTML(url=resume_url).write_pdf(
+        response,
+        stylesheets=[
+            # pylint: disable=line-too-long
+            # We use the default CSS API from Google Fonts to load the font
+            # CSS2 requires boldness specification for bold fonts
+            f"https://fonts.googleapis.com/css?family={full_font}&display=swap",
+        ],
+    )
     return response
```

### Comparing `wagtail_resume-2.7.2/PKG-INFO` & `wagtail_resume-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-resume
-Version: 2.7.2
+Version: 2.8.0
 Summary: A Wagtail project made to simplify creation of resumes for developers.
 Home-page: https://github.com/adinhodovic/wagtail-resume
 License: MIT
 Keywords: Resume,Django,Wagtail,CMS
 Author: Adin Hodovic
 Author-email: hodovicadin@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -21,19 +21,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2.0,<6.0.0)
 Requires-Dist: wagtail (>=4.0.0,<7.0.0)
-Requires-Dist: wagtail-markdown (>=0.10,<0.12)
+Requires-Dist: wagtail-markdown (>=0.10,<0.14)
 Requires-Dist: wagtail-metadata (>=4.0.0,<6.0.0)
-Requires-Dist: weasyprint (>=52,<53)
+Requires-Dist: weasyprint (>=59,<62)
 Project-URL: Documentation, https://github.com/adinhodovic/wagtail-resume
 Project-URL: Repository, https://github.com/adinhodovic/wagtail-resume
 Description-Content-Type: text/markdown
 
 # Wagtail resume
 
 ![Lint](https://github.com/adinhodovic/wagtail-resume/workflows/Test/badge.svg)
```

