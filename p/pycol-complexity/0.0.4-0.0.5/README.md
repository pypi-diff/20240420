# Comparing `tmp/pycol_complexity-0.0.4.tar.gz` & `tmp/pycol_complexity-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycol_complexity-0.0.4.tar", last modified: Tue Apr  9 05:30:16 2024, max compression
+gzip compressed data, was "pycol_complexity-0.0.5.tar", last modified: Sat Apr 20 09:55:29 2024, max compression
```

## Comparing `pycol_complexity-0.0.4.tar` & `pycol_complexity-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 05:30:16.000533 pycol_complexity-0.0.4/
--rw-rw-rw-   0        0        0     1103 2024-04-09 05:21:21.000000 pycol_complexity-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     5569 2024-04-09 05:30:15.999533 pycol_complexity-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5104 2024-03-21 06:37:06.000000 pycol_complexity-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 05:30:15.983136 pycol_complexity-0.0.4/pycol_complexity/
--rw-rw-rw-   0        0        0        0 2024-03-21 03:21:50.000000 pycol_complexity-0.0.4/pycol_complexity/__init__.py
--rw-rw-rw-   0        0        0    93388 2024-03-21 04:47:59.000000 pycol_complexity-0.0.4/pycol_complexity/complexity.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:30:15.999533 pycol_complexity-0.0.4/pycol_complexity.egg-info/
--rw-rw-rw-   0        0        0     5569 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-09 05:30:15.000000 pycol_complexity-0.0.4/pycol_complexity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      215 2024-03-21 04:48:10.000000 pycol_complexity-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      559 2024-04-09 05:30:16.001963 pycol_complexity-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-20 09:55:29.858829 pycol_complexity-0.0.5/
+-rw-rw-rw-   0        0        0     1103 2024-04-09 05:21:21.000000 pycol_complexity-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5569 2024-04-20 09:55:29.858829 pycol_complexity-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2024-03-21 06:37:06.000000 pycol_complexity-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 09:55:29.837396 pycol_complexity-0.0.5/pycol_complexity/
+-rw-rw-rw-   0        0        0        0 2024-03-21 03:21:50.000000 pycol_complexity-0.0.5/pycol_complexity/__init__.py
+-rw-rw-rw-   0        0        0    96143 2024-04-20 09:41:29.000000 pycol_complexity-0.0.5/pycol_complexity/complexity.py
+drwxrwxrwx   0        0        0        0 2024-04-20 09:55:29.857830 pycol_complexity-0.0.5/pycol_complexity.egg-info/
+-rw-rw-rw-   0        0        0     5569 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-20 09:55:29.000000 pycol_complexity-0.0.5/pycol_complexity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      215 2024-03-21 04:48:10.000000 pycol_complexity-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      559 2024-04-20 09:55:29.860826 pycol_complexity-0.0.5/setup.cfg
```

### Comparing `pycol_complexity-0.0.4/LICENSE.txt` & `pycol_complexity-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycol_complexity-0.0.4/PKG-INFO` & `pycol_complexity-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycol_complexity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Package for complexity measures
 Home-page: https://github.com/DiogoApostolo/pycol
 Author: Diogo Apostolo
 Author-email: ogoid.478@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycol_complexity-0.0.4/README.md` & `pycol_complexity-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pycol_complexity-0.0.4/pycol_complexity/complexity.py` & `pycol_complexity-0.0.5/pycol_complexity/complexity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import copy
 import math
 from operator import itemgetter
 import numpy as np
 from numpy.core.fromnumeric import shape, transpose, var
 import arff
+from sklearn.calibration import LabelEncoder
 from sklearn.cluster import KMeans
 import sklearn
+from sklearn.metrics import DistanceMetric
 import sklearn.pipeline
 import scipy.spatial
 import pandas as pd
 
 
+from catboost.datasets import epsilon,higgs,adult
 
+import pickle
 
 
 
 
 
 
 class Complexity:
@@ -35,35 +39,37 @@
         It then calculates the distance matrix that contains the distance between all points in X (self.dist_matrix).
         It also saves in an array the unique labels of all existing classes (self.classes), the number of samples in each class (self.class_count) and
         the indexes in X of every class (self.class_inxs).
         -----
         Parameters:
         file_name (string): Location of the file that contains the dataset.
         distance_func (string): The distance function to be used to calculate the distance matrix. Only available option right now is "HEOM".
-        file_type (string): The type of file where the dataset is stored. Only available option right now is "arff".
+        file_type (string): The type of file where the dataset is stored. Only available option right now is "arff" and "pickle".
         
         '''
         if(file_type=="arff"):
             [X,y,meta]=self.__read_file(file_name)
-        if(file_type=="nparray"):
-            [X,y,meta]=self.__prepare_array()
-
-
+        elif(file_type=="pickle"):
+            [X,y,meta]=self.__prepare_array(file_name)
         else:
             print("Only arff files are available for now")
             return
 
         self.X=np.array(X)
       
         self.y=np.array(y)
         classes=np.unique(self.y)
 
         self.classes = classes
         self.meta=meta
         self.dist_matrix,self.unnorm_dist_matrix = self.__calculate_distance_matrix(self.X,distance_func=distance_func)
+        
+        
+
+        
         self.class_count = self.__count_class_instances()
 
 
         self.class_inxs = self.__get_class_inxs()
 
         if(len(self.class_count)<2):
            print("ERROR: Less than two classes are in the dataset.")
@@ -82,17 +88,72 @@
         class_count (numpy.array): An (Nx1) array with the number of intances for each of the N classes in the dataset 
         '''
         class_count = np.zeros(len(self.classes))
         for i in range(len(self.classes)):
             count=len(np.where(self.y == self.classes[i])[0])
             class_count[i]+=count
         return class_count
-
     
+    def encode(self,X,meta):
+        for i in range(len(meta)):
+            
+            if meta[i]==1:
+                label_encoder = LabelEncoder()
+                # Fit the LabelEncoder to your categorical values and transform them to numerical values
+                numerical_values = label_encoder.fit_transform(X[:,i])
+                X[:,i] = numerical_values
+
+        if 1 in meta:
+            X = X.astype(np.float64)
+
+        return X
+
+    def is_categorical(self,X):
+        meta = []
+        # Iterate through each column in the array
+        for i in range(X.shape[1]):
+            column = X[:, i]
+            # Check if all elements in the column can be converted to float (numerical)
+            try:
+                float_column = column.astype(float)
+                meta.append(0)
+            except ValueError:
+                # If conversion to float raises an error, the column likely contains non-numeric values (categorical)
+                meta.append(1)
+
+        # Print the detected numerical and categorical feature indices
+        return meta
     
