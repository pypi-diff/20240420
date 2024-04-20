# Comparing `tmp/basek2-0.0.0.2.tar.gz` & `tmp/basek2-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basek2-0.0.0.2.tar", last modified: Fri Apr 12 07:10:33 2024, max compression
+gzip compressed data, was "basek2-0.0.0.3.tar", last modified: Sat Apr 20 16:30:46 2024, max compression
```

## Comparing `basek2-0.0.0.2.tar` & `basek2-0.0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:10:33.440325 basek2-0.0.0.2/
--rw-rw-rw-   0        0        0      218 2024-04-12 07:10:33.439324 basek2-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 basek2-0.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 07:10:33.431317 basek2-0.0.0.2/basek2/
--rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 basek2-0.0.0.2/basek2/__init__.py
--rw-rw-rw-   0        0        0     5318 2024-04-12 07:09:18.000000 basek2-0.0.0.2/basek2/player.py
--rw-rw-rw-   0        0        0     2970 2024-04-12 05:40:47.000000 basek2-0.0.0.2/basek2/team.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:10:33.438324 basek2-0.0.0.2/basek2.egg-info/
--rw-rw-rw-   0        0        0      218 2024-04-12 07:10:33.000000 basek2-0.0.0.2/basek2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-12 07:10:33.000000 basek2-0.0.0.2/basek2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:10:33.000000 basek2-0.0.0.2/basek2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 07:10:33.000000 basek2-0.0.0.2/basek2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 07:10:33.000000 basek2-0.0.0.2/basek2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 07:10:33.440325 basek2-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      769 2024-04-12 07:09:48.000000 basek2-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:30:46.186653 basek2-0.0.0.3/
+-rw-rw-rw-   0        0        0      218 2024-04-20 16:30:46.186653 basek2-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-23 11:02:11.000000 basek2-0.0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 16:30:46.178115 basek2-0.0.0.3/basek2/
+-rw-rw-rw-   0        0        0       41 2024-03-29 03:51:58.000000 basek2-0.0.0.3/basek2/__init__.py
+-rw-rw-rw-   0        0        0     5318 2024-04-12 07:09:18.000000 basek2-0.0.0.3/basek2/player.py
+-rw-rw-rw-   0        0        0     2950 2024-04-20 16:30:00.000000 basek2-0.0.0.3/basek2/team.py
+drwxrwxrwx   0        0        0        0 2024-04-20 16:30:46.185121 basek2-0.0.0.3/basek2.egg-info/
+-rw-rw-rw-   0        0        0      218 2024-04-20 16:30:46.000000 basek2-0.0.0.3/basek2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-20 16:30:46.000000 basek2-0.0.0.3/basek2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 16:30:46.000000 basek2-0.0.0.3/basek2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-20 16:30:46.000000 basek2-0.0.0.3/basek2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-20 16:30:46.000000 basek2-0.0.0.3/basek2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 16:30:46.186653 basek2-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2024-04-20 16:30:19.000000 basek2-0.0.0.3/setup.py
```

### Comparing `basek2-0.0.0.2/basek2/player.py` & `basek2-0.0.0.3/basek2/player.py`

 * *Files identical despite different names*

### Comparing `basek2-0.0.0.2/basek2/team.py` & `basek2-0.0.0.3/basek2/team.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 
         # 테이블 형태로 출력하기 위한 데이터 가공
         data = [columns]  # 헤더 추가
         for wl in team_wl:
             data.append(list(wl))
 
         # 테이블 형태로 출력
-        print(tabulate(data, tablefmt="grid"))
+        return tabulate(data, tablefmt="grid")
 
     except pymysql.Error as err:
-        print(f"MySQL 오류: {err}")
+        print("")
 
     finally:
         if 'conn' in locals() and conn.open:
             cursor.close()
             conn.close()
```

### Comparing `basek2-0.0.0.2/setup.py` & `basek2-0.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as f: # README.md 내용 읽어오기
     long_description = f.read()
 
 setup(
     name='basek2', # 패키지 이름
-    version='0.0.0.2', # 버전 등록
+    version='0.0.0.3', # 버전 등록
     long_description=long_description, # readme.md 등록
     long_description_content_type='text/markdown',  # readme.md 포맷
     description='testbase', # 패키지 설명
     author='basekk', # 작성자 등록
     author_email='jino152637@gmail.com', # 이메일 등록
     url='', # url 등록
     license='MIT', # 라이센스 등록
```

