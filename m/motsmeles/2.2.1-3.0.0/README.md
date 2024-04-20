# Comparing `tmp/motsmeles-2.2.1.tar.gz` & `tmp/motsmeles-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motsmeles-2.2.1.tar", max compression
+gzip compressed data, was "motsmeles-3.0.0.tar", max compression
```

## Comparing `motsmeles-2.2.1.tar` & `motsmeles-3.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      930 2024-04-08 09:40:56.625407 motsmeles-2.2.1/README.md
--rw-r--r--   0        0        0     6146 2024-04-15 16:20:29.263152 motsmeles-2.2.1/motsmeles.py
--rw-r--r--   0        0        0      402 2024-04-15 16:20:47.782644 motsmeles-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 motsmeles-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      748 2024-04-20 11:07:18.603141 motsmeles-3.0.0/README.md
+-rw-r--r--   0        0        0     6107 2024-04-20 11:10:08.408837 motsmeles-3.0.0/motsmeles.py
+-rw-r--r--   0        0        0      402 2024-04-20 11:08:49.715339 motsmeles-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 motsmeles-3.0.0/PKG-INFO
```

### Comparing `motsmeles-2.2.1/motsmeles.py` & `motsmeles-3.0.0/motsmeles.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,148 +2,148 @@
 import numpy
 import pandas as pd
 import random
 import sys
 import builtins
 
 
-alphabet="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
-# TODO remplacer sensPossible par allow_inverse, allow_diagonal
+ALPHABET="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
+debug_mode = hasattr(sys, 'gettrace') and sys.gettrace()
+# 1TODO remplacer sensPossible par allow_inverse, allow_diagonal
 class GenerateError(Exception):
     pass
+DEFAULT_WIDTH=10
+DEFAULT_HEIGHT=10
 def generate(
-    mots,
-    dimensionsx=10,
-    dimensionsy=10,
+    words,
+    width=DEFAULT_WIDTH,
+    height=DEFAULT_HEIGHT,
     #sensPossible={"b","d","h","g","bg","bd","hd","hg"}
     no_diagonal=False,
     no_reverse=False,
     ):
 
-    sensPossible={"b","d","h","g","bg","bd","hd","hg"}
+    possible_directions={"b","d","h","g","bg","bd","hd","hg"}
     if no_diagonal:
-        sensPossible -= {"bg","bd","hd","hg"}
+        possible_directions -= {"bg","bd","hd","hg"}
     if no_reverse:
-        sensPossible -= {"h","g","hd","bg"}
+        possible_directions -= {"h","g","hd","bg"}
         
-    grille = numpy.empty((dimensionsy, dimensionsx), dtype=str)
-    answers = pd.DataFrame(columns=['mot', 'sens', 'x', 'y','xh', 'yh'])
+    grid = numpy.empty((height, width), dtype=str)
+    answers = pd.DataFrame(columns=['word', 'direction', 'x1', 'y1','x2', 'y2'])
     
     def _generate():
         # 1. Placer les mots
-        for mot in mots:
+        for word in words:
             #Vérification du mot
-            mot = mot.upper()
-            for letter in mot:
-                assert letter in alphabet,f"Mot invalid: {mot}"
-            dim = min(dimensionsx, dimensionsy)
-            assert len(mot) <= dim, f"Mot trop long: {mot}"
+            word = word.upper()
+            for letter in word:
+                assert letter in ALPHABET,f"Mot invalid: {word}"
+            dim = min(width, height)
+            assert len(word) <= dim, f"Mot trop long: {word}"
             
             #choix de rangey, rangex, addy, addx
-            sens = random.choice(tuple(sensPossible))
-            if "h" in sens:
+            direction = random.choice(tuple(possible_directions))
+            if "h" in direction:
 
-                rangey=range((dimensionsy-len(mot))+1)
+                rangey=range((height-len(word))+1)
                 addy=1
-            elif "b" in sens:
-                rangey=range(len(mot)-1,dimensionsy)
+            elif "b" in direction:
+                rangey=range(len(word)-1,height)
                 addy=-1
             else:
-                rangey=range(dimensionsy)
+                rangey=range(height)
                 addy=0
-            if "d" in sens:
-                rangex=range((dimensionsx-len(mot))+1)
+            if "d" in direction:
+                rangex=range((width-len(word))+1)
                 addx=1
-            elif "g" in sens:
-                rangex=range(len(mot)-1,dimensionsx)
+            elif "g" in direction:
+                rangex=range(len(word)-1,width)
                 addx=-1
             else:
-                rangex=range(dimensionsx)
+                rangex=range(width)
                 addx=0
 
             choixcoordonnees=[]
-            for y in rangey:
+            for y1 in rangey:
 
-                for x in rangex:
+                for x1 in rangex:
 
-                    xh,yh=x,y #create copy of x,y
+                    x2,y2=x1,y1 #create copy of x,y
                     Break=False
-                    for letter in mot:
+                    for letter in word:
 
                         #Verify if it's a good emplacement mean: verify if it's blank OR filled with the right letter
-                        if grille[yh,xh]!="":
-                            if grille[yh,xh]!=letter:
+                        if grid[y2,x2]!="":
+                            if grid[y2,x2]!=letter:
                                 break
-                        xh+=addx
-                        yh+=addy
+                        x2+=addx
+                        y2+=addy
                     else:               