+    def __prepare_array(self,dataset_name):
+        
+        
+
+
+        #change this
+        with open(dataset_name, 'rb') as f:
+            epsilon_train = pickle.load(f)
+
+        print(epsilon_train)
+        X = epsilon_train[:,0:len(epsilon_train[0])-1]
+        y = epsilon_train[:,-1]
+
+        meta = self.is_categorical(X)
+
+        X = self.encode(X,meta)
+
+        #indentify the existing classes
+        classes = np.unique(y)
+
+        #create new class labels from 0 to n, where n is the number of classes
+        y = [np.where(classes == i)[0][0] for i in y]
+        
+
+             
+
+        return [X,y,meta]
     
     
     def __read_file(self,file_name):
         '''
         Is called by the __init__ method.
         Read an arff file containing the dataset.
         --------
@@ -139,15 +200,15 @@
         for i in range(len(meta)):
             if meta[i]==1:
                 
                 b, c = np.unique(X[:,i], return_inverse=True)
                 X[:,i] = c
 
         if 1 in meta:
-            X = X.astype(np.float)
+            X = X.astype(float)
 
 
         #indentify the existing classes
         classes = np.unique(y)
 
         #create new class labels from 0 to n, where n is the number of classes
         y = [np.where(classes == i[-1])[0][0] for i in data]
@@ -436,22 +497,23 @@
                     n_plus+=line[i]
                 else:
                     n_minus+=line[i]
         return [n_minus,n_plus]
 
 
     
-    def R_value(self,k=5,theta=2):
+    def R_value(self,k=5,theta=2,imb=False):
         '''
         Calculate the Augmented R value complexity measure defined in [1].
 
         --------
         Parameters:
         k (int): Number of neighbours, for the knn function
         tetha (int): threshold of neighbours that can have a different class label
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         --------
         Returns:
         r_values (array): An array with the R values of the pair wise combinations of all classes (One VS One)
         --------
         References:
 
         [1] Borsos Z, Lemnaru C, Potolea R (2018) Dealing with overlap and imbalance:
@@ -475,32 +537,38 @@
         
         for i in range(len(r_matrix)):
             for j in range(len(r_matrix[0])):
                 r_matrix[i,j]=r_matrix[i,j]/self.class_count[i]
 
 
         
-
+       
         r_values = []
         for i in range(len(r_matrix)):
             for j in range(i+1,len(r_matrix)):
-                imbalanced_ratio = 0
-                maj_r = 0
-                min_r = 0
+                
+            
                 if(self.class_count[i]>self.class_count[j]):
-                    imbalanced_ratio = self.class_count[j]/self.class_count[i]
-                    maj_r = r_matrix[i,j]
-                    min_r = r_matrix[j,i]
-                else:
                     imbalanced_ratio = self.class_count[i]/self.class_count[j]
-                    maj_r = r_matrix[j,i]
-                    min_r = r_matrix[i,j]
+                    
+                    overlap_ci_cj = r_matrix[i,j]
+                    overlap_cj_ci = r_matrix[j,i]
+                else:
+                    imbalanced_ratio = self.class_count[j]/self.class_count[i]
+                    overlap_ci_cj = r_matrix[j,i]
+                    overlap_cj_ci = r_matrix[i,j]
 
-                r=(1/(imbalanced_ratio+1))*(maj_r+imbalanced_ratio*min_r)
-                r_values.append(r)
+
+                if(imb):
+                    r = [overlap_cj_ci,overlap_ci_cj]
+                    r_values.append(r)
+                else:
+                    r=(1/(imbalanced_ratio+1))*(overlap_ci_cj+imbalanced_ratio*overlap_cj_ci)
+                    
+                    r_values.append(r)
         
         
         return r_values
        
     def D3_value(self,k=5):
         '''
         Calculate the D3 value complexity measure defined in [1].
@@ -527,69 +595,80 @@
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             if(0.5>(count[cls_inx]/k)): 
                 d3_matrix[cls_inx]+=1 
         return d3_matrix
 
 
     
-    def kDN(self,k=5):
+    def kDN(self,k=5,imb=False):
         '''
         Calculate the kDN value complexity measure defined in [1]
 
         --------
         Parameters:
         k (int): Number of neighbours, for the knn function
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         --------
         Returns:
         kDN (float): The value of the complexity measure
         --------
         References:
 
         [1] Smith MR, Martinez T, Giraud-Carrier C (2014) An instance level analysis
         of data complexity. Machine learning 95(2):225-256
         --------
         '''
 
 
-        kDN_value = 0
+        kDN_value = np.zeros(len(self.classes))
         for i in range(len(self.dist_matrix)):
             line = self.dist_matrix[i]
             count=self.__knn(i,copy.copy(line),k)
             cls_inx = np.where( self.classes == self.y[i])[0][0]
-            kDN_value+= (k-count[cls_inx])/k
-        kDN_value/=len(self.X)       
+            kDN_value[cls_inx]+= (k-count[cls_inx])/k
+        
+        if(imb):
+            kDN_value = np.divide(kDN_value,self.class_count)
+        else:
+            kDN_value = sum(kDN_value)/len(self.X)       
+        
         return kDN_value
 
-    def CM(self,k=5):
+    def CM(self,k=5,imb=False):
         '''
         Calculate the CM value complexity measure defined in [1].
 
         -------
         Parameters:
         k (int): Number of neighbours, for the knn function
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         CM_value (float): The value of the complexity measure
         -------
         References:
 
         [1] Anwar N, Jones G, Ganesh S (2014) Measurement of data complexity
         for classification problems with unbalanced data. Statistical Analysis and
         Data Mining: The ASA Data Science Journal 7(3):194-211
         -------
         '''
-        CM_value = 0
+        CM_value = np.zeros(len(self.classes))
         for i in range(len(self.dist_matrix)):
             line = self.dist_matrix[i]
             count=self.__knn(i,copy.copy(line),k)
             cls_inx = np.where( self.classes == self.y[i])[0]
             kDN_value = (k-count[cls_inx])/k
             if(kDN_value>0.5):
-                CM_value+=1
-        CM_value/=len(self.X)
+                CM_value[cls_inx]+=1
+        
+        if(imb):
+            CM_value = np.divide(CM_value,self.class_count)
+        else:
+            CM_value = sum(CM_value)/len(self.X)
         return CM_value   
 
     
 
     def __MRI_p(self,profile):
         '''
         Calculate the MRI value of a pattern.
