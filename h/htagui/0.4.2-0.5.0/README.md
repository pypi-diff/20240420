# Comparing `tmp/htagui-0.4.2.tar.gz` & `tmp/htagui-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.4.2.tar", max compression
+gzip compressed data, was "htagui-0.5.0.tar", max compression
```

## Comparing `htagui-0.4.2.tar` & `htagui-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1065 2024-04-18 16:52:00.346388 htagui-0.4.2/LICENSE
--rw-r--r--   0        0        0     7636 2024-04-18 16:52:00.346388 htagui-0.4.2/README.md
--rw-r--r--   0        0        0      330 2024-04-18 16:52:00.618389 htagui-0.4.2/htagui/__init__.py
--rw-r--r--   0        0        0     1363 2024-04-18 16:52:00.346388 htagui-0.4.2/htagui/basics/__init__.py
--rw-r--r--   0        0        0    10564 2024-04-18 16:52:00.346388 htagui-0.4.2/htagui/basics/bases.py
--rw-r--r--   0        0        0     1364 2024-04-18 16:52:00.346388 htagui-0.4.2/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   655217 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/bulma/bases.py
--rw-r--r--   0        0        0     3444 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/common.py
--rw-r--r--   0        0        0     3037 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/flex.py
--rw-r--r--   0        0        0      771 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/form.py
--rw-r--r--   0        0        0     3552 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/ifields.py
--rw-r--r--   0        0        0     1367 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     7742 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     8884 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-04-18 16:52:00.350388 htagui-0.4.2/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-18 16:52:00.618389 htagui-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8869 1970-01-01 00:00:00.000000 htagui-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-20 10:33:41.180238 htagui-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8119 2024-04-20 10:33:41.180238 htagui-0.5.0/README.md
+-rw-r--r--   0        0        0      330 2024-04-20 10:33:41.416238 htagui-0.5.0/htagui/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/all.py
+-rw-r--r--   0        0        0      750 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/basics/__init__.py
+-rw-r--r--   0        0        0    11061 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/basics/bases.py
+-rw-r--r--   0        0        0      771 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   656090 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     3444 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/common.py
+-rw-r--r--   0        0        0     3281 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/flex.py
+-rw-r--r--   0        0        0      771 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/form.py
+-rw-r--r--   0        0        0     3795 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/ifields.py
+-rw-r--r--   0        0        0      746 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/md/__init__.py
+-rw-r--r--   0        0        0    10475 2024-04-20 10:33:41.180238 htagui-0.5.0/htagui/md/bases.py
+-rw-r--r--   0        0        0      774 2024-04-20 10:33:41.184238 htagui-0.5.0/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     8221 2024-04-20 10:33:41.184238 htagui-0.5.0/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     8884 2024-04-20 10:33:41.184238 htagui-0.5.0/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-04-20 10:33:41.184238 htagui-0.5.0/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-20 10:33:41.416238 htagui-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 htagui-0.5.0/PKG-INFO
```

### Comparing `htagui-0.4.2/LICENSE` & `htagui-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.4.2/README.md` & `htagui-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -76,24 +76,34 @@
 
 
 ```python
 import htagui as ui
 self <= ui.Input(_value="my value", _name="myfield", _class="myclass", _required=True )
 ```
 
+Availables managed `type`s (setted with `_type`) params:
+ * `text` : the default one (if omitted): an input text
+ * `checkbox` : a checkbox
+ * `radio` : a radio button (non sense : use ui.Radios or uiIRadios !)
+ * `range` : a slider/range
+
+For `text`: a special field "_label" will set the html "placeholder" attribut.
+
 ## Object Textarea
 
 A simple surcharge of Tag.textarea(...), to define a css class 
 
 
 ```python
 import htagui as ui
 self <= ui.Textarea("my value", _name="myfield", _class="myclass", _required=True )
 ```
 
+A special field "_label" will set the html "placeholder" attribut.
+
 ## Object Spinner
 
 A spinner object.
 
 ```python
 import htagui as ui
 self <= ui.Spinner()
@@ -188,30 +198,29 @@
 Note that, there can be only one dialog at a time (except toast notification)
 
 ```python
 import htagui as ui
 dialog = ui.Dialog( self )
 ```
 
-### method dialog.alert(obj)
+### method dialog.alert(obj, size:float=None)
 
 (like js window.alert(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able)
 
+size is a float to force the percent of width on the dialog box. If None, it will use the default from the ui used.
+
 ### method dialog.confirm(obj, cbresponse=lambda bool:bool)
 
 (like js window.confirm(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able), and let the user click on Yes|No buttons, which will call the cbresponse callback with True or False ...
 
 ### method dialog.prompt(value:str, title, cbresponse=lambda val:val)
 
 (like js window.prompt(...)) Display a modal dialog letting the user edit the `value` in an Input box, with a `title` (title must be str'able). When the user click the OK button the value is sent in the callback cbresponse. (clicking the cancel button does nothing, except close the dialog)
 
 
-### method dialog.box(obj,size:float=0.5)
-
-Like dialog.alert(), but display modal dialog box containing the object 'obj' (obj must be str'able), which takes 50% of size.
 
 ### method dialog.notify(obj, time=2000)
 
 Display a toast message (notification), in the right-bottom ... during 2000 ms.
 (currently toast messages are not stacked)
 
 ### method dialog.pop(obj, xy:tuple)
@@ -226,17 +235,21 @@
     "menu1": lambda: dialog.notify("menu1"),
     "menu2": lambda: dialog.notify("menu2"),
     "menu3": lambda: dialog.notify("menu3"),
 }  
 self <= ui.Button("pop menu", _onclick=lambda ev: dialog.pop( ui.Menu(entries) ,(ev.clientX,ev.clientY)) )
 ```
 
-### method dialog.drawer(obj, mode="left", size:float=0.5)
+### method dialog.drawer(obj, mode="left")
+
+Display a drawer, in the left-side. mode can be left,right,top,bottom.
+
+### method dialog.page(obj=None)
 
-Display a drawer, in the left-side, which takes 50% of the page.
+Display a full page 'obj', or remove page if obj is None. (note that ui.close() does not close the page) 
 
 ### method dialog.block(obj=None)
 
 Display a modal dialog box containing the object 'obj'. But the dialog is not closable, so be sure to provide a way to close it.
 
 ### method dialog.close()
