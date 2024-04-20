# Comparing `tmp/kodekloud_downloader-0.1.2.tar.gz` & `tmp/kodekloud_downloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodekloud_downloader-0.1.2.tar", max compression
+gzip compressed data, was "kodekloud_downloader-0.1.3.tar", max compression
```

## Comparing `kodekloud_downloader-0.1.2.tar` & `kodekloud_downloader-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    14806 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/README.md
--rw-r--r--   0        0        0     1102 2023-09-24 18:13:40.595047 kodekloud_downloader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/src/kodekloud_downloader/__init__.py
--rw-r--r--   0        0        0     1883 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/src/kodekloud_downloader/cli.py
--rw-r--r--   0        0        0      134 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/src/kodekloud_downloader/enums.py
--rw-r--r--   0        0        0     4643 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/src/kodekloud_downloader/helpers.py
--rw-r--r--   0        0        0     4663 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/src/kodekloud_downloader/main.py
--rw-r--r--   0        0        0     2039 2023-09-24 18:13:28.842994 kodekloud_downloader-0.1.2/src/kodekloud_downloader/models.py
--rw-r--r--   0        0        0    15745 1970-01-01 00:00:00.000000 kodekloud_downloader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    15716 2024-04-20 05:02:41.814072 kodekloud_downloader-0.1.3/README.md
+-rw-r--r--   0        0        0     1102 2024-04-20 05:02:51.122010 kodekloud_downloader-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-20 05:02:41.814072 kodekloud_downloader-0.1.3/src/kodekloud_downloader/__init__.py
+-rw-r--r--   0        0        0     2753 2024-04-20 05:02:41.814072 kodekloud_downloader-0.1.3/src/kodekloud_downloader/cli.py
+-rw-r--r--   0        0        0      134 2024-04-20 05:02:41.814072 kodekloud_downloader-0.1.3/src/kodekloud_downloader/enums.py
+-rw-r--r--   0        0        0     4661 2024-04-20 05:02:41.814072 kodekloud_downloader-0.1.3/src/kodekloud_downloader/helpers.py
+-rw-r--r--   0        0        0     7516 2024-04-20 05:02:41.814072 kodekloud_downloader-0.1.3/src/kodekloud_downloader/main.py
+-rw-r--r--   0        0        0     3361 2024-04-20 05:02:41.818072 kodekloud_downloader-0.1.3/src/kodekloud_downloader/models.py
+-rw-r--r--   0        0        0    16655 1970-01-01 00:00:00.000000 kodekloud_downloader-0.1.3/PKG-INFO
```

### Comparing `kodekloud_downloader-0.1.2/README.md` & `kodekloud_downloader-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -215,10 +215,35 @@
 | 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 Enter the courses you want to select (Multiple courses can be passes using this format 1,6-9,10-11): 1-3,7-9,10,13,55
 ```
 
 ![](static/demo-select-download.gif)
 
+You can also use `kodekloud dl-quiz` to download all quiz in a markdown file.
+
+```css
+kodekloud dl-quiz --help
+Usage: kodekloud dl-quiz [OPTIONS]
+
+Options:
+  -o, --output-dir TEXT  Output directory where quiz markdown file will be
+                         saved.
+  --sep                  Write in seperate markdown files.
+  --help                 Show this message and exit.
+```
+
+Here is an example:
+
+`kodekloud dl-quiz -o KodeKloudQuiz`
+
+or download seperate markdown file.
+
+`kodekloud dl-quiz -o KodeKloudQuiz --sep`
+
+To convert the quiz markdown to PDF you can use any online PDF converter like [aconvert](https://www.aconvert.com/pdf/md-to-pdf/), or [md2pdf](https://md2pdf.netlify.app/). You can also use [`grip`](https://github.com/joeyespo/grip). Or you can also create a [GitHub Gist](https://gist.github.com/) and then use your browser to convert the page into PDF.
+
+![](./static/KodeKloud_Quiz.png)
+
 ## Colab Notebook to download directly in Personal GDrive
 
 You can open [this notebook](https://colab.research.google.com/drive/1GsgFcqa_43GYeDKmoa0CXsRfDySrzvzT?usp=sharing) with your google account were you want to download the course. Please note that you should open with the same account for which you want to link the drive.
```

### Comparing `kodekloud_downloader-0.1.2/pyproject.toml` & `kodekloud_downloader-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodekloud-downloader"
-version = "v0.1.2"
+version = "v0.1.3"
 description = "Simple downloaded for https://kodekloud.com/"
 readme = "README.md"
 authors = ["Roy, Debakar <debakar.roy@outlook.com>"]
 repository = "https://github.com/debakarr/kodekloud-downloader"
 packages = [
     { include = "kodekloud_downloader", from = "src" },
 ]
```

### Comparing `kodekloud_downloader-0.1.2/src/kodekloud_downloader/cli.py` & `kodekloud_downloader-0.1.3/src/kodekloud_downloader/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from typing import Union
 
 import click
 import validators
 
 from kodekloud_downloader.enums import Quality
 from kodekloud_downloader.helpers import select_courses
-from kodekloud_downloader.main import download_course
+from kodekloud_downloader.main import download_course, download_quiz
 from kodekloud_downloader.models import get_all_course
 
 
 @click.group()
 @click.option("-v", "--verbose", count=True, help="Increase log level verbosity")
 def kodekloud(verbose):
-    logging.basicConfig(format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO)
+    logging.basicConfig(
+        format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
+    )
     if verbose == 1:
         logging.getLogger().setLevel(logging.INFO)
     elif verbose >= 2:
         logging.getLogger().setLevel(logging.DEBUG)
 
 
 @kodekloud.command()