@@ -701,31 +780,35 @@
                     inx = np.where( kmeans.labels_ == i)[0]
                     cluster = profiles[inx]
                     
                     mrca[i]=self.__MRI_k(cluster)
 
                 return mrca
                 
-    def C1(self,max_k=5):
+    
+
+    def C1(self,max_k=5,imb=False):
         '''
         Calculate the C1 value complexity measure defined in [1].
 
         -------
         Parameters:
         sigmas (float): An array with the multiple hypersphere radius
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         c1_val (float): The value of the complexity measure 
         -------
         References:
 
         [1] Massie S, Craw S, Wiratunga N (2005) Complexity-guided case discovery
         for case based reasoning. In: AAAI, vol 5, pp 216-221
         '''
-        c1_sum = 0
+
+        c1_sum = np.zeros(len(self.classes))
         for i in range(len(self.X)):
             c1_instance_sum = 0
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             #for each radius sigma
             for k in range(1,max_k+1):
                 #draw a hypersphere with radius sigma around the point and check which points inside are from the same class and
                 #which are not.
@@ -733,90 +816,46 @@
                 
                 count=self.__knn(i,copy.copy(self.dist_matrix[i]),k)
                
                 pkj=count[cls_inx]/k
                 c1_instance_sum += pkj
 
             c1_instance_val = 1-(c1_instance_sum/max_k)
-            c1_sum += c1_instance_val
-        c1_val = c1_sum/len(self.X)
-
+            c1_sum[cls_inx] += c1_instance_val
+        
+        if(imb):
+            c1_val = np.divide(c1_sum,self.class_count)
+        else:
+            c1_val = sum(c1_sum)/len(self.X)
         return c1_val
+    
+    
+
 
-    def C1_imb(self,max_k=5):
+    
+
+
+    def C2(self,max_k=5,imb=False):
         '''
-        Calculate the C1 value complexity measure defined in [1].
+        Calculate the C2 value complexity measure defined in [1].
 
         -------
         Parameters:
         sigmas (float): An array with the multiple hypersphere radius
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
-        c1_val (float): The value of the complexity measure 
+        c2_val (float): The value of the complexity measure 
         -------
         References:
 
         [1] Massie S, Craw S, Wiratunga N (2005) Complexity-guided case discovery
         for case based reasoning. In: AAAI, vol 5, pp 216-221
         '''
 
-        c1_sum = np.zeros(len(self.classes))
-        for i in range(len(self.X)):
-            c1_instance_sum = 0
-            cls_inx = np.where( self.classes == self.y[i])[0][0]
-            #for each radius sigma
-            for k in range(1,max_k+1):
-                #draw a hypersphere with radius sigma around the point and check which points inside are from the same class and
-                #which are not.
-                #n = self.__hypersphere(i,sigma)
-                
-                count=self.__knn(i,copy.copy(self.dist_matrix[i]),k)
-               
-                pkj=count[cls_inx]/k
-                c1_instance_sum += pkj
-
-            c1_instance_val = 1-(c1_instance_sum/max_k)
-            c1_sum[cls_inx] += c1_instance_val
-        c1_val = np.divide(c1_sum,self.class_count)
-
-        return c1_val
-    
-    
-
-
-    def C2(self,max_k=5):
-        c2_sum = 0
-        for i in range(len(self.X)):
-            c2_instance_sum = 0
-
-            #for each radius sigma
-            for k in range(1,max_k+1):
-                #draw a hypersphere with radius sigma around the point and check which points inside are from the same class and
-                #which are not.
-                #n = self.__hypersphere(i,sigma)
-                
-                dists=self.__knn_dists(i,copy.copy(self.dist_matrix[i]),k)
-            
-                pkj = 0
-                for d in dists:
-                    pkj+=1-d
-                pkj/= k
-
-                #cls_inx = np.where( self.classes == self.y[i])[0][0]
-                #pkj=count[cls_inx]/k
-                c2_instance_sum += pkj
-
-            c2_instance_val = 1-(c2_instance_sum/max_k)
-            c2_sum += c2_instance_val
-        c2_val = c2_sum/len(self.X)
-
-        return c2_val
-
-
-    def C2_imb(self,max_k=5):
         c2_sum = np.zeros(len(self.classes))
         for i in range(len(self.X)):
             c2_instance_sum = 0
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             #for each radius sigma
             for k in range(1,max_k+1):
                 #draw a hypersphere with radius sigma around the point and check which points inside are from the same class and
@@ -832,15 +871,18 @@
 
                 #cls_inx = np.where( self.classes == self.y[i])[0][0]
                 #pkj=count[cls_inx]/k
                 c2_instance_sum += pkj
 
             c2_instance_val = 1-(c2_instance_sum/max_k)
             c2_sum[cls_inx] += c2_instance_val
-        c2_val = np.divide(c2_sum,self.class_count)
+        if(imb):
+            c2_val = np.divide(c2_sum,self.class_count)
+        else:
+            c2_val = sum(c2_sum)/len(self.X)
 
         return c2_val
 
 
 
     def __calculate_n_inter(self,dist_matrix=[],y=[],imb=False):
         '''
@@ -903,168 +945,119 @@
             for inx in unique_vertix:
                 cls_inx = np.where( self.classes == self.y[inx])[0][0]
                 count[cls_inx]+=1
 
 
         return count
 
-    def N1_imb(self):
-        count = self.__calculate_n_inter(imb=True)
-        
-        n1 = np.divide(count,self.class_count)
-        return n1
-
-    def N1(self):
+    def N1(self,imb=False):
         '''
         Calculate the N1 value complexity measure defined in [1].
-
+        -------
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         n1 (float): The value of the complexity measure 
         -------
         References:
 
