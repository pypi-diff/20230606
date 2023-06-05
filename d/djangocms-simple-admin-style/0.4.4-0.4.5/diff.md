# Comparing `tmp/djangocms-simple-admin-style-0.4.4.tar.gz` & `tmp/djangocms-simple-admin-style-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-simple-admin-style-0.4.4.tar", last modified: Fri May 26 12:33:35 2023, max compression
+gzip compressed data, was "djangocms-simple-admin-style-0.4.5.tar", last modified: Mon Jun  5 22:39:56 2023, max compression
```

## Comparing `djangocms-simple-admin-style-0.4.4.tar` & `djangocms-simple-admin-style-0.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/templates/admin/inc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/templates/admin/inc/extrastyle.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-26 12:33:35.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-26 12:33:35.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:33:35.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:33:35.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 12:33:35.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 12:33:35.000000 djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-26 12:33:35.732013 djangocms-simple-admin-style-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-26 12:33:25.000000 djangocms-simple-admin-style-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.369207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.369207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     8271 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.369207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/templates/admin/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/templates/admin/inc/extrastyle.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-06-05 22:39:56.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-05 22:39:56.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:39:56.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 22:39:56.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 22:39:56.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-05 22:39:56.000000 djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-05 22:39:56.373207 djangocms-simple-admin-style-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-05 22:39:47.000000 djangocms-simple-admin-style-0.4.5/setup.py
```

### Comparing `djangocms-simple-admin-style-0.4.4/LICENSE` & `djangocms-simple-admin-style-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.4.4/PKG-INFO` & `djangocms-simple-admin-style-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.4.4
+Version: 0.4.5
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-simple-admin-style-0.4.4/README.rst` & `djangocms-simple-admin-style-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css` & `djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css`

 * *Files 5% similar despite different names*

```diff
@@ -1 +1 @@
-:root,body{--font-family-primary:Helvetica,Arial,sans-serif;--primary:var(--dca-primary);--secondary:var(--dca-white);--accent:var(--primary);--primary-fg:var(--dca-white);--body-fg:var(--dca-gray-darkest);--body-bg:var(--dca-white);--header-color:var(--dca-black);--header-branding-color:var(--accent);--header-bg:var(--secondary);--header-link-color:var(--body-fg);--breadcrumbs-fg:var(--dca-gray);--breadcrumbs-link-fg:var(--dca-primary);--breadcrumbs-bg:var(--dca-gray-lightest);--link-fg:var(--dca-primary);--darkened-bg:var(--dca-gray-lightest);--button-fg:var(--dca-gray-darker);--button-bg:var(--dca-white);--button-hover-bg:var(--dca-gray-lighter);--default-button-fg:var(--dca-white);--default-button-bg:var(--dca-primary);--object-tools-fg:var(--body-fg);--object-tools-bg:vaR(--dca-white);--object-tools-hover-bg:var(--dca-gray-lighter)}:root[data-color-scheme=light],:root[data-theme=light],html,html[data-color-scheme=light],html[data-theme=light],root{--dca-light-mode:1;--dca-dark-mode:0;--dca-white:#fff;--dca-black:#000;--dca-primary:#0bf;--dca-gray:#666;--dca-gray-lightest:#f2f2f2;--dca-gray-lighter:#ddd;--dca-gray-light:#999;--dca-gray-darker:#454545;--dca-gray-darkest:#333;--dca-gray-super-lightest:#f7f7f7;color-scheme:light}@media (prefers-color-scheme:dark){:root{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}}:root[data-theme=dark],html[data-color-scheme=dark],html[data-theme=dark],root[data-color-scheme=dark]{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}.dashboard #content{width:calc(100% - 340px)}h1{font-size:1.4rem}h2{font-size:1.25rem}h3{font-size:1rem}.inline-group h2,.module caption,h4,td,th{font-size:.875rem}.help,.small,div.help,div.help li,form div.help,form p.help,h5,p.help{font-size:.75rem}.mini{font-size:.6815rem}dd,dt,li{font-size:.875rem;line-height:1.4rem}.inline-group h2,.module caption,.module h2{background:var(--body-bg);color:var(--body-fg)}#nav-sidebar .module caption{background:var(--primary)}#nav-sidebar .current-app .section:link,#nav-sidebar .current-app .section:visited,#nav-sidebar .section:link,#nav-sidebar .section:visited{color:var(--dca-white)}#nav-sidebar a{color:var(--body-fg)}.submit-row{background:var(--dca-white,#fff)}.button.default,.submit-row a.deletelink,.submit-row input.default,input[type=submit].default{color:var(--dca-white,#fff)}.object-tools a{border:1px solid var(--dca-gray-lighter);border-radius:3px}.object-tools a.addlink{background-color:var(--default-button-bg);border-color:var(--default-button-fg);color:var(--default-button-fg)}.object-tools a.addlink:focus,.object-tools a.addlink:hover{background-color:var(--default-button-hover-bg)}th{font-weight:400}.inline-group h2,.module caption,.module h2{font-weight:600}.aligned label:not(.btn){color:var(--body-fg);float:unset;font-weight:600;width:unset}.aligned label.btn{display:inline-block}#user-tools #logout-form button,#user-tools a:link,#user-tools a:visited{color:var(--primary)}#logout-form button:active,#logout-form button:hover{margin-bottom:2px;padding-bottom:1px}.aligned .fieldBox>label:first-child,.flex-container,.form-row>div>label{display:block}.required label:not(.vCheckboxLabel):after,label.required:not(.vCheckboxLabel):after{color:var(--delete-button-bg);content:"*"}form .aligned div.help,form .aligned p.help{margin-left:0;padding-left:0}form button{background-color:var(--default-button-bg);border:1px solid var(--default-button-bg);border-radius:3px;color:var(--default-button-fg);font-family:var(--font-family-primary);font-size:.8125rem;font-weight:400;margin:2px 0;padding:5px 6px;vertical-align:middle}.aligned label+div.help,.aligned label+div.readonly,.aligned label+p,form .aligned input+div.help,form .aligned input+p.help,form .aligned select+div.help,form .aligned select+p.help,form .aligned textarea+div.help,form .aligned textarea+p.help,form .aligned ul{margin-left:0;padding-left:0}.button,.submit-row input,a.button,input[type=button],input[type=submit]{border:1px solid var(--dca-gray-lighter,#ddd);font-size:14px}a.btn{border:1px solid var(--dca-gray-lighter,#ddd);color:var(--body-fg)}.colM .aligned .vLargeTextField,.colM .aligned .vXMLLargeTextField,.vLargeTextField,.vTextField,.vURLField,.vUUIDField,.vXMLLargeTextField,input[type=email],input[type=text],input[type=url],textarea{width:calc(100% - 10px)}#changelist-search input[type=text]{width:unset}.form-row p,form .button,input,select,textarea{font-family:unset}div.form-row{display:flex;flex-wrap:wrap}.form-row>div{flex:1 0 0;width:100%}.form-row>ul.errorlist{width:100%}fieldset.collapse.collapsed .form-row{display:none}.related-widget-wrapper{width:100%}.select2-container,select{width:calc(100% - 92px)}.select2{width:calc(100% - 92px)!important}select[multiple]{min-width:200px}.related-widget-wrappxer select{width:calc(100% - 92px)}.colMS .aligned .vLargeTextField,.colMS .aligned .vXMLLargeTextField{width:unset}@media (max-width:1024px){.djangocms-simple-admin-style fieldset .fieldBox+.fieldBox{border-top:unset;margin-top:0;padding-top:0}}body.cms-admin a.skip-to-content-link,body.cms-admin-modal #header,body.cms-admin-sideframe #header{display:none}body.cms-admin-sideframe #container{padding-top:46px}body.cms-admin-sideframe #content>h1{display:none}body.cms-admin-sideframe .object-tools{margin-right:92px}body.cms-admin-modal #content>h2,body.cms-admin-modal #nav-sidebar,body.cms-admin-modal #toggle-nav-sidebar,body.cms-admin-modal .breadcrumbs,body.cms-admin-modal .hide-in-modal{display:none}body.cms-admin-modal .main.shifted>#nav-sidebar+.content,body.cms-admin-modal .main>#nav-sidebar+.content{max-width:100%}.main.shifted>#nav-sidebar+.content{max-width:calc(100% - 299px)}body.cms-admin-sideframe.djangocms-simple-admin-style{margin-top:0}.djangocms-simple-admin-style .parler-language-tabs span.current{background-color:var(--primary);border-color:var(--primary);color:var(--dca-white)}.djangocms-simple-admin-style .parler-language-tabs span.available,.djangocms-simple-admin-style .parler-language-tabs span.current,.djangocms-simple-admin-style .parler-language-tabs span.empty{border-radius:3px 3px 0 0}.djangocms-simple-admin-style .parler-language-tabs{border-bottom-color:var(--primary)}.parler-language-tabs a:link,.parler-language-tabs a:visited{color:var(--body-fg)}#page_form_lang_tabs{border-bottom:2px solid var(--primary)}#page_form_lang_tabs input[type=button]{border-bottom:none;border-radius:3px 3px 0 0;margin-bottom:0;padding:5px 15px}.djangocms-simple-admin-style #page_form_lang_tabs input[type=button].language_button.selected{background-color:var(--default-button-bg);border-color:var(--default-button-bg);color:var(--default-button-fg)}.cms-btn-group{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:0;line-height:15px;margin-left:-5px;margin-right:0;padding:10px 15px}.cms-btn,.cms-btn-group{background:var(--button-bg);color:var(--button-fg);display:inline-block}.cms-btn{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:4px;margin-left:5px}a.cms-btn-group,a.cms-btn-group:hover,a.cms-btn-group:link{color:var(--button-fg)}.cms-btn-group:first-child{border-bottom-left-radius:4px;border-top-left-radius:4px;margin-left:5px}.cms-btn-group:last-child{border-bottom-right-radius:4px;border-top-right-radius:4px}.cms-btn-active{background-color:var(--dca-gray-lighter)}.delete-confirmation form .cancel-link,.delete-confirmation form input[type=submit]{color:var(--dca-white)}.cms-admin-modal.delete-confirmation .cancel-link,.cms_modal-window.delete-confirmation .cancel-link,.popup.delete-confirmation .cancel-link{display:none}
+:root,body{--font-family-primary:Helvetica,Arial,sans-serif;--primary:var(--dca-primary);--secondary:var(--dca-white);--accent:var(--primary);--primary-fg:var(--dca-white);--body-fg:var(--dca-gray-darkest);--body-bg:var(--dca-white);--header-color:var(--dca-black);--header-branding-color:var(--accent);--header-bg:var(--secondary);--header-link-color:var(--dca-primary);--breadcrumbs-fg:var(--dca-gray);--breadcrumbs-link-fg:var(--dca-primary);--breadcrumbs-bg:var(--dca-gray-lightest);--link-fg:var(--dca-primary);--darkened-bg:var(--dca-gray-lightest);--button-fg:var(--dca-gray-darker);--button-bg:var(--dca-white);--button-hover-bg:var(--dca-gray-lighter);--default-button-fg:var(--dca-white);--default-button-bg:var(--dca-primary);--object-tools-fg:var(--body-fg);--object-tools-bg:vaR(--dca-white);--object-tools-hover-bg:var(--dca-gray-lighter)}:root[data-color-scheme=light],:root[data-theme=light],html,html[data-color-scheme=light],html[data-theme=light],root{--dca-light-mode:1;--dca-dark-mode:0;--dca-white:#fff;--dca-black:#000;--dca-primary:#0bf;--dca-gray:#666;--dca-gray-lightest:#f2f2f2;--dca-gray-lighter:#ddd;--dca-gray-light:#999;--dca-gray-darker:#454545;--dca-gray-darkest:#333;--dca-gray-super-lightest:#f7f7f7;color-scheme:light}@media (prefers-color-scheme:dark){:root{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}}:root[data-theme=dark],html[data-color-scheme=dark],html[data-theme=dark],root[data-color-scheme=dark]{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}.dashboard #content{width:calc(100% - 340px)}h1{font-size:1.4rem}h2{font-size:1.25rem}h3{font-size:1rem}.inline-group h2,.module caption,h4,td,th{font-size:.875rem}.help,.small,div.help,div.help li,form div.help,form p.help,h5,p.help{font-size:.75rem}.mini{font-size:.6815rem}dd,dt,li{font-size:.875rem;line-height:1.4rem}.inline-group h2,.module caption,.module h2{background:var(--body-bg);color:var(--body-fg)}#nav-sidebar .module caption{background:var(--primary)}#nav-sidebar .current-app .section:link,#nav-sidebar .current-app .section:visited,#nav-sidebar .section:link,#nav-sidebar .section:visited{color:var(--dca-white)}#nav-sidebar a{color:var(--body-fg)}.submit-row{background:var(--dca-white,#fff)}.button.default,.submit-row a.deletelink,.submit-row input.default,input[type=submit].default{color:var(--dca-white,#fff)}.object-tools a{border:1px solid var(--dca-gray-lighter);border-radius:3px}.object-tools a.addlink{background-color:var(--default-button-bg);border-color:var(--default-button-fg);color:var(--default-button-fg)}.object-tools a.addlink:focus,.object-tools a.addlink:hover{background-color:var(--default-button-hover-bg)}th{font-weight:400}.inline-group h2,.module caption,.module h2{font-weight:600}.aligned label:not(.btn){color:var(--body-fg);float:unset;font-weight:600;width:unset}.aligned label.btn{display:inline-block}#user-tools #logout-form button,#user-tools a:link,#user-tools a:visited{color:var(--primary)}#logout-form button:active,#logout-form button:hover{margin-bottom:2px;padding-bottom:1px}.aligned .fieldBox>label:first-child,.flex-container,.form-row>div>label{display:block}.required label:not(.vCheckboxLabel):after,label.required:not(.vCheckboxLabel):after{color:var(--delete-button-bg);content:"*"}form .aligned div.help,form .aligned p.help{margin-left:0;padding-left:0}form button{background-color:var(--default-button-bg);border:1px solid var(--default-button-bg);border-radius:3px;color:var(--default-button-fg);font-family:var(--font-family-primary);font-size:.8125rem;font-weight:400;margin:2px 0;padding:5px 6px;vertical-align:middle}.aligned label+div.help,.aligned label+div.readonly,.aligned label+p,form .aligned input+div.help,form .aligned input+p.help,form .aligned select+div.help,form .aligned select+p.help,form .aligned textarea+div.help,form .aligned textarea+p.help,form .aligned ul{margin-left:0;padding-left:0}.button,.submit-row input,a.button,input[type=button],input[type=submit]{border:1px solid var(--dca-gray-lighter,#ddd);font-size:14px}a.cms-action-btn{border:1px solid var(--dca-gray-lighter,#ddd);color:var(--body-fg)}.colM .aligned .vLargeTextField,.colM .aligned .vXMLLargeTextField,.vLargeTextField,.vTextField,.vURLField,.vUUIDField,.vXMLLargeTextField,input[type=email],input[type=text],input[type=url],textarea{width:calc(100% - 10px)}#changelist-search input[type=text]{width:unset}.form-row p,form .button,input,select,textarea{font-family:unset}div.form-row:not([hidden]){display:flex;flex-wrap:wrap;overflow:unset;padding-left:0;padding-right:0}.auth-user.change-form div.form-row:not([hidden]){display:block}div.form-row>div:not(.help){flex:1 0 0;width:100%}.form-row>ul.errorlist{width:100%}fieldset.collapse.collapsed .form-row{display:none}.related-widget-wrapper{width:100%}.select2-container,select{width:calc(100% - 92px)}.select2{width:calc(100% - 92px)!important}select[multiple]{min-width:200px}.related-widget-wrappxer select{width:calc(100% - 92px)}.colMS .aligned .vLargeTextField,.colMS .aligned .vXMLLargeTextField{width:unset}@media (max-width:1024px){.djangocms-simple-admin-style fieldset .fieldBox+.fieldBox{border-top:unset;margin-top:0;padding-top:0}}body.cms-admin a.skip-to-content-link,body.cms-admin-modal #header,body.cms-admin-sideframe #header{display:none}body.cms-admin-sideframe #container{padding-top:46px}body.cms-admin-sideframe #content>h1{display:none}body.cms-admin-sideframe .object-tools{margin-right:92px}body.cms-admin-modal #content>h2,body.cms-admin-modal #nav-sidebar,body.cms-admin-modal #toggle-nav-sidebar,body.cms-admin-modal .breadcrumbs,body.cms-admin-modal .hide-in-modal{display:none}body.cms-admin-modal .main.shifted>#nav-sidebar+.content,body.cms-admin-modal .main>#nav-sidebar+.content{max-width:100%}.main.shifted>#nav-sidebar+.content{max-width:calc(100% - 299px)}body.cms-admin-sideframe.djangocms-simple-admin-style{margin-top:0}.djangocms-simple-admin-style .parler-language-tabs span.current{background-color:var(--primary);border-color:var(--primary);color:var(--dca-white)}.djangocms-simple-admin-style .parler-language-tabs span.available,.djangocms-simple-admin-style .parler-language-tabs span.current,.djangocms-simple-admin-style .parler-language-tabs span.empty{border-radius:3px 3px 0 0}.djangocms-simple-admin-style .parler-language-tabs{border-bottom-color:var(--primary)}.parler-language-tabs a:link,.parler-language-tabs a:visited{color:var(--body-fg)}#page_form_lang_tabs{border-bottom:2px solid var(--primary)}#page_form_lang_tabs input[type=button]{border-bottom:none;border-radius:3px 3px 0 0;margin-bottom:0;padding:5px 15px}.djangocms-simple-admin-style #page_form_lang_tabs input[type=button].language_button.selected{background-color:var(--default-button-bg);border-color:var(--default-button-bg);color:var(--default-button-fg)}.cms-btn-group{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:0;line-height:15px;margin-left:-5px;margin-right:0;padding:10px 15px}.cms-btn,.cms-btn-group{background:var(--button-bg);color:var(--button-fg);display:inline-block}.cms-btn{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:4px;margin-left:5px}a.cms-btn-group,a.cms-btn-group:hover,a.cms-btn-group:link{color:var(--button-fg)}.cms-btn-group:first-child{border-bottom-left-radius:4px;border-top-left-radius:4px;margin-left:5px}.cms-btn-group:last-child{border-bottom-right-radius:4px;border-top-right-radius:4px}.cms-btn-active{background-color:var(--dca-gray-lighter)}.delete-confirmation form .cancel-link,.delete-confirmation form input[type=submit]{color:var(--dca-white)}.cms-admin-modal.delete-confirmation .cancel-link,.cms_modal-window.delete-confirmation .cancel-link,.popup.delete-confirmation .cancel-link{display:none}
```

### Comparing `djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style/templates/admin/base_site.html` & `djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/PKG-INFO` & `djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.4.4
+Version: 0.4.5
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-simple-admin-style-0.4.4/djangocms_simple_admin_style.egg-info/SOURCES.txt` & `djangocms-simple-admin-style-0.4.5/djangocms_simple_admin_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.4.4/setup.cfg` & `djangocms-simple-admin-style-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.4.4/setup.py` & `djangocms-simple-admin-style-0.4.5/setup.py`

 * *Files identical despite different names*

