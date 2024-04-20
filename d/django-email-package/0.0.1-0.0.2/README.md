# Comparing `tmp/django_email_package-0.0.1.tar.gz` & `tmp/django_email_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_email_package-0.0.1.tar", last modified: Wed Apr  3 23:29:50 2024, max compression
+gzip compressed data, was "django_email_package-0.0.2.tar", last modified: Sat Apr 20 15:58:48 2024, max compression
```

## Comparing `django_email_package-0.0.1.tar` & `django_email_package-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 23:29:50.393458 django_email_package-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-31 16:06:54.000000 django_email_package-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       51 2024-04-03 23:24:10.000000 django_email_package-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      774 2024-04-03 23:29:50.392459 django_email_package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-03-31 16:06:43.000000 django_email_package-0.0.1/README.md
--rw-rw-rw-   0        0        0      584 2024-04-03 23:29:12.000000 django_email_package-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 23:29:50.393458 django_email_package-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 23:29:50.363909 django_email_package-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:29:50.369088 django_email_package-0.0.1/src/django_email/
--rw-rw-rw-   0        0        0        0 2024-03-31 19:16:38.000000 django_email_package-0.0.1/src/django_email/__init__.py
--rw-rw-rw-   0        0        0      645 2024-04-01 15:15:06.000000 django_email_package-0.0.1/src/django_email/email_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:29:50.383459 django_email_package-0.0.1/src/django_email/templates/
--rw-rw-rw-   0        0        0     1813 2024-04-01 14:43:02.000000 django_email_package-0.0.1/src/django_email/templates/email_interest.html
--rw-rw-rw-   0        0        0     2590 2024-04-01 13:45:30.000000 django_email_package-0.0.1/src/django_email/templates/email_login.html
--rw-rw-rw-   0        0        0     1931 2024-04-01 14:09:31.000000 django_email_package-0.0.1/src/django_email/templates/email_ticket.html
--rw-rw-rw-   0        0        0     1868 2024-04-01 16:43:13.000000 django_email_package-0.0.1/src/django_email/templates/email_welcome.html
-drwxrwxrwx   0        0        0        0 2024-04-03 23:29:50.392459 django_email_package-0.0.1/src/django_email_package.egg-info/
--rw-rw-rw-   0        0        0      774 2024-04-03 23:29:50.000000 django_email_package-0.0.1/src/django_email_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      479 2024-04-03 23:29:50.000000 django_email_package-0.0.1/src/django_email_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 23:29:50.000000 django_email_package-0.0.1/src/django_email_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 23:29:50.000000 django_email_package-0.0.1/src/django_email_package.egg-info/top_level.txt
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-20 15:58:48.470469 django_email_package-0.0.2/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1073 2024-04-20 15:56:39.000000 django_email_package-0.0.2/LICENSE
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       51 2024-04-20 15:56:39.000000 django_email_package-0.0.2/MANIFEST.in
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      755 2024-04-20 15:58:48.470469 django_email_package-0.0.2/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      171 2024-04-20 15:56:39.000000 django_email_package-0.0.2/README.md
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      566 2024-04-20 15:57:42.000000 django_email_package-0.0.2/pyproject.toml
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2024-04-20 15:58:48.470469 django_email_package-0.0.2/setup.cfg
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-20 15:58:48.470469 django_email_package-0.0.2/src/
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-20 15:58:48.470469 django_email_package-0.0.2/src/django_email/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-20 15:56:39.000000 django_email_package-0.0.2/src/django_email/__init__.py
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      626 2024-04-20 15:56:39.000000 django_email_package-0.0.2/src/django_email/email_utils.py
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-20 15:58:48.470469 django_email_package-0.0.2/src/django_email/templates/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1764 2024-04-20 15:56:39.000000 django_email_package-0.0.2/src/django_email/templates/email_interest.html
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2508 2024-04-20 15:56:39.000000 django_email_package-0.0.2/src/django_email/templates/email_login.html
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1906 2024-04-20 15:56:39.000000 django_email_package-0.0.2/src/django_email/templates/email_ticket.html
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1812 2024-04-20 15:56:39.000000 django_email_package-0.0.2/src/django_email/templates/email_welcome.html
+drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2024-04-20 15:58:48.470469 django_email_package-0.0.2/src/django_email_package.egg-info/
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      755 2024-04-20 15:58:48.000000 django_email_package-0.0.2/src/django_email_package.egg-info/PKG-INFO
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      479 2024-04-20 15:58:48.000000 django_email_package-0.0.2/src/django_email_package.egg-info/SOURCES.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2024-04-20 15:58:48.000000 django_email_package-0.0.2/src/django_email_package.egg-info/dependency_links.txt
+-rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       13 2024-04-20 15:58:48.000000 django_email_package-0.0.2/src/django_email_package.egg-info/top_level.txt
```

### Comparing `django_email_package-0.0.1/LICENSE` & `django_email_package-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018 The Python Packaging Authority
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+Copyright (c) 2018 The Python Packaging Authority
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `django_email_package-0.0.1/PKG-INFO` & `django_email_package-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1
-Name: django_email_package
-Version: 0.0.1
-Summary: A Python package for sending HTML-formatted emails in Django
-Author-email: Didheemose <sebastiandidheemose2002@gmail.com>
-Project-URL: Homepage, https://github.com/DidheemosePS/django_email_package
-Project-URL: Issues, https://github.com/DidheemosePS/django_email_package/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Example Package
-
-This is a simple example package. You can use
-[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
-to write your content.
+Metadata-Version: 2.1
+Name: django_email_package
+Version: 0.0.2
+Summary: A Python package for sending HTML-formatted emails in Django
+Author-email: Didheemose <sebastiandidheemose2002@gmail.com>
+Project-URL: Homepage, https://github.com/DidheemosePS/django_email_package
+Project-URL: Issues, https://github.com/DidheemosePS/django_email_package/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Example Package
+
+This is a simple example package. You can use
+[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
+to write your content.
```