-        Ho T, Basu M (2002) Complexity measures of supervised classification
+        [1] Ho T, Basu M (2002) Complexity measures of supervised classification
         problems. IEEE transactions on pattern analysis and machine intelligence 24(3):289-300
         '''
-        count = self.__calculate_n_inter()
-       
-        n1 = count/len(self.y)
-        return n1
-    
-    def N2_imb(self):
-        count_inter = np.zeros(len(self.classes))
-        count_intra = np.zeros(len(self.classes))
-
-
-        #for each sample
-        for i in range(len(self.dist_matrix)):
-            min_inter = np.inf
-            min_intra = np.inf
-
-            #iterate over every sample and check which is the nearest neighbour from the same class and
-            #which is the nearest neighbour from the opposite class.
-            for j in range(len(self.dist_matrix[0])):
-                if(self.y[i]==self.y[j] and i!=j and self.dist_matrix[i][j]<min_intra):
-                    min_intra=self.dist_matrix[i][j]
-                if(self.y[i]!=self.y[j] and self.dist_matrix[i][j]<min_inter):
-                    min_inter=self.dist_matrix[i][j]
-
-            cls_inx = np.where( self.classes == self.y[i])[0][0]
-            count_inter[cls_inx]+=min_inter
-            count_intra[cls_inx]+=min_intra
+        count = self.__calculate_n_inter(imb=imb)
         
+        if(imb):
+            n1 = np.divide(count,self.class_count)
+        else:
+            n1 = count/len(self.y)
+        return n1
 
-        
-        r = np.array([])
-        for i in range(len(count_inter)):
-            if(count_inter[i]==0):
-                r=np.append(r,0)
-            else:
-                r=np.append(r,(count_intra[i]/count_inter[i]))
-        
-        
-        N2 = np.divide(r,(1+r))
-        return N2
-
-    def N2(self):
+  
+    
+    def N2(self,imb=False):
         '''
         Calculate the N2 value complexity measure defined in [1].
-
+        -------
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         n2 (float): The value of the complexity measure 
         -------
         References:
 
-        Ho T, Basu M (2002) Complexity measures of supervised classification
+        [1] Ho T, Basu M (2002) Complexity measures of supervised classification
         problems. IEEE transactions on pattern analysis and machine intelligence 24(3):289-300
         '''
-        count_inter = 0
-        count_intra = 0
+        count_inter = np.zeros(len(self.classes))
+        count_intra = np.zeros(len(self.classes))
 
 
         #for each sample
         for i in range(len(self.dist_matrix)):
             min_inter = np.inf
             min_intra = np.inf
 
             #iterate over every sample and check which is the nearest neighbour from the same class and
             #which is the nearest neighbour from the opposite class.
             for j in range(len(self.dist_matrix[0])):
                 if(self.y[i]==self.y[j] and i!=j and self.dist_matrix[i][j]<min_intra):
                     min_intra=self.dist_matrix[i][j]
                 if(self.y[i]!=self.y[j] and self.dist_matrix[i][j]<min_inter):
                     min_inter=self.dist_matrix[i][j]
-            count_inter+=min_inter
-            count_intra+=min_intra
-
-
-        if(count_inter==0):
-            r = 0
-        else:
-            r = count_intra/count_inter
 
+            cls_inx = np.where( self.classes == self.y[i])[0][0]
+            count_inter[cls_inx]+=min_inter
+            count_intra[cls_inx]+=min_intra
         
-        
+        if(imb):
+            r = np.array([])
+            for i in range(len(count_inter)):
+                if(count_inter[i]==0):
+                    r=np.append(r,0)
+                else:
+                    r=np.append(r,(count_intra[i]/count_inter[i]))
 
-        N2 = r/(1+r)
-        return N2
+            N2 = np.divide(r,(1+r))
 
-   
-    def N3(self,k=1):
-        '''
-        Calculate the N3 value complexity measure in [1].
-        By default k=1 in accordance to the definition in the paper. However it is possible to select a different value for k.
-        -------
-        Parameters:
-        k (int): number of nearest neighbours to consider
-        -------
-        Returns:
-        n3 (float): the value of the complexity measure 
-        -------
-        References: 
 
-        Ho T, Basu M (2002) Complexity measures of supervised classification
-        problems. IEEE transactions on pattern analysis and machine intelligence 24(3):289-300
-        ''' 
-       
-        sample_count=0
-        #for each sample
-        for sample in range(len(self.X)):
-            #calculate the nearest neighbour
-            count=self.__knn(sample,copy.copy(self.dist_matrix[sample]),k)
-            cls_inx = np.where( self.classes == self.y[sample])[0][0]
+        else:
             
+            if(sum(count_inter)==0):
+                r = 0
+            else:
+                r = sum(count_intra)/sum(count_inter)
+
             
-            class_count=count[cls_inx]
-            max_count=np.max(count)
-            #are there more instances with the same class label or with a different class label. 
-            if(class_count<max_count):
-                sample_count+=1
+        
+            N2 = r/(1+r)
 
+        
+        return N2
 
-        n3 = sample_count/len(self.y)
-        return n3
     
-    #todo: change comments
-    def N3_imb(self,k=1):
+   
+    
+    
+    
+    def N3(self,k=1,imb=False):
         '''
         Calculate the N3 value complexity measure in [1].
         By default k=1 in accordance to the definition in the paper. However it is possible to select a different value for k.
         -------
         Parameters:
         k (int): number of nearest neighbours to consider
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         n3 (float): the value of the complexity measure 
         -------
         References: 
-
-        Ho T, Basu M (2002) Complexity measures of supervised classification
+        [1] Ho T, Basu M (2002) Complexity measures of supervised classification
         problems. IEEE transactions on pattern analysis and machine intelligence 24(3):289-300
         ''' 
         n3_counts=np.zeros(len(self.classes))
         #sample_count=0
         #for each sample
         for sample in range(len(self.X)):
             #calculate the nearest neighbour
@@ -1074,15 +1067,19 @@
             
             class_count=count[cls_inx]
             max_count=np.max(count)
             #are there more instances with the same class label or with a different class label. 
             if(class_count<max_count):
                 #sample_count+=1
                 n3_counts[cls_inx]+=1
-        n3 = np.divide(n3_counts,self.class_count)
+
+        if(imb):
+            n3 = np.divide(n3_counts,self.class_count)
+        else:
+            n3 = sum(n3_counts)/len(self.X)
         #n3 = sample_count/len(self.y)
         return n3
     
     def __interpolate_samples(self,class_inxs=[]):
         '''
         Create new interpolated samples from the sample array X.
         To achieve this 2 samples in X from the same class are selected and a new sample is created by interpolating these 2.
@@ -1121,74 +1118,23 @@
        
         return X_interp, y_interp
 
     
     
     
     
