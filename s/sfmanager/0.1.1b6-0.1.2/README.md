# Comparing `tmp/sfmanager-0.1.1b6.tar.gz` & `tmp/sfmanager-0.1.2.tar.gz`

## Comparing `sfmanager-0.1.1b6.tar` & `sfmanager-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/sfmanager/__init__.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/sfmanager/about.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/sfmanager/app.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/LICENSE
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/pyproject.toml
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 sfmanager-0.1.1b6/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sfmanager-0.1.2/sfmanager/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sfmanager-0.1.2/sfmanager/about.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 sfmanager-0.1.2/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 sfmanager-0.1.2/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 sfmanager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 sfmanager-0.1.2/PKG-INFO
```

### Comparing `sfmanager-0.1.1b6/sfmanager/about.py` & `sfmanager-0.1.2/sfmanager/about.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from time import sleep
 
 def whatIsIt():
 	print("Hello dear user!")
 	sleep(1)
 	print("Thanks for download my library!")
 	sleep(2)
-	print("Homepage on github: https://github.com/grandescobar/sfmanager")
+	print("Homepage on github: https://github.com/GrandTheBest/sfmanager")
 	sleep(2)
-	print("Issues page on github: https://github.com/grandescobar/sfmanager/issues")
+	print("Issues page on github: https://github.com/GrandTheBest/sfmanager/issues")
 	sleep(2)
 	print("By this library you can work with text, image and other files.")
 	sleep(2)
 	print("You can read, set, add and replace content in text files.")
 	sleep(2)
 	print("Also you can create, copy, move, rename and remove any files.")
 	sleep(2)
-	print("You can open images...")
-	sleep(2)
-	print("Yes, just open...")
-	sleep(2)
-	print("But this will be supplemented!")
-	sleep(2)
 	print("That's all. Stay tuned!")
 	sleep(2)
 	print("Thanks for using! Good luck!")
 	sleep(1)
```

### Comparing `sfmanager-0.1.1b6/sfmanager/app.py` & `sfmanager-0.1.2/sfmanager/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,39 +69,26 @@
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 2")
 
 	# Replace certain content in text file
 
-	def replace(self, target, text):
+	def replace(self, _from, _to):
 		if self.level >= 3:
 			try:
 				with open(f"{self.filename}", "r") as f:
-					data = f.read().replace(target, text)
+					data = f.read().replace(_from, _to)
 				with open(f"{self.filename}", "w") as f:
 					f.write(data)
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 3")
 
-	# Funcs for work with images(.png, .jpg, .jpeg, etc.)
-
-	# Open image
-
-	def openImage(self):
-		if self.level >= 1:
-			try:
-				Image.open(f"{self.filename}").show()
-			except FileNotFoundError:
-				print("Something went wrong...")
-		else:
-			print(f"Low access level! {self.level}, but need 1")
-
 	# Funcs for general work with files
 
 	# Rename file(from self.filename to name)
 
 	def rename(self, name):
 		if self.level >= 4:
 			try:
@@ -120,18 +107,18 @@
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 5")
 
 	# Copy file
 
-	def copy(self, directory):
+	def copy(self, dst):
 		if self.level >= 4:
 			try:
-				shutil.copy2(f"{self.filename}", f"{directory}")
+				shutil.copy2(f"{self.filename}", f"{dst}")
 			except FileNotFoundError:
 				print("Something went wrong...")
 		else:
 			print(f"Low access level! {self.level}, but need 4")
 
 	# Move file
```

### Comparing `sfmanager-0.1.1b6/.gitignore` & `sfmanager-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b6/LICENSE` & `sfmanager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sfmanager-0.1.1b6/pyproject.toml` & `sfmanager-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "sfmanager"
-version = "0.1.1b6"
+version = "0.1.2"
 authors = [
 	{name="GrandTheBest", email="grandinfo-cm@gmail.com"},
 ]
 description = "This library is not that useful. Perhaps someday it will become great."
 readme = "README.md"
 requires-python = ">=3.10.0"
 dependencies = [
@@ -17,9 +17,9 @@
    "Programming Language :: Python :: 3",
    "License :: OSI Approved :: MIT License",
    "Operating System :: OS Independent",
 ]
 [project.scripts]
 sfmanager = "sfmanager:whatIsIt"
 [project.urls]
-Homepage = "https://github.com/grandescobar/sfmanager"
-Issues = "https://github.com/grandescobar/sfmanager/issues"
+Homepage = "https://github.com/GrandTheBest/sfmanager"
+Issues = "https://github.com/GrandTheBest/sfmanager/issues"
```

