# Comparing `tmp/django-imagefit-0.6.2.tar.gz` & `tmp/django-imagefit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-imagefit-0.6.2.tar", last modified: Thu Mar 22 19:25:30 2018, max compression
+gzip compressed data, was "django-imagefit-0.7.0.tar", last modified: Mon Jun  5 21:22:36 2023, max compression
```

## Comparing `django-imagefit-0.6.2.tar` & `django-imagefit-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/
-drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/
--rw-r--r--   0 vinyll     (501) staff       (20)     9632 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/PKG-INFO
--rw-r--r--   0 vinyll     (501) staff       (20)        1 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/not-zip-safe
--rw-r--r--   0 vinyll     (501) staff       (20)      430 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/SOURCES.txt
--rw-r--r--   0 vinyll     (501) staff       (20)       15 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/requires.txt
--rw-r--r--   0 vinyll     (501) staff       (20)        9 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/top_level.txt
--rw-r--r--   0 vinyll     (501) staff       (20)        1 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/django_imagefit.egg-info/dependency_links.txt
--rw-r--r--   0 vinyll     (501) staff       (20)     9632 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/PKG-INFO
--rw-r--r--   0 vinyll     (501) staff       (20)     1531 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/LICENSE
--rw-r--r--   0 vinyll     (501) staff       (20)       34 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/MANIFEST.in
--rw-r--r--   0 vinyll     (501) staff       (20)     6880 2018-03-20 05:44:35.000000 django-imagefit-0.6.2/README.md
--rw-r--r--   0 vinyll     (501) staff       (20)      931 2018-03-22 19:23:35.000000 django-imagefit-0.6.2/setup.py
-drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/imagefit/
-drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/imagefit/templatetags/
--rw-r--r--   0 vinyll     (501) staff       (20)      876 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/imagefit/templatetags/imagefit.py
--rw-r--r--   0 vinyll     (501) staff       (20)        0 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/imagefit/templatetags/__init__.py
--rw-r--r--   0 vinyll     (501) staff       (20)     3602 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/imagefit/models.py
--rw-r--r--   0 vinyll     (501) staff       (20)     1863 2018-03-22 17:34:51.000000 django-imagefit-0.6.2/imagefit/conf.py
--rw-r--r--   0 vinyll     (501) staff       (20)        0 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/imagefit/__init__.py
--rw-r--r--   0 vinyll     (501) staff       (20)      208 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/imagefit/urls.py
--rw-r--r--   0 vinyll     (501) staff       (20)     2261 2018-03-07 19:07:06.000000 django-imagefit-0.6.2/imagefit/views.py
--rw-r--r--   0 vinyll     (501) staff       (20)       59 2018-03-22 19:25:30.000000 django-imagefit-0.6.2/setup.cfg
+drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2023-06-05 21:22:36.437893 django-imagefit-0.7.0/
+-rw-r--r--   0 vinyll     (501) staff       (20)      528 2023-06-05 21:13:25.000000 django-imagefit-0.7.0/AUTHORS
+-rw-r--r--   0 vinyll     (501) staff       (20)     1531 2023-06-05 21:11:24.000000 django-imagefit-0.7.0/LICENSE
+-rw-r--r--   0 vinyll     (501) staff       (20)       34 2020-01-28 19:33:43.000000 django-imagefit-0.7.0/MANIFEST.in
+-rw-r--r--   0 vinyll     (501) staff       (20)     8103 2023-06-05 21:22:36.437767 django-imagefit-0.7.0/PKG-INFO
+-rw-r--r--   0 vinyll     (501) staff       (20)     7376 2023-06-05 21:10:22.000000 django-imagefit-0.7.0/README.md
+drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2023-06-05 21:22:36.436080 django-imagefit-0.7.0/django_imagefit.egg-info/
+-rw-r--r--   0 vinyll     (501) staff       (20)     8103 2023-06-05 21:22:36.000000 django-imagefit-0.7.0/django_imagefit.egg-info/PKG-INFO
+-rw-r--r--   0 vinyll     (501) staff       (20)      438 2023-06-05 21:22:36.000000 django-imagefit-0.7.0/django_imagefit.egg-info/SOURCES.txt
+-rw-r--r--   0 vinyll     (501) staff       (20)        1 2023-06-05 21:22:36.000000 django-imagefit-0.7.0/django_imagefit.egg-info/dependency_links.txt
+-rw-r--r--   0 vinyll     (501) staff       (20)        1 2023-06-05 21:22:36.000000 django-imagefit-0.7.0/django_imagefit.egg-info/not-zip-safe
+-rw-r--r--   0 vinyll     (501) staff       (20)       31 2023-06-05 21:22:36.000000 django-imagefit-0.7.0/django_imagefit.egg-info/requires.txt
+-rw-r--r--   0 vinyll     (501) staff       (20)        9 2023-06-05 21:22:36.000000 django-imagefit-0.7.0/django_imagefit.egg-info/top_level.txt
+drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2023-06-05 21:22:36.437219 django-imagefit-0.7.0/imagefit/
+-rw-r--r--   0 vinyll     (501) staff       (20)        0 2020-01-28 21:08:45.000000 django-imagefit-0.7.0/imagefit/__init__.py
+-rw-r--r--   0 vinyll     (501) staff       (20)     1883 2023-06-05 21:10:22.000000 django-imagefit-0.7.0/imagefit/conf.py
+-rw-r--r--   0 vinyll     (501) staff       (20)     3924 2023-06-05 21:10:22.000000 django-imagefit-0.7.0/imagefit/models.py
+drwxr-xr-x   0 vinyll     (501) staff       (20)        0 2023-06-05 21:22:36.437524 django-imagefit-0.7.0/imagefit/templatetags/
+-rw-r--r--   0 vinyll     (501) staff       (20)        0 2020-01-28 19:33:43.000000 django-imagefit-0.7.0/imagefit/templatetags/__init__.py
+-rw-r--r--   0 vinyll     (501) staff       (20)     1079 2023-06-05 21:10:22.000000 django-imagefit-0.7.0/imagefit/templatetags/imagefit.py
+-rw-r--r--   0 vinyll     (501) staff       (20)      504 2023-06-05 21:00:59.000000 django-imagefit-0.7.0/imagefit/urls.py
+-rw-r--r--   0 vinyll     (501) staff       (20)     2269 2023-06-05 21:10:22.000000 django-imagefit-0.7.0/imagefit/views.py
+-rw-r--r--   0 vinyll     (501) staff       (20)       38 2023-06-05 21:22:36.437935 django-imagefit-0.7.0/setup.cfg
+-rw-r--r--   0 vinyll     (501) staff       (20)      998 2023-06-05 21:22:19.000000 django-imagefit-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-imagefit-0.6.2/LICENSE` & `django-imagefit-0.7.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012-2017 Vincent Agnano.
+Copyright (c) 2012-2023 Vincent Agnano.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice,
        this list of conditions and the following disclaimer.