```

### Comparing `htagui-0.4.2/htagui/basics/bases.py` & `htagui-0.5.0/htagui/basics/bases.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # #############################################################################
 
 from htag import Tag
 from ..form import Form
 from ..common import ensuredict,ListOrDict
 
 CSS="""
+
 html,body {
     width:100%;
     font-family: ubuntu;
     padding:0px;
     margin:0px;
 }
 
@@ -26,29 +27,14 @@
     border-radius:6px;
     padding:10px;
     margin:1px;
     cursor:pointer;
     font-family: ubuntu;
 }
 
-.button.red {
-    background: #F77;
-    color:white;
-}
-
-.button.green {
-    background: #7C7;
-    color:white;
-}
-
-.button.blue {
-    background: #77F;
-    color:white;
-}
-
 .button:hover {
     filter: brightness(0.95);
 }
 
 .input[type="text"] {
     font-family: ubuntu;
     padding:4px;
@@ -155,40 +141,52 @@
 
 class Input(Tag.input):
     statics=CSS
     def init(self,**a):
         self["class"].add("input")
         if not self.attrs.get("type"):
             self["type"]="text"
-
+        self["placeholder"] = self.attrs.get("label")
 
 class Textarea(Tag.textarea):
     statics=CSS
     def init(self,txt:str, **a):
         self["class"].add("textarea")
         self <= txt
 
+        self["placeholder"] = self.attrs.get("label")
+
 class Select(Tag.select):
     statics=CSS
     def init(self,options:ListOrDict, **a):
-        options=ensuredict(options)
+        self.options=ensuredict(options)
+        self.rerender( self.attrs.get("value") )
         self["class"].add("select")
-        for k,v in options.items():
-            self <= Tag.option(v,_value=k,_selected=(str(self.attrs.get("value"))==str(k)))
+
+    def rerender(self,value):
+        """ special method (see ifields), to rerender all the widget (to avoid to deal with js)"""
+        self.clear()
+        for k,v in self.options.items():
+            self <= Tag.option(v,_value=k,_selected=(str(value)==str(k)))
 
 
 class Radios(Tag.span):
     def init(self,options:ListOrDict, **a):
-        options = ensuredict(options)
-        for k,v in options.items():
+        self.options = ensuredict(options)
+        self.rerender( self.attrs.get("value",None) )
+
+    def rerender(self,value):
+        """ special method (see ifields), to rerender all the widget (to avoid to deal with js)"""
+        self.clear()
+        for k,v in self.options.items():
             ipt=Tag.input(
                 _type="radio",
                 _value=k,
                 _name=self.attrs.get("name",str(id(self))),             # need a name to be valid
-                _checked=(str(self.attrs.get("value",None))==str(k)),
+                _checked=(str(value)==str(k)),
                 _required=bool(self.attrs.get("required",None)),
                 _readonly=bool(self.attrs.get("readonly",None)),
                 _onchange=f"document.getElementById('{id(self)}').value='{k}';"
             )
             self <= Tag.div(Tag.label( ipt +" "+ v ))
 
 # class SelectButtons(Tag.span):
@@ -278,29 +276,35 @@
 
 
 class ModalBlock(Tag.div):
     def init(self,metatag,obj):
         modal=Tag.div( obj, _style="position:fixed;left:0px;right:0px;top:0px;bottom:0px;z-index:1001;    display:flex;align-items:center;justify-content:center;")
         self <= Voile() + modal
 
+class PopPage(Tag.div):
+    def init(self,metatag,obj):
+        self["style"].set("position","fixed")
+        self["style"].set("top","0px")
+        self["style"].set("bottom","0px")
+        self["style"].set("right","0px")
+        self["style"].set("left","0px")
+        self["style"].set("z-index","1000")
+        self["style"].set("background","white")
+        self <= obj
+
+
 class ModalAlert(ModalBlock):
-    def __init__(self,metatag,obj,pwidth="60%",pheight=None):
+    def __init__(self,metatag,obj,wsize:float=None):
+        if wsize is None: wsize=0.6
+        pwidth=f"{int(wsize*100)}%"
         bc = Tag.button("X",_onclick=metatag.stepevent(),_style="float:right;border-radius:50%;border:0px;cursor:pointer;background:white")
-        box = Tag.div( [bc,obj],_style=f"width:{pwidth};background:white;overflow-y: auto;background:white;border-radius:6px;box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;padding:10px",_onmousedown="event.stopPropagation();")
-        if pheight:
-            box["style"].set("height",pheight)
-        else:
-            box["style"].set("max-height","80%")
-                
+        box = Tag.div( [bc,obj],_style=f"width:{pwidth};max-height:80%;background:white;overflow-y: auto;background:white;border-radius:6px;box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;padding:10px",_onmousedown="event.stopPropagation();")
         ModalBlock.__init__(self,metatag,box)
         self.childs[1]["onmousedown"]=metatag.stepevent()
 
-class ModalBox(ModalAlert):
-    def __init__(self,metatag,obj,size:float=.6):
-        ModalAlert.__init__(self,metatag,obj,pwidth=f"{size*100}%",pheight=f"{size*100}%")
 
 class ModalConfirm(ModalAlert):
     def __init__(self,metatag,obj,cb):
         def call(ev):
             metatag.step()
             return cb( ev.target.val )
          
@@ -342,15 +346,15 @@
     def init(self,metatag,obj,xy:tuple):
         x,y=xy
         self <= Voile(_onmousedown=metatag.stepevent())
         self <= Tag.div( obj ,_style=f"position:fixed;top:{y}px;left:{x}px;z-index:1001;background:white")
 
 class Toast(Tag.div):
     def init(self,main_non_used,obj,timeout=1000):
-        self <= Tag.div(obj,_style="position:fixed;right:10px;bottom:10px;z-index:1001;background:white;padding:10px;border:2px solid black")
+        self <= Tag.div(obj,_style="position:fixed;right:10px;bottom:10px;z-index:1001;background:white;padding:10px;border:2px solid black;border-radius:10px;min-width:200px")
         self.js="setTimeout( function() {self.remove()} , %s)" % timeout
 
 ######################################################################################
 
 
 
 class Tabs(Tag.div):
```

### Comparing `htagui-0.4.2/htagui/bulma/bases.py` & `htagui-0.5.0/htagui/bulma/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -40524,429 +40524,483 @@
 0009e4b0: 7474 7273 5b22 7479 7065 225d 3d22 7465  ttrs["type"]="te
 0009e4c0: 7874 220a 2020 2020 2020 2020 0a20 2020  xt".        .   
 0009e4d0: 2020 2020 2069 6620 7365 6c66 2e61 7474       if self.att
 0009e4e0: 7273 2e67 6574 2822 7479 7065 2229 3d3d  rs.get("type")==
 0009e4f0: 2274 6578 7422 3a0a 2020 2020 2020 2020  "text":.        
 0009e500: 2020 2020 7365 6c66 5b22 636c 6173 7322      self["class"
 0009e510: 5d2e 6164 6428 2269 6e70 7574 2229 0a0a  ].add("input")..
-0009e520: 636c 6173 7320 5465 7874 6172 6561 2854  class Textarea(T
-0009e530: 6167 2e74 6578 7461 7265 6129 3a0a 2020  ag.textarea):.  
-0009e540: 2020 7374 6174 6963 733d 4255 4c4d 410a    statics=BULMA.
-0009e550: 2020 2020 6465 6620 696e 6974 2873 656c      def init(sel
-0009e560: 662c 7478 743a 7374 722c 2a2a 6129 3a0a  f,txt:str,**a):.
-0009e570: 2020 2020 2020 2020 7365 6c66 5b22 636c          self["cl
-0009e580: 6173 7322 5d2e 6164 6428 2274 6578 7461  ass"].add("texta
-0009e590: 7265 6122 290a 2020 2020 2020 2020 7365  rea").        se
-0009e5a0: 6c66 203c 3d20 7478 740a 0a63 6c61 7373  lf <= txt..class
-0009e5b0: 2042 7574 746f 6e28 5461 672e 6275 7474   Button(Tag.butt
-0009e5c0: 6f6e 293a 0a20 2020 2073 7461 7469 6373  on):.    statics
-0009e5d0: 3d20 4255 4c4d 410a 2020 2020 6465 6620  = BULMA.    def 
-0009e5e0: 696e 6974 2873 656c 662c 7469 746c 652c  init(self,title,
-0009e5f0: 2a2a 6129 3a0a 2020 2020 2020 2020 7365  **a):.        se
-0009e600: 6c66 203c 3d20 7469 746c 650a 2020 2020  lf <= title.    
-0009e610: 2020 2020 7365 6c66 5b22 636c 6173 7322      self["class"
-0009e620: 5d2e 6164 6428 2262 7574 746f 6e22 290a  ].add("button").
-0009e630: 0a63 6c61 7373 2056 6f69 6c65 2854 6167  .class Voile(Tag
-0009e640: 2e64 6976 293a 200a 2020 2020 7374 6174  .div): .    stat
-0009e650: 6963 733d 2042 554c 4d41 0a20 2020 2064  ics= BULMA.    d
-0009e660: 6566 2069 6e69 7428 7365 6c66 2c2a 2a61  ef init(self,**a
-0009e670: 293a 0a20 2020 2020 2020 2073 656c 665b  ):.        self[
-0009e680: 2273 7479 6c65 225d 2e73 6574 2822 706f  "style"].set("po
-0009e690: 7369 7469 6f6e 222c 2266 6978 6564 2229  sition","fixed")
-0009e6a0: 0a20 2020 2020 2020 2073 656c 665b 2273  .        self["s
-0009e6b0: 7479 6c65 225d 2e73 6574 2822 746f 7022  tyle"].set("top"
-0009e6c0: 2c22 3070 7822 290a 2020 2020 2020 2020  ,"0px").        
-0009e6d0: 7365 6c66 5b22 7374 796c 6522 5d2e 7365  self["style"].se
-0009e6e0: 7428 2262 6f74 746f 6d22 2c22 3070 7822  t("bottom","0px"
-0009e6f0: 290a 2020 2020 2020 2020 7365 6c66 5b22  ).        self["
-0009e700: 7374 796c 6522 5d2e 7365 7428 2272 6967  style"].set("rig
-0009e710: 6874 222c 2230 7078 2229 0a20 2020 2020  ht","0px").     
-0009e720: 2020 2073 656c 665b 2273 7479 6c65 225d     self["style"]
-0009e730: 2e73 6574 2822 6c65 6674 222c 2230 7078  .set("left","0px
-0009e740: 2229 0a20 2020 2020 2020 2073 656c 665b  ").        self[
-0009e750: 2273 7479 6c65 225d 2e73 6574 2822 7a2d  "style"].set("z-
-0009e760: 696e 6465 7822 2c22 3130 3030 2229 0a20  index","1000"). 
-0009e770: 2020 2020 2020 2073 656c 665b 2273 7479         self["sty
-0009e780: 6c65 225d 2e73 6574 2822 6261 636b 6772  le"].set("backgr
-0009e790: 6f75 6e64 222c 2223 4343 4322 290a 2020  ound","#CCC").  
-0009e7a0: 2020 2020 2020 7365 6c66 5b22 7374 796c        self["styl
-0009e7b0: 6522 5d2e 7365 7428 226f 7061 6369 7479  e"].set("opacity
-0009e7c0: 222c 2230 2e35 2229 0a0a 0a0a 636c 6173  ","0.5")....clas
-0009e7d0: 7320 4d65 6e75 2854 6167 2e61 7369 6465  s Menu(Tag.aside
-0009e7e0: 293a 0a20 2020 2064 6566 2069 6e69 7428  ):.    def init(
-0009e7f0: 7365 6c66 2c65 6e74 7269 6573 3a64 6963  self,entries:dic
-0009e800: 7429 3a0a 2020 2020 2020 2020 7365 6c66  t):.        self
-0009e810: 5b22 636c 6173 7322 5d2e 6164 6428 226d  ["class"].add("m
-0009e820: 656e 7522 290a 2020 2020 2020 2020 6465  enu").        de
-0009e830: 6620 6361 6c6c 2865 7629 3a0a 2020 2020  f call(ev):.    
-0009e840: 2020 2020 2020 2020 2361 7574 6f20 636c          #auto cl
-0009e850: 6f73 6520 7468 6520 7569 2e44 6961 6c6f  ose the ui.Dialo
-0009e860: 672c 2069 6620 7468 6973 2022 4d65 6e75  g, if this "Menu
-0009e870: 2220 6973 2069 6e20 6120 4469 616c 6f67  " is in a Dialog
-0009e880: 2069 6e74 6572 6163 7469 6f6e 0a20 2020   interaction.   
-0009e890: 2020 2020 2020 2020 2023 2d2d 2d2d 2d2d           #------
-0009e8a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009e8b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009e8c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009e8d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009e8e0: 2d2d 0a20 2020 2020 2020 2020 2020 2063  --.            c
-0009e8f0: 7572 7265 6e74 203d 2073 656c 662e 7061  urrent = self.pa
-0009e900: 7265 6e74 0a20 2020 2020 2020 2020 2020  rent.           
-0009e910: 2077 6869 6c65 2063 7572 7265 6e74 2069   while current i
-0009e920: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0009e930: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0009e940: 6570 7228 6375 7272 656e 7429 2e73 7461  epr(current).sta
-0009e950: 7274 7377 6974 6828 223c 4469 616c 6f67  rtswith("<Dialog
-0009e960: 2764 6976 2229 3a20 2354 4f44 4f3a 206e  'div"): #TODO: n
-0009e970: 6f74 2074 6f70 2028 6361 6e20 646f 2062  ot top (can do b
-0009e980: 6574 7465 7229 0a20 2020 2020 2020 2020  etter).         
-0009e990: 2020 2020 2020 2020 2020 2063 7572 7265             curre
-0009e9a0: 6e74 2e63 6c6f 7365 2829 0a20 2020 2020  nt.close().     
-0009e9b0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0009e9c0: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-0009e9d0: 2020 2020 2063 7572 7265 6e74 203d 2063       current = c
-0009e9e0: 7572 7265 6e74 2e70 6172 656e 740a 2020  urrent.parent.  
-0009e9f0: 2020 2020 2020 2020 2020 232d 2d2d 2d2d            #-----
-0009ea00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009ea10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009ea20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009ea30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0009ea40: 2d2d 2d0a 0a20 2020 2020 2020 2020 2020  ---..           
-0009ea50: 2072 6574 7572 6e20 6576 2e74 6172 6765   return ev.targe
-0009ea60: 742e 6d65 7468 6f64 2829 0a0a 2020 2020  t.method()..    
-0009ea70: 2020 2020 7769 7468 2054 6167 2e75 6c28      with Tag.ul(
-0009ea80: 5f63 6c61 7373 3d22 6d65 6e75 2d6c 6973  _class="menu-lis
-0009ea90: 7422 2920 6173 2075 6c3a 0a20 2020 2020  t") as ul:.     
-0009eaa0: 2020 2020 2020 2066 6f72 206b 2c76 2069         for k,v i
-0009eab0: 6e20 656e 7472 6965 732e 6974 656d 7328  n entries.items(
-0009eac0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0009ead0: 2020 2075 6c20 2b3d 2054 6167 2e6c 6928     ul += Tag.li(
-0009eae0: 2054 6167 2e61 286b 292c 6d65 7468 6f64   Tag.a(k),method
-0009eaf0: 3d76 2c5f 6f6e 636c 6963 6b3d 6361 6c6c  =v,_onclick=call
-0009eb00: 290a 2020 2020 2020 2020 7365 6c66 3c3d  ).        self<=
-0009eb10: 756c 0a0a 636c 6173 7320 5370 696e 6e65  ul..class Spinne
-0009eb20: 7228 5461 672e 7370 616e 293a 0a20 2020  r(Tag.span):.   
-0009eb30: 2073 7461 7469 6373 3d22 2222 0a2e 7370   statics="""..sp
-0009eb40: 696e 6e65 7220 7b0a 2020 2020 7769 6474  inner {.    widt
-0009eb50: 683a 2033 3270 783b 0a20 2020 2068 6569  h: 32px;.    hei
-0009eb60: 6768 743a 2033 3270 783b 0a20 2020 2062  ght: 32px;.    b
-0009eb70: 6f72 6465 723a 2038 7078 2073 6f6c 6964  order: 8px solid
-0009eb80: 2023 3333 463b 0a20 2020 2062 6f72 6465   #33F;.    borde
-0009eb90: 722d 626f 7474 6f6d 2d63 6f6c 6f72 3a20  r-bottom-color: 
-0009eba0: 7472 616e 7370 6172 656e 743b 0a20 2020  transparent;.   
-0009ebb0: 2062 6f72 6465 722d 7261 6469 7573 3a20   border-radius: 
-0009ebc0: 3530 253b 0a20 2020 2064 6973 706c 6179  50%;.    display
-0009ebd0: 3a20 696e 6c69 6e65 2d62 6c6f 636b 3b0a  : inline-block;.
-0009ebe0: 2020 2020 626f 782d 7369 7a69 6e67 3a20      box-sizing: 
-0009ebf0: 626f 7264 6572 2d62 6f78 3b0a 2020 2020  border-box;.    
-0009ec00: 616e 696d 6174 696f 6e3a 2072 6f74 6174  animation: rotat
-0009ec10: 696f 6e20 3173 206c 696e 6561 7220 696e  ion 1s linear in
-0009ec20: 6669 6e69 7465 3b0a 2020 2020 7d0a 0a20  finite;.    }.. 
-0009ec30: 2020 2040 6b65 7966 7261 6d65 7320 726f     @keyframes ro
-0009ec40: 7461 7469 6f6e 207b 0a20 2020 2030 2520  tation {.    0% 
-0009ec50: 7b0a 2020 2020 2020 2020 7472 616e 7366  {.        transf
-0009ec60: 6f72 6d3a 2072 6f74 6174 6528 3064 6567  orm: rotate(0deg
-0009ec70: 293b 0a20 2020 207d 0a20 2020 2031 3030  );.    }.    100
-0009ec80: 2520 7b0a 2020 2020 2020 2020 7472 616e  % {.        tran
-0009ec90: 7366 6f72 6d3a 2072 6f74 6174 6528 3336  sform: rotate(36
-0009eca0: 3064 6567 293b 0a20 2020 207d 0a20 2020  0deg);.    }.   
-0009ecb0: 207d 2020 2020 2020 2020 200a 2222 2220   }         .""" 
-0009ecc0: 2020 200a 2020 2020 6465 6620 696e 6974     .    def init
-0009ecd0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0009ece0: 7365 6c66 5b22 636c 6173 7322 5d3d 2273  self["class"]="s
-0009ecf0: 7069 6e6e 6572 220a 0a0a 636c 6173 7320  pinner"...class 
-0009ed00: 5365 6c65 6374 2854 6167 2e73 656c 6563  Select(Tag.selec
-0009ed10: 7429 3a0a 2020 2020 7374 6174 6963 733d  t):.    statics=
-0009ed20: 4255 4c4d 410a 2020 2020 6465 6620 696e  BULMA.    def in
-0009ed30: 6974 2873 656c 662c 6f70 7469 6f6e 733a  it(self,options:
-0009ed40: 4c69 7374 4f72 4469 6374 2c20 2a2a 6129  ListOrDict, **a)
-0009ed50: 3a0a 2020 2020 2020 2020 6f70 7469 6f6e  :.        option
-0009ed60: 733d 656e 7375 7265 6469 6374 286f 7074  s=ensuredict(opt
-0009ed70: 696f 6e73 290a 2020 2020 2020 2020 7365  ions).        se
-0009ed80: 6c66 5b22 636c 6173 7322 5d2e 6164 6428  lf["class"].add(
-0009ed90: 2273 656c 6563 7422 290a 2020 2020 2020  "select").      
-0009eda0: 2020 666f 7220 6b2c 7620 696e 206f 7074    for k,v in opt
-0009edb0: 696f 6e73 2e69 7465 6d73 2829 3a0a 2020  ions.items():.  
-0009edc0: 2020 2020 2020 2020 2020 7365 6c66 203c            self <
-0009edd0: 3d20 5461 672e 6f70 7469 6f6e 2876 2c5f  = Tag.option(v,_
-0009ede0: 7661 6c75 653d 6b2c 5f73 656c 6563 7465  value=k,_selecte
-0009edf0: 643d 2828 7374 7228 7365 6c66 2e61 7474  d=((str(self.att
-0009ee00: 7273 2e67 6574 2822 7661 6c75 6522 2929  rs.get("value"))
-0009ee10: 3d3d 7374 7228 6b29 2929 290a 0a63 6c61  ==str(k))))..cla
-0009ee20: 7373 2052 6164 696f 7328 5461 672e 7370  ss Radios(Tag.sp
-0009ee30: 616e 293a 0a20 2020 2073 7461 7469 6373  an):.    statics
-0009ee40: 3d42 554c 4d41 0a20 2020 2064 6566 2069  =BULMA.    def i
-0009ee50: 6e69 7428 7365 6c66 2c6f 7074 696f 6e73  nit(self,options
-0009ee60: 3a4c 6973 744f 7244 6963 742c 202a 2a61  :ListOrDict, **a
-0009ee70: 293a 0a20 2020 2020 2020 206f 7074 696f  ):.        optio
-0009ee80: 6e73 203d 2065 6e73 7572 6564 6963 7428  ns = ensuredict(
-0009ee90: 6f70 7469 6f6e 7329 0a20 2020 2020 2020  options).       
-0009eea0: 2073 656c 665b 2263 6c61 7373 225d 2e61   self["class"].a
-0009eeb0: 6464 2822 636f 6e74 726f 6c22 290a 2020  dd("control").  
-0009eec0: 2020 2020 2020 666f 7220 6b2c 7620 696e        for k,v in
-0009eed0: 206f 7074 696f 6e73 2e69 7465 6d73 2829   options.items()
-0009eee0: 3a0a 2020 2020 2020 2020 2020 2020 6970  :.            ip
-0009eef0: 743d 5461 672e 696e 7075 7428 0a20 2020  t=Tag.input(.   
-0009ef00: 2020 2020 2020 2020 2020 2020 205f 7479               _ty
-0009ef10: 7065 3d22 7261 6469 6f22 2c0a 2020 2020  pe="radio",.    
-0009ef20: 2020 2020 2020 2020 2020 2020 5f76 616c              _val
-0009ef30: 7565 3d6b 2c0a 2020 2020 2020 2020 2020  ue=k,.          
-0009ef40: 2020 2020 2020 5f6e 616d 653d 7365 6c66        _name=self
-0009ef50: 2e61 7474 7273 2e67 6574 2822 6e61 6d65  .attrs.get("name
-0009ef60: 222c 7374 7228 6964 2873 656c 6629 2929  ",str(id(self)))
-0009ef70: 2c20 2020 2020 2020 2020 2020 2020 2320  ,             # 
-0009ef80: 6e65 6564 2061 206e 616d 6520 746f 2062  need a name to b
-0009ef90: 6520 7661 6c69 640a 2020 2020 2020 2020  e valid.        
-0009efa0: 2020 2020 2020 2020 5f63 6865 636b 6564          _checked
-0009efb0: 3d28 7374 7228 7365 6c66 2e61 7474 7273  =(str(self.attrs
-0009efc0: 2e67 6574 2822 7661 6c75 6522 2c4e 6f6e  .get("value",Non
-0009efd0: 6529 293d 3d73 7472 286b 2929 2c0a 2020  e))==str(k)),.  
-0009efe0: 2020 2020 2020 2020 2020 2020 2020 5f72                _r
-0009eff0: 6571 7569 7265 643d 626f 6f6c 2873 656c  equired=bool(sel
-0009f000: 662e 6174 7472 732e 6765 7428 2272 6571  f.attrs.get("req
-0009f010: 7569 7265 6422 2c4e 6f6e 6529 292c 0a20  uired",None)),. 
-0009f020: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0009f030: 7265 6164 6f6e 6c79 3d62 6f6f 6c28 7365  readonly=bool(se
-0009f040: 6c66 2e61 7474 7273 2e67 6574 2822 7265  lf.attrs.get("re
-0009f050: 6164 6f6e 6c79 222c 4e6f 6e65 2929 2c0a  adonly",None)),.
-0009f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0009f070: 5f6f 6e63 6861 6e67 653d 6622 646f 6375  _onchange=f"docu
-0009f080: 6d65 6e74 2e67 6574 456c 656d 656e 7442  ment.getElementB
-0009f090: 7949 6428 277b 6964 2873 656c 6629 7d27  yId('{id(self)}'
-0009f0a0: 292e 7661 6c75 653d 277b 6b7d 273b 220a  ).value='{k}';".
-0009f0b0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0009f0c0: 2020 2020 2020 2020 2020 7365 6c66 203c            self <
-0009f0d0: 3d20 5461 672e 6469 7628 5461 672e 6c61  = Tag.div(Tag.la
-0009f0e0: 6265 6c28 2069 7074 202b 2220 222b 2076  bel( ipt +" "+ v
-0009f0f0: 202c 5f63 6c61 7373 3d22 7261 6469 6f22   ,_class="radio"
-0009f100: 2929 0a0a 2323 2323 2323 2323 2323 2323  ))..############
-0009f110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f150: 2323 2323 2323 2323 2323 0a23 2320 4469  ##########.## Di
-0009f160: 616c 6f67 206f 626a 6563 7473 0a23 2323  alog objects.###
-0009f170: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f180: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f190: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f1a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f1b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009f1c0: 2323 230a 636c 6173 7320 456d 7074 7928  ###.class Empty(
-0009f1d0: 5461 672e 6469 7629 3a0a 2020 2020 6465  Tag.div):.    de
-0009f1e0: 6620 696e 6974 2873 656c 662c 6d65 7461  f init(self,meta
-0009f1f0: 7461 6729 3a0a 2020 2020 2020 2020 7365  tag):.        se
-0009f200: 6c66 2e63 6c65 6172 2829 0a0a 0a63 6c61  lf.clear()...cla
-0009f210: 7373 204d 6f64 616c 426c 6f63 6b28 5461  ss ModalBlock(Ta
-0009f220: 672e 6469 7629 3a0a 2020 2020 6465 6620  g.div):.    def 
-0009f230: 696e 6974 2873 656c 662c 6d65 7461 7461  init(self,metata
-0009f240: 672c 6f62 6a29 3a0a 2020 2020 2020 2020  g,obj):.        
-0009f250: 7365 6c66 5b27 636c 6173 7327 5d3d 226d  self['class']="m
-0009f260: 6f64 616c 2069 732d 6163 7469 7665 220a  odal is-active".
-0009f270: 2020 2020 2020 2020 7365 6c66 203c 3d20          self <= 
-0009f280: 5461 672e 6469 7628 5f63 6c61 7373 3d22  Tag.div(_class="
-0009f290: 6d6f 6461 6c2d 6261 636b 6772 6f75 6e64  modal-background
-0009f2a0: 2229 202b 206f 626a 0a0a 636c 6173 7320  ") + obj..class 
-0009f2b0: 4d6f 6461 6c41 6c65 7274 284d 6f64 616c  ModalAlert(Modal
-0009f2c0: 426c 6f63 6b29 3a0a 2020 2020 6465 6620  Block):.    def 
-0009f2d0: 5f5f 696e 6974 5f5f 2873 656c 662c 6d65  __init__(self,me
-0009f2e0: 7461 7461 672c 6f62 6a2c 706d 6178 696d  tatag,obj,pmaxim
-0009f2f0: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
-0009f300: 2020 206f 626a 203d 2054 6167 2e64 6976     obj = Tag.div
-0009f310: 286f 626a 2c5f 636c 6173 733d 2262 6f78  (obj,_class="box
-0009f320: 2229 0a20 2020 2020 2020 2069 6620 706d  ").        if pm
-0009f330: 6178 696d 697a 653a 0a20 2020 2020 2020  aximize:.       
-0009f340: 2020 2020 206f 626a 5b22 7374 796c 6522       obj["style"
-0009f350: 5d3d 2268 6569 6768 743a 3130 3025 3b6f  ]="height:100%;o
-0009f360: 7665 7266 6c6f 772d 793a 6175 746f 220a  verflow-y:auto".
-0009f370: 2020 2020 2020 2020 6f62 6a3d 5461 672e          obj=Tag.
-0009f380: 6469 7628 6f62 6a2c 5f63 6c61 7373 3d22  div(obj,_class="
-0009f390: 6d6f 6461 6c2d 636f 6e74 656e 7422 290a  modal-content").
-0009f3a0: 2020 2020 2020 2020 4d6f 6461 6c42 6c6f          ModalBlo
-0009f3b0: 636b 2e5f 5f69 6e69 745f 5f28 7365 6c66  ck.__init__(self
-0009f3c0: 2c6d 6574 6174 6167 2c6f 626a 290a 2020  ,metatag,obj).  
-0009f3d0: 2020 2020 2020 7365 6c66 2e63 6869 6c64        self.child
-0009f3e0: 735b 305d 5b22 6f6e 636c 6963 6b22 5d3d  s[0]["onclick"]=
-0009f3f0: 6d65 7461 7461 672e 7374 6570 6576 656e  metatag.stepeven
-0009f400: 7428 290a 2020 2020 2020 2020 6966 2070  t().        if p
-0009f410: 6d61 7869 6d69 7a65 3a0a 2020 2020 2020  maximize:.      
-0009f420: 2020 2020 2020 6f62 6a5b 2273 7479 6c65        obj["style
-0009f430: 225d 3d66 2277 6964 7468 3a7b 706d 6178  "]=f"width:{pmax
-0009f440: 696d 697a 657d 3b68 6569 6768 743a 7b70  imize};height:{p
-0009f450: 6d61 7869 6d69 7a65 7d3b 220a 2020 2020  maximize};".    
-0009f460: 2020 2020 7365 6c66 202b 3d20 5461 672e      self += Tag.
-0009f470: 6275 7474 6f6e 285f 636c 6173 733d 226d  button(_class="m
-0009f480: 6f64 616c 2d63 6c6f 7365 2069 732d 6c61  odal-close is-la
-0009f490: 7267 6522 2c5f 6172 6961 5f6c 6162 656c  rge",_aria_label
-0009f4a0: 3d22 636c 6f73 6522 2c5f 6f6e 636c 6963  ="close",_onclic
-0009f4b0: 6b3d 6d65 7461 7461 672e 7374 6570 6576  k=metatag.stepev
-0009f4c0: 656e 7428 2929 0a0a 636c 6173 7320 4d6f  ent())..class Mo
-0009f4d0: 6461 6c42 6f78 284d 6f64 616c 416c 6572  dalBox(ModalAler
-0009f4e0: 7429 3a0a 2020 2020 6465 6620 5f5f 696e  t):.    def __in
-0009f4f0: 6974 5f5f 2873 656c 662c 6d65 7461 7461  it__(self,metata
-0009f500: 672c 6f62 6a2c 7369 7a65 3a66 6c6f 6174  g,obj,size:float
-0009f510: 3d2e 3629 3a0a 2020 2020 2020 2020 4d6f  =.6):.        Mo
-0009f520: 6461 6c41 6c65 7274 2e5f 5f69 6e69 745f  dalAlert.__init_
-0009f530: 5f28 7365 6c66 2c6d 6574 6174 6167 2c6f  _(self,metatag,o
-0009f540: 626a 2c70 6d61 7869 6d69 7a65 3d66 227b  bj,pmaximize=f"{
-0009f550: 7369 7a65 2a31 3030 7d25 2229 0a0a 636c  size*100}%")..cl
-0009f560: 6173 7320 4d6f 6461 6c43 6f6e 6669 726d  ass ModalConfirm
-0009f570: 284d 6f64 616c 416c 6572 7429 3a0a 2020  (ModalAlert):.  
-0009f580: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0009f590: 656c 662c 6d65 7461 7461 672c 6f62 6a2c  elf,metatag,obj,
-0009f5a0: 6362 293a 0a20 2020 2020 2020 2064 6566  cb):.        def
-0009f5b0: 2063 616c 6c28 6576 293a 0a20 2020 2020   call(ev):.     
-0009f5c0: 2020 2020 2020 206d 6574 6174 6167 2e73         metatag.s
-0009f5d0: 7465 7028 290a 2020 2020 2020 2020 2020  tep().          
-0009f5e0: 2020 7265 7475 726e 2063 6228 2065 762e    return cb( ev.
-0009f5f0: 7461 7267 6574 2e76 616c 2029 0a20 2020  target.val ).   
-0009f600: 2020 2020 2020 0a20 2020 2020 2020 2062        .        b
-0009f610: 6f78 3d5b 200a 2020 2020 2020 2020 2020  ox=[ .          
-0009f620: 2020 5461 672e 6469 7628 6f62 6a29 2c0a    Tag.div(obj),.
-0009f630: 2020 2020 2020 2020 2020 2020 4275 7474              Butt
-0009f640: 6f6e 2822 5965 7322 2c76 616c 3d54 7275  on("Yes",val=Tru
-0009f650: 652c 5f6f 6e63 6c69 636b 3d63 616c 6c29  e,_onclick=call)
-0009f660: 2c0a 2020 2020 2020 2020 2020 2020 4275  ,.            Bu
-0009f670: 7474 6f6e 2822 4e6f 222c 7661 6c3d 4661  tton("No",val=Fa
-0009f680: 6c73 652c 5f6f 6e63 6c69 636b 3d63 616c  lse,_onclick=cal
-0009f690: 6c29 2c0a 2020 2020 2020 2020 5d0a 2020  l),.        ].  
-0009f6a0: 2020 2020 2020 4d6f 6461 6c41 6c65 7274        ModalAlert
-0009f6b0: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c6d  .__init__(self,m
-0009f6c0: 6574 6174 6167 2c62 6f78 290a 0a63 6c61  etatag,box)..cla
-0009f6d0: 7373 204d 6f64 616c 5072 6f6d 7074 284d  ss ModalPrompt(M
-0009f6e0: 6f64 616c 416c 6572 7429 3a0a 2020 2020  odalAlert):.    
-0009f6f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0009f700: 662c 6d65 7461 7461 672c 2076 616c 7565  f,metatag, value
-0009f710: 2c74 6974 6c65 2c63 6229 3a0a 2020 2020  ,title,cb):.    
-0009f720: 2020 2020 6465 6620 6361 6c6c 2864 6963      def call(dic
-0009f730: 6f29 3a0a 2020 2020 2020 2020 2020 2020  o):.            
-0009f740: 6d65 7461 7461 672e 7374 6570 2829 0a20  metatag.step(). 
-0009f750: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0009f760: 6e20 6362 2820 6469 636f 5b22 7072 6f6d  n cb( dico["prom
-0009f770: 7074 7661 6c75 6522 5d20 290a 2020 2020  ptvalue"] ).    
-0009f780: 2020 2020 7769 7468 2046 6f72 6d28 6f6e      with Form(on
-0009f790: 7375 626d 6974 3d63 616c 6c29 2061 7320  submit=call) as 
-0009f7a0: 663a 0a20 2020 2020 2020 2020 2020 2066  f:.            f
-0009f7b0: 2b3d 5461 672e 6469 7628 2074 6974 6c65  +=Tag.div( title
-0009f7c0: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
-0009f7d0: 2b3d 5461 672e 6469 7628 2049 6e70 7574  +=Tag.div( Input
-0009f7e0: 285f 7661 6c75 653d 7661 6c75 652c 5f6e  (_value=value,_n
-0009f7f0: 616d 653d 2270 726f 6d70 7476 616c 7565  ame="promptvalue
-0009f800: 222c 6a73 3d22 7365 6c66 2e66 6f63 7573  ",js="self.focus
-0009f810: 2829 3b73 656c 662e 7365 6c65 6374 2829  ();self.select()
-0009f820: 222c 205f 6175 746f 666f 6375 733d 5472  ", _autofocus=Tr
-0009f830: 7565 2920 2c5f 7374 796c 653d 2270 6164  ue) ,_style="pad
-0009f840: 6469 6e67 3a34 7078 2030 2229 0a20 2020  ding:4px 0").   
-0009f850: 2020 2020 2020 2020 2066 2b3d 4275 7474           f+=Butt
-0009f860: 6f6e 2822 4f6b 2220 290a 2020 2020 2020  on("Ok" ).      
-0009f870: 2020 2020 2020 662b 3d42 7574 746f 6e28        f+=Button(
-0009f880: 2243 616e 6365 6c22 2c5f 7479 7065 3d22  "Cancel",_type="
-0009f890: 6275 7474 6f6e 222c 5f6f 6e63 6c69 636b  button",_onclick
-0009f8a0: 3d6d 6574 6174 6167 2e73 7465 7065 7665  =metatag.stepeve
-0009f8b0: 6e74 2829 290a 2020 2020 2020 2020 4d6f  nt()).        Mo
-0009f8c0: 6461 6c41 6c65 7274 2e5f 5f69 6e69 745f  dalAlert.__init_
-0009f8d0: 5f28 7365 6c66 2c6d 6574 6174 6167 2c66  _(self,metatag,f
-0009f8e0: 290a 2020 2020 2020 2020 0a63 6c61 7373  ).        .class
-0009f8f0: 2044 7261 7765 7228 5461 672e 6469 7629   Drawer(Tag.div)
-0009f900: 3a0a 2020 2020 6465 6620 696e 6974 2873  :.    def init(s
-0009f910: 656c 662c 6d65 7461 7461 672c 6f62 6a2c  elf,metatag,obj,
-0009f920: 6d6f 6465 3a73 7472 293a 0a20 2020 2020  mode:str):.     
-0009f930: 2020 2073 697a 653d 3530 0a20 2020 2020     size=50.     
-0009f940: 2020 2069 6620 6d6f 6465 3d3d 226c 6566     if mode=="lef
-0009f950: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
-0009f960: 742c 722c 622c 6c3d 2028 2230 7078 222c  t,r,b,l= ("0px",
-0009f970: 6622 7b73 697a 657d 2522 2c22 3070 7822  f"{size}%","0px"
-0009f980: 2c22 3070 7822 290a 2020 2020 2020 2020  ,"0px").        
-0009f990: 656c 6966 206d 6f64 653d 3d22 7269 6768  elif mode=="righ
-0009f9a0: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
-0009f9b0: 742c 722c 622c 6c3d 2028 2230 7078 222c  t,r,b,l= ("0px",
-0009f9c0: 2230 7078 222c 2230 7078 222c 6622 7b73  "0px","0px",f"{s
-0009f9d0: 697a 657d 2522 290a 2020 2020 2020 2020  ize}%").        
-0009f9e0: 656c 6966 206d 6f64 653d 3d22 626f 7474  elif mode=="bott
-0009f9f0: 6f6d 223a 0a20 2020 2020 2020 2020 2020  om":.           
-0009fa00: 2074 2c72 2c62 2c6c 3d28 6622 7b73 697a   t,r,b,l=(f"{siz
-0009fa10: 657d 2522 2c22 3070 7822 2c22 3070 7822  e}%","0px","0px"
-0009fa20: 2c22 3070 7822 290a 2020 2020 2020 2020  ,"0px").        
-0009fa30: 656c 6966 206d 6f64 653d 3d22 746f 7022  elif mode=="top"
-0009fa40: 3a0a 2020 2020 2020 2020 2020 2020 742c  :.            t,
-0009fa50: 722c 622c 6c3d 2028 2230 7078 222c 2230  r,b,l= ("0px","0
-0009fa60: 7078 222c 6622 7b73 697a 657d 2522 2c22  px",f"{size}%","
-0009fa70: 3070 7822 290a 0a20 2020 2020 2020 2073  0px")..        s
-0009fa80: 656c 6620 3c3d 2056 6f69 6c65 285f 6f6e  elf <= Voile(_on
-0009fa90: 6d6f 7573 6564 6f77 6e3d 6d65 7461 7461  mousedown=metata
-0009faa0: 672e 7374 6570 6576 656e 7428 2929 0a20  g.stepevent()). 
-0009fab0: 2020 2020 2020 2073 656c 6620 3c3d 2054         self <= T
-0009fac0: 6167 2e64 6976 2820 6f62 6a20 2c5f 7374  ag.div( obj ,_st
-0009fad0: 796c 653d 6622 706f 7369 7469 6f6e 3a66  yle=f"position:f
-0009fae0: 6978 6564 3b74 6f70 3a7b 747d 3b62 6f74  ixed;top:{t};bot
-0009faf0: 746f 6d3a 7b62 7d3b 6c65 6674 3a7b 6c7d  tom:{b};left:{l}
-0009fb00: 3b72 6967 6874 3a7b 727d 3b62 6163 6b67  ;right:{r};backg
-0009fb10: 726f 756e 643a 7768 6974 653b 626f 7264  round:white;bord
-0009fb20: 6572 2d72 6164 6975 733a 3070 783b 626f  er-radius:0px;bo
-0009fb30: 782d 7368 6164 6f77 3a20 7267 6261 2830  x-shadow: rgba(0
-0009fb40: 2c20 302c 2030 2c20 302e 3335 2920 3070  , 0, 0, 0.35) 0p
-0009fb50: 7820 3570 7820 3135 7078 3b3b 7a2d 696e  x 5px 15px;;z-in
-0009fb60: 6465 783a 3130 3031 3b70 6164 6469 6e67  dex:1001;padding
-0009fb70: 3a31 3070 7822 290a 0a63 6c61 7373 2050  :10px")..class P
-0009fb80: 6f70 2854 6167 2e64 6976 293a 0a20 2020  op(Tag.div):.   
-0009fb90: 2064 6566 2069 6e69 7428 7365 6c66 2c6d   def init(self,m
-0009fba0: 6574 6174 6167 2c6f 626a 2c78 793a 7475  etatag,obj,xy:tu
-0009fbb0: 706c 6529 3a0a 2020 2020 2020 2020 782c  ple):.        x,
-0009fbc0: 793d 7879 0a20 2020 2020 2020 2073 656c  y=xy.        sel
-0009fbd0: 6620 3c3d 2056 6f69 6c65 285f 6f6e 6d6f  f <= Voile(_onmo
-0009fbe0: 7573 6564 6f77 6e3d 6d65 7461 7461 672e  usedown=metatag.
-0009fbf0: 7374 6570 6576 656e 7428 2929 0a20 2020  stepevent()).   
-0009fc00: 2020 2020 2073 656c 6620 3c3d 2054 6167       self <= Tag
-0009fc10: 2e64 6976 2820 6f62 6a20 2c5f 7374 796c  .div( obj ,_styl
-0009fc20: 653d 6622 706f 7369 7469 6f6e 3a66 6978  e=f"position:fix
-0009fc30: 6564 3b74 6f70 3a7b 797d 7078 3b6c 6566  ed;top:{y}px;lef
-0009fc40: 743a 7b78 7d70 783b 7a2d 696e 6465 783a  t:{x}px;z-index:
-0009fc50: 3130 3031 3b62 6163 6b67 726f 756e 643a  1001;background:
-0009fc60: 7768 6974 6522 290a 0a63 6c61 7373 2054  white")..class T
-0009fc70: 6f61 7374 2854 6167 2e64 6976 293a 0a20  oast(Tag.div):. 
-0009fc80: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
-0009fc90: 2c6d 6169 6e5f 6e6f 6e5f 7573 6564 2c6f  ,main_non_used,o
-0009fca0: 626a 2c74 696d 656f 7574 3d31 3030 3029  bj,timeout=1000)
-0009fcb0: 3a0a 2020 2020 2020 2020 7365 6c66 203c  :.        self <
-0009fcc0: 3d20 5461 672e 6469 7628 6f62 6a2c 5f73  = Tag.div(obj,_s
-0009fcd0: 7479 6c65 3d22 706f 7369 7469 6f6e 3a66  tyle="position:f
-0009fce0: 6978 6564 3b72 6967 6874 3a31 3070 783b  ixed;right:10px;
-0009fcf0: 626f 7474 6f6d 3a31 3070 783b 7a2d 696e  bottom:10px;z-in
-0009fd00: 6465 783a 3130 3031 3b22 2c20 5f63 6c61  dex:1001;", _cla
-0009fd10: 7373 3d22 6e6f 7469 6669 6361 7469 6f6e  ss="notification
-0009fd20: 2069 732d 6c69 6e6b 2069 732d 6c69 6768   is-link is-ligh
-0009fd30: 7422 290a 2020 2020 2020 2020 7365 6c66  t").        self
-0009fd40: 2e6a 733d 2273 6574 5469 6d65 6f75 7428  .js="setTimeout(
-0009fd50: 2066 756e 6374 696f 6e28 2920 7b73 656c   function() {sel
-0009fd60: 662e 7265 6d6f 7665 2829 7d20 2c20 2573  f.remove()} , %s
-0009fd70: 2922 2025 2074 696d 656f 7574 0a0a 2323  )" % timeout..##
-0009fd80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009fd90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009fda0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009fdb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009fdc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0009fdd0: 2323 2323 0a0a 636c 6173 7320 5461 6273  ####..class Tabs
-0009fde0: 2854 6167 2e64 6976 293a 0a20 2020 2064  (Tag.div):.    d
-0009fdf0: 6566 2069 6e69 7428 7365 6c66 2c6d 6574  ef init(self,met
-0009fe00: 6174 6167 2c73 656c 6563 7465 643d 3029  atag,selected=0)
-0009fe10: 3a0a 2020 2020 2020 2020 756c 203d 2054  :.        ul = T
-0009fe20: 6167 2e75 6c28 290a 2020 2020 2020 2020  ag.ul().        
-0009fe30: 666f 7220 6964 782c 6920 696e 2065 6e75  for idx,i in enu
-0009fe40: 6d65 7261 7465 286d 6574 6174 6167 2e5f  merate(metatag._
-0009fe50: 7461 6273 293a 0a20 2020 2020 2020 2020  tabs):.         
-0009fe60: 2020 206e 616d 6520 3d20 6861 7361 7474     name = hasatt
-0009fe70: 7228 692c 226e 616d 6522 2920 616e 6420  r(i,"name") and 
-0009fe80: 692e 6e61 6d65 206f 7220 223f 286e 616d  i.name or "?(nam
-0009fe90: 6529 3f22 0a20 2020 2020 2020 2020 2020  e)?".           
-0009fea0: 2075 6c2b 3d54 6167 2e6c 6928 2054 6167   ul+=Tag.li( Tag
-0009feb0: 2e61 286e 616d 6529 2c20 5f6f 6e63 6c69  .a(name), _oncli
-0009fec0: 636b 203d 206d 6574 6174 6167 2e73 7465  ck = metatag.ste
-0009fed0: 7065 7665 6e74 2873 656c 6563 743d 6964  pevent(select=id
-0009fee0: 7829 2c20 5f63 6c61 7373 3d22 6973 2d61  x), _class="is-a
-0009fef0: 6374 6976 6522 2069 6620 6964 783d 3d73  ctive" if idx==s
-0009ff00: 656c 6563 7465 6420 656c 7365 2022 2229  elected else "")
-0009ff10: 0a20 2020 2020 2020 2073 656c 663c 3d54  .        self<=T
-0009ff20: 6167 2e64 6976 2875 6c2c 5f63 6c61 7373  ag.div(ul,_class
-0009ff30: 3d22 7461 6273 2229 0a20 2020 2020 2020  ="tabs").       
-0009ff40: 2069 6620 6d65 7461 7461 672e 5f74 6162   if metatag._tab
-0009ff50: 733a 2073 656c 663c 3d6d 6574 6174 6167  s: self<=metatag
-0009ff60: 2e5f 7461 6273 5b73 656c 6563 7465 645d  ._tabs[selected]
-0009ff70: 0a                                       .
+0009e520: 2020 2020 2020 2020 7365 6c66 5b22 706c          self["pl
+0009e530: 6163 6568 6f6c 6465 7222 5d20 3d20 7365  aceholder"] = se
+0009e540: 6c66 2e61 7474 7273 2e67 6574 2822 6c61  lf.attrs.get("la
+0009e550: 6265 6c22 290a 0a63 6c61 7373 2054 6578  bel")..class Tex
+0009e560: 7461 7265 6128 5461 672e 7465 7874 6172  tarea(Tag.textar
+0009e570: 6561 293a 0a20 2020 2073 7461 7469 6373  ea):.    statics
+0009e580: 3d42 554c 4d41 0a20 2020 2064 6566 2069  =BULMA.    def i
+0009e590: 6e69 7428 7365 6c66 2c74 7874 3a73 7472  nit(self,txt:str
+0009e5a0: 2c2a 2a61 293a 0a20 2020 2020 2020 2073  ,**a):.        s
+0009e5b0: 656c 665b 2263 6c61 7373 225d 2e61 6464  elf["class"].add
+0009e5c0: 2822 7465 7874 6172 6561 2229 0a20 2020  ("textarea").   
+0009e5d0: 2020 2020 2073 656c 6620 3c3d 2074 7874       self <= txt
+0009e5e0: 0a0a 2020 2020 2020 2020 7365 6c66 5b22  ..        self["
+0009e5f0: 706c 6163 6568 6f6c 6465 7222 5d20 3d20  placeholder"] = 
+0009e600: 7365 6c66 2e61 7474 7273 2e67 6574 2822  self.attrs.get("
+0009e610: 6c61 6265 6c22 290a 0a63 6c61 7373 2042  label")..class B
+0009e620: 7574 746f 6e28 5461 672e 6275 7474 6f6e  utton(Tag.button
+0009e630: 293a 0a20 2020 2073 7461 7469 6373 3d20  ):.    statics= 
+0009e640: 4255 4c4d 410a 2020 2020 6465 6620 696e  BULMA.    def in
+0009e650: 6974 2873 656c 662c 7469 746c 652c 2a2a  it(self,title,**
+0009e660: 6129 3a0a 2020 2020 2020 2020 7365 6c66  a):.        self
+0009e670: 203c 3d20 7469 746c 650a 2020 2020 2020   <= title.      
+0009e680: 2020 7365 6c66 5b22 636c 6173 7322 5d2e    self["class"].
+0009e690: 6164 6428 2262 7574 746f 6e22 290a 0a63  add("button")..c
+0009e6a0: 6c61 7373 2056 6f69 6c65 2854 6167 2e64  lass Voile(Tag.d
+0009e6b0: 6976 293a 200a 2020 2020 7374 6174 6963  iv): .    static
+0009e6c0: 733d 2042 554c 4d41 0a20 2020 2064 6566  s= BULMA.    def
+0009e6d0: 2069 6e69 7428 7365 6c66 2c2a 2a61 293a   init(self,**a):
+0009e6e0: 0a20 2020 2020 2020 2073 656c 665b 2273  .        self["s
+0009e6f0: 7479 6c65 225d 2e73 6574 2822 706f 7369  tyle"].set("posi
+0009e700: 7469 6f6e 222c 2266 6978 6564 2229 0a20  tion","fixed"). 
+0009e710: 2020 2020 2020 2073 656c 665b 2273 7479         self["sty
+0009e720: 6c65 225d 2e73 6574 2822 746f 7022 2c22  le"].set("top","
+0009e730: 3070 7822 290a 2020 2020 2020 2020 7365  0px").        se
+0009e740: 6c66 5b22 7374 796c 6522 5d2e 7365 7428  lf["style"].set(
+0009e750: 2262 6f74 746f 6d22 2c22 3070 7822 290a  "bottom","0px").
+0009e760: 2020 2020 2020 2020 7365 6c66 5b22 7374          self["st
+0009e770: 796c 6522 5d2e 7365 7428 2272 6967 6874  yle"].set("right
+0009e780: 222c 2230 7078 2229 0a20 2020 2020 2020  ","0px").       
+0009e790: 2073 656c 665b 2273 7479 6c65 225d 2e73   self["style"].s
+0009e7a0: 6574 2822 6c65 6674 222c 2230 7078 2229  et("left","0px")
+0009e7b0: 0a20 2020 2020 2020 2073 656c 665b 2273  .        self["s
+0009e7c0: 7479 6c65 225d 2e73 6574 2822 7a2d 696e  tyle"].set("z-in
+0009e7d0: 6465 7822 2c22 3130 3030 2229 0a20 2020  dex","1000").   
+0009e7e0: 2020 2020 2073 656c 665b 2273 7479 6c65       self["style
+0009e7f0: 225d 2e73 6574 2822 6261 636b 6772 6f75  "].set("backgrou
+0009e800: 6e64 222c 2223 4343 4322 290a 2020 2020  nd","#CCC").    
+0009e810: 2020 2020 7365 6c66 5b22 7374 796c 6522      self["style"
+0009e820: 5d2e 7365 7428 226f 7061 6369 7479 222c  ].set("opacity",
+0009e830: 2230 2e35 2229 0a0a 0a0a 636c 6173 7320  "0.5")....class 
+0009e840: 4d65 6e75 2854 6167 2e64 6976 293a 0a20  Menu(Tag.div):. 
+0009e850: 2020 2064 6566 2069 6e69 7428 7365 6c66     def init(self
+0009e860: 2c65 6e74 7269 6573 3a64 6963 7429 3a0a  ,entries:dict):.
+0009e870: 2020 2020 2020 2020 7365 6c66 5b22 636c          self["cl
+0009e880: 6173 7322 5d2e 6164 6428 226d 656e 7522  ass"].add("menu"
+0009e890: 290a 2020 2020 2020 2020 6465 6620 6361  ).        def ca
+0009e8a0: 6c6c 2865 7629 3a0a 2020 2020 2020 2020  ll(ev):.        
+0009e8b0: 2020 2020 2361 7574 6f20 636c 6f73 6520      #auto close 
+0009e8c0: 7468 6520 7569 2e44 6961 6c6f 672c 2069  the ui.Dialog, i
+0009e8d0: 6620 7468 6973 2022 4d65 6e75 2220 6973  f this "Menu" is
+0009e8e0: 2069 6e20 6120 4469 616c 6f67 2069 6e74   in a Dialog int
+0009e8f0: 6572 6163 7469 6f6e 0a20 2020 2020 2020  eraction.       
+0009e900: 2020 2020 2023 2d2d 2d2d 2d2d 2d2d 2d2d       #----------
+0009e910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0009e920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0009e930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0009e940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+0009e950: 2020 2020 2020 2020 2020 2063 7572 7265             curre
+0009e960: 6e74 203d 2073 656c 662e 7061 7265 6e74  nt = self.parent
+0009e970: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+0009e980: 6c65 2063 7572 7265 6e74 2069 7320 6e6f  le current is no
+0009e990: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0009e9a0: 2020 2020 2020 2020 6966 2072 6570 7228          if repr(
+0009e9b0: 6375 7272 656e 7429 2e73 7461 7274 7377  current).startsw
+0009e9c0: 6974 6828 223c 4469 616c 6f67 2764 6976  ith("<Dialog'div
+0009e9d0: 2229 3a20 2354 4f44 4f3a 206e 6f74 2074  "): #TODO: not t
+0009e9e0: 6f70 2028 6361 6e20 646f 2062 6574 7465  op (can do bette
+0009e9f0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0009ea00: 2020 2020 2020 2063 7572 7265 6e74 2e63         current.c
+0009ea10: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
+0009ea20: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0009ea30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0009ea40: 2063 7572 7265 6e74 203d 2063 7572 7265   current = curre
+0009ea50: 6e74 2e70 6172 656e 740a 2020 2020 2020  nt.parent.      
+0009ea60: 2020 2020 2020 232d 2d2d 2d2d 2d2d 2d2d        #---------
+0009ea70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0009ea80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0009ea90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0009eaa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0009eab0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0009eac0: 7572 6e20 6576 2e74 6172 6765 742e 6d65  urn ev.target.me
+0009ead0: 7468 6f64 2829 0a0a 2020 2020 2020 2020  thod()..        
+0009eae0: 7769 7468 2054 6167 2e64 6976 285f 636c  with Tag.div(_cl
+0009eaf0: 6173 733d 226d 656e 752d 6c69 7374 2229  ass="menu-list")
+0009eb00: 2061 7320 756c 3a0a 2020 2020 2020 2020   as ul:.        
+0009eb10: 2020 2020 666f 7220 6b2c 7620 696e 2065      for k,v in e
+0009eb20: 6e74 7269 6573 2e69 7465 6d73 2829 3a0a  ntries.items():.
+0009eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0009eb40: 756c 203c 3d20 5461 672e 6469 7628 2054  ul <= Tag.div( T
+0009eb50: 6167 2e61 286b 292c 6d65 7468 6f64 3d76  ag.a(k),method=v
+0009eb60: 2c5f 6f6e 636c 6963 6b3d 6361 6c6c 290a  ,_onclick=call).
+0009eb70: 2020 2020 2020 2020 7365 6c66 3c3d 756c          self<=ul
+0009eb80: 0a0a 636c 6173 7320 5370 696e 6e65 7228  ..class Spinner(
+0009eb90: 5461 672e 7370 616e 293a 0a20 2020 2073  Tag.span):.    s
+0009eba0: 7461 7469 6373 3d22 2222 0a2e 7370 696e  tatics="""..spin
+0009ebb0: 6e65 7220 7b0a 2020 2020 7769 6474 683a  ner {.    width:
+0009ebc0: 2033 3270 783b 0a20 2020 2068 6569 6768   32px;.    heigh
+0009ebd0: 743a 2033 3270 783b 0a20 2020 2062 6f72  t: 32px;.    bor
+0009ebe0: 6465 723a 2038 7078 2073 6f6c 6964 2023  der: 8px solid #
+0009ebf0: 3333 463b 0a20 2020 2062 6f72 6465 722d  33F;.    border-
+0009ec00: 626f 7474 6f6d 2d63 6f6c 6f72 3a20 7472  bottom-color: tr
+0009ec10: 616e 7370 6172 656e 743b 0a20 2020 2062  ansparent;.    b
+0009ec20: 6f72 6465 722d 7261 6469 7573 3a20 3530  order-radius: 50
+0009ec30: 253b 0a20 2020 2064 6973 706c 6179 3a20  %;.    display: 
+0009ec40: 696e 6c69 6e65 2d62 6c6f 636b 3b0a 2020  inline-block;.  
+0009ec50: 2020 626f 782d 7369 7a69 6e67 3a20 626f    box-sizing: bo
+0009ec60: 7264 6572 2d62 6f78 3b0a 2020 2020 616e  rder-box;.    an
+0009ec70: 696d 6174 696f 6e3a 2072 6f74 6174 696f  imation: rotatio
+0009ec80: 6e20 3173 206c 696e 6561 7220 696e 6669  n 1s linear infi
+0009ec90: 6e69 7465 3b0a 2020 2020 7d0a 0a20 2020  nite;.    }..   
+0009eca0: 2040 6b65 7966 7261 6d65 7320 726f 7461   @keyframes rota
+0009ecb0: 7469 6f6e 207b 0a20 2020 2030 2520 7b0a  tion {.    0% {.
+0009ecc0: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+0009ecd0: 6d3a 2072 6f74 6174 6528 3064 6567 293b  m: rotate(0deg);
+0009ece0: 0a20 2020 207d 0a20 2020 2031 3030 2520  .    }.    100% 
+0009ecf0: 7b0a 2020 2020 2020 2020 7472 616e 7366  {.        transf
+0009ed00: 6f72 6d3a 2072 6f74 6174 6528 3336 3064  orm: rotate(360d
+0009ed10: 6567 293b 0a20 2020 207d 0a20 2020 207d  eg);.    }.    }
+0009ed20: 2020 2020 2020 2020 200a 2222 2220 2020           ."""   
+0009ed30: 200a 2020 2020 6465 6620 696e 6974 2873   .    def init(s
+0009ed40: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0009ed50: 6c66 5b22 636c 6173 7322 5d3d 2273 7069  lf["class"]="spi
+0009ed60: 6e6e 6572 220a 0a0a 636c 6173 7320 5365  nner"...class Se
+0009ed70: 6c65 6374 2854 6167 2e64 6976 293a 0a20  lect(Tag.div):. 
+0009ed80: 2020 2073 7461 7469 6373 3d42 554c 4d41     statics=BULMA
+0009ed90: 0a20 2020 2064 6566 2069 6e69 7428 7365  .    def init(se
+0009eda0: 6c66 2c6f 7074 696f 6e73 3a4c 6973 744f  lf,options:ListO
+0009edb0: 7244 6963 742c 202a 2a61 293a 0a20 2020  rDict, **a):.   
+0009edc0: 2020 2020 2073 656c 662e 6f70 7469 6f6e       self.option
+0009edd0: 733d 656e 7375 7265 6469 6374 286f 7074  s=ensuredict(opt
+0009ede0: 696f 6e73 290a 2020 2020 2020 2020 7365  ions).        se
+0009edf0: 6c66 5b22 636c 6173 7322 5d2e 6164 6428  lf["class"].add(
+0009ee00: 2273 656c 6563 7422 290a 2020 2020 2020  "select").      
+0009ee10: 2020 7365 6c66 2e72 6572 656e 6465 7228    self.rerender(
+0009ee20: 7365 6c66 2e61 7474 7273 2e67 6574 2822  self.attrs.get("
+0009ee30: 7661 6c75 6522 2929 0a0a 2020 2020 6465  value"))..    de
+0009ee40: 6620 7265 7265 6e64 6572 2873 656c 662c  f rerender(self,
+0009ee50: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+0009ee60: 7769 7468 2054 6167 2e73 656c 6563 7428  with Tag.select(
+0009ee70: 205f 6f6e 6368 616e 6765 3d66 2264 6f63   _onchange=f"doc
+0009ee80: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
+0009ee90: 4279 4964 2827 7b69 6428 7365 6c66 297d  ById('{id(self)}
+0009eea0: 2729 2e76 616c 7565 3d65 7665 6e74 2e74  ').value=event.t
+0009eeb0: 6172 6765 742e 7661 6c75 6522 2c5f 6e61  arget.value",_na
+0009eec0: 6d65 3d73 656c 662e 6174 7472 732e 6765  me=self.attrs.ge
+0009eed0: 7428 226e 616d 6522 292c 5f72 6571 7569  t("name"),_requi
+0009eee0: 7265 643d 7365 6c66 2e61 7474 7273 2e67  red=self.attrs.g
+0009eef0: 6574 2822 7265 7175 6972 6564 2229 2029  et("required") )
+0009ef00: 2061 7320 7365 6c65 6374 3a0a 2020 2020   as select:.    
+0009ef10: 2020 2020 2020 2020 666f 7220 6b2c 7620          for k,v 
+0009ef20: 696e 2073 656c 662e 6f70 7469 6f6e 732e  in self.options.
+0009ef30: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0009ef40: 2020 2020 2020 2020 2073 656c 6563 7420           select 
+0009ef50: 3c3d 2054 6167 2e6f 7074 696f 6e28 762c  <= Tag.option(v,
+0009ef60: 5f76 616c 7565 3d6b 2c5f 7365 6c65 6374  _value=k,_select
+0009ef70: 6564 3d28 2873 7472 2876 616c 7565 293d  ed=((str(value)=
+0009ef80: 3d73 7472 286b 2929 2929 0a20 2020 2020  =str(k)))).     
+0009ef90: 2020 2073 656c 662e 636c 6561 7228 2073     self.clear( s
+0009efa0: 656c 6563 7420 290a 0a63 6c61 7373 2052  elect )..class R
+0009efb0: 6164 696f 7328 5461 672e 7370 616e 293a  adios(Tag.span):
+0009efc0: 0a20 2020 2073 7461 7469 6373 3d42 554c  .    statics=BUL
+0009efd0: 4d41 0a20 2020 2064 6566 2069 6e69 7428  MA.    def init(
+0009efe0: 7365 6c66 2c6f 7074 696f 6e73 3a4c 6973  self,options:Lis
+0009eff0: 744f 7244 6963 742c 202a 2a61 293a 0a20  tOrDict, **a):. 
+0009f000: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
+0009f010: 6f6e 7320 3d20 656e 7375 7265 6469 6374  ons = ensuredict
+0009f020: 286f 7074 696f 6e73 290a 2020 2020 2020  (options).      
+0009f030: 2020 7365 6c66 5b22 636c 6173 7322 5d2e    self["class"].
+0009f040: 6164 6428 2263 6f6e 7472 6f6c 2229 0a20  add("control"). 
+0009f050: 2020 2020 2020 2073 656c 662e 7265 7265         self.rere
+0009f060: 6e64 6572 2820 7365 6c66 2e61 7474 7273  nder( self.attrs
+0009f070: 2e67 6574 2822 7661 6c75 6522 2c4e 6f6e  .get("value",Non
+0009f080: 6529 2029 0a20 2020 200a 2020 2020 6465  e) ).    .    de
+0009f090: 6620 7265 7265 6e64 6572 2873 656c 662c  f rerender(self,
+0009f0a0: 7661 6c75 6529 3a0a 2020 2020 2020 2020  value):.        
+0009f0b0: 2222 2220 7370 6563 6961 6c20 6d65 7468  """ special meth
+0009f0c0: 6f64 2028 7365 6520 6966 6965 6c64 7329  od (see ifields)
+0009f0d0: 2c20 746f 2072 6572 656e 6465 7220 616c  , to rerender al
+0009f0e0: 6c20 7468 6520 7769 6467 6574 2028 746f  l the widget (to
+0009f0f0: 2061 766f 6964 2074 6f20 6465 616c 2077   avoid to deal w
+0009f100: 6974 6820 6a73 2922 2222 0a20 2020 2020  ith js)""".     
+0009f110: 2020 2073 656c 662e 636c 6561 7228 290a     self.clear().
+0009f120: 2020 2020 2020 2020 666f 7220 6b2c 7620          for k,v 
+0009f130: 696e 2073 656c 662e 6f70 7469 6f6e 732e  in self.options.
+0009f140: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+0009f150: 2020 2020 2069 7074 3d54 6167 2e69 6e70       ipt=Tag.inp
+0009f160: 7574 280a 2020 2020 2020 2020 2020 2020  ut(.            
+0009f170: 2020 2020 5f74 7970 653d 2272 6164 696f      _type="radio
+0009f180: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0009f190: 2020 205f 7661 6c75 653d 6b2c 0a20 2020     _value=k,.   
+0009f1a0: 2020 2020 2020 2020 2020 2020 205f 6e61               _na
+0009f1b0: 6d65 3d73 656c 662e 6174 7472 732e 6765  me=self.attrs.ge
+0009f1c0: 7428 226e 616d 6522 2c73 7472 2869 6428  t("name",str(id(
+0009f1d0: 7365 6c66 2929 292c 2020 2020 2020 2020  self))),        
+0009f1e0: 2020 2020 2023 206e 6565 6420 6120 6e61       # need a na
+0009f1f0: 6d65 2074 6f20 6265 2076 616c 6964 0a20  me to be valid. 
+0009f200: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0009f210: 6368 6563 6b65 643d 2873 7472 2876 616c  checked=(str(val
+0009f220: 7565 293d 3d73 7472 286b 2929 2c0a 2020  ue)==str(k)),.  
+0009f230: 2020 2020 2020 2020 2020 2020 2020 5f72                _r
+0009f240: 6571 7569 7265 643d 626f 6f6c 2873 656c  equired=bool(sel
+0009f250: 662e 6174 7472 732e 6765 7428 2272 6571  f.attrs.get("req
+0009f260: 7569 7265 6422 2c4e 6f6e 6529 292c 0a20  uired",None)),. 
+0009f270: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0009f280: 7265 6164 6f6e 6c79 3d62 6f6f 6c28 7365  readonly=bool(se
+0009f290: 6c66 2e61 7474 7273 2e67 6574 2822 7265  lf.attrs.get("re
+0009f2a0: 6164 6f6e 6c79 222c 4e6f 6e65 2929 2c0a  adonly",None)),.
+0009f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0009f2c0: 5f6f 6e63 6861 6e67 653d 6622 646f 6375  _onchange=f"docu
+0009f2d0: 6d65 6e74 2e67 6574 456c 656d 656e 7442  ment.getElementB
+0009f2e0: 7949 6428 277b 6964 2873 656c 6629 7d27  yId('{id(self)}'
+0009f2f0: 292e 7661 6c75 653d 277b 6b7d 273b 220a  ).value='{k}';".
+0009f300: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0009f310: 2020 2020 2020 2020 2020 7365 6c66 203c            self <
+0009f320: 3d20 5461 672e 6469 7628 5461 672e 6c61  = Tag.div(Tag.la
+0009f330: 6265 6c28 2069 7074 202b 2220 222b 2076  bel( ipt +" "+ v
+0009f340: 202c 5f63 6c61 7373 3d22 7261 6469 6f22   ,_class="radio"
+0009f350: 2929 0a0a 2323 2323 2323 2323 2323 2323  ))..############
+0009f360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f3a0: 2323 2323 2323 2323 2323 0a23 2320 4469  ##########.## Di
+0009f3b0: 616c 6f67 206f 626a 6563 7473 0a23 2323  alog objects.###
+0009f3c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f3d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f3e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f3f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0009f410: 2323 230a 636c 6173 7320 456d 7074 7928  ###.class Empty(
+0009f420: 5461 672e 6469 7629 3a0a 2020 2020 6465  Tag.div):.    de
+0009f430: 6620 696e 6974 2873 656c 662c 6d65 7461  f init(self,meta
+0009f440: 7461 6729 3a0a 2020 2020 2020 2020 7365  tag):.        se
+0009f450: 6c66 2e63 6c65 6172 2829 0a0a 0a63 6c61  lf.clear()...cla
+0009f460: 7373 204d 6f64 616c 426c 6f63 6b28 5461  ss ModalBlock(Ta
+0009f470: 672e 6469 7629 3a0a 2020 2020 6465 6620  g.div):.    def 
+0009f480: 696e 6974 2873 656c 662c 6d65 7461 7461  init(self,metata
+0009f490: 672c 6f62 6a29 3a0a 2020 2020 2020 2020  g,obj):.        
+0009f4a0: 7365 6c66 5b27 636c 6173 7327 5d3d 226d  self['class']="m
+0009f4b0: 6f64 616c 2069 732d 6163 7469 7665 220a  odal is-active".
+0009f4c0: 2020 2020 2020 2020 7365 6c66 203c 3d20          self <= 
+0009f4d0: 5461 672e 6469 7628 5f63 6c61 7373 3d22  Tag.div(_class="
+0009f4e0: 6d6f 6461 6c2d 6261 636b 6772 6f75 6e64  modal-background
+0009f4f0: 2229 202b 206f 626a 0a0a 636c 6173 7320  ") + obj..class 
+0009f500: 506f 7050 6167 6528 5461 672e 6469 7629  PopPage(Tag.div)
+0009f510: 3a0a 2020 2020 6465 6620 696e 6974 2873  :.    def init(s
+0009f520: 656c 662c 6d65 7461 7461 672c 6f62 6a29  elf,metatag,obj)
+0009f530: 3a0a 2020 2020 2020 2020 7365 6c66 5b27  :.        self['
+0009f540: 636c 6173 7327 5d2e 6164 6428 2263 6f6e  class'].add("con
+0009f550: 7465 6e74 2229 0a20 2020 2020 2020 2073  tent").        s
+0009f560: 656c 665b 2273 7479 6c65 225d 2e73 6574  elf["style"].set
+0009f570: 2822 706f 7369 7469 6f6e 222c 2266 6978  ("position","fix
+0009f580: 6564 2229 0a20 2020 2020 2020 2073 656c  ed").        sel
+0009f590: 665b 2273 7479 6c65 225d 2e73 6574 2822  f["style"].set("
+0009f5a0: 746f 7022 2c22 3070 7822 290a 2020 2020  top","0px").    
+0009f5b0: 2020 2020 7365 6c66 5b22 7374 796c 6522      self["style"
+0009f5c0: 5d2e 7365 7428 2262 6f74 746f 6d22 2c22  ].set("bottom","
+0009f5d0: 3070 7822 290a 2020 2020 2020 2020 7365  0px").        se
+0009f5e0: 6c66 5b22 7374 796c 6522 5d2e 7365 7428  lf["style"].set(
+0009f5f0: 2272 6967 6874 222c 2230 7078 2229 0a20  "right","0px"). 
+0009f600: 2020 2020 2020 2073 656c 665b 2273 7479         self["sty
+0009f610: 6c65 225d 2e73 6574 2822 6c65 6674 222c  le"].set("left",
+0009f620: 2230 7078 2229 0a20 2020 2020 2020 2073  "0px").        s
+0009f630: 656c 665b 2273 7479 6c65 225d 2e73 6574  elf["style"].set
+0009f640: 2822 7a2d 696e 6465 7822 2c22 3130 3030  ("z-index","1000
+0009f650: 2229 0a20 2020 2020 2020 2073 656c 665b  ").        self[
+0009f660: 2273 7479 6c65 225d 2e73 6574 2822 6261  "style"].set("ba
+0009f670: 636b 6772 6f75 6e64 222c 2277 6869 7465  ckground","white
+0009f680: 2229 0a20 2020 2020 2020 2073 656c 6620  ").        self 
+0009f690: 3c3d 206f 626a 0a0a 636c 6173 7320 4d6f  <= obj..class Mo
+0009f6a0: 6461 6c41 6c65 7274 284d 6f64 616c 426c  dalAlert(ModalBl
+0009f6b0: 6f63 6b29 3a0a 2020 2020 6465 6620 5f5f  ock):.    def __
+0009f6c0: 696e 6974 5f5f 2873 656c 662c 6d65 7461  init__(self,meta
+0009f6d0: 7461 672c 6f62 6a2c 7773 697a 653a 666c  tag,obj,wsize:fl
+0009f6e0: 6f61 743d 4e6f 6e65 293a 0a20 2020 2020  oat=None):.     
+0009f6f0: 2020 2069 6620 7773 697a 6520 6973 206e     if wsize is n
+0009f700: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0009f710: 2020 2020 2070 7769 6474 683d 6622 7b69       pwidth=f"{i
+0009f720: 6e74 2877 7369 7a65 2a31 3030 297d 2522  nt(wsize*100)}%"
+0009f730: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0009f740: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0009f750: 2020 2070 7769 6474 683d 4e6f 6e65 0a20     pwidth=None. 
+0009f760: 2020 2020 2020 206f 626a 203d 2054 6167         obj = Tag
+0009f770: 2e64 6976 286f 626a 2c5f 636c 6173 733d  .div(obj,_class=
+0009f780: 2262 6f78 2229 0a20 2020 2020 2020 206f  "box").        o
+0009f790: 626a 3d54 6167 2e64 6976 286f 626a 2c5f  bj=Tag.div(obj,_
+0009f7a0: 636c 6173 733d 226d 6f64 616c 2d63 6f6e  class="modal-con
+0009f7b0: 7465 6e74 2229 0a20 2020 2020 2020 204d  tent").        M
+0009f7c0: 6f64 616c 426c 6f63 6b2e 5f5f 696e 6974  odalBlock.__init
+0009f7d0: 5f5f 2873 656c 662c 6d65 7461 7461 672c  __(self,metatag,
+0009f7e0: 6f62 6a29 0a20 2020 2020 2020 2073 656c  obj).        sel
+0009f7f0: 662e 6368 696c 6473 5b30 5d5b 226f 6e63  f.childs[0]["onc
+0009f800: 6c69 636b 225d 3d6d 6574 6174 6167 2e73  lick"]=metatag.s
+0009f810: 7465 7065 7665 6e74 2829 0a20 2020 2020  tepevent().     
+0009f820: 2020 2069 6620 7077 6964 7468 3a0a 2020     if pwidth:.  
+0009f830: 2020 2020 2020 2020 2020 6f62 6a5b 2273            obj["s
+0009f840: 7479 6c65 225d 3d66 2277 6964 7468 3a7b  tyle"]=f"width:{
+0009f850: 7077 6964 7468 7d3b 220a 2020 2020 2020  pwidth};".      
+0009f860: 2020 7365 6c66 202b 3d20 5461 672e 6275    self += Tag.bu
+0009f870: 7474 6f6e 285f 636c 6173 733d 226d 6f64  tton(_class="mod
+0009f880: 616c 2d63 6c6f 7365 2069 732d 6c61 7267  al-close is-larg
+0009f890: 6522 2c5f 6172 6961 5f6c 6162 656c 3d22  e",_aria_label="
+0009f8a0: 636c 6f73 6522 2c5f 6f6e 636c 6963 6b3d  close",_onclick=
+0009f8b0: 6d65 7461 7461 672e 7374 6570 6576 656e  metatag.stepeven
+0009f8c0: 7428 2929 0a0a 0a63 6c61 7373 204d 6f64  t())...class Mod
+0009f8d0: 616c 436f 6e66 6972 6d28 4d6f 6461 6c41  alConfirm(ModalA
+0009f8e0: 6c65 7274 293a 0a20 2020 2064 6566 205f  lert):.    def _
+0009f8f0: 5f69 6e69 745f 5f28 7365 6c66 2c6d 6574  _init__(self,met
+0009f900: 6174 6167 2c6f 626a 2c63 6229 3a0a 2020  atag,obj,cb):.  
+0009f910: 2020 2020 2020 6465 6620 6361 6c6c 2865        def call(e
+0009f920: 7629 3a0a 2020 2020 2020 2020 2020 2020  v):.            
+0009f930: 6d65 7461 7461 672e 7374 6570 2829 0a20  metatag.step(). 
+0009f940: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0009f950: 6e20 6362 2820 6576 2e74 6172 6765 742e  n cb( ev.target.
+0009f960: 7661 6c20 290a 2020 2020 2020 2020 200a  val ).         .
+0009f970: 2020 2020 2020 2020 626f 783d 5b20 0a20          box=[ . 
+0009f980: 2020 2020 2020 2020 2020 2054 6167 2e64             Tag.d
+0009f990: 6976 286f 626a 292c 0a20 2020 2020 2020  iv(obj),.       
+0009f9a0: 2020 2020 2042 7574 746f 6e28 2259 6573       Button("Yes
+0009f9b0: 222c 7661 6c3d 5472 7565 2c5f 6f6e 636c  ",val=True,_oncl
+0009f9c0: 6963 6b3d 6361 6c6c 292c 0a20 2020 2020  ick=call),.     
+0009f9d0: 2020 2020 2020 2042 7574 746f 6e28 224e         Button("N
+0009f9e0: 6f22 2c76 616c 3d46 616c 7365 2c5f 6f6e  o",val=False,_on
+0009f9f0: 636c 6963 6b3d 6361 6c6c 292c 0a20 2020  click=call),.   
+0009fa00: 2020 2020 205d 0a20 2020 2020 2020 204d       ].        M
+0009fa10: 6f64 616c 416c 6572 742e 5f5f 696e 6974  odalAlert.__init
+0009fa20: 5f5f 2873 656c 662c 6d65 7461 7461 672c  __(self,metatag,
+0009fa30: 626f 7829 0a0a 636c 6173 7320 4d6f 6461  box)..class Moda
+0009fa40: 6c50 726f 6d70 7428 4d6f 6461 6c41 6c65  lPrompt(ModalAle
+0009fa50: 7274 293a 0a20 2020 2064 6566 205f 5f69  rt):.    def __i
+0009fa60: 6e69 745f 5f28 7365 6c66 2c6d 6574 6174  nit__(self,metat
+0009fa70: 6167 2c20 7661 6c75 652c 7469 746c 652c  ag, value,title,
+0009fa80: 6362 293a 0a20 2020 2020 2020 2064 6566  cb):.        def
+0009fa90: 2063 616c 6c28 6469 636f 293a 0a20 2020   call(dico):.   
+0009faa0: 2020 2020 2020 2020 206d 6574 6174 6167           metatag
+0009fab0: 2e73 7465 7028 290a 2020 2020 2020 2020  .step().        
+0009fac0: 2020 2020 7265 7475 726e 2063 6228 2064      return cb( d
+0009fad0: 6963 6f5b 2270 726f 6d70 7476 616c 7565  ico["promptvalue
+0009fae0: 225d 2029 0a20 2020 2020 2020 2077 6974  "] ).        wit
+0009faf0: 6820 466f 726d 286f 6e73 7562 6d69 743d  h Form(onsubmit=
+0009fb00: 6361 6c6c 2920 6173 2066 3a0a 2020 2020  call) as f:.    
+0009fb10: 2020 2020 2020 2020 662b 3d54 6167 2e64          f+=Tag.d
+0009fb20: 6976 2820 7469 746c 6520 290a 2020 2020  iv( title ).    
+0009fb30: 2020 2020 2020 2020 662b 3d54 6167 2e64          f+=Tag.d
+0009fb40: 6976 2820 496e 7075 7428 5f76 616c 7565  iv( Input(_value
+0009fb50: 3d76 616c 7565 2c5f 6e61 6d65 3d22 7072  =value,_name="pr
+0009fb60: 6f6d 7074 7661 6c75 6522 2c6a 733d 2273  omptvalue",js="s
+0009fb70: 656c 662e 666f 6375 7328 293b 7365 6c66  elf.focus();self
+0009fb80: 2e73 656c 6563 7428 2922 2c20 5f61 7574  .select()", _aut
+0009fb90: 6f66 6f63 7573 3d54 7275 6529 202c 5f73  ofocus=True) ,_s
+0009fba0: 7479 6c65 3d22 7061 6464 696e 673a 3470  tyle="padding:4p
+0009fbb0: 7820 3022 290a 2020 2020 2020 2020 2020  x 0").          
+0009fbc0: 2020 662b 3d42 7574 746f 6e28 224f 6b22    f+=Button("Ok"
+0009fbd0: 2029 0a20 2020 2020 2020 2020 2020 2066   ).            f
+0009fbe0: 2b3d 4275 7474 6f6e 2822 4361 6e63 656c  +=Button("Cancel
+0009fbf0: 222c 5f74 7970 653d 2262 7574 746f 6e22  ",_type="button"
+0009fc00: 2c5f 6f6e 636c 6963 6b3d 6d65 7461 7461  ,_onclick=metata
+0009fc10: 672e 7374 6570 6576 656e 7428 2929 0a20  g.stepevent()). 
+0009fc20: 2020 2020 2020 204d 6f64 616c 416c 6572         ModalAler
+0009fc30: 742e 5f5f 696e 6974 5f5f 2873 656c 662c  t.__init__(self,
+0009fc40: 6d65 7461 7461 672c 6629 0a20 2020 2020  metatag,f).     
+0009fc50: 2020 200a 636c 6173 7320 4472 6177 6572     .class Drawer
+0009fc60: 2854 6167 2e64 6976 293a 0a20 2020 2064  (Tag.div):.    d
+0009fc70: 6566 2069 6e69 7428 7365 6c66 2c6d 6574  ef init(self,met
+0009fc80: 6174 6167 2c6f 626a 2c6d 6f64 653a 7374  atag,obj,mode:st
+0009fc90: 7229 3a0a 2020 2020 2020 2020 7369 7a65  r):.        size
+0009fca0: 3d35 300a 2020 2020 2020 2020 6966 206d  =50.        if m
+0009fcb0: 6f64 653d 3d22 6c65 6674 223a 0a20 2020  ode=="left":.   
+0009fcc0: 2020 2020 2020 2020 2074 2c72 2c62 2c6c           t,r,b,l
+0009fcd0: 3d20 2822 3070 7822 2c66 227b 7369 7a65  = ("0px",f"{size
+0009fce0: 7d25 222c 2230 7078 222c 2230 7078 2229  }%","0px","0px")
+0009fcf0: 0a20 2020 2020 2020 2065 6c69 6620 6d6f  .        elif mo
+0009fd00: 6465 3d3d 2272 6967 6874 223a 0a20 2020  de=="right":.   
+0009fd10: 2020 2020 2020 2020 2074 2c72 2c62 2c6c           t,r,b,l
+0009fd20: 3d20 2822 3070 7822 2c22 3070 7822 2c22  = ("0px","0px","
+0009fd30: 3070 7822 2c66 227b 7369 7a65 7d25 2229  0px",f"{size}%")
+0009fd40: 0a20 2020 2020 2020 2065 6c69 6620 6d6f  .        elif mo
+0009fd50: 6465 3d3d 2262 6f74 746f 6d22 3a0a 2020  de=="bottom":.  
+0009fd60: 2020 2020 2020 2020 2020 742c 722c 622c            t,r,b,
+0009fd70: 6c3d 2866 227b 7369 7a65 7d25 222c 2230  l=(f"{size}%","0
+0009fd80: 7078 222c 2230 7078 222c 2230 7078 2229  px","0px","0px")
+0009fd90: 0a20 2020 2020 2020 2065 6c69 6620 6d6f  .        elif mo
+0009fda0: 6465 3d3d 2274 6f70 223a 0a20 2020 2020  de=="top":.     
+0009fdb0: 2020 2020 2020 2074 2c72 2c62 2c6c 3d20         t,r,b,l= 
+0009fdc0: 2822 3070 7822 2c22 3070 7822 2c66 227b  ("0px","0px",f"{
+0009fdd0: 7369 7a65 7d25 222c 2230 7078 2229 0a0a  size}%","0px")..
+0009fde0: 2020 2020 2020 2020 7365 6c66 203c 3d20          self <= 
+0009fdf0: 566f 696c 6528 5f6f 6e6d 6f75 7365 646f  Voile(_onmousedo
+0009fe00: 776e 3d6d 6574 6174 6167 2e73 7465 7065  wn=metatag.stepe
+0009fe10: 7665 6e74 2829 290a 2020 2020 2020 2020  vent()).        
+0009fe20: 7365 6c66 203c 3d20 5461 672e 6469 7628  self <= Tag.div(
+0009fe30: 206f 626a 202c 5f73 7479 6c65 3d66 2270   obj ,_style=f"p
+0009fe40: 6f73 6974 696f 6e3a 6669 7865 643b 746f  osition:fixed;to
+0009fe50: 703a 7b74 7d3b 626f 7474 6f6d 3a7b 627d  p:{t};bottom:{b}
+0009fe60: 3b6c 6566 743a 7b6c 7d3b 7269 6768 743a  ;left:{l};right:
+0009fe70: 7b72 7d3b 6261 636b 6772 6f75 6e64 3a77  {r};background:w
+0009fe80: 6869 7465 3b62 6f72 6465 722d 7261 6469  hite;border-radi
+0009fe90: 7573 3a30 7078 3b62 6f78 2d73 6861 646f  us:0px;box-shado
+0009fea0: 773a 2072 6762 6128 302c 2030 2c20 302c  w: rgba(0, 0, 0,
+0009feb0: 2030 2e33 3529 2030 7078 2035 7078 2031   0.35) 0px 5px 1
+0009fec0: 3570 783b 3b7a 2d69 6e64 6578 3a31 3030  5px;;z-index:100
+0009fed0: 313b 7061 6464 696e 673a 3130 7078 2229  1;padding:10px")
+0009fee0: 0a0a 636c 6173 7320 506f 7028 5461 672e  ..class Pop(Tag.
+0009fef0: 6469 7629 3a0a 2020 2020 6465 6620 696e  div):.    def in
+0009ff00: 6974 2873 656c 662c 6d65 7461 7461 672c  it(self,metatag,
+0009ff10: 6f62 6a2c 7879 3a74 7570 6c65 293a 0a20  obj,xy:tuple):. 
+0009ff20: 2020 2020 2020 2078 2c79 3d78 790a 2020         x,y=xy.  
+0009ff30: 2020 2020 2020 7365 6c66 203c 3d20 566f        self <= Vo
+0009ff40: 696c 6528 5f6f 6e6d 6f75 7365 646f 776e  ile(_onmousedown
+0009ff50: 3d6d 6574 6174 6167 2e73 7465 7065 7665  =metatag.stepeve
+0009ff60: 6e74 2829 290a 2020 2020 2020 2020 7365  nt()).        se
+0009ff70: 6c66 203c 3d20 5461 672e 6469 7628 206f  lf <= Tag.div( o
+0009ff80: 626a 202c 5f73 7479 6c65 3d66 2270 6f73  bj ,_style=f"pos
+0009ff90: 6974 696f 6e3a 6669 7865 643b 746f 703a  ition:fixed;top:
+0009ffa0: 7b79 7d70 783b 6c65 6674 3a7b 787d 7078  {y}px;left:{x}px
+0009ffb0: 3b7a 2d69 6e64 6578 3a31 3030 313b 6261  ;z-index:1001;ba
+0009ffc0: 636b 6772 6f75 6e64 3a77 6869 7465 2229  ckground:white")
+0009ffd0: 0a0a 636c 6173 7320 546f 6173 7428 5461  ..class Toast(Ta
+0009ffe0: 672e 6469 7629 3a0a 2020 2020 6465 6620  g.div):.    def 
+0009fff0: 696e 6974 2873 656c 662c 6d61 696e 5f6e  init(self,main_n
+000a0000: 6f6e 5f75 7365 642c 6f62 6a2c 7469 6d65  on_used,obj,time
+000a0010: 6f75 743d 3130 3030 293a 0a20 2020 2020  out=1000):.     
+000a0020: 2020 2073 656c 6620 3c3d 2054 6167 2e64     self <= Tag.d
+000a0030: 6976 286f 626a 2c5f 7374 796c 653d 2270  iv(obj,_style="p
+000a0040: 6f73 6974 696f 6e3a 6669 7865 643b 7269  osition:fixed;ri
+000a0050: 6768 743a 3130 7078 3b62 6f74 746f 6d3a  ght:10px;bottom:
+000a0060: 3130 7078 3b7a 2d69 6e64 6578 3a31 3030  10px;z-index:100
+000a0070: 313b 222c 205f 636c 6173 733d 226e 6f74  1;", _class="not
+000a0080: 6966 6963 6174 696f 6e20 6973 2d6c 696e  ification is-lin
+000a0090: 6b20 6973 2d6c 6967 6874 2229 0a20 2020  k is-light").   
+000a00a0: 2020 2020 2073 656c 662e 6a73 3d22 7365       self.js="se
+000a00b0: 7454 696d 656f 7574 2820 6675 6e63 7469  tTimeout( functi
+000a00c0: 6f6e 2829 207b 7365 6c66 2e72 656d 6f76  on() {self.remov
+000a00d0: 6528 297d 202c 2025 7329 2220 2520 7469  e()} , %s)" % ti
+000a00e0: 6d65 6f75 740a 0a23 2323 2323 2323 2323  meout..#########
+000a00f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0100: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0110: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0120: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000a0130: 2323 2323 2323 2323 2323 2323 230a 0a63  #############..c
+000a0140: 6c61 7373 2054 6162 7328 5461 672e 6469  lass Tabs(Tag.di
+000a0150: 7629 3a0a 2020 2020 6465 6620 696e 6974  v):.    def init
+000a0160: 2873 656c 662c 6d65 7461 7461 672c 7365  (self,metatag,se
+000a0170: 6c65 6374 6564 3d30 293a 0a20 2020 2020  lected=0):.     
+000a0180: 2020 2075 6c20 3d20 5461 672e 756c 2829     ul = Tag.ul()
+000a0190: 0a20 2020 2020 2020 2066 6f72 2069 6478  .        for idx
+000a01a0: 2c69 2069 6e20 656e 756d 6572 6174 6528  ,i in enumerate(
+000a01b0: 6d65 7461 7461 672e 5f74 6162 7329 3a0a  metatag._tabs):.
+000a01c0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000a01d0: 203d 2068 6173 6174 7472 2869 2c22 6e61   = hasattr(i,"na
+000a01e0: 6d65 2229 2061 6e64 2069 2e6e 616d 6520  me") and i.name 
+000a01f0: 6f72 2022 3f28 6e61 6d65 293f 220a 2020  or "?(name)?".  
+000a0200: 2020 2020 2020 2020 2020 756c 2b3d 5461            ul+=Ta
+000a0210: 672e 6c69 2820 5461 672e 6128 6e61 6d65  g.li( Tag.a(name
+000a0220: 292c 205f 6f6e 636c 6963 6b20 3d20 6d65  ), _onclick = me
+000a0230: 7461 7461 672e 7374 6570 6576 656e 7428  tatag.stepevent(
+000a0240: 7365 6c65 6374 3d69 6478 292c 205f 636c  select=idx), _cl
+000a0250: 6173 733d 2269 732d 6163 7469 7665 2220  ass="is-active" 
+000a0260: 6966 2069 6478 3d3d 7365 6c65 6374 6564  if idx==selected
+000a0270: 2065 6c73 6520 2222 290a 2020 2020 2020   else "").      
+000a0280: 2020 7365 6c66 3c3d 5461 672e 6469 7628    self<=Tag.div(
+000a0290: 756c 2c5f 636c 6173 733d 2274 6162 7322  ul,_class="tabs"
+000a02a0: 290a 2020 2020 2020 2020 6966 206d 6574  ).        if met
+000a02b0: 6174 6167 2e5f 7461 6273 3a20 7365 6c66  atag._tabs: self
+000a02c0: 3c3d 6d65 7461 7461 672e 5f74 6162 735b  <=metatag._tabs[
+000a02d0: 7365 6c65 6374 6564 5d0a                 selected].
```

### Comparing `htagui-0.4.2/htagui/common.py` & `htagui-0.5.0/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.2/htagui/dialog.py` & `htagui-0.5.0/htagui/dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,81 +15,87 @@
 
 class Dialog(Tag.div,MetaTag):
     imports=[cui.Voile,cui.Button,cui.Input]
 
     def init(self,parent):
         self["info"]="UI.current object"
         self._toasts = Tag.div(_info="UI.toasts objects")
-        self._previous=None
+        self._page = Tag.div(_info="UI.page objects")
         parent += self  # auto add
         parent += self._toasts  # add a personnal place for toasts
+        parent += self._page  # add a personnal place for page
         MetaTag.init(self)
 
     def clipboard_copy(self,txt:str):
         self.call(f"""
 let ta = document.createElement('textarea');
 ta.value = `{txt}`;
 self.appendChild(ta);
 ta.select();
 document.execCommand('copy');
 self.removeChild(ta);
 """)
 
-    def alert(self,obj):
-        self.step( alert = obj )
+    def alert(self,obj,size:float=None):
+        """if no size is provided : use the default width size of the dialog (depending of ui used)"""
+        self.step( alert = obj, size=size )
 
-    def box(self,obj,size:float=0.5):
-        self.step( box = obj, size=size )
-        
     def confirm(self,obj,cbresponse=lambda bool:bool):
         self.step( confirm = obj, cb=cbresponse )
         
     def prompt(self,value:str,title,cbresponse=lambda val:val):
         self.step( prompt = value, title=title, cb=cbresponse )
 
+    #DEPRECATED
+    def box(self,obj,size:float=0.5):
+        self.step( alert = obj, size=size )
+        
+
     def notify(self,obj,time=2000):
         self.step( toast = obj, time=time )
 
     def pop(self, obj, xy:tuple):
         self.step( pop = obj, xy=xy )
 
     def drawer(self, obj, mode="left"):
         assert mode in ["left","right","bottom","top"]
         self.step( drawer = obj, mode=mode )
 
     def block(self,obj=None):
         self.step( block=obj )
 
+    def page(self,obj=None):
+        self.step( page = obj)
+
     def close(self):
         self.step()
 
-    def previous(self): # just the previous one (no history yet)
-        if self._previous is None:
-            self.close()
-        else:
-            self._current = self._previous
-            self._previous = None
+    # DEPRECATED
+    def previous(self): 
+        pass
 
     def step(self,**params):
 
         def set(*a,**k):
-            self._previous = self._current
             self(*a,**k)
 
         if "block" in params:
             set( cui.ModalBlock, params["block"] )
+        elif "page" in params:
+            # set( cui.PopPage, params["page"] )
+            if params["page"] is None:
+                self._page.clear()
+            else:
+                self._page.clear( cui.PopPage( self,  params["page"] ))
         elif "alert" in params:
-            set( cui.ModalAlert, params["alert"] )
+            set( cui.ModalAlert, params["alert"], wsize=params.get("size") )
         elif "confirm" in params:
             set( cui.ModalConfirm, params["confirm"], params["cb"] )
         elif "prompt" in params:
             set( cui.ModalPrompt, params["prompt"],params["title"], params["cb"] )
-        elif "box" in params: # NEW
-            size=params["size"]
-            set( cui.ModalBox, params["box"], size )
         elif "pop" in params:
             set( cui.Pop, params["pop"],params["xy"] )
         elif "drawer" in params:
             self( cui.Drawer, params["drawer"], params["mode"] )
         elif "toast" in params:
             self._toasts.clear( cui.Toast( self, params["toast"], params["time"] ))
         else:
```

### Comparing `htagui-0.4.2/htagui/flex.py` & `htagui-0.5.0/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.2/htagui/form.py` & `htagui-0.5.0/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.2/htagui/ifields.py` & `htagui-0.5.0/htagui/ifields.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,23 @@
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
         """ set from serverside, and update UI """
-        #TODO: clean that
-        self.object.attrs["nimp_nawak"] = time.time()
-        self._value = self.caster(value) 
-        if self.prop:
-            self.object.attrs[ self.prop ] = self._value
-        else:
-            self.object.clear( self._value )
+        if hasattr(self,"rerender"):
+            self.rerender( value )
+        else:            
+            self.object.attrs["nimp_nawak"] = time.time()
+            self._value = self.caster(value) 
+            if self.prop:
+                self.object.attrs[ self.prop ] = self._value
+            else:
+                self.object.clear( self._value )
         
 
 class IText(ui.Input,IField):
     def __init__(self, value:str, onchange=lambda ev: None,**k):
         self.onchange = onchange
         ui.Input.__init__(self,_value=value,_type="text",**k)
         IField.__init__(self, self, "value", b"this.value",lambda x: str(x) )
@@ -70,15 +72,18 @@
         ui.Textarea.__init__(self,value,**k)
         IField.__init__(self, self, None, b"this.value",lambda x: str(x) )
 
 class IBool(ui.Input,IField):
     def __init__(self, value:bool, onchange=lambda ev: None,**k):
         self.onchange = onchange
         ui.Input.__init__(self,_checked=bool(value),_type="checkbox",**k)
-        IField.__init__(self, self, "checked", b"this.checked", lambda x: bool(x) )
+        if self.tag.startswith("md-"):
+            IField.__init__(self, self, "selected", b"this.selected", lambda x: bool(x) )
+        else:
+            IField.__init__(self, self, "checked", b"this.checked", lambda x: bool(x) )
 
 class IRange(ui.Input,IField):
     def __init__(self, value:int, onchange=lambda ev: None,**k):
         self.onchange = onchange
         ui.Input.__init__(self,_value=value,_type="range",**k)
         IField.__init__(self, self, "value", b"this.value", lambda x: int(x) )
```

### Comparing `htagui-0.4.2/htagui/shoelace/bases.py` & `htagui-0.5.0/htagui/shoelace/bases.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,17 +111,16 @@
 
 
 class Select(Tag.sl_select):
     statics=SHOELACE
     def init(self,options:ListOrDict, **a):
         options = ensuredict(options)
         self["class"].add("select")
-        default = a.get("_value")
         for k,v in options.items():
-            self <= Tag.sl_option(v,_value=k,_selected=(default==k))
+            self <= Tag.sl_option(v,_value=k,_selected=(str(self.attrs["value"])==str(k)))
 
 class Radios(Tag.sl_radio_group):
     statics=SHOELACE
     def init(self,options:ListOrDict, **a):
         options = ensuredict(options)
         for k,v in options.items():
             self <= Tag.sl_radio(v,_value=k)
@@ -129,17 +128,33 @@
 
 ######################################################################################
 ## Dialog objects
 ######################################################################################
 class Empty(Tag.div):
     def init(self,metatag):
         self.clear()
-        
+
+class PopPage(Tag.div):
+    def init(self,metatag,obj):
+        self["style"].set("position","fixed")
+        self["style"].set("top","0px")
+        self["style"].set("bottom","0px")
+        self["style"].set("right","0px")
+        self["style"].set("left","0px")
+        self["style"].set("z-index","1000")
+        self["style"].set("background","white")
+        self <= obj
+
 class ModalAlert(Tag.sl_dialog):
-    def init(self,metatag,obj,closable=True,pwidth=None):
+    def init(self,metatag,obj,closable=True,wsize:float=None):
+        if wsize is not None:
+            pwidth=f"{int(wsize*100)}%"        
+        else:
+            pwidth=None
+
         self.metatag=metatag
         # self["open"]=True
         self["no-header"]=True
         if pwidth:
             self["style"] = f"--width: {pwidth};"
         self.js = "window.customElements.whenDefined('sl-dialog').then( function() { document.getElementById('%s').show() });" % id(self)
         self.js += """
