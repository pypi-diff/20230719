# Comparing `tmp/django-mp-shop-offers-2.0.tar.gz` & `tmp/django-mp-shop-offers-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mp-shop-offers-2.0.tar", last modified: Tue Sep 13 06:10:22 2022, max compression
+gzip compressed data, was "django-mp-shop-offers-2.0.1.tar", last modified: Wed Jul 19 11:01:46 2023, max compression
```

## Comparing `django-mp-shop-offers-2.0.tar` & `django-mp-shop-offers-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      175 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      350 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      659 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/django_mp_shop_offers.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      350 2022-09-13 06:10:22.000000 django-mp-shop-offers-2.0/django_mp_shop_offers.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      858 2022-09-13 06:10:22.000000 django-mp-shop-offers-2.0/django_mp_shop_offers.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2022-09-13 06:10:22.000000 django-mp-shop-offers-2.0/django_mp_shop_offers.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        7 2022-09-13 06:10:22.000000 django-mp-shop-offers-2.0/django_mp_shop_offers.egg-info/top_level.txt
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/
--rw-rw-r--   0 dev       (1000) dev       (1000)      226 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0/offers/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      752 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0/offers/admin.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      300 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/forms.py
--rw-rw-r--   0 dev       (1000) dev       (1000)      782 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0/offers/lib.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/en/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/en/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)      337 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     2453 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/ru/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2239 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     3453 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/uk/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/locale/uk/LC_MESSAGES/
--rw-rw-r--   0 dev       (1000) dev       (1000)     2111 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/locale/uk/LC_MESSAGES/django.mo
--rw-rw-r--   0 dev       (1000) dev       (1000)     3322 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/locale/uk/LC_MESSAGES/django.po
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/migrations/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1785 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/migrations/0001_initial.py
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/migrations/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1578 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0/offers/models.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/static/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/static/offers/
--rw-rw-r--   0 dev       (1000) dev       (1000)     1128 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/static/offers/offers.js
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/templates/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/templates/offers/
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/offers/templates/offers/notifications/
--rw-rw-r--   0 dev       (1000) dev       (1000)      739 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/templates/offers/notifications/email.html
--rw-rw-r--   0 dev       (1000) dev       (1000)       86 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/templates/offers/notifications/sms.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)     1198 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/templates/offers/price_offer_form.html
--rw-rw-r--   0 dev       (1000) dev       (1000)     1263 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/templates/offers/price_offer_modal.html
--rw-rw-r--   0 dev       (1000) dev       (1000)      254 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0/offers/urls.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     1713 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0/offers/views.py
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2022-09-13 06:10:22.449853 django-mp-shop-offers-2.0/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      447 2022-09-13 06:09:46.000000 django-mp-shop-offers-2.0/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      175 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      354 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      659 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/django_mp_shop_offers.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      354 2023-07-19 11:01:46.000000 django-mp-shop-offers-2.0.1/django_mp_shop_offers.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      816 2023-07-19 11:01:46.000000 django-mp-shop-offers-2.0.1/django_mp_shop_offers.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-07-19 11:01:46.000000 django-mp-shop-offers-2.0.1/django_mp_shop_offers.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        7 2023-07-19 11:01:46.000000 django-mp-shop-offers-2.0.1/django_mp_shop_offers.egg-info/top_level.txt
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      226 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0.1/offers/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      752 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0.1/offers/admin.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      595 2023-03-04 07:30:55.000000 django-mp-shop-offers-2.0.1/offers/forms.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)      782 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0.1/offers/lib.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/locale/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/locale/ru/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2362 2023-07-19 11:01:04.000000 django-mp-shop-offers-2.0.1/offers/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3383 2023-07-19 11:01:02.000000 django-mp-shop-offers-2.0.1/offers/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/locale/uk/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/locale/uk/LC_MESSAGES/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     2232 2023-07-19 11:01:04.000000 django-mp-shop-offers-2.0.1/offers/locale/uk/LC_MESSAGES/django.mo
+-rw-rw-r--   0 dev       (1000) dev       (1000)     3250 2023-07-19 11:00:36.000000 django-mp-shop-offers-2.0.1/offers/locale/uk/LC_MESSAGES/django.po
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/migrations/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1785 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/migrations/0001_initial.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/migrations/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1578 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0.1/offers/models.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/static/
+-rw-rw-r--   0 dev       (1000) dev       (1000)    10301 2021-07-06 15:36:05.000000 django-mp-shop-offers-2.0.1/offers/static/jquery.maskedinput.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/static/offers/
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1128 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/static/offers/offers.js
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/templates/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/templates/offers/
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/offers/templates/offers/notifications/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      739 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/templates/offers/notifications/email.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)       86 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/templates/offers/notifications/sms.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1339 2023-03-04 07:30:00.000000 django-mp-shop-offers-2.0.1/offers/templates/offers/price_offer_form.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1263 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/templates/offers/price_offer_modal.html
+-rw-rw-r--   0 dev       (1000) dev       (1000)      254 2022-09-13 06:06:43.000000 django-mp-shop-offers-2.0.1/offers/urls.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)     1713 2022-09-13 06:07:37.000000 django-mp-shop-offers-2.0.1/offers/views.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-07-19 11:01:46.984046 django-mp-shop-offers-2.0.1/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      449 2023-07-19 11:01:28.000000 django-mp-shop-offers-2.0.1/setup.py
```

### Comparing `django-mp-shop-offers-2.0/LICENSE` & `django-mp-shop-offers-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/README.md` & `django-mp-shop-offers-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/django_mp_shop_offers.egg-info/SOURCES.txt` & `django-mp-shop-offers-2.0.1/django_mp_shop_offers.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 offers/__init__.py
 offers/admin.py
 offers/forms.py
 offers/lib.py
 offers/models.py
 offers/urls.py
 offers/views.py