```

### Comparing `django-imagefit-0.6.2/README.md` & `django-imagefit-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+<p align="center"><img src="icons/logo.svg" alt="django-imagefit" height="200px"></p>
+
 # Django Image Fit - Resize an image on the fly
 
 [![Build Status](https://api.travis-ci.org/vinyll/django-imagefit.png)](http://travis-ci.org/vinyll/django-imagefit)
 
 Imagefit allows you to render an image in a template and specify its dimensions.
 It preserves the original image file.
 
 It is compatible with various sources of images such as django-filebrowser's
 FileBrowseField, user uploaded images, static images, …
 
-Works on Python 3.x and Python 2.6 or more; Django 1.4 > 2.0.
+Works on Python 3.x and Python 2.6 or more; Django 1.4 > 2.0. Compatible with Django 4.0
 
 
 #### Benefits
 
 * only 1 image file exists on the server, therefore it's always easy to replace
 and adapt the image per template or zone.
 * no model to adapt for large image and thumbnail that may vary when redesigning
@@ -33,20 +35,26 @@
 
 Example 2: render model's _news.image_ as a thumbnail:
 
 ```html
 {{ news.image|resize:"thumbnail" }}
 ```
 
-Example 1: render _/static/myimage.png_ image at a maximum cropped size of 150 x 150 px:
+Example 3: render _/static/myimage.png_ image at a maximum cropped size of 150 x 150 px:
 
 ```html
 {{ "/static/myimage.png"|resize:"150x150,C" }}
 ```
 
+Example 4: render _https://example.com/test.png_ image at a maximum cropped size of 150 x 150 px:
+
+```html
+{{ "https://example.com/test.png"|external_resize:"150x150,C" }}
+```
+
 #### What this is not
 
 * For creating specific model fields that resize image when model saves, see
 [django-imagekit](https://github.com/matthewwithanm/django-imagekit)
 * If you wish to avoid very large image on the server, consider resizing your original image
 before uploading it
 
@@ -106,14 +114,15 @@
 
 ```html
 {% load imagefit %}
 
 <img src="{{ "/static/image.png"|resize:'thumbnail' }}" />
 <img src="{{ "/static/image.png"|resize:'320x240' }}" />
 <img src="{{ "/static/image.png"|resize:'320x240,C' }}" />
+<img src="{{ "https://example.com/test.png"|external_resize:'320x240' }}" />
 ```
 
 This will display your _/static/image.png_:
 
 1. in the _thumbnail_ format (80 x 80 px)
 2. resized in a custom 320 x 240 pixels
 3. resized and cropped in a custom 320 x 240 pixels
@@ -140,20 +149,22 @@
 _/PATH/TO/YOUR/PROJECT/**public/static/image.png**_
 
 #### Templatetags
 
     resize(value, size)  # path is relative to you settings.IMAGE_ROOT
     static_resize(value, size)  # path is relative to you settings.STATIC_ROOT
     media_resize(value, size)  # path is relative to you settings.MEDIA_ROOT
+    external_resize(value, size) # path is an http/https url
 
 Can be used in templates as so :
 
     {{ "/static/logo.png"|resize:'320x240' }}
     {{ "logo.png"|static_resize:'320x240' }}
     {{ "user_avatar.png"|media_resize:'320x240' }}
+    {{ "https://example.com/test.png"|external_resize:'320x240' }}
 
 
 #### Presets
 
 Presets are configuration names that hold width and height (and maybe more later on).
 Imagefit is already shipped with 3 presets : _thumbnail_ (80x80), _medium_ (320x240)
 and _original_ (no resizing).
```

### Comparing `django-imagefit-0.6.2/setup.py` & `django-imagefit-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='django-imagefit',
-    version='0.6.2',
+    version='0.7.0',
+    long_description_content_type='text/markdown',
     description='Render an optimized version of your original image on display. Ability to resize and crop.',
     long_description=open('README.md').read(),
     author='Vincent Agnano',
-    author_email='vincent.agnano@scopyleft.fr',
+    author_email='vinyll@protonmail.com',
     url='http://github.com/vinyll/django-imagefit',
     license='BSD',
     packages=find_packages(),
     zip_safe=False,
-    install_requires=['django-appconf'],
+    install_requires=['django-appconf', 'Pillow', 'requests'],
     include_package_data=True,
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `django-imagefit-0.6.2/imagefit/templatetags/imagefit.py` & `django-imagefit-0.7.0/imagefit/templatetags/imagefit.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,7 +30,15 @@
 @register.filter
 def static_resize(value, size):
     """
     Generates the url for the resized image prefixing with STATIC_ROOT
     return string url
     """
     return resize(value, size, 'static_resize')
+
+@register.filter
+def external_resize(value, size):
+    """
+    Generates the url for the resized image for external image
+    return string url
+    """
+    return resize(value, size, 'external_resize')
```

### Comparing `django-imagefit-0.6.2/imagefit/models.py` & `django-imagefit-0.7.0/imagefit/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import division
 from imagefit.conf import ext_to_format, settings
 from PIL import Image as PilImage
 
 import mimetypes
+import time
+import requests
+
 try:
     import BytesIO
 except ImportError:
     from io import BytesIO
 import re
 import os
 
@@ -14,28 +17,35 @@
 class Image(object):
     """
     Represents an Image file on the system.
     """
 
     def __init__(self, path, cache=None, cached_name=None, *args, **kwargs):
         self.path = path
-        self.pil = PilImage.open(path)
+        self.is_external = path.startswith(('http://', 'https://'))
+        if self.is_external:
+            response = requests.get(path)
+            self.pil = PilImage.open(BytesIO(response.content))
+        else:
+            self.pil = PilImage.open(path)
         self.cache = cache
         self.cached_name = cached_name
 
         # force RGB
         if self.pil.mode not in ('L', 'RGB', 'LA', 'RGBA'):
             self.pil = self.pil.convert('RGB')
 
     @property
     def mimetype(self):
         return mimetypes.guess_type(self.path)[0]
 
     @property
     def modified(self):
+        if self.is_external:
+            return int(round(time.time()))
         return os.path.getmtime(self.path)
 
     @property
     def is_cached(self):
         return self.cache and self.cached_name in self.cache
 
     def resize(self, width=None, height=None):
```

### Comparing `django-imagefit-0.6.2/imagefit/conf.py` & `django-imagefit-0.7.0/imagefit/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.conf import settings
 from appconf import AppConf
 
 import tempfile
 import os
-
+settings.configure()
 
 class ImagefitConf(AppConf):
 
     #: dictionary of preset names that have width and height values
     IMAGEFIT_PRESETS = {
         'thumbnail': {'width': 80, 'height': 80, 'crop': True},
         'medium': {'width': 320, 'height': 240},
```

### Comparing `django-imagefit-0.6.2/imagefit/views.py` & `django-imagefit-0.7.0/imagefit/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 from imagefit.conf import settings
 from imagefit.models import Image, Presets
 
 import os
 import stat
 import time
 
-
 cache = caches[settings.IMAGEFIT_CACHE_BACKEND_NAME]
 
 
 def _image_response(image):
     response = HttpResponse(
         image.render(),
         image.mimetype
     )
     response['Last-Modified'] = http_date(image.modified)
-    expire_time = getattr(settings, 'IMAGEFIT_EXPIRE_HEADER', 3600*24*30)
+    expire_time = getattr(settings, 'IMAGEFIT_EXPIRE_HEADER', 3600 * 24 * 30)
     response['Expires'] = http_date(time.time() + expire_time)
     return response
 
 
 def resize(request, path_name, format, url):
     if path_name == 'static_resize':
         prefix = settings.STATIC_ROOT
@@ -33,36 +32,38 @@
         prefix = settings.MEDIA_ROOT
     else:
         prefix = settings.IMAGEFIT_ROOT
     # remove prepending slash
     if url[0] == '/':
         url = url[1:]
     # generate Image instance
-    image = Image(path=os.path.join(prefix, url))
-    if not os.path.exists(image.path):
+    path = os.path.join(prefix, url)
+    if not os.path.exists(path):
         return HttpResponse(status=404)
+    image = Image(path=path)
 
     statobj = os.stat(image.path)
     if not was_modified_since(request.META.get('HTTP_IF_MODIFIED_SINCE'),
                               statobj[stat.ST_MTIME], statobj[stat.ST_SIZE]):
         return HttpResponseNotModified(content_type=image.mimetype)
 
+    image.cached_name = request.META.get('PATH_INFO')
+
     if settings.IMAGEFIT_CACHE_ENABLED:
         image.cache = cache
-        image.cached_name = request.META.get('PATH_INFO')
         # shortcut everything, render cached version
         if image.is_cached:
             return _image_response(image)
 
     # retrieve preset from format argument
     preset = Presets.get(format) or Presets.from_string(format)
     if not preset:
         raise ImproperlyConfigured(
-            " \"%s\" is neither a \"WIDTHxHEIGHT\" format nor a key in " +
-            "IMAGEFIT_PRESETS." % format
+            f" \"{format}\" is neither a \"WIDTHxHEIGHT\" format nor a key in " +
+            "IMAGEFIT_PRESETS."
         )
 
     # Resize and cache image
     if preset.get('crop'):
         image.crop(preset.get('width'), preset.get('height'))
     else:
         image.resize(preset.get('width'), preset.get('height'))
```