```

### Comparing `htagui-0.4.2/htagui/splitters.py` & `htagui-0.5.0/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.2/htagui/tabs.py` & `htagui-0.5.0/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.2/pyproject.toml` & `htagui-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.4.2" # auto-updated
+version = "0.5.0" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.4.2/PKG-INFO` & `htagui-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.4.2
+Version: 0.5.0
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -103,24 +103,34 @@
 
 
 ```python
 import htagui as ui
 self <= ui.Input(_value="my value", _name="myfield", _class="myclass", _required=True )
 ```
 
+Availables managed `type`s (setted with `_type`) params:
+ * `text` : the default one (if omitted): an input text
+ * `checkbox` : a checkbox
+ * `radio` : a radio button (non sense : use ui.Radios or uiIRadios !)
+ * `range` : a slider/range
+
+For `text`: a special field "_label" will set the html "placeholder" attribut.
+
 ## Object Textarea
 
 A simple surcharge of Tag.textarea(...), to define a css class 
 
 
 ```python
 import htagui as ui
 self <= ui.Textarea("my value", _name="myfield", _class="myclass", _required=True )
 ```
 
+A special field "_label" will set the html "placeholder" attribut.
+
 ## Object Spinner
 
 A spinner object.
 
 ```python
 import htagui as ui
 self <= ui.Spinner()
@@ -215,30 +225,29 @@
 Note that, there can be only one dialog at a time (except toast notification)
 
 ```python
 import htagui as ui
 dialog = ui.Dialog( self )
 ```
 
-### method dialog.alert(obj)
+### method dialog.alert(obj, size:float=None)
 
 (like js window.alert(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able)
 
+size is a float to force the percent of width on the dialog box. If None, it will use the default from the ui used.
+
 ### method dialog.confirm(obj, cbresponse=lambda bool:bool)
 
 (like js window.confirm(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able), and let the user click on Yes|No buttons, which will call the cbresponse callback with True or False ...
 
 ### method dialog.prompt(value:str, title, cbresponse=lambda val:val)
 
 (like js window.prompt(...)) Display a modal dialog letting the user edit the `value` in an Input box, with a `title` (title must be str'able). When the user click the OK button the value is sent in the callback cbresponse. (clicking the cancel button does nothing, except close the dialog)
 
 
-### method dialog.box(obj,size:float=0.5)
-
-Like dialog.alert(), but display modal dialog box containing the object 'obj' (obj must be str'able), which takes 50% of size.
 
 ### method dialog.notify(obj, time=2000)
 
 Display a toast message (notification), in the right-bottom ... during 2000 ms.
 (currently toast messages are not stacked)
 
 ### method dialog.pop(obj, xy:tuple)
@@ -253,17 +262,21 @@
     "menu1": lambda: dialog.notify("menu1"),
     "menu2": lambda: dialog.notify("menu2"),
     "menu3": lambda: dialog.notify("menu3"),
 }  
 self <= ui.Button("pop menu", _onclick=lambda ev: dialog.pop( ui.Menu(entries) ,(ev.clientX,ev.clientY)) )
 ```
 
-### method dialog.drawer(obj, mode="left", size:float=0.5)
+### method dialog.drawer(obj, mode="left")
+
+Display a drawer, in the left-side. mode can be left,right,top,bottom.
+
+### method dialog.page(obj=None)
 
-Display a drawer, in the left-side, which takes 50% of the page.
+Display a full page 'obj', or remove page if obj is None. (note that ui.close() does not close the page) 
 
 ### method dialog.block(obj=None)
 
 Display a modal dialog box containing the object 'obj'. But the dialog is not closable, so be sure to provide a way to close it.
 
 ### method dialog.close()
```

