# Comparing `tmp/simple_neural_works-0.5.5.tar.gz` & `tmp/simple_neural_works-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_neural_works-0.5.5.tar", last modified: Tue Mar 19 21:08:27 2024, max compression
+gzip compressed data, was "simple_neural_works-1.0.0.tar", last modified: Sat Apr 20 18:04:19 2024, max compression
```

## Comparing `simple_neural_works-0.5.5.tar` & `simple_neural_works-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 21:08:27.695331 simple_neural_works-0.5.5/
--rw-rw-rw-   0        0        0     4690 2024-03-19 21:08:27.695331 simple_neural_works-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     3817 2024-03-07 21:33:23.000000 simple_neural_works-0.5.5/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 21:08:27.697333 simple_neural_works-0.5.5/setup.cfg
--rw-rw-rw-   0        0        0      866 2024-03-19 21:06:08.000000 simple_neural_works-0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 21:08:27.642328 simple_neural_works-0.5.5/simple_neural_works/
--rw-rw-rw-   0        0        0       19 2024-03-08 14:50:16.000000 simple_neural_works-0.5.5/simple_neural_works/__init__.py
--rw-rw-rw-   0        0        0    17663 2024-03-15 11:03:30.000000 simple_neural_works-0.5.5/simple_neural_works/main.py
-drwxrwxrwx   0        0        0        0 2024-03-19 21:08:27.681335 simple_neural_works-0.5.5/simple_neural_works.egg-info/
--rw-rw-rw-   0        0        0     4690 2024-03-19 21:08:27.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-03-19 21:08:27.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       19 2024-03-08 14:50:16.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/__init__.py
--rw-rw-rw-   0        0        0        1 2024-03-19 21:08:27.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    17663 2024-03-15 11:03:30.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/main.py
--rw-rw-rw-   0        0        0       20 2024-03-19 21:08:27.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/requires.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 21:08:27.694333 simple_neural_works-0.5.5/simple_neural_works.egg-info/simple_neural_works/
--rw-rw-rw-   0        0        0       19 2024-03-08 14:46:23.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/simple_neural_works/__init__.py
--rw-rw-rw-   0        0        0    17648 2024-03-07 21:02:33.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/simple_neural_works/main.py
--rw-rw-rw-   0        0        0       20 2024-03-19 21:08:27.000000 simple_neural_works-0.5.5/simple_neural_works.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 18:04:19.558036 simple_neural_works-1.0.0/
+-rw-rw-rw-   0        0        0     4580 2024-04-20 18:04:19.559036 simple_neural_works-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3707 2024-04-20 15:43:14.000000 simple_neural_works-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-20 18:04:19.561036 simple_neural_works-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      866 2024-04-20 13:40:29.000000 simple_neural_works-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:04:19.496031 simple_neural_works-1.0.0/simple_neural_works/
+-rw-rw-rw-   0        0        0       19 2024-03-08 14:50:16.000000 simple_neural_works-1.0.0/simple_neural_works/__init__.py
+-rw-rw-rw-   0        0        0    14094 2024-04-20 18:01:51.000000 simple_neural_works-1.0.0/simple_neural_works/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 18:04:19.542036 simple_neural_works-1.0.0/simple_neural_works.egg-info/
+-rw-rw-rw-   0        0        0     4580 2024-04-20 18:04:19.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-04-20 18:04:19.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       19 2024-03-08 14:50:16.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/__init__.py
+-rw-rw-rw-   0        0        0        1 2024-04-20 18:04:19.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    14094 2024-04-20 18:01:51.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/main.py
+-rw-rw-rw-   0        0        0       20 2024-04-20 18:04:19.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/requires.txt
+drwxrwxrwx   0        0        0        0 2024-04-20 18:04:19.557037 simple_neural_works-1.0.0/simple_neural_works.egg-info/simple_neural_works/
+-rw-rw-rw-   0        0        0       19 2024-03-08 14:46:23.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/simple_neural_works/__init__.py
+-rw-rw-rw-   0        0        0    17648 2024-03-07 21:02:33.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/simple_neural_works/main.py
+-rw-rw-rw-   0        0        0       20 2024-04-20 18:04:19.000000 simple_neural_works-1.0.0/simple_neural_works.egg-info/top_level.txt
```

### Comparing `simple_neural_works-0.5.5/PKG-INFO` & `simple_neural_works-1.0.0/simple_neural_works.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple_neural_works
-Version: 0.5.5
+Name: simple-neural-works
+Version: 1.0.0
 Summary: This is the simplest module for quick work with neural networks.
 Home-page: https://github.com/TwentyOneError/simple_neural_works
 Author: TwentyOneError
 Author-email: ourmail20210422@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/TwentyOneError
 Keywords: neural networks simple backpropagation