-    
-    
-    
-   
-    def N4(self,k=1):
-        '''
-        Calculate the N4 value complexity measure defined in [1].
-        -------
-        Parameters:
-        k (int): Number of nearest neighbours to consider
-        -------
-        Returns:
-        n4 (float): The value of the complexity measure 
-        -------
-        References:
-
-        [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How complex
-        is your classification problem? a survey on measuring classification
-        complexity. ACM Computing Surveys (CSUR) 52(5):1-34
-        '''
-
-
-        #create new interpolated samples
-        X_interp, y_interp=self.__interpolate_samples()
-        
-       
-       
-
-        new_dist = self.__distance_HEOM_different_arrays(self.X,X_interp)
-
-        sample_count=0
-
-        #for each sample in X_interpol check calculate their k nearest neighbours in X and determine if there
-        #are more neighbours from the same class or more neighbours from the opposite classes.
-        for sample in range(len(X_interp)):
-            
-            
-            count=self.__knn(sample,copy.copy(new_dist[sample]),k,clear_diag=False)
-            cls_inx = np.where( self.classes == y_interp[sample])[0][0]
-            
-            #number of neighbours with the same class label
-            class_count=count[cls_inx]
-
-            
-            max_count=np.max(count)
-            if(class_count<max_count):
-                sample_count+=1
-                
-
-        n4 = sample_count/len(y_interp)
-        return n4
-    
 
     #todo change this
-    def N4_imb(self,k=1):
+    def N4(self,k=1,imb=False):
         '''
         Calculate the N4 value complexity measure defined in [1].
         -------
         Parameters:
         k (int): Number of nearest neighbours to consider
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         -------
         Returns:
         n4 (float): The value of the complexity measure 
         -------
         References:
 
         [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How complex
@@ -1219,57 +1165,66 @@
             class_count=count[cls_inx]
 
             
             max_count=np.max(count)
             if(class_count<max_count):
                 #sample_count+=1
                 n4_counts[cls_inx]+=1
-        n4 = np.divide(n4_counts,self.class_count)
+        if(imb):
+            n4 = np.divide(n4_counts,self.class_count)
+        else:
+            n4 = sum(n4_counts)/len(self.X)
 
         #n4 = sample_count/len(y_interp)
         return n4
         
        
     
-    def SI(self,k=1):
+    def SI(self,k=1,imb=False):
         '''
         Calculate the Separability index (SI) complexity measure defined in [1].
 
+        ------
+        Parameters:
+        k (int): The number of nearest neighbours to consider.
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         --------
         Returns:
         si_measure (float): The SI complexity measure value calculated.
         --------
         References:
 
-        Thornton C (1998) Separability is a learner's best friend. In: 4th Neural
+        [1] Thornton C (1998) Separability is a learner's best friend. In: 4th Neural
         Computation and Psychology Workshop, London, 9-11 April 1997,
         Springer, pp 40-46
 
 
         
         '''
         
 
-        sample_count=0
+        sample_count= np.zeros(len(self.classes))
         #for each sample
         for sample in range(len(self.X)):
             #calculate the nearest neighbour
             count=self.__knn(sample,copy.copy(self.dist_matrix[sample]),k)
             cls_inx = np.where( self.classes == self.y[sample])[0][0]
             
             
             class_count=count[cls_inx]
             max_count=np.max(count)
             #are there more instances with the same class label or with a different class label. 
             if(class_count==max_count):
-                sample_count+=1
+                sample_count[cls_inx]+=1
 
 
-        
-        si_measure = sample_count/len(self.y)
+        if(imb):        
+            si_measure = np.divide(sample_count,self.class_count)
+        else:
+            si_measure = sum(sample_count)/len(self.y)
         return si_measure
         
 
 
 
     def __find_nearest_oposite_class(self,x_inx,x_dist):
         '''
@@ -2004,146 +1959,179 @@
                 f1v=(np.matmul(d.T,np.matmul(B,d)))/(np.matmul(d.T,np.matmul(W,d)))
 
                 f1v = 1/(1+f1v)
                 f1vs.append(f1v)
         return f1vs
 
 
-    #only for datasets with no categorical features
-    def F2(self):
+
+    
+
+    def F2(self,imb=False):
         '''
         Calculates the F2 measure defined in [1]. 
         Uses One vs One method to handle multiclass datasets.
         -----
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
+        -----
         Returns:
         f2s (array): The value of f2 measure for each one vs one combination of classes.
         -----
         References:
 
-        [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How com-
-        plex is your classification problem? a survey on measuring classification
+        [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How complex is your classification problem? a survey on measuring classification
         complexity. ACM Computing Surveys (CSUR) 52(5):1-34
         '''
         f2s=[]
         #one vs one method
         for i in range(len(self.class_inxs)):
             for j in range(i+1,len(self.class_inxs)):
                 sample_c1 = self.X[self.class_inxs[i]]
                 sample_c2 = self.X[self.class_inxs[j]]
 
-                
-                maxmax = np.max([np.max(sample_c1,axis=0),np.max(sample_c2,axis=0)],axis=0)
+
                 maxmin = np.max([np.min(sample_c1,axis=0),np.min(sample_c2,axis=0)],axis=0)
-                minmin = np.min([np.min(sample_c1,axis=0),np.min(sample_c2,axis=0)],axis=0)
                 minmax = np.min([np.max(sample_c1,axis=0),np.max(sample_c2,axis=0)],axis=0)
-
+                
                 numer=np.maximum(0.0, minmax - maxmin) 
-            
-                denom=(maxmax - minmin)
+                if(imb):
+                    if(len(sample_c1) > len(sample_c2)):
+                        maxmax_minority = np.max(sample_c2,axis=0)
+                        minmin_minority = np.min(sample_c2,axis=0)
+
+                        maxmax_majority = np.max(sample_c1,axis=0)
+                        minmin_majority = np.min(sample_c1,axis=0)
+                    else:
+                        maxmax_minority = np.max(sample_c1,axis=0)
+                        minmin_minority = np.min(sample_c1,axis=0)
+
+                        maxmax_majority = np.max(sample_c2,axis=0)
+                        minmin_majority = np.min(sample_c2,axis=0)
+
+                    denom_maj = (maxmax_majority-minmin_majority)
+                    denom_min = (maxmax_minority-minmin_minority)
+
+                    n_d_min = numer/denom_min
+                    n_d_maj = numer/denom_maj
+
+                    n_d_min[np.isinf(n_d_min)]=0
+                    n_d_min[np.isnan(n_d_min)]=0 
 
