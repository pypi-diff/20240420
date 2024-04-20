# Comparing `tmp/turkish_profile_generator-0.2.tar.gz` & `tmp/turkish_profile_generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish_profile_generator-0.2.tar", last modified: Fri Apr 12 21:45:05 2024, max compression
+gzip compressed data, was "turkish_profile_generator-0.2.1.tar", last modified: Sat Apr 20 20:49:39 2024, max compression
```

## Comparing `turkish_profile_generator-0.2.tar` & `turkish_profile_generator-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 21:45:05.248331 turkish_profile_generator-0.2/
--rw-rw-rw-   0        0        0     1085 2024-04-12 21:18:22.000000 turkish_profile_generator-0.2/LICENSE
--rw-rw-rw-   0        0        0       85 2020-12-21 21:19:00.000000 turkish_profile_generator-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2721 2024-04-12 21:45:05.248331 turkish_profile_generator-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1414 2024-04-12 21:20:56.000000 turkish_profile_generator-0.2/README.md
--rw-rw-rw-   0        0        0       98 2020-12-21 21:19:00.000000 turkish_profile_generator-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      136 2024-04-12 21:45:05.248331 turkish_profile_generator-0.2/setup.cfg
--rw-rw-rw-   0        0        0     2009 2024-04-12 21:44:34.000000 turkish_profile_generator-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 21:45:05.132470 turkish_profile_generator-0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 21:45:05.163663 turkish_profile_generator-0.2/src/turkish_profile_generator/
--rw-rw-rw-   0        0        0     4366 2024-04-12 21:36:34.000000 turkish_profile_generator-0.2/src/turkish_profile_generator/UserProfileGenerator.py
--rw-rw-rw-   0        0        0      164 2024-04-12 21:44:56.000000 turkish_profile_generator-0.2/src/turkish_profile_generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 21:45:05.232707 turkish_profile_generator-0.2/src/turkish_profile_generator/data/
--rw-rw-rw-   0        0        0    20676 2024-04-12 01:05:54.000000 turkish_profile_generator-0.2/src/turkish_profile_generator/data/firstname_female.txt
--rw-rw-rw-   0        0        0    47005 2024-04-12 01:05:54.000000 turkish_profile_generator-0.2/src/turkish_profile_generator/data/firstname_male.txt
--rw-rw-rw-   0        0        0     6981 2024-04-12 01:05:54.000000 turkish_profile_generator-0.2/src/turkish_profile_generator/data/firstname_uni.txt
--rw-rw-rw-   0        0        0    22277 2024-04-12 00:44:40.000000 turkish_profile_generator-0.2/src/turkish_profile_generator/data/lastname.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 21:45:05.248331 turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/
--rw-rw-rw-   0        0        0     2721 2024-04-12 21:45:05.000000 turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      656 2024-04-12 21:45:05.000000 turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 21:45:05.000000 turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-12 21:45:05.000000 turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-12 21:45:05.000000 turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 21:45:05.232707 turkish_profile_generator-0.2/tests/
--rw-rw-rw-   0        0        0      256 2024-04-12 21:24:39.000000 turkish_profile_generator-0.2/tests/test_module1.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:49:39.764982 turkish_profile_generator-0.2.1/
+-rw-rw-rw-   0        0        0     1072 2024-04-13 11:08:29.000000 turkish_profile_generator-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       85 2020-12-21 21:19:00.000000 turkish_profile_generator-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2890 2024-04-20 20:49:39.763879 turkish_profile_generator-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-04-13 11:12:38.000000 turkish_profile_generator-0.2.1/README.md
+-rw-rw-rw-   0        0        0       98 2020-12-21 21:19:00.000000 turkish_profile_generator-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      136 2024-04-20 20:49:39.769426 turkish_profile_generator-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2009 2024-04-12 21:44:34.000000 turkish_profile_generator-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:49:39.614955 turkish_profile_generator-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-20 20:49:39.646213 turkish_profile_generator-0.2.1/src/turkish_profile_generator/
+-rw-rw-rw-   0        0        0     4382 2024-04-20 20:49:17.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator/UserProfileGenerator.py
+-rw-rw-rw-   0        0        0      164 2024-04-20 20:49:30.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 20:49:39.754173 turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/
+-rw-rw-rw-   0        0        0    20676 2024-04-12 01:05:54.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/firstname_female.txt
+-rw-rw-rw-   0        0        0    47005 2024-04-12 01:05:54.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/firstname_male.txt
+-rw-rw-rw-   0        0        0     6981 2024-04-12 01:05:54.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/firstname_uni.txt
+-rw-rw-rw-   0        0        0    22277 2024-04-12 00:44:40.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/lastname.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 20:49:39.761927 turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/
+-rw-rw-rw-   0        0        0     2890 2024-04-20 20:49:39.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      656 2024-04-20 20:49:39.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 20:49:39.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-20 20:49:39.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-20 20:49:39.000000 turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 20:49:39.756898 turkish_profile_generator-0.2.1/tests/
+-rw-rw-rw-   0        0        0      256 2024-04-12 21:24:39.000000 turkish_profile_generator-0.2.1/tests/test_module1.py
```

### Comparing `turkish_profile_generator-0.2/LICENSE` & `turkish_profile_generator-0.2.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Mustafa Buyruk (tomchen.org)
+Copyright (c) 2021 Mustafa Buyruk 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `turkish_profile_generator-0.2/PKG-INFO` & `turkish_profile_generator-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-profile-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bossturk/turkish-profile-generator
 Author: Mustafa Buyruk
 Author-email: bossturk@hotmail.com
 Project-URL: Documentation, https://github.com/bossturk/turkish-profile-generator
 Project-URL: Bug Reports, https://github.com/bossturk/turkish-profile-generator/issues
 Project-URL: Source Code, https://github.com/bossturk/turkish-profile-generator
@@ -38,28 +38,32 @@
 pip install turkish-profile-generator
 
 
 from turkish_profile_generator import UserProfileGenerator
 
 # Create an instance of UserProfileGenerator class
 generator = UserProfileGenerator(min_age=18, max_age=50)
+#generator = UserProfileGenerator(min_age=18, max_age=50, gender='Female')
+#generator = UserProfileGenerator(min_age=18, max_age=50, gender='Male')
 
 # Generate a random user profile
 profile = generator.generate_profile()
 
 # Print the generated profile attributes
 print("Generated Profile:")
 print("First Name:", profile['firstname'])
 print("Last Name:", profile['lastname'])
 print("Age:", profile['age'])
 print("Birthday:", profile['birthday'])
 print("Email:", profile['email'])
 print("Password:", profile['password'])
 print("Gender:", profile['gender'])
 
+profile.reset()
+
 Features
 Generates random Turkish names.
 Generates random age, birth date, email address, and password.
 Generates names compatible with the Turkish alphabet.
 Can generate user profiles in the desired age range.
 Contributing
 If you'd like to contribute to this project, please visit the GitHub repository: https://github.com/bossturk/turkish-profile-generator
```