@@ -19,22 +19,23 @@
 ## What is this? ##
 The module allows you to work with simple neural networks (At the moment, the simplest convolutional neural network model is used with the method of backpropagation of error and sigmoidal activation function).
 
 ## Quick Guide ##
 The module is based on the following structure:
 
     
-    ne = Neuro(10,5,5,0.1,False)
-    ne.init_m()
-    ne.fill_m()
+    from simple_neural_works import Neuro
+    a = [25,30,30,20,10]
+    ne = Neuro(a,0.1)
+    ne.fill(False)
     in = [0.5,1,1,0,0.001] # some values to input
-    a = ne.getv(in)
+    a = ne.get_result(in,False)
     ou = [1,1,1,1,0,1,0,0,1] # some values to train
-    ne.bpn(ou)
-    ne.save_m("filename.res")
+    ne.backpropagation(ou,False)
+    ne.save_m("filename.res",False)
     
     
 
 Which Python provides by standard.
 
 
 ----------
@@ -43,60 +44,56 @@
 ### Using ###
 
 
 Using the library is as simple and convenient as possible:
 
 First, import main module using "from simple_neural_works import Neuro"
 
-The second, you need to initialize the creation of an array with data using the init_m function.
+The second, you need to load or create an array with data using the load() or fill() function.
 
 Examples of all operations:
 
 Creating an instance of a neural network with which you will then work.
 
-    ne = Neuro(wide, height, depth, speed of backpropagation, Muting the console output)
-
-Initializing an array of the required size before work (required):
-
-    ne.init_m()
+    ne = Neuro(array_width_of_slices_neaural_network,speed of backpropagation)
 
 
 Filling the weights with initial random values is used to create a neural network from scratch:
 
-    ne.fill_m()
+    ne.fill(mute)
 
 
 To load previously saved values from a file:
 
-    ne.load_m("filenamehere.txt")
+    ne.load("filenamehere.txt",mute)
     
 
 Function used to obtain the result of a neural network calculation:
 
-    ne.getv([some float or int values to input])
+    ne.get_result([some float or int values to input in array],mute)
 
 
-To train a neural network, use the following function. The input is an array, which should be the output of the neural network, the learning rate is controlled by the internal variable `ne.spd`, set manually and during network initialization. Only used after the `getv()` or `imgg()` function.
+To train a neural network, use the following function. The input is an array, which should be the output of the neural network, the learning rate is controlled by the internal variable `ne.spd`, set manually and during network initialization. Only used after the `get_result()` or `image_get_result()` function.
 
-    ne.bpn([some int or float values to train])
+    ne.backpropagation([some int or float values to train in array],mute)
 
 
 To quickly save an array of weights:
 
-    ne.save_m("filename.txt")
+    ne.save("filenamehere.txt",mute)
 
 
 For compact (up to two times smaller) but slower saving:
 
-    ne.zip_save_m("filename.txt")
+    ne.zip_save("filename.txt",mute)
 
 
 Blank for recognizing monochrome numbers. To read data from a PNG image (the image is inverted in color, that is, you need to draw it black, although this is not so important). To avoid specifying the entire path to the file, start the file name with "./".
 
-    ne.imgg("filename.png")
+    ne.image_get_result("filename.png",mute)
 
 
 ----------
 
 
 ### Structure ###
 