+                    n_d_maj[np.isinf(n_d_maj)]=0
+                    n_d_maj[np.isnan(n_d_maj)]=0 
 
-                n_d = numer/denom
+                    f2_min = np.prod(n_d_min)
+                    f2_maj = np.prod(n_d_maj)
+
+                    f2s.append([f2_maj,f2_min])
+                else:
+                    maxmax = np.max([np.max(sample_c1,axis=0),np.max(sample_c2,axis=0)],axis=0)
+                    minmin = np.min([np.min(sample_c1,axis=0),np.min(sample_c2,axis=0)],axis=0)
+                    denom=(maxmax - minmin)
+
+
+                    n_d = numer/denom
                
-                n_d[np.isinf(n_d)]=0
-                n_d[np.isnan(n_d)]=0
+                    n_d[np.isinf(n_d)]=0
+                    n_d[np.isnan(n_d)]=0
                 
-                f2 = np.prod(n_d)
-                f2s.append(f2)
+                    f2 = np.prod(n_d)
+                    f2s.append(f2)
 
         return f2s
 
+    def __F3_counter(self,t_X,maxmin,minmax):
+        overlap_count = []
+        #for every feature
+        for k in  range(len(t_X)):
+            feature = t_X[k]
+            count = 0
 
-    #only for datasets with no categorical features
-    def F3(self):
+            #for every sample
+            for value in feature:
+                #check if the sample is inside the bounds
+                if(value>=maxmin[k] and value<=minmax[k]):
+                    count+=1
+            overlap_count.append(count)
+        return overlap_count
+
+    def F3(self,imb=False):
         '''
         Calculates the F3 measure defined in [1]. 
         Uses One vs One method to handle multiclass datasets.
         -----
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
+        -----
         Returns:
         f3s (array): The value of f3 measure for each one vs one combination of classes.
         -----
         References:
 
         [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How com-
         plex is your classification problem? a survey on measuring classification
         complexity. ACM Computing Surveys (CSUR) 52(5):1-34
         '''
         f3s=[]
-        #one vs one method
-        for i in range(len(self.class_inxs)):
-            for j in range(i+1,len(self.class_inxs)):
-                sample_c1 = self.X[self.class_inxs[i]]
-                sample_c2 = self.X[self.class_inxs[j]]
-
-                maxmin = np.max([np.min(sample_c1,axis=0),np.min(sample_c2,axis=0)],axis=0)
-                minmax = np.min([np.max(sample_c1,axis=0),np.max(sample_c2,axis=0)],axis=0)
-
-                transpose_X = np.transpose(self.X)
-
-                overlap_count = []
-
-                #for every feature
-                for k in  range(len(transpose_X)):
-                    feature = transpose_X[k]
-                    count = 0
-
-                    #for every sample
-                    for value in feature:
-                        #check if the sample is inside the bounds
-                        if(value>=maxmin[k] and value<=minmax[k]):
-                            count+=1
-                    overlap_count.append(count)
-            
-
-                min_overlap = min(overlap_count)
-                f3 = min_overlap/(len(self.X[self.class_inxs[i]])+len(self.X[self.class_inxs[j]]))
-                f3s.append(f3)
-        return f3s
-    
-
-    def F3_imb(self):
-        f3s=[]
 
 
         #one vs one method
         for i in range(len(self.class_inxs)):
             for j in range(i+1,len(self.class_inxs)):
                 sample_c1 = self.X[self.class_inxs[i]]
                 sample_c2 = self.X[self.class_inxs[j]]
 
                 maxmin = np.max([np.min(sample_c1,axis=0),np.min(sample_c2,axis=0)],axis=0)
                 minmax = np.min([np.max(sample_c1,axis=0),np.max(sample_c2,axis=0)],axis=0)
 
+                transpose_sample_c1 = np.transpose(sample_c1)
+                transpose_sample_c2 = np.transpose(sample_c2)
                 transpose_X = np.transpose(self.X)
+                
 
-                overlap_count = []
+                if(imb):
+                    
+                    c1_count = self.__F3_counter(transpose_sample_c1,maxmin,minmax)
+                    c2_count = self.__F3_counter(transpose_sample_c2,maxmin,minmax)
+                    if(len(sample_c1)>len(sample_c2)):
+                        maj_count = c1_count
+                        min_count = c2_count
+                        len_min = len(sample_c2)
+                        len_maj = len(sample_c1)
+                    else:
+                        maj_count = c2_count
+                        min_count = c1_count
+                        len_min = len(sample_c1)
+                        len_maj = len(sample_c2)
+
+                    min_overlap_min = min(min_count)
+                    min_overlap_maj = min(maj_count)
+                    f3_min = min_overlap_min/len_min
+                    f3_maj = min_overlap_maj/len_maj
 
-                #for every feature
-                for k in  range(len(transpose_X)):
-                    feature = transpose_X[k]
-                    count = 0
-
-                    #for every sample
-                    for value in feature:
-                        #check if the sample is inside the bounds
-                        if(value>=maxmin[k] and value<=minmax[k]):
-                            count+=1
-                    overlap_count.append(count)
-            
+                    f3 = [f3_maj,f3_min]
 
-                min_overlap = min(overlap_count)
-                f3 = min_overlap/(len(self.X[self.class_inxs[i]])+len(self.X[self.class_inxs[j]]))
+                else:
+                    overlap_count = self.__F3_counter(transpose_X,maxmin,minmax)
+                    min_overlap = min(overlap_count)
+                    f3 = min_overlap/(len(self.X[self.class_inxs[i]])+len(self.X[self.class_inxs[j]]))
                 f3s.append(f3)
         return f3s