@@ -38,27 +40,66 @@
 )
 @click.option(
     "--cookie",
     "-c",
     required=True,
     help="Cookie file. Course should be accessible via this.",
 )
-def dl(course_url, quality: str, output_dir: Union[Path, str], cookie):
+@click.option(
+    "--max-duplicate-count",
+    "-mdc",
+    default=3,
+    type=int,
+    help="If same video is downloaded this many times, then download stops",
+)
+def dl(
+    course_url,
+    quality: str,
+    output_dir: Union[Path, str],
+    cookie,
+    max_duplicate_count: int,
+):
     if course_url is None:
         courses = get_all_course()
         selected_courses = select_courses(courses)
         for selected_course in selected_courses:
             download_course(
                 url=selected_course.link,
                 cookie=cookie,
                 quality=quality,
                 output_dir=output_dir,
+                max_duplicate_count=max_duplicate_count,
             )
     elif validators.url(course_url):
-        download_course(url=course_url, cookie=cookie, quality=quality, output_dir=output_dir)
+        download_course(
+            url=course_url,
+            cookie=cookie,
+            quality=quality,
+            output_dir=output_dir,
+            max_duplicate_count=max_duplicate_count,
+        )
     else:
         logging.error("Please enter a valid URL")
         SystemExit(1)
 
 
+@kodekloud.command()
+@click.option(
+    "--output-dir",
+    "-o",
+    default=Path.home() / "Downloads",
+    help="Output directory where quiz markdown file will be saved.",
+)
+@click.option(
+    "--sep",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Write in seperate markdown files.",
+)
+def dl_quiz(output_dir: Union[Path, str], sep: bool):
+    Path(output_dir).mkdir(parents=True, exist_ok=True)
+    download_quiz(output_dir, sep)
+
+
 if __name__ == "__main__":
     kodekloud()
```

### Comparing `kodekloud_downloader-0.1.2/src/kodekloud_downloader/helpers.py` & `kodekloud_downloader-0.1.3/src/kodekloud_downloader/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 import yt_dlp
 
 from kodekloud_downloader.models import Course
 
 logger = logging.getLogger(__name__)
 
 
-from typing import List
-
-
 def parse_input(input_str: str) -> List[int]:
     """
     Parse the input string and return a list of integers based on the given logic.
 
     :param input_str: A string representing the input ranges.
     :rtype: A list of integers.
     :raises ValueError: If an invalid range is encountered.
@@ -53,26 +50,30 @@
     :param courses: A list of Course objects to choose from
     :return: The selected list of Course object
     """
     table = prettytable.PrettyTable()
     table.field_names = ["No.", "Name", "Type", "Categories"]
 
     for i, course in enumerate(courses):
-        table.add_row([i + 1, course.name, course.course_type, ", ".join(course.categories)])
+        table.add_row(
+            [i + 1, course.name, course.course_type, ", ".join(course.categories)]
+        )
 
     table.align["No."] = "l"
     table.align["Name"] = "l"
     table.align["Type"] = "l"
     table.align["Categories"] = "l"
 
     print(table)
 
     user_selected_courses = []
     selected_courses = parse_input(
-        input("Enter the courses you want to select (Multiple courses can be passes using this format 1,6-9,10-11): ")
+        input(
+            "Enter the courses you want to select (Multiple courses can be passes using this format 1,6-9,10-11): "
+        )
     )
     for selected_course in selected_courses:
         user_selected_courses.append(courses[int(selected_course) - 1])
 
     return user_selected_courses
```

### Comparing `kodekloud_downloader-0.1.2/PKG-INFO` & `kodekloud_downloader-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodekloud-downloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple downloaded for https://kodekloud.com/
 Home-page: https://github.com/debakarr/kodekloud-downloader
 Author: Roy, Debakar
 Author-email: debakar.roy@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -238,11 +238,36 @@
 | 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |
 +-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+
 Enter the courses you want to select (Multiple courses can be passes using this format 1,6-9,10-11): 1-3,7-9,10,13,55
 ```
 
 ![](static/demo-select-download.gif)
 
+You can also use `kodekloud dl-quiz` to download all quiz in a markdown file.
+
+```css
+kodekloud dl-quiz --help
+Usage: kodekloud dl-quiz [OPTIONS]
+
+Options:
+  -o, --output-dir TEXT  Output directory where quiz markdown file will be
+                         saved.
+  --sep                  Write in seperate markdown files.
+  --help                 Show this message and exit.
+```
+
+Here is an example:
+
+`kodekloud dl-quiz -o KodeKloudQuiz`
+
+or download seperate markdown file.
+
+`kodekloud dl-quiz -o KodeKloudQuiz --sep`
+
+To convert the quiz markdown to PDF you can use any online PDF converter like [aconvert](https://www.aconvert.com/pdf/md-to-pdf/), or [md2pdf](https://md2pdf.netlify.app/). You can also use [`grip`](https://github.com/joeyespo/grip). Or you can also create a [GitHub Gist](https://gist.github.com/) and then use your browser to convert the page into PDF.
+
+![](./static/KodeKloud_Quiz.png)
+
 ## Colab Notebook to download directly in Personal GDrive
 
 You can open [this notebook](https://colab.research.google.com/drive/1GsgFcqa_43GYeDKmoa0CXsRfDySrzvzT?usp=sharing) with your google account were you want to download the course. Please note that you should open with the same account for which you want to link the drive.
```