### Comparing `django_email_package-0.0.1/pyproject.toml` & `django_email_package-0.0.2/src/django_email_package.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-[project]
-name = "django_email_package"
-version = "0.0.1"
-authors = [
-  { name="Didheemose", email="sebastiandidheemose2002@gmail.com" },
-]
-description = "A Python package for sending HTML-formatted emails in Django"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/DidheemosePS/django_email_package"
-Issues = "https://github.com/DidheemosePS/django_email_package/issues"
+Metadata-Version: 2.1
+Name: django_email_package
+Version: 0.0.2
+Summary: A Python package for sending HTML-formatted emails in Django
+Author-email: Didheemose <sebastiandidheemose2002@gmail.com>
+Project-URL: Homepage, https://github.com/DidheemosePS/django_email_package
+Project-URL: Issues, https://github.com/DidheemosePS/django_email_package/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Example Package
+
+This is a simple example package. You can use
+[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
+to write your content.
```

### Comparing `django_email_package-0.0.1/src/django_email/templates/email_interest.html` & `django_email_package-0.0.2/src/django_email/templates/email_interest.html`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-<!DOCTYPE html>
-<html lang="en">
-  <head>
-    <meta charset="UTF-8" />
-  </head>
-  <body style="font-family: Arial, sans-serif; margin: 0; padding: 0">
-    <div
-      style="
-        max-width: 600px;
-        margin: 20px auto;
-        background-color: #f9f9f9;
-        padding: 20px;
-        border-radius: 8px;
-        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
-      "
-    >
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        Hello,
-      </p>
-      {% if context.body %} {% for body in context.body %}
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        {{ body }}
-      </p>
-      {% endfor %} {% else %}
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        I hope this email finds you well. I wanted to reach out to express my
-        interest in adopting a pet from your shelter.
-      </p>
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        Could you please provide me with more information about the adoption
-        process, including any requirements or paperwork needed? Additionally, I
-        would love to learn more about the pets currently available for
-        adoption.
-      </p>
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        Thank you for considering me as a potential adopter. I am looking
-        forward to hearing from you and hopefully welcoming a new furry friend
-        into my home.
-      </p>
-      {% endif %}
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        Best regards,
-      </p>
-      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
-        {{ context.name | default:'[Your Name]' }}
-      </p>
-    </div>
-  </body>
-</html>
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="UTF-8" />
+  </head>
+  <body style="font-family: Arial, sans-serif; margin: 0; padding: 0">
+    <div
+      style="
+        max-width: 600px;
+        margin: 20px auto;
+        background-color: #f9f9f9;
+        padding: 20px;
+        border-radius: 8px;
+        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
+      "
+    >
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        Hello,
+      </p>
+      {% if context.body %} {% for body in context.body %}
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        {{ body }}
+      </p>
+      {% endfor %} {% else %}
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        I hope this email finds you well. I wanted to reach out to express my
+        interest in adopting a pet from your shelter.
+      </p>
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        Could you please provide me with more information about the adoption
+        process, including any requirements or paperwork needed? Additionally, I
+        would love to learn more about the pets currently available for
+        adoption.
+      </p>
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        Thank you for considering me as a potential adopter. I am looking
+        forward to hearing from you and hopefully welcoming a new furry friend
+        into my home.
+      </p>
+      {% endif %}
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        Best regards,
+      </p>
+      <p style="font-size: 16px; line-height: 1.6; margin-bottom: 10px">
+        {{ context.name | default:'[Your Name]' }}
+      </p>
+    </div>
+  </body>
+</html>
```

### Comparing `django_email_package-0.0.1/src/django_email/templates/email_login.html` & `django_email_package-0.0.2/src/django_email/templates/email_ticket.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,59 @@
-<!DOCTYPE html>
-<html lang="en">
-  <head>
-    <meta charset="UTF-8" />
-  </head>
-  <body
-    style="
-      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
-        Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;
-      margin: 0;
-      padding: 0;
-    "
-  >
-    <div
-      style="
-        max-width: 37.5em;
-        margin: 20px auto;
-        border: 1px solid rgba(0, 0, 0, 0.1);
-        border-radius: 3px;
-        overflow: hidden;
-      "
-    >
-      <div style="padding: 20px">
-        <h1
-          style="
-            font-size: 32px;
-            font-weight: bold;
-            text-align: center;
-            margin: 0;
-          "
-        >
-          Hi {{ context.name | default:'Apple' }},
-        </h1>
-        <h2
-          style="
-            font-size: 26px;
-            font-weight: bold;
-            text-align: center;
-            margin: 0;
-          "
-        >
-          We noticed a recent login to your {{ context.company | default:'Apple'}} account.
-        </h2>
-        <p style="font-size: 16px; line-height: 24px; margin: 16px 0">
-          <b>Time:</b> {{ context.date }} at {{ context.time | default:'August 1, 2002 at 6:30 AM' }}
-        </p>
-        <p style="font-size: 16px; line-height: 24px; margin: 16px 0">
-          <b>Device:</b> {{ context.device | default:'Chrome on Mac OS X' }}
-        </p>
-        <p style="font-size: 16px; line-height: 24px; margin: 16px 0">
-          <b>Location:</b> {{ context.location | default:'Upland, California,United States' }}
-        </p>
-        <p style="font-size: 16px; line-height: 24px; margin: 16px 0">
-          If this was you, there's nothing else you need to do.
-        </p>
-        <p style="font-size: 16px; line-height: 24px; margin: 16px 0">
-          If this wasn't you or if you have additional questions, please see our
-          support page.
-        </p>
-        <div style="text-align: center">
-          <a
-            href="{{ context.link | default:'' }}"
-            style="
-              background-color: #e00707;
-              border-radius: 3px;
-              color: #fff;
-              font-weight: bold;
-              border: 1px solid rgba(0, 0, 0, 0.1);
-              cursor: pointer;
-              padding: 12px 30px;
-              line-height: 100%;
-              text-decoration: none;
-              display: inline-block;
-              max-width: 100%;
-            "
-            >Learn More</a
-          >
-        </div>
-      </div>
-    </div>
-  </body>
-</html>
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="UTF-8" />
+    <title>Event Ticket Booking Confirmation</title>
+  </head>
+  <body style="font-family: Arial, sans-serif; margin: 0; padding: 0">
+    <div
+      style="
+        max-width: 600px;
+        margin: 20px auto;
+        background-color: #f9f9f9;
+        padding: 20px;
+        border-radius: 8px;
+        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
+      "
+    >
+      <h2 style="margin: 0; color: #333; font-size: 24px; line-height: 1.4">
+        Event Ticket Booking Confirmation
+      </h2>
+      <p style="font-size: 16px; line-height: 1.6; margin: 16px 0">Hello,</p>
+      <p style="font-size: 16px; line-height: 1.6; margin: 16px 0">
+        We're delighted to confirm your booking for the following event:
+      </p>
+      <ul
+        style="
+          font-size: 16px;
+          line-height: 1.6;
+          margin: 16px 0;
+          padding-left: 20px;
+        "
+      >
+        <li>
+          <strong>Event:</strong> {{ context.event | default:'Music Concert' }}
+        </li>
+        <li>
+          <strong>Venue:</strong> {{ context.venue | default:'Concert Hall' }}
+        </li>
+        <li>
+          <strong>Date:</strong> {{ context.date | default:'January 1, 2025' }}
+        </li>
+        <li><strong>Time:</strong> {{ context.time | default:'8:00 PM' }}</li>
+        <li>
+          <strong>Number of Tickets:</strong> {{ context.tickets | default:'2' }}
+        </li>
+      </ul>
+      <p style="font-size: 16px; line-height: 1.6; margin: 16px 0">
+        Thank you for choosing to attend our event. We look forward to seeing
+        you there!
+      </p>
+      <p style="font-size: 16px; line-height: 1.6; margin: 16px 0">
+        Best regards,
+      </p>
+      <p style="font-size: 16px; line-height: 1.6; margin: 16px 0">
+        {{ context.company | default:'[Your Name]' }}
+      </p>
+    </div>
+  </body>
+</html>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-************ HHii {{{{ ccoonntteexxtt..nnaammee || ddeeffaauulltt::''AAppppllee'' }}}},, ************
-********** WWee nnoottiicceedd aa rreecceenntt llooggiinn ttoo yyoouurr {{{{ ccoonntteexxtt..ccoommppaannyy || ddeeffaauulltt::''AAppppllee''}}}}
-aaccccoouunntt.. **********
-TTiimmee:: {{ context.date }} at {{ context.time | default:'August 1, 2002 at 6:30
-AM' }}
-DDeevviiccee:: {{ context.device | default:'Chrome on Mac OS X' }}
-LLooccaattiioonn:: {{ context.location | default:'Upland, California,United States' }}
-If this was you, there's nothing else you need to do.
-If this wasn't you or if you have additional questions, please see our support
-page.
-_L_e_a_r_n_ _M_o_r_e
+********** EEvveenntt TTiicckkeett BBooookkiinngg CCoonnffiirrmmaattiioonn **********
+Hello,
+We're delighted to confirm your booking for the following event:
+    * EEvveenntt:: {{ context.event | default:'Music Concert' }}
+    * VVeennuuee:: {{ context.venue | default:'Concert Hall' }}
+    * DDaattee:: {{ context.date | default:'January 1, 2025' }}
+    * TTiimmee:: {{ context.time | default:'8:00 PM' }}
+    * NNuummbbeerr ooff TTiicckkeettss:: {{ context.tickets | default:'2' }}
+Thank you for choosing to attend our event. We look forward to seeing you
+there!
+Best regards,
+{{ context.company | default:'[Your Name]' }}
```

### Comparing `django_email_package-0.0.1/src/django_email/templates/email_welcome.html` & `django_email_package-0.0.2/src/django_email/templates/email_welcome.html`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-<!DOCTYPE html>
-<html lang="en">
-  <head>
-    <meta charset="UTF-8" />
-  </head>
-  <body
-    style="
-      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
-        Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;
-      margin: 0;
-      padding: 0;
-    "
-  >
-    <div style="max-width: 37.5em; margin: 0 auto; padding: 20px 0 48px">
-      <img
-        height="50"
-        src="{{ context.image | default:'https://media.designrush.com/inspiration_images/134802/conversions/_1511456315_653_apple-desktop.jpg' }}"
-        alt="Apple Logo"
-        style="display: block; margin: 0 auto; max-width: 100%"
-      />
-      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
-        Hi {{ context.name | default:'Apple' }},
-      </p>
-
-      {% if context.body %} {% for body in context.body %}
-      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
-        {{ body }}
-      </p>
-      {% endfor %} {% else %}
-      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
-        {{ context.body | default:'Welcome to Apple, the sales intelligence platform that helps you uncover qualified leads and close deals faster.'}}
-      </p>
-      {% endif %}
-      <a
-        href="{{ context.link | default:'' }}"
-        style="
-          background-color: #5f51e8;
-          border-radius: 3px;
-          color: #fff;
-          font-size: 16px;
-          text-decoration: none;
-          text-align: center;
-          display: inline-block;
-          padding: 12px;
-          line-height: 100%;
-          max-width: 100%;
-        "
-      >
-        <span>Get started</span>
-      </a>
-      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
-        Best,<br />The {{ context.company | default:'Apple' }} team
-      </p>
-    </div>
-  </body>
-</html>
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="UTF-8" />
+  </head>
+  <body
+    style="
+      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
+        Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;
+      margin: 0;
+      padding: 0;
+    "
+  >
+    <div style="max-width: 37.5em; margin: 0 auto; padding: 20px 0 48px">
+      <img
+        height="50"
+        src="{{ context.image | default:'https://media.designrush.com/inspiration_images/134802/conversions/_1511456315_653_apple-desktop.jpg' }}"
+        alt="Apple Logo"
+        style="display: block; margin: 0 auto; max-width: 100%"
+      />
+      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
+        Hi {{ context.name | default:'Apple' }},
+      </p>
+
+      {% if context.body %} {% for body in context.body %}
+      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
+        {{ body }}
+      </p>
+      {% endfor %} {% else %}
+      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
+        {{ context.body | default:'Welcome to Apple, the sales intelligence platform that helps you uncover qualified leads and close deals faster.'}}
+      </p>
+      {% endif %}
+      <a
+        href="{{ context.link | default:'' }}"
+        style="
+          background-color: #5f51e8;
+          border-radius: 3px;
+          color: #fff;
+          font-size: 16px;
+          text-decoration: none;
+          text-align: center;
+          display: inline-block;
+          padding: 12px;
+          line-height: 100%;
+          max-width: 100%;
+        "
+      >
+        <span>Get started</span>
+      </a>
+      <p style="font-size: 16px; line-height: 26px; margin: 16px 0">
+        Best,<br />The {{ context.company | default:'Apple' }} team
+      </p>
+    </div>
+  </body>
+</html>
```