-    #only for datasets with no categorical features
-    def F4(self):
+    
+    
+
+    def F4(self,imb=False):
         '''
         Calculates the F4 measure defined in [1]. 
         Uses One vs One method to handle multiclass datasets.
         -----
+        Parameters:
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
+        -----
         Returns:
         f4s (array): The value of f4 measure for each one vs one combination of classes.
         -----
         References:
 
         [1] Lorena AC, Garcia LP, Lehmann J, Souto MC, Ho TK (2019) How com-
         plex is your classification problem? a survey on measuring classification
@@ -2174,16 +2162,16 @@
                 transpose_X = np.transpose(X)
 
                 #while there are still samples in X
                 while len(X)>0:
 
                     #check if one of the classes is not represented
                     if(len(sample_c1)==0 or len(sample_c2)==0):
-                        maxmin = np.full(len(X[1]),np.inf)
-                        minmax = np.full(len(X[1]),-np.inf)
+                        maxmin = np.full(len(X[0]),np.inf)
+                        minmax = np.full(len(X[0]),-np.inf)
                     else:
                         maxmin = np.max([np.min(sample_c1,axis=0),np.min(sample_c2,axis=0)],axis=0)
                         minmax = np.min([np.max(sample_c1,axis=0),np.max(sample_c2,axis=0)],axis=0)
 
                     overlap_count = []
                     inx_lists = []
 
@@ -2205,65 +2193,103 @@
                         
                     
                     #determine the feature with the least overlap
                     min_overlap = min(overlap_count)
                     min_inx = overlap_count.index(min_overlap)
                     min_overlap_inx = inx_lists[min_inx]
 
-
+                    
                     #remove that feature
                     valid_features = list(range(0,min_inx)) + list(range(min_inx+1,len(transpose_X)))
 
                     if(len(min_overlap_inx)==0 or len(valid_features)==0):
-                        break
+                        
+                        new_X = []
+                        new_y = []
+                    
+                        for inx in range(len(X)):
+                            if inx in min_overlap_inx:
+                                new_X.append(sample)
+                                new_y.append(y[inx])
+                        X = np.array(new_X)
+                        y = np.array(new_y)
+                        transpose_X = np.transpose(X)
+                        
+                        valid_inxs_c1 = []
+                        sample_c1 = []
+                        for inx in range(len(y)):
+                            if y[inx]==self.classes[i2]:
+                                valid_inxs_c1.append(inx)
+                                sample_c1.append(X[inx])
 
 
-                    
-                    
+                        valid_inxs_c2 = []
+                        sample_c2 = []
+                        for inx in range(len(y)):
+                            if y[inx]==self.classes[j2]:
+                                valid_inxs_c2.append(inx)
+                                sample_c2.append(X[inx])                        
+                        
+                        
+                        break
 
                     new_X = []
                     new_y = []
                     
 
 
-                    #create the new values for X and y after removing the feature and remove the samples that can correctly classified with just that feature
+                    #create the new values for X and y after removing the feature and remove the samples that can be correctly classified with just that feature
                     for inx in range(len(X)):
                        
                         if inx in min_overlap_inx:
                             sample = []
                             for ft in valid_features:
                                
                                 sample.append(X[inx,ft])
                             new_X.append(sample)
                             new_y.append(y[inx])
+                    
+
                     X = np.array(new_X)
                     y = np.array(new_y)
                     transpose_X = np.transpose(X)
                     
                     valid_inxs_c1 = []
                     sample_c1 = []
                     for inx in range(len(y)):
                         if y[inx]==self.classes[i2]:
                             valid_inxs_c1.append(inx)
                             sample_c1.append(X[inx])
+
+
                     valid_inxs_c2 = []
                     sample_c2 = []
                     for inx in range(len(y)):
                         if y[inx]==self.classes[j2]:
                             valid_inxs_c2.append(inx)
                             sample_c2.append(X[inx])
 
                     sample_c1 = np.array(sample_c1)
                     sample_c2 = np.array(sample_c2)
-                    
-                f4=len(min_overlap_inx)/(len(sample_c1_y)+len(sample_c2_y))
+                
+                
+
+                if(imb):
+                    if(len(sample_c2_y)>len(sample_c1_y)):
+                        f4_min = len(valid_inxs_c1)/len(sample_c1_y)
+                        f4_maj = len(valid_inxs_c2)/len(sample_c2_y)
+                    else:
+                        f4_min = len(valid_inxs_c2)/len(sample_c2_y)
+                        f4_maj = len(valid_inxs_c1)/len(sample_c1_y)
+                    f4 = [f4_maj,f4_min]
+                else:   
+                    f4=(len(valid_inxs_c1)+len(valid_inxs_c2))/(len(sample_c1_y)+len(sample_c2_y))
                 f4s.append(f4)
         return f4s
 
-
     
     def __class_overlap(self,class_samples,other_samples):
         '''
         Called by the input_noise function.
         Calculates the class overlap between two classes.
         -------
         Parameters:
@@ -2313,97 +2339,110 @@
                 total_count+=self.__class_overlap(sample_c1,sample_c2)
                 total_count+=self.__class_overlap(sample_c2,sample_c1)
 
                 ins.append(total_count/(len(X)*len(X[0])))
         return ins
 
     
-    def borderline(self,k=5):
+
+    
+    def borderline(self,k=5,imb=False):
         '''
         Calculates the borderline examples metric defined in [1].
 
         ------
         Parameters:
         k (int): The number of nearest neighbours to consider.
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         ------
         Returns:
         borderline (float): the percentage of borderline examples in the dataset.
         ------
         References:
 
         [1] Napiera la K, Stefanowski J, Wilk S (2010) Learning from imbalanced data
         in presence of noisy and borderline examples. In: International Conference
         on Rough Sets and Current Trends in Computing, Springer, pp 158-167
         
         '''
-        borderline_count=0
+        borderline_count = np.zeros(len(self.classes))
         for i in range(len(self.X)):
             count=self.__knn(i,copy.copy(self.dist_matrix[i]),k)
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             #check this
             if((sum(count)-count[cls_inx])>=2):
-                borderline_count+=1
-        borderline = borderline_count*100/len(self.X)
+                borderline_count[cls_inx]+=1
+        
+        if(imb):
+            borderline = np.divide(borderline_count,self.class_count)
+        else:
+            borderline = sum(borderline_count)/len(self.X)
+        
         return borderline
 
-    def deg_overlap(self,k=5):
+    def deg_overlap(self,k=5,imb=False):
         '''
         Calculates the degree of overlap metric defined in [1].
 
         ------
         Parameters:
         k (int): The number of nearest neighbours to consider.
+        imb (bool): If True the the values for minority and majority will both be returned individually, if False a single value for the whole dataset is returned
         ------
         Returns:
         deg_ov (float): The degree of overlap complexity measure.
         ------
         References:
 
         [1] Mercier M, Santos M, Abreu P, Soares C, Soares J, Santos J (2018)
         Analysing the footprint of classifiers in overlapped and imbalanced con-
         texts. In: International Symposium on Intelligent Data Analysis, Springer,
         pp 200-212
         '''