@@ -106,23 +103,20 @@
     
     ne.w
 
 An array storing the output values of the activation function:
 
     ne.ou
 
-Variable switching the output of intermediate data (number of operations per execution, execution progress, response accuracy for the `bpn()` function:
-
-    ne.mute
 
 Speed of backpropagation (between 0 and 1). If you donвЂ™t want to bother, then set it to 0.1. In more detail, at first you can use 1, towards the end of training 0.1:
 
-    ne.spd
+    ne.speed
 
-Please do not change the width, height and depth values while working, this will cause the operation to malfunction.
+Please do not change the width array while working, this will cause the operation to malfunction.
 ----------
 
 ----------
 
 ## Developer ##
 
 My GitHub: [link](https://github.com/TwentyOneError)
```

### Comparing `simple_neural_works-0.5.5/README.md` & `simple_neural_works-1.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 ## What is this? ##
 The module allows you to work with simple neural networks (At the moment, the simplest convolutional neural network model is used with the method of backpropagation of error and sigmoidal activation function).
 
 ## Quick Guide ##
 The module is based on the following structure:
 
     
-    ne = Neuro(10,5,5,0.1,False)
-    ne.init_m()
-    ne.fill_m()
+    from simple_neural_works import Neuro
+    a = [25,30,30,20,10]
+    ne = Neuro(a,0.1)
+    ne.fill(False)
     in = [0.5,1,1,0,0.001] # some values to input
-    a = ne.getv(in)
+    a = ne.get_result(in,False)
     ou = [1,1,1,1,0,1,0,0,1] # some values to train
-    ne.bpn(ou)
-    ne.save_m("filename.res")
+    ne.backpropagation(ou,False)
+    ne.save_m("filename.res",False)
     
     
 
 Which Python provides by standard.
 
 
 ----------
@@ -27,60 +28,56 @@
 ### Using ###
 
 
 Using the library is as simple and convenient as possible:
 
 First, import main module using "from simple_neural_works import Neuro"
 
-The second, you need to initialize the creation of an array with data using the init_m function.
+The second, you need to load or create an array with data using the load() or fill() function.
 
 Examples of all operations:
 
 Creating an instance of a neural network with which you will then work.
 
-    ne = Neuro(wide, height, depth, speed of backpropagation, Muting the console output)
-
-Initializing an array of the required size before work (required):
-
-    ne.init_m()
+    ne = Neuro(array_width_of_slices_neaural_network,speed of backpropagation)
 
 
 Filling the weights with initial random values is used to create a neural network from scratch:
 
-    ne.fill_m()
+    ne.fill(mute)
 
 
 To load previously saved values from a file:
 
-    ne.load_m("filenamehere.txt")
+    ne.load("filenamehere.txt",mute)
     
 
 Function used to obtain the result of a neural network calculation:
 
-    ne.getv([some float or int values to input])
+    ne.get_result([some float or int values to input in array],mute)
 
 
-To train a neural network, use the following function. The input is an array, which should be the output of the neural network, the learning rate is controlled by the internal variable `ne.spd`, set manually and during network initialization. Only used after the `getv()` or `imgg()` function.
+To train a neural network, use the following function. The input is an array, which should be the output of the neural network, the learning rate is controlled by the internal variable `ne.spd`, set manually and during network initialization. Only used after the `get_result()` or `image_get_result()` function.
 
-    ne.bpn([some int or float values to train])
+    ne.backpropagation([some int or float values to train in array],mute)
 
 
 To quickly save an array of weights:
 
-    ne.save_m("filename.txt")
+    ne.save("filenamehere.txt",mute)
 
 
 For compact (up to two times smaller) but slower saving:
 
-    ne.zip_save_m("filename.txt")
+    ne.zip_save("filename.txt",mute)
 
 
 Blank for recognizing monochrome numbers. To read data from a PNG image (the image is inverted in color, that is, you need to draw it black, although this is not so important). To avoid specifying the entire path to the file, start the file name with "./".
 
-    ne.imgg("filename.png")
+    ne.image_get_result("filename.png",mute)
 
 
 ----------
 
 
 ### Structure ###
 
@@ -90,23 +87,20 @@
     
     ne.w
 
 An array storing the output values of the activation function:
 
     ne.ou
 
-Variable switching the output of intermediate data (number of operations per execution, execution progress, response accuracy for the `bpn()` function:
-
-    ne.mute
 
 Speed of backpropagation (between 0 and 1). If you don’t want to bother, then set it to 0.1. In more detail, at first you can use 1, towards the end of training 0.1:
 
-    ne.spd
+    ne.speed
 
-Please do not change the width, height and depth values while working, this will cause the operation to malfunction.
+Please do not change the width array while working, this will cause the operation to malfunction.
 ----------
 
 ----------
 
 ## Developer ##
 
 My GitHub: [link](https://github.com/TwentyOneError)
```

### Comparing `simple_neural_works-0.5.5/setup.py` & `simple_neural_works-1.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def readme():
     with open("README.md","r") as f:
         return f.read()
 
 
 setup(
     name='simple_neural_works',
-    version='0.5.5',
+    version='1.0.0',
     author='TwentyOneError',
     author_email='ourmail20210422@gmail.com',
     description='This is the simplest module for quick work with neural networks.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/TwentyOneError/simple_neural_works',
     packages=find_packages(),
```

### Comparing `simple_neural_works-0.5.5/simple_neural_works/main.py` & `simple_neural_works-1.0.0/simple_neural_works.egg-info/simple_neural_works/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,32 +177,30 @@
 
     # ---------------------------------------------loading weights
     def load_m(self, fl_nm):
         try:
             f = open(fl_nm, "r")
         except Exception:
             raise Exception("Unable to load file. The file may not exist.")
-
-        ___ = f.readline()
-        if "zip" in ___: # If you used the compressed saving method
+        if "zip" in f.readline(): # If you used the compressed saving method
             uuu = self.dpt * (self.lenm + 1) * (self.lenm + 1)  # "uuu" means the number of elements to process
             if not self.mute:
                 print("start loading...")
                 print(uuu, "elements")
             kc = 0
             t = time()
             for i in range(self.dpt):
                 for j in range(self.lenm + 1):
                     for k in range(self.lenm + 1):
                         self.w[i][j][k] = ne__rconvfl(f.readline())  # outstanding move (check comments later)
                         kc += 1
                 if time() - t > 60 and not self.mute:
                     print(kc, "/", uuu)
                     t = time()
-        elif "text" in ___: # If you used the standard saving method
+        elif "text" in f.readline(): # If you used the standard saving method
             uuu = self.dpt * (self.lenm + 1) * (self.lenm + 1)  # "uuu" means the number of elements to process
             if not self.mute:
                 print("start loading...")
                 print(uuu, "elements")
             kc = 0
             t = time()
             for i in range(self.dpt):
@@ -289,15 +287,15 @@
             print(uuu, "elements")
         kc = 0
         t = time()
         ts = t
         hm = [0] * (self.lenm + 1)
         i: int
         for i in range(len(oua)):
-            hm[i] = float(oua[i])
+            hm[i] = float(oua)
         dem = []
         dem1 = [0] * (self.lenm + 1)
         i: int
         for i in range(self.lenm + 1):
             de = self.ou[-1][i] * (1 - self.ou[-1][i]) * (hm[i] - self.ou[-1][i])
             dem1[i] = de
             kc += 1
```

### Comparing `simple_neural_works-0.5.5/simple_neural_works.egg-info/PKG-INFO` & `simple_neural_works-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple-neural-works
-Version: 0.5.5
+Name: simple_neural_works
+Version: 1.0.0
 Summary: This is the simplest module for quick work with neural networks.
 Home-page: https://github.com/TwentyOneError/simple_neural_works
 Author: TwentyOneError
 Author-email: ourmail20210422@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/TwentyOneError
 Keywords: neural networks simple backpropagation
@@ -19,22 +19,23 @@
 ## What is this? ##
 The module allows you to work with simple neural networks (At the moment, the simplest convolutional neural network model is used with the method of backpropagation of error and sigmoidal activation function).
 
 ## Quick Guide ##
 The module is based on the following structure:
 
     
-    ne = Neuro(10,5,5,0.1,False)
-    ne.init_m()
-    ne.fill_m()
+    from simple_neural_works import Neuro
+    a = [25,30,30,20,10]
+    ne = Neuro(a,0.1)
+    ne.fill(False)
     in = [0.5,1,1,0,0.001] # some values to input
-    a = ne.getv(in)
+    a = ne.get_result(in,False)
     ou = [1,1,1,1,0,1,0,0,1] # some values to train
-    ne.bpn(ou)
-    ne.save_m("filename.res")
+    ne.backpropagation(ou,False)
+    ne.save_m("filename.res",False)
     
     
 
 Which Python provides by standard.
 
 
 ----------
@@ -43,60 +44,56 @@
 ### Using ###
 
 
 Using the library is as simple and convenient as possible:
 
 First, import main module using "from simple_neural_works import Neuro"
 
-The second, you need to initialize the creation of an array with data using the init_m function.
+The second, you need to load or create an array with data using the load() or fill() function.
 
 Examples of all operations:
 
 Creating an instance of a neural network with which you will then work.
 
-    ne = Neuro(wide, height, depth, speed of backpropagation, Muting the console output)
-
-Initializing an array of the required size before work (required):
-
-    ne.init_m()
+    ne = Neuro(array_width_of_slices_neaural_network,speed of backpropagation)
 
 
 Filling the weights with initial random values is used to create a neural network from scratch:
 
-    ne.fill_m()
+    ne.fill(mute)
 
 
 To load previously saved values from a file:
 
-    ne.load_m("filenamehere.txt")
+    ne.load("filenamehere.txt",mute)
     
 
 Function used to obtain the result of a neural network calculation:
 
-    ne.getv([some float or int values to input])
+    ne.get_result([some float or int values to input in array],mute)
 
 
-To train a neural network, use the following function. The input is an array, which should be the output of the neural network, the learning rate is controlled by the internal variable `ne.spd`, set manually and during network initialization. Only used after the `getv()` or `imgg()` function.
+To train a neural network, use the following function. The input is an array, which should be the output of the neural network, the learning rate is controlled by the internal variable `ne.spd`, set manually and during network initialization. Only used after the `get_result()` or `image_get_result()` function.
 
-    ne.bpn([some int or float values to train])
+    ne.backpropagation([some int or float values to train in array],mute)
 
 
 To quickly save an array of weights:
 
-    ne.save_m("filename.txt")
+    ne.save("filenamehere.txt",mute)
 
 
 For compact (up to two times smaller) but slower saving:
 
-    ne.zip_save_m("filename.txt")
+    ne.zip_save("filename.txt",mute)
 
 
 Blank for recognizing monochrome numbers. To read data from a PNG image (the image is inverted in color, that is, you need to draw it black, although this is not so important). To avoid specifying the entire path to the file, start the file name with "./".
 
-    ne.imgg("filename.png")
+    ne.image_get_result("filename.png",mute)
 
 
 ----------
 
 
 ### Structure ###
 
@@ -106,23 +103,20 @@
     
     ne.w
 
 An array storing the output values of the activation function:
 
     ne.ou
 
-Variable switching the output of intermediate data (number of operations per execution, execution progress, response accuracy for the `bpn()` function:
-
-    ne.mute
 
 Speed of backpropagation (between 0 and 1). If you donвЂ™t want to bother, then set it to 0.1. In more detail, at first you can use 1, towards the end of training 0.1:
 
-    ne.spd
+    ne.speed
 
-Please do not change the width, height and depth values while working, this will cause the operation to malfunction.
+Please do not change the width array while working, this will cause the operation to malfunction.
 ----------
 
 ----------
 
 ## Developer ##
 
 My GitHub: [link](https://github.com/TwentyOneError)
```