-                        choixcoordonnees.append((y,x))
+                        choixcoordonnees.append((y1,x1))
             if not choixcoordonnees: 
                 
-                raise GenerateError(f"Impossible de placer le mot {mot}")
-            y,x=random.choice(choixcoordonnees)
+                raise GenerateError(f"Unable to place the word {word}")
+            y1,x1=random.choice(choixcoordonnees)
             #xh,yh=coordonnees(index)
-            xh,yh=x,y
-            for letter in mot:
-                grille[yh,xh]=letter # a big debug: replace with yh, xh
-
-                xh+=addx
-                yh+=addy
-            answers.loc[len(answers)] = {'mot': mot, 'sens': sens, 'x': x, 'y': y,'xh': xh, 'yh': yh}
+            x2,y2=x1,y1
+            for letter in word:
+                grid[y2,x2]=letter # a big debug: replace with yh, xh
+
+                x2+=addx
+                y2+=addy
+            answers.loc[len(answers)] = {'word': word, 'direction': direction, 'x1': x1, 'y1': y1,'x2': x2, 'y2': y2}
 
         def verifsens(addx,addy):
 
-            grille[y,x]=letter 
-            mot=letter
-            xh,yh=x,y
-            while 0<=xh<dimensionsx and 0<=yh<dimensionsy:
-                if grille[yh,xh]=="":
+            grid[y1,x1]=letter 
+            word=letter
+            xh,yh=x1,y1
+            while 0<=xh<width and 0<=yh<height:
+                if grid[yh,xh]=="":
                     return True
-                if mot in mots:
+                if word in words:
                     return False
                 #lettrespossible.append(letter)
-                mot+=grille[yh,xh]
+                word+=grid[yh,xh]
                 xh+=addx
                 yh+=addy 
             return True
 
-        for y in range(dimensionsy):
-            for x in range(dimensionsx):
+        for y1 in range(height):
+            for x1 in range(width):
                 for _ in range(1):
-                    xs,ys=x,y
+                    xs,ys=x1,y1
                     lettrespossible=[]
-                    if grille[y,x]:
+                    if grid[y1,x1]:
                         #print(repr(letters[y,x]))
                         break
-                    for letter in alphabet:
+                    for letter in ALPHABET:
                         for addx,addy in [(0,1),(1,1),(1,0),(1,-1),(0,-1),(-1,-1),(-1,0),(-1,1)]:
                             if not verifsens(addx,addy):
                                 lettrespossible.append(letter)
                                 break
                         else:
                             lettrespossible.append(letter)
                     if not lettrespossible:
-                        raise GenerateError(f"Impossible de placer une lettre à {x},{y}")
-                    grille[y,x]=random.choice(lettrespossible)
-                if grille[ys,xs] not in alphabet:
+                        raise GenerateError(f"Unable to place {x1},{y1}")
+                    grid[y1,x1]=random.choice(lettrespossible)
+                if grid[ys,xs] not in ALPHABET:
                     pass
             
-        return grille,answers
+        return grid,answers
+    errs=[]
     for _ in range(10):
         try:
             return _generate()
-        except GenerateError:
-            pass
-    
-    # for y in range(dimensionsy):
-    #     for x in range(dimensionsx):
-    #         if letters[y,x]=="":
-    #             pass
-                #letters[y,x]=random.choice(alphabet)
-    return grille,answers
+        except GenerateError as err:
+            if debug_mode:
+                print(err)
+    else:
+        raise GenerateError("Unable to generate a grid")
 
 def print(grille,file=sys.stdout):
     for y in range(len(grille)):
         for x in range(len(grille[0])):
             builtins.print(grille[y,x],end="",file=file)
         builtins.print(file=file)
 
@@ -153,29 +153,29 @@
 def save_answers(answers,file="motsmeles-answers.csv"):
     answers.to_csv(file,index=False)
         
 def main():
     import argparse
     
     parser = argparse.ArgumentParser(description="générateur de mots mêlés")
-    parser.add_argument("mots", nargs="+", help="les mots à placer")
-    parser.add_argument("-x", "--dimensionsx", type=int, default=10, help="la largeur de la grille")
-    parser.add_argument("-y", "--dimensionsy", type=int, default=10, help="la hauteur de la grille")
+    parser.add_argument("words", nargs="+", help="les mots à placer")
+    parser.add_argument("-W", "--width", type=int, default=DEFAULT_WIDTH, help="the width of the grid")
+    parser.add_argument("-H", "--height", type=int, default=DEFAULT_HEIGHT, help="the height of the grid")
     #parser.add_argument("-o", "--output-file", help="fichier de sortie")
-    parser.add_argument("-d","--no-diagonal", action="store_true", help="ne pas autoriser les mots en diagonale")
-    parser.add_argument("-r","--no-reverse", action="store_true", help="ne pas autoriser les mots en sens inverse")
+    parser.add_argument("-d","--no-diagonal", action="store_true", help="no diagonal words")
+    parser.add_argument("-r","--no-reverse", action="store_true", help="no reverse words")
     args=parser.parse_args()
-    grille,answers=generate(
-        args.mots,
-        args.dimensionsx,
-        args.dimensionsy,
+    grid,answers=generate(
+        args.words,
+        args.width,
+        args.height,
         no_diagonal=args.no_diagonal,
         no_reverse=args.no_reverse,
         )
-    print(grille)
+    print(grid)
     builtins.print(answers)
 if __name__=="__main__":
     main()
```