-        deg=0
+        deg= np.zeros(len(self.classes))
         for i in range(len(self.X)):
             count=self.__knn(i,copy.copy(self.dist_matrix[i]),k)
             cls_inx = np.where( self.classes == self.y[i])[0][0]
             if(count[cls_inx]!=k):
-                deg+=1
-        deg_ov = deg/len(self.X)
+                deg[cls_inx]+=1
+        
+        if(imb):
+            deg_ov = np.divide(deg,self.class_count)
+        else:
+            deg_ov = sum(deg)/len(self.X)
         return deg_ov
+    
+
+  
 
     # -*- coding: utf-8 -*-
 
 
 
-    def ONB_avg(self,dist_id = "manhattan"):
+    def ONB_avg(self):
 
         """
 
         ONB complexity metric differentiating (averaged) by class
 
-        dataset is the dataframe of the dataset that will be evaluated, where the last column is the class
-
-        dist_id is the type of distance metric that will be utilised (with "manhattan" as the default metric, but "euclidean" was also used in the study)
 
         """
         featu = pd.DataFrame(self.X) #feature part of the dataframe
         
         clas = pd.DataFrame(self.y) #class part of the dataframe
         
         clas.rename(columns = {0 : 'class'}, inplace = True)
         
         dataset = featu.join(clas)
 
         clas_dif = np.unique(clas) #array of the different clases in the dataset   
 
-        dist= 0 #DistanceMetric.get_metric(dist_id) #indicating which distance metric will be used    
+        
 
-        dtf_dist =  pd.DataFrame(dist.pairwise(featu)) #distance matrix as a dataframe    
+        dtf_dist =  pd.DataFrame(self.dist_matrix) #distance matrix as a dataframe    
 
         lista_el_cla = [] #empty list for the elements of each class
 
         el_cla = [] #empty list for the number of elements in each class
 
         for cla in clas_dif:
 
@@ -2425,15 +2464,15 @@
 
                 bolaslist=[] #empty list for the elements of the ball that covers the most instances for this iteration
 
                 for j in falta: #for each uncovered element
 
                     mininter = min(dtf_dist.loc[j,dataset["class"]!=cla]) #the biggest possible radius that does not cover elements from other classes is computed
 
-                    s=dtf_dist.iloc[j, falta]<mininter #the instances included in that ball are obtained
+                    s=dtf_dist.iloc[j, falta]<=mininter #the instances included in that ball are obtained
 
                     bolas = [falta.index(i) for i in s[s].index.values] #said instances are saved as a list
 
                     if len(bolas) > len(bolaslist): #if this ball covers more instances than the previous best candidate
 
                         bolaslist = bolas #its covered elements are saved
 
@@ -2449,24 +2488,21 @@
 
         return avg / len(clas_dif) #return the average of the ratios between the number of balls necessary to cover the points of a class and the number of points of that class
 
 
 
 
 
-    def ONB_tot(self, dist_id = "manhattan"):
+    def ONB_tot(self):
 
         """
 
         ONB complexity metric using the total number of balls
 
-        dataset is the dataframe of the dataset that will be evaluated, where the last column is the class
-
-        dist_id is the type of distance metric that will be utilised (with "manhattan" as the default metric, but "euclidean" was also used in the study)
-
+    
         """
         
         featu = pd.DataFrame(self.X) #feature part of the dataframe
         
         clas = pd.DataFrame(self.y) #class part of the dataframe
         
         clas.rename(columns = {0 : 'class'}, inplace = True)
@@ -2474,17 +2510,17 @@
         dataset = featu.join(clas)
 
         
         tam = dataset.shape[0] #number of instances of the dataframe
 
         clas_dif = np.unique(clas) #array of the different clases in the dataset   
 
-        dist= 0 #DistanceMetric.get_metric(dist_id) #indicating which distance metric will be used     
+    
 
-        dtf_dist = pd.DataFrame(dist.pairwise(featu)) #distance matrix as a dataframe   
+        dtf_dist = pd.DataFrame(self.dist_matrix) #distance matrix as a dataframe   
 
         lista_el_cla = [] #empty list for the elements of each class
 
         for cla in clas_dif:
 
             lista_el_cla = lista_el_cla + [list(dataset.loc[dataset["class"]==cla].index.values)] #add the elements of each class
 
@@ -2500,15 +2536,15 @@
 
                 bolaslist=[] #empty list for the elements of the ball that covers the most instances for this iteration
 
                 for j in falta: #for each uncovered element
 
                     mininter = min(dtf_dist.loc[j,dataset["class"]!=cla]) #the biggest possible radius that does not cover elements from other classes is computed
 
-                    s=dtf_dist.iloc[j, falta]<mininter #the instances included in that ball are obtained
+                    s=dtf_dist.iloc[j, falta]<=mininter #the instances included in that ball are obtained
 
                     bolas = [falta.index(i) for i in s[s].index.values] #said instances are saved as a list
 
                     if len(bolas) > len(bolaslist): #if this ball covers more instances than the previous best candidate
 
                         bolaslist = bolas #its covered elements are saved
```

### Comparing `pycol_complexity-0.0.4/pycol_complexity.egg-info/PKG-INFO` & `pycol_complexity-0.0.5/pycol_complexity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycol_complexity
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Package for complexity measures
 Home-page: https://github.com/DiogoApostolo/pycol
 Author: Diogo Apostolo
 Author-email: ogoid.478@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycol_complexity-0.0.4/setup.cfg` & `pycol_complexity-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7963 6f6c 5f63 6f6d 706c 6578   = pycol_complex
 00000020: 6974 790d 0a76 6572 7369 6f6e 203d 2030  ity..version = 0
-00000030: 2e30 2e34 0d0a 6175 7468 6f72 203d 2044  .0.4..author = D
+00000030: 2e30 2e35 0d0a 6175 7468 6f72 203d 2044  .0.5..author = D
 00000040: 696f 676f 2041 706f 7374 6f6c 6f0d 0a61  iogo Apostolo..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6f67  uthor_email = og
 00000060: 6f69 642e 3437 3840 676d 6169 6c2e 636f  oid.478@gmail.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2050 7974 686f 6e20 5061 636b 6167 6520   Python Package 
 00000090: 666f 7220 636f 6d70 6c65 7869 7479 206d  for complexity m
 000000a0: 6561 7375 7265 730d 0a6c 6f6e 675f 6465  easures..long_de
```