### Comparing `turkish_profile_generator-0.2/README.md` & `turkish_profile_generator-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 pip install turkish-profile-generator
 
 
 from turkish_profile_generator import UserProfileGenerator
 
 # Create an instance of UserProfileGenerator class
 generator = UserProfileGenerator(min_age=18, max_age=50)
+#generator = UserProfileGenerator(min_age=18, max_age=50, gender='Female')
+#generator = UserProfileGenerator(min_age=18, max_age=50, gender='Male')
 
 # Generate a random user profile
 profile = generator.generate_profile()
 
 # Print the generated profile attributes
 print("Generated Profile:")
 print("First Name:", profile['firstname'])
 print("Last Name:", profile['lastname'])
 print("Age:", profile['age'])
 print("Birthday:", profile['birthday'])
 print("Email:", profile['email'])
 print("Password:", profile['password'])
 print("Gender:", profile['gender'])
 
+profile.reset()
+
 Features
 Generates random Turkish names.
 Generates random age, birth date, email address, and password.
 Generates names compatible with the Turkish alphabet.
 Can generate user profiles in the desired age range.
 Contributing
 If you'd like to contribute to this project, please visit the GitHub repository: https://github.com/bossturk/turkish-profile-generator
```

### Comparing `turkish_profile_generator-0.2/setup.py` & `turkish_profile_generator-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator/UserProfileGenerator.py` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator/UserProfileGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
             self.gender = random.choice(self.genders)
 
     def read_names_from_file(self, filename):
         with open(filename, 'r',encoding='utf-8') as file:
             return [name.strip() for name in file.readlines()]
 
     def generate_profile(self):
-        firstname = self.get_firstname()
-        lastname = self.get_lastname()
+        firstname = self.get_firstname().lower()
+        lastname = self.get_lastname().lower()
         current_year = datetime.now().year
         birth_year = random.randint(current_year - self.max_age, current_year - self.min_age)
         birth_month = random.randint(1, 12)
         birth_day = random.randint(1, 28)  # Assuming all months have 28 days
         birthday = f"{birth_year}-{birth_month:02d}-{birth_day:02d}"
         age = current_year - birth_year - ((birth_month, birth_day) > (datetime.now().month, datetime.now().day))
         email = self.get_email(firstname, lastname, birth_year)
```

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator/data/firstname_female.txt` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/firstname_female.txt`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator/data/firstname_male.txt` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/firstname_male.txt`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator/data/firstname_uni.txt` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/firstname_uni.txt`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator/data/lastname.txt` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator/data/lastname.txt`

 * *Files identical despite different names*

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/PKG-INFO` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turkish-profile-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Example PyPI (Python Package Index) Package
 Home-page: https://github.com/bossturk/turkish-profile-generator
 Author: Mustafa Buyruk
 Author-email: bossturk@hotmail.com
 Project-URL: Documentation, https://github.com/bossturk/turkish-profile-generator
 Project-URL: Bug Reports, https://github.com/bossturk/turkish-profile-generator/issues
 Project-URL: Source Code, https://github.com/bossturk/turkish-profile-generator
@@ -38,28 +38,32 @@
 pip install turkish-profile-generator
 
 
 from turkish_profile_generator import UserProfileGenerator
 
 # Create an instance of UserProfileGenerator class
 generator = UserProfileGenerator(min_age=18, max_age=50)
+#generator = UserProfileGenerator(min_age=18, max_age=50, gender='Female')
+#generator = UserProfileGenerator(min_age=18, max_age=50, gender='Male')
 
 # Generate a random user profile
 profile = generator.generate_profile()
 
 # Print the generated profile attributes
 print("Generated Profile:")
 print("First Name:", profile['firstname'])
 print("Last Name:", profile['lastname'])
 print("Age:", profile['age'])
 print("Birthday:", profile['birthday'])
 print("Email:", profile['email'])
 print("Password:", profile['password'])
 print("Gender:", profile['gender'])
 
+profile.reset()
+
 Features
 Generates random Turkish names.
 Generates random age, birth date, email address, and password.
 Generates names compatible with the Turkish alphabet.
 Can generate user profiles in the desired age range.
 Contributing
 If you'd like to contribute to this project, please visit the GitHub repository: https://github.com/bossturk/turkish-profile-generator
```

### Comparing `turkish_profile_generator-0.2/src/turkish_profile_generator.egg-info/SOURCES.txt` & `turkish_profile_generator-0.2.1/src/turkish_profile_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