-offers/locale/en/LC_MESSAGES/django.mo
-offers/locale/en/LC_MESSAGES/django.po
 offers/locale/ru/LC_MESSAGES/django.mo
 offers/locale/ru/LC_MESSAGES/django.po
 offers/locale/uk/LC_MESSAGES/django.mo
 offers/locale/uk/LC_MESSAGES/django.po
 offers/migrations/0001_initial.py
 offers/migrations/__init__.py
+offers/static/jquery.maskedinput.js
 offers/static/offers/offers.js
 offers/templates/offers/price_offer_form.html
 offers/templates/offers/price_offer_modal.html
 offers/templates/offers/notifications/email.html
 offers/templates/offers/notifications/sms.txt
```

### Comparing `django-mp-shop-offers-2.0/offers/admin.py` & `django-mp-shop-offers-2.0.1/offers/admin.py`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/lib.py` & `django-mp-shop-offers-2.0.1/offers/lib.py`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/locale/ru/LC_MESSAGES/django.mo` & `django-mp-shop-offers-2.0.1/offers/locale/ru/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -51,14 +51,17 @@
 
 msgid "Offer successfully sent"
 msgstr "Предложение успешно отправлено"
 
 msgid "Offers"
 msgstr "Ценовые предложения"
 
+msgid "Phone number could not start with `+3800`"
+msgstr "Телефон не может начинаться на `+3800`"
+
 msgid "Processing"
 msgstr "В обработке"
 
 msgid "Product"
 msgstr "Товар"
 
 msgid "Product price offer"
```

### Comparing `django-mp-shop-offers-2.0/offers/locale/uk/LC_MESSAGES/django.mo` & `django-mp-shop-offers-2.0.1/offers/locale/uk/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -50,14 +50,17 @@
 
 msgid "Offer successfully sent"
 msgstr "Пропозиція успішно надіслана"
 
 msgid "Offers"
 msgstr "Цінові пропозиції"
 
+msgid "Phone number could not start with `+3800`"
+msgstr "Телефон не може починатись на `+3800`"
+
 msgid "Processing"
 msgstr "В обробці"
 
 msgid "Product"
 msgstr "Товар"
 
 msgid "Product price offer"
```

### Comparing `django-mp-shop-offers-2.0/offers/migrations/0001_initial.py` & `django-mp-shop-offers-2.0.1/offers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/models.py` & `django-mp-shop-offers-2.0.1/offers/models.py`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/static/offers/offers.js` & `django-mp-shop-offers-2.0.1/offers/static/offers/offers.js`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/templates/offers/notifications/email.html` & `django-mp-shop-offers-2.0.1/offers/templates/offers/notifications/email.html`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/templates/offers/price_offer_form.html` & `django-mp-shop-offers-2.0.1/offers/templates/offers/price_offer_form.html`

 * *Files 16% similar despite different names*

```diff
@@ -68,8 +68,17 @@
 00000430: 0a20 2020 207b 7b20 666f 726d 2e63 6170  .    {{ form.cap
 00000440: 7463 6861 2e6c 6162 656c 5f74 6167 207d  tcha.label_tag }
 00000450: 7d20 2a0a 2020 2020 7b7b 2066 6f72 6d2e  } *.    {{ form.
 00000460: 6361 7074 6368 6120 7d7d 0a20 2020 203c  captcha }}.    <
 00000470: 6469 7620 636c 6173 733d 2268 656c 702d  div class="help-
 00000480: 626c 6f63 6b22 3e7b 7b20 666f 726d 2e63  block">{{ form.c
 00000490: 6170 7463 6861 2e65 7272 6f72 7320 7d7d  aptcha.errors }}
-000004a0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a       </div>.</div>.
+000004a0: 3c2f 6469 763e 0a3c 2f64 6976 3e0a 0a3c  </div>.</div>..<
+000004b0: 7363 7269 7074 2073 7263 3d22 7b7b 2053  script src="{{ S
+000004c0: 5441 5449 435f 5552 4c20 7d7d 6a71 7565  TATIC_URL }}jque
+000004d0: 7279 2e6d 6173 6b65 6469 6e70 7574 2e6a  ry.maskedinput.j
+000004e0: 7322 3e3c 2f73 6372 6970 743e 0a3c 7363  s"></script>.<sc
+000004f0: 7269 7074 3e0a 2020 2020 2428 2723 7b7b  ript>.    $('#{{
+00000500: 2066 6f72 6d2e 6d6f 6269 6c65 2e61 7574   form.mobile.aut
+00000510: 6f5f 6964 207d 7d27 292e 6d61 736b 2827  o_id }}').mask('
+00000520: 2b33 3830 3939 3939 3939 3939 3927 293b  +380999999999');
+00000530: 0a3c 2f73 6372 6970 743e 0a              .</script>.
```

### Comparing `django-mp-shop-offers-2.0/offers/templates/offers/price_offer_modal.html` & `django-mp-shop-offers-2.0.1/offers/templates/offers/price_offer_modal.html`

 * *Files identical despite different names*

### Comparing `django-mp-shop-offers-2.0/offers/views.py` & `django-mp-shop-offers-2.0.1/offers/views.py`

 * *Files identical despite different names*

