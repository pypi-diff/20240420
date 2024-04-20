# Comparing `tmp/mongo_objects-1.0.22.tar.gz` & `tmp/mongo_objects-1.0.26.tar.gz`

## Comparing `mongo_objects-1.0.22.tar` & `mongo_objects-1.0.26.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/requirements.txt
--rw-r--r--   0        0        0    30263 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/src/mongo_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/__init__.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/conftest.py
--rw-r--r--   0        0        0    27835 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoDictProxy.py
--rw-r--r--   0        0        0    31199 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoListProxy.py
--rw-r--r--   0        0        0    27029 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoSingleProxy.py
--rw-r--r--   0        0        0    30057 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_MongoUserDict.py
--rw-r--r--   0        0        0    13782 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoDictProxy.py
--rw-r--r--   0        0        0    15804 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoListProxy.py
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoSingleProxy.py
--rw-r--r--   0        0        0    13699 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_PolymorphicMongoUserDict.py
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tests/test_proxy_combo.py
--rwxr-xr-x   0        0        0      973 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/buildProject
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/runTests
--rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/setupPythonVenv
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/tools/updateRequirements
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/.hgignore
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/pyproject.toml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mongo_objects-1.0.22/PKG-INFO
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/requirements.txt
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/docs/source/conf.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/docs/source/index.rst
+-rw-r--r--   0        0        0    30788 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/src/mongo_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/__init__.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/conftest.py
+-rw-r--r--   0        0        0    27988 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoDictProxy.py
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoListProxy.py
+-rw-r--r--   0        0        0    27139 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoSingleProxy.py
+-rw-r--r--   0        0        0    30562 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_MongoUserDict.py
+-rw-r--r--   0        0        0    13920 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoDictProxy.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoListProxy.py
+-rw-r--r--   0        0        0    15550 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoSingleProxy.py
+-rw-r--r--   0        0        0    13745 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_PolymorphicMongoUserDict.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tests/test_proxy_combo.py
+-rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/buildProject
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/runTests
+-rwxr-xr-x   0        0        0     1960 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/setupPythonVenv
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/tools/updateRequirements
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/.hgignore
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/README.rst
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/pyproject.toml
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 mongo_objects-1.0.26/PKG-INFO
```

### Comparing `mongo_objects-1.0.22/src/mongo_objects.py` & `mongo_objects-1.0.26/src/mongo_objects.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     collection_name = None
     database = None
 
     # The character sequence used to separate the document ID from proxy subdocument keys
     # This may be overriden but it is the user's responsibility to guarantee that this
     # sequence will never appear in any ID or subdoc key.
     # Since the default IDs and subdoc keys are hex, 'g' is a safe separator
-    subdocKeySep = 'g'
+    subdoc_key_sep = 'g'
 
 
     def __init__( self, doc={}, readonly=False ):
         '''Initialize the custom UserDict object
         Flag readonly objects appropriately'''
         super().__init__( doc )
         self.readonly = readonly
@@ -85,15 +85,15 @@
 
     def authorize_read( self ):
         '''Called after a document has been read but before the
         data is returned to the user.
         If the return value is not truthy, the data will
         not be returned.
 
-        Note that if find_one() only inspects the first document
+        Note that find_one() only inspects the first document
         returned by the underlying MongoDB find_one() call. If the
         document returned does not pass authorization, no attempt is
         made to locate another matching document.'''
         return True
 
     def authorize_save( self ):
         '''Called before the current document is saved.
@@ -133,81 +133,87 @@
             obj = cls(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 yield obj
 
 
     @classmethod
-    def find_one( cls, filter={}, projection=None, readonly=False, noMatch=None, **kwargs ):
+    def find_one( cls, filter={}, projection=None, readonly=False, no_match=None, **kwargs ):
         '''Return a single matching document as an instance of this class or None'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
             raise MongoObjectAuthFailed
 
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
             obj = cls(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 return obj
-        return noMatch
+        return no_match
 
 
-    def getUniqueInteger( self, autosave=True ):
+    def get_unique_integer( self, autosave=True ):
         '''Provide the next unique integer for this document.
         These integers are convenient for use as keys of subdocuments.
         Start with 1; 0 is reserved for single proxy documents which don't have a key.
         By default, the document is saved.'''
-        self.setdefault( '_lastUniqueInteger', 0 )
-        self['_lastUniqueInteger'] += 1
+
+        # migrate existing _lastUniqueInteger objects to _last_unique_integer
+        if '_lastUniqueInteger' in self:
+            self['_last_unique_integer'] = self['_lastUniqueInteger']
+            del self['_lastUniqueInteger']
+        else:
+            self.setdefault( '_last_unique_integer', 0 )
+        self['_last_unique_integer'] += 1
         if autosave:
             self.save()
-        return self['_lastUniqueInteger']
+        return self['_last_unique_integer']
 
 
-    def getUniqueKey( self, autosave=True ):
+    def get_unique_key( self, autosave=True ):
         '''Format the next unique integer as a hexidecimal string'''
-        return f"{self.getUniqueInteger( autosave ):x}"
+        return f"{self.get_unique_integer( autosave ):x}"
 
 
     def id( self ):
         '''Convert this document's database ID to a string'''
         return str( self['_id'] )
 
 
     @classmethod
-    def loadById( cls, docId, **kwargs ):
+    def load_by_id( cls, doc_id, **kwargs ):
         '''Locate a document by its database ID'''
-        return cls.find_one( { '_id' : ObjectId( docId ) }, **kwargs )
+        return cls.find_one( { '_id' : ObjectId( doc_id ) }, **kwargs )
 
 
     @classmethod
-    def loadProxyById( cls, id, *args, readonly=False ):
+    def load_proxy_by_id( cls, id, *args, readonly=False ):
         '''Based on a subdocument ID and a list of classes, load the Mongo parent
         documents, create any intermediate proxies and return the requested
         proxy object.
 
-        id is a subdocument ID string separated by subdocKeySep. It includes the
+        id is a subdocument ID string separated by subdoc_key_sep. It includes the
         ObjectId of the top-level MongoDB document
 
         args is a list of proxy objects in descending order. It does not include
         the top-level MongoUserDict class'''
 
-        # split the subdocumentId into its components
-        ids = cls.splitId( id )
+        # split the subdocument_id into its components
+        ids = cls.split_id( id )
 
         # load the MongoDB document and remove the ID from the list of ids
-        obj = cls.loadById( ids.pop(0), readonly=readonly )
+        obj = cls.load_by_id( ids.pop(0), readonly=readonly )
 
         # loop through each level of proxy using the previous object as the parent
-        for (proxyClass, id) in zip( args, ids, strict=True ):
-            obj = proxyClass.getProxy( obj, id )
+        for (proxy_subclass, id) in zip( args, ids, strict=True ):
+            obj = proxy_subclass.get_proxy( obj, id )
 
         # return the lowest-level object
         return obj
 
 
 
     def save( self, force=False ):
@@ -227,21 +233,21 @@
 
         # refuse to save a read-only document
         if self.readonly:
             raise MongoObjectReadOnly( f"Can't save readonly object {type(self)} at {id(self)}" )
 
         # set updated timestamp
         # Note the original value in case we need to roll back
-        addedUpdated = '_updated' not in self
-        originalUpdated = self.get('_updated')
+        added_updated = '_updated' not in self
+        original_updated = self.get('_updated')
         self['_updated'] = self.utcnow()
 
         # add created timestamp if it doesn't exist
         # set flag in case we need to roll back
-        addedCreated = '_created' not in self
+        added_created = '_created' not in self
         self.setdefault( '_created', self['_updated'] )
 
         try:
             # if the document has never been written to the database, write it now and record the ID
             if '_id' not in self:
                 result = self.collection().insert_one( self.data )
                 self['_id'] = result.inserted_id
@@ -249,74 +255,74 @@
             # Force-save a document regardless of timestamp
             elif force:
                 result = self.collection().replace_one( { '_id' : self['_id'] }, self.data, upsert=True )
 
             # Otherwise, only update a document with the same updated timestamp as our in-memory object
             else:
                 result = self.collection().find_one_and_replace(
-                    { '_id' : self['_id'], '_updated' : originalUpdated },
+                    { '_id' : self['_id'], '_updated' : original_updated },
                     self.data,
                     return_document=ReturnDocument.AFTER )
 
                 # on failure, we assume the document has been updated elsewhere and raise an exception
                 assert result is not None, f"document {self.id()} already updated"
 
         # on any error roll back _updated and _created to the original value or remove if we added them
         except Exception as e:
-            if addedCreated:
+            if added_created:
                 del self['_created']
-            if addedUpdated:
+            if added_updated:
                 del self['_updated']
             else:
-                self['_updated'] = originalUpdated
+                self['_updated'] = original_updated
             raise(e)
 
 
     @classmethod
-    def splitId( cls, subdocId ):
+    def split_id( cls, subdoc_id ):
         '''Split a subdocument ID into its component document ID and one or more subdocument keys.'''
-        return subdocId.split( cls.subdocKeySep )
+        return subdoc_id.split( cls.subdoc_key_sep )
 
 
     @staticmethod
     def utcnow():
         '''MongoDB stores milliseconds, not microseconds.
         Drop microseconds from the standard utcnow() so database time comparisons will work.'''
         now = datetime.utcnow()
         return now.replace( microsecond=(now.microsecond // 1000) * 1000 )
 
 
 
 class PolymorphicMongoUserDict( MongoUserDict ):
     '''Like MongoUserDict but supports polymorphic document objects within the same collection.
 
-    Each subclass needs to define a unique subclassKey'''
+    Each subclass needs to define a unique subclass_key'''
 
-    # Map subclassKeys to subclasses
+    # Map subclass_keys to subclasses
     # Override this with an empty dictionary in the base class
     # of your subclass tree to create a separate namespace
-    subclassMap = {}
+    subclass_map = {}
 
     # Must be unique and non-None for each subclass
     # Base classes may define this key as well
-    subclassKey = None
+    subclass_key = None
 
-    # Name of internal key added to each document to record the subclassKey
-    subclassKeyName = '_sckey'
+    # Name of internal key added to each document to record the subclass_key
+    subclass_key_name = '_sckey'
 
 
 
     @classmethod
     def __init_subclass__( cls, **kwargs):
         '''auto-register every PolymorphicMongoUserDict subclass'''
         super().__init_subclass__(**kwargs)
         try:
-            if getattr( cls, 'subclassKey', None ) is not None:
-                assert cls.subclassKey not in cls.subclassMap, f"duplicate subclassKey for {type(cls)}"
-                cls.subclassMap[ cls.subclassKey ] = cls
+            if getattr( cls, 'subclass_key', None ) is not None:
+                assert cls.subclass_key not in cls.subclass_map, f"duplicate subclass_key for {type(cls)}"
+                cls.subclass_map[ cls.subclass_key ] = cls
         except Exception as e:
             raise Exception( 'PolymorphicMongoUserDict(): unable to register subclass' ) from e
 
 
     @classmethod
     def find( cls, filter={}, projection=None, readonly=False, **kwargs ):
         '''Return matching documents as appropriate subclass instances'''
@@ -331,430 +337,430 @@
             obj = cls.instantiate(doc, readonly=readonly)
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 yield obj
 
 
     @classmethod
-    def find_one( cls, filter={}, projection=None, readonly=False, noMatch=None, **kwargs ):
+    def find_one( cls, filter={}, projection=None, readonly=False, no_match=None, **kwargs ):
         '''Return a single matching document as the appropriate subclass or None'''
         # Authorize reading at all
         if not cls.authorize_pre_read():
             raise MongoObjectAuthFailed
 
         # if a projection is provided, force the resulting object to be read-only
         readonly = readonly or projection is not None
 
         doc = cls.collection().find_one( filter, projection, **kwargs )
         if doc is not None:
             obj = cls.instantiate( doc, readonly=readonly )
             # Authorize reading this particular document object before returning it
             if obj.authorize_read():
                 return obj
-        return noMatch
+        return no_match
 
 
     @classmethod
-    def getSubclassByKey( cls, subclassKey ):
-        '''Look up a subclass in the subclassMap by its subclassKey
+    def get_subclass_by_key( cls, subclass_key ):
+        '''Look up a subclass in the subclass_map by its subclass_key
         If the subclass can't be located, return the base class'''
-        return cls.subclassMap.get( subclassKey, cls )
+        return cls.subclass_map.get( subclass_key, cls )
 
 
     @classmethod
-    def getSubclassFromDoc( cls, doc ):
+    def get_subclass_from_doc( cls, doc ):
         '''Return the correct subclass to represent this document.
-        If the document doesn't contain a subclassKeyName value or the value
-        doesn't exist in the subclassMap, return the base class'''
-        return cls.getSubclassByKey( doc.get( cls.subclassKeyName ) )
+        If the document doesn't contain a subclass_key_name value or the value
+        doesn't exist in the subclass_map, return the base class'''
+        return cls.get_subclass_by_key( doc.get( cls.subclass_key_name ) )
 
 
     @classmethod
     def instantiate( cls, doc, readonly=False ):
         '''Instantiate a PolymorphicMongoUserDict subclass based on the content
         of the provided MongoDB document'''
         # Looks like a bug but isn't
         # The first function call determines the correct subclass
         # The second function call populates a new UserDict subclass with data from the document
-        return cls.getSubclassFromDoc( doc )( doc, readonly=readonly )
+        return cls.get_subclass_from_doc( doc )( doc, readonly=readonly )
 
 
     def save( self, force=False ):
-        '''Add the subclassKey and save the document'''
-        if self.subclassKey is not None:
-            self[ self.subclassKeyName ] = self.subclassKey
+        '''Add the subclass_key and save the document'''
+        if self.subclass_key is not None:
+            self[ self.subclass_key_name ] = self.subclass_key
         return super().save( force=force )
 
 
 
 
 ################################################################################
 ## MongoDB subdocument proxies
 ################################################################################
 
 class MongoBaseProxy( object ):
     '''Intended for interal use. Base of all other proxy objects'''
 
     # Users must override this to provide the name of the dictionary or list container
-    containerName = None
+    container_name = None
 
 
     def __contains__( self, key ):
-        return key in self.getSubdoc()
+        return key in self.get_subdoc()
 
 
     def __delitem__( self, key ):
-        del self.getSubdoc()[ key ]
+        del self.get_subdoc()[ key ]
 
 
     def __getitem__( self, key ):
-        return self.getSubdoc()[ key ]
+        return self.get_subdoc()[ key ]
 
 
     def __iter__( self ):
-        return iter( self.getSubdoc().keys() )
+        return iter( self.get_subdoc().keys() )
 
 
     def __setitem__( self, key, value ):
-        self.getSubdoc()[ key ] = value
+        self.get_subdoc()[ key ] = value
 
 
     @classmethod
-    def createKey( cls, parent ):
+    def create_key( cls, parent ):
         '''Create a unique key value for this subdocument.
         The default implementation requests a hex string for the next unique integer
         as saved in the ultimate MongoUserDict parent object.
         Users may override this using data from the subdoc or other methods to generate a unique key.'''
-        return getattr( parent, 'ultimateParent', parent ).getUniqueKey( autosave=False )
+        return getattr( parent, 'ultimate_parent', parent ).get_unique_key( autosave=False )
 
 
     def data( self ):
         '''Convenience function to behave similar to UserDict'''
-        return self.getSubdoc()
+        return self.get_subdoc()
 
 
     def get( self, key, default=None ):
-        return self.getSubdoc().get( key, default )
+        return self.get_subdoc().get( key, default )
 
 
     def id( self ):
-        return f"{self.parent.id()}{self.ultimateParent.subdocKeySep}{self.key}"
+        return f"{self.parent.id()}{self.ultimate_parent.subdoc_key_sep}{self.key}"
 
 
     def items( self ):
-        return self.getSubdoc().items()
+        return self.get_subdoc().items()
 
 
     def keys( self ):
-        return self.getSubdoc().keys()
+        return self.get_subdoc().keys()
 
 
     def setdefault( self, key, default=None ):
-        return self.getSubdoc().setdefault( key, default )
+        return self.get_subdoc().setdefault( key, default )
 
 
     def update( self, values ):
-        self.getSubdoc().update( values )
+        self.get_subdoc().update( values )
 
 
     def save( self ):
         return self.parent.save()
 
 
     def values( self ):
-        return self.getSubdoc().values()
+        return self.get_subdoc().values()
 
 
 
 
 class PolymorphicMongoBaseProxy( MongoBaseProxy ):
     '''Like MongoBaseProxy but supports polymorphic subdocument objects within the same parent document.
 
-    Each subclass needs to define a unique proxySubclassKey
+    Each subclass needs to define a unique proxy_subclass_key
 
     Parent objects need to call instantiate() to create the correct subclass type'''
 
-    # Map proxySubclassKeys to subclasses
+    # Map proxy_subclass_keys to subclasses
     # Override this with an empty dictionary in the base class
     # of your subclass tree to create a separate namespace
-    proxySubclassMap = {}
+    proxy_subclass_map = {}
 
     # Must be unique and non-None for each subclass
     # Base classes may define this key as well
-    proxySubclassKey = None
+    proxy_subclass_key = None
 
-    # Name of internal key added to each subdocument to record the proxySubclassKey
-    proxySubclassKeyName = '_psckey'
+    # Name of internal key added to each subdocument to record the proxy_subclass_key
+    proxy_subclass_key_name = '_psckey'
 
 
     @classmethod
     def __init_subclass__( cls, **kwargs):
         '''auto-register every PolymorphicMongoBaseProxy subclass'''
         super().__init_subclass__(**kwargs)
         try:
-            if getattr( cls, 'proxySubclassKey', None ) is not None:
-                assert cls.proxySubclassKey not in cls.proxySubclassMap, f"duplicate proxySubclassKey for {type(cls)}"
-                cls.proxySubclassMap[ cls.proxySubclassKey ] = cls
+            if getattr( cls, 'proxy_subclass_key', None ) is not None:
+                assert cls.proxy_subclass_key not in cls.proxy_subclass_map, f"duplicate proxy_subclass_key for {type(cls)}"
+                cls.proxy_subclass_map[ cls.proxy_subclass_key ] = cls
         except Exception as e:
             raise Exception( 'PolymorphicMongoBaseProxy(): unable to register subclass' ) from e
 
 
     @classmethod
     def create( cls, parent, subdoc={}, autosave=True ):
-        '''Add the proxySubclassKey before passing to the base class create()'''
-        if cls.proxySubclassKey is not None:
-            subdoc[ cls.proxySubclassKeyName ] = cls.proxySubclassKey
+        '''Add the proxy_subclass_key before passing to the base class create()'''
+        if cls.proxy_subclass_key is not None:
+            subdoc[ cls.proxy_subclass_key_name ] = cls.proxy_subclass_key
         return super().create( parent, subdoc, autosave=autosave )
 
 
     @classmethod
-    def getSubclassByKey( cls, proxySubclassKey ):
-        '''Look up a proxySubclass in the proxySubclassMap by its proxySubclassKey
+    def get_subclass_by_key( cls, proxy_subclass_key ):
+        '''Look up a proxy_subclass in the proxy_subclass_map by its proxy_subclass_key
         If the subclass can't be located, return the called class'''
-        return cls.proxySubclassMap.get( proxySubclassKey, cls )
+        return cls.proxy_subclass_map.get( proxy_subclass_key, cls )
 
 
     @classmethod
-    def getSubclassFromDoc( cls, doc ):
+    def get_subclass_from_doc( cls, doc ):
         '''Return the correct subclass to represent this document.
-        If the document doesn't contain a proxySubclassKeyName value or the value
-        doesn't exist in the proxySubclassMap, return the base class'''
-        return cls.getSubclassByKey( doc.get( cls.proxySubclassKeyName ) )
+        If the document doesn't contain a proxy_subclass_key_name value or the value
+        doesn't exist in the proxy_subclass_map, return the base class'''
+        return cls.get_subclass_by_key( doc.get( cls.proxy_subclass_key_name ) )
 
 
 
 
 class AccessDictProxy( object ):
     '''Intended for internal multiple-inheritance use.
 
     Organize functions to reference subdocuments within a parent MongoDB dictionary.
     Individual subdocuments are stored in a dictionary container.
 
     Keys must be strings as required by MongoDB documents.
 
-    MongoUserDict.getUniqueKey() is a convenient way to generate unique keys
+    MongoUserDict.get_unique_key() is a convenient way to generate unique keys
     within a MongoDB document.
     '''
 
     def __init__( self, parent, key ):
         self.parent = parent
-        self.ultimateParent = getattr( parent, 'ultimateParent', parent )
+        self.ultimate_parent = getattr( parent, 'ultimate_parent', parent )
         self.key = str(key)
 
         # make sure this key actually exists before we return successfully
-        assert self.key in self.getSubdocContainer()
+        assert self.key in self.get_subdoc_container()
 
 
     @classmethod
     def create( cls, parent, subdoc={}, autosave=True ):
         '''Add a new subdocument to the container.
         Auto-assign the ID
         Return the new proxy object'''
-        key = cls.createKey( parent )
+        key = cls.create_key( parent )
 
         # insure the container exists before adding the document
-        parent.setdefault( cls.containerName, {} )[ key ] = subdoc
+        parent.setdefault( cls.container_name, {} )[ key ] = subdoc
         if autosave:
             parent.save()
-        return cls.getProxy( parent, key )
+        return cls.get_proxy( parent, key )
 
 
 
     def delete( self, autosave=True ):
         '''Delete the subdocument from the container dictionary.
         Remove the key so the proxy can't be referenced again.
         By default save the parent document'''
-        del self.getSubdocContainer()[ self.key ]
+        del self.get_subdoc_container()[ self.key ]
         if autosave:
             self.parent.save()
         self.key = None
 
 
     @classmethod
-    def getProxies( cls, parent ):
-        return [ cls.getProxy( parent, key ) for key in parent.get( cls.containerName, {} ).keys() ]
+    def get_proxies( cls, parent ):
+        return [ cls.get_proxy( parent, key ) for key in parent.get( cls.container_name, {} ).keys() ]
 
 
-    def getSubdoc( self ):
-        return self.getSubdocContainer()[ self.key ]
+    def get_subdoc( self ):
+        return self.get_subdoc_container()[ self.key ]
 
 
-    def getSubdocContainer( self ):
-        return self.parent.get( self.containerName, {} )
+    def get_subdoc_container( self ):
+        return self.parent.get( self.container_name, {} )
 
 
 
 
 class MongoDictProxy( MongoBaseProxy, AccessDictProxy ):
     '''Implement proxy object using a dictionary as a container'''
 
     @classmethod
-    def getProxy( cls, parent, key ):
+    def get_proxy( cls, parent, key ):
         '''Return a single proxy object. For non-polymorphic use,
         this simply calls __init__()'''
         return cls( parent, key )
 
 
 
 
 class PolymorphicMongoDictProxy( PolymorphicMongoBaseProxy, AccessDictProxy ):
     '''Polymorphic version of MongoDictProxy'''
 
     @classmethod
-    def getProxy( cls, parent, key ):
+    def get_proxy( cls, parent, key ):
         '''Return a single proxy object. For PolymorphicMongoDictProxy,
         determine the correct subclass type and call __init__()'''
         # use an anonymous base-class proxy to get access to the subdocument
-        # so that getSubclassFromDoc can inspect the data and determine the
+        # so that get_subclass_from_doc can inspect the data and determine the
         # appropriate subclass.
         # Return a separate proxy object with that class
-        return cls.getSubclassFromDoc( cls( parent, key ) )( parent, key )
+        return cls.get_subclass_from_doc( cls( parent, key ) )( parent, key )
 
 
 
 
 class AccessListProxy( object ):
     '''Intended for internal multiple-inheritance use.
 
     Organize functions to reference subdocuments within a parent MongoDB dictionary.
     Individual subdocuments are stored in a list container.
 
     Since the container object is a list, not a dictionary, we can't use the key
     to look up items directly.
 
-    Instead, we use getKey() to extract a key from a subdocument
+    Instead, we use get_key() to extract a key from a subdocument
     and use the result to determine if a given document matches.
 
     For convenience, if no key is given but a sequence provided, we initialize the key from
     the subdocument at that index'''
 
     # The name of the internal key added to each subdoc to store the unique subdocument "key" value
     # Subclasses may override this name or
-    # override getKey() and setKey() to implement their own mechanism of locating subdocuments
-    subdocKeyName = '_sdkey'
+    # override get_key() and set_key() to implement their own mechanism of locating subdocuments
+    subdoc_key_name = '_sdkey'
 
 
     def __init__( self, parent, key=None, seq=None ):
         self.parent = parent
-        self.ultimateParent = getattr( parent, 'ultimateParent', parent )
+        self.ultimate_parent = getattr( parent, 'ultimate_parent', parent )
 
         if key is not None:
             self.key = key
             self.seq = seq
         elif seq is not None:
-            self.key = self.getKey( self.getSubdocContainer()[ seq ] )
+            self.key = self.get_key( self.get_subdoc_container()[ seq ] )
             self.seq = seq
         else:
             raise Exception( "MongoListProxy(): key or seq must be provided" )
 
 
     @classmethod
     def create( cls, parent, subdoc={}, autosave=True ):
         '''Add a new subdocument to the container.
         Auto-assign the ID
         Return the new proxy object.
         '''
         # Create a unique key for this subdocument
-        key = cls.createKey( parent )
+        key = cls.create_key( parent )
 
         # Add the key to the subdocument
-        cls.setKey( subdoc, key )
+        cls.set_key( subdoc, key )
 
         # Append the new subdocument to the list
-        container = parent.setdefault( cls.containerName, [] )
+        container = parent.setdefault( cls.container_name, [] )
         container.append( subdoc )
 
         # Save if requested
         if autosave:
             parent.save()
 
         # Since we know we just appended to the end of the list, provide
         # the sequence as well as the key
-        return cls.getProxy( parent, key, len( container ) - 1 )
+        return cls.get_proxy( parent, key, len( container ) - 1 )
 
 
     def delete( self, autosave=True ):
         '''Delete the subdocument from the container list.
         Remove the key and sequence so the proxy can't be referenced again.
         By default save the parent document.
         '''
 
         # First make sure the sequence number is accurate
-        self.getSubdoc()
+        self.get_subdoc()
         # Then pop that item from the list
-        self.getSubdocContainer().pop( self.seq )
+        self.get_subdoc_container().pop( self.seq )
         if autosave:
             self.parent.save()
         self.key = self.seq = None
 
 
     @classmethod
-    def getKey( cls, subdoc ):
+    def get_key( cls, subdoc ):
         '''Extract the key from a subdocument dictionary.'''
-        return subdoc[ cls.subdocKeyName ]
+        return subdoc[ cls.subdoc_key_name ]
 
 
     @classmethod
-    def getProxies( cls, parent ):
-        return [ cls.getProxy( parent, seq=seq ) for seq in range( len( parent.get( cls.containerName, [] ) ) ) ]
+    def get_proxies( cls, parent ):
+        return [ cls.get_proxy( parent, seq=seq ) for seq in range( len( parent.get( cls.container_name, [] ) ) ) ]
 
 
-    def getSubdoc( self ):
+    def get_subdoc( self ):
         # We don't want to iterate the list each time looking for the subdoc that matches
         # EAFTP: If the document at self.seq is a match, return it
         # Otherwise, scan the list for a match.
         # Since __init__() sets self.seq to None, the item will automatically be located on first use
         try:
-            subdoc = self.getSubdocContainer()[ self.seq ]
-            assert self.key == self.getKey( subdoc )
+            subdoc = self.get_subdoc_container()[ self.seq ]
+            assert self.key == self.get_key( subdoc )
             return subdoc
         except:
-            for (seq, subdoc) in enumerate( self.getSubdocContainer() ):
-                if self.key == self.getKey( subdoc ):
+            for (seq, subdoc) in enumerate( self.get_subdoc_container() ):
+                if self.key == self.get_key( subdoc ):
                     self.seq = seq
                     return subdoc
-            raise Exception( "MongoListProxy.getSubdoc(): no match found" )
+            raise Exception( "MongoListProxy.get_subdoc(): no match found" )
 
 
-    def getSubdocContainer( self ):
-        return self.parent.get( self.containerName, [] )
+    def get_subdoc_container( self ):
+        return self.parent.get( self.container_name, [] )
 
 
     @classmethod
-    def setKey( cls, subdoc, key ):
+    def set_key( cls, subdoc, key ):
         '''Set the key in a subdocument dictionary.'''
-        subdoc[ cls.subdocKeyName ] = key
+        subdoc[ cls.subdoc_key_name ] = key
 
 
 
 
 class MongoListProxy( MongoBaseProxy, AccessListProxy ):
     '''Implement proxy object using a list as a container'''
 
     @classmethod
-    def getProxy( cls, parent, key=None, seq=None ):
+    def get_proxy( cls, parent, key=None, seq=None ):
         '''Return a single proxy object. For non-polymorphic use,
         this simply calls __init__()'''
         return cls( parent, key, seq )
 
 
 
 
 class PolymorphicMongoListProxy( PolymorphicMongoBaseProxy, AccessListProxy ):
     '''Polymorphic version of MongoListProxy'''
 
     @classmethod
-    def getProxy( cls, parent, key=None, seq=None ):
+    def get_proxy( cls, parent, key=None, seq=None ):
         '''Return a single proxy object. For PolymorphicMongoDictProxy,
         determine the correct subclass type and call __init__()'''
         # use an anonymous base-class proxy to get access to the subdocument
-        # so that getSubclassFromDoc can inspect the data and determine the
+        # so that get_subclass_from_doc can inspect the data and determine the
         # appropriate subclass.
         # Return a separate proxy object with that class
-        return cls.getSubclassFromDoc( cls( parent, key, seq ) )( parent, key, seq )
+        return cls.get_subclass_from_doc( cls( parent, key, seq ) )( parent, key, seq )
 
 
 
 
 class AccessSingleProxy( AccessDictProxy ):
     '''Intended for internal multiple-inheritance use.
 
@@ -766,84 +772,84 @@
     Keys must be strings as required by MongoDB documents.
     '''
 
     @classmethod
     def create( cls, parent, subdoc={}, key=None, autosave=True ):
         '''Add a new single subdocument dictionary to the parent object.
         No new key is auto-assigned as single subdocuments are assigned to fixed keys.
-        The key can be defined in the class as "containerName"
+        The key can be defined in the class as "container_name"
         or overriden on the command line as "key".
         Return the new proxy object.
         '''
         if key is None:
-            key = cls.containerName
+            key = cls.container_name
         parent[ key ] = subdoc
         if autosave:
             parent.save()
-        return cls.getProxy( parent, key )
+        return cls.get_proxy( parent, key )
 
 
     @classmethod
-    def getProxies( cls, parent ):
-        '''getProxies() doesn't make sense for single proxy use.
+    def get_proxies( cls, parent ):
+        '''get_proxies() doesn't make sense for single proxy use.
         This is a class method and we don't know the key, so
         we don't know which of the parent's subdocuments to return'''
-        raise Exception( 'single proxy objects do not support getProxies()' )
+        raise Exception( 'single proxy objects do not support get_proxies()' )
 
 
-    def getSubdocContainer( self ):
+    def get_subdoc_container( self ):
         '''For a single subdocument dictionary, the container is the parent document.'''
         return self.parent
 
 
     def id( self ):
         '''Force the subdocument ID for single proxies to "0". We
         can't use the actual key as we risk exposing the actual
         dictionary key name.'''
-        return f"{self.parent.id()}{self.ultimateParent.subdocKeySep}0"
+        return f"{self.parent.id()}{self.ultimate_parent.subdoc_key_sep}0"
 
 
 
 
 
 
 class MongoSingleProxy( AccessSingleProxy, MongoBaseProxy ):
     '''Implement proxy object for a single subdocument dictionary'''
 
     @classmethod
-    def getProxy( cls, parent, key=None ):
+    def get_proxy( cls, parent, key=None ):
         '''Return a single proxy object. For non-polymorphic use,
         this simply calls __init__()'''
         if key is None:
-            key = cls.containerName
+            key = cls.container_name
         return cls( parent, key )
 
 
 
 
 class PolymorphicMongoSingleProxy( AccessSingleProxy, PolymorphicMongoBaseProxy ):
     '''Polymorphic version of MongoSingleProxy'''
 
     @classmethod
     def create( cls, parent, subdoc={}, key=None, autosave=True ):
-        '''Add the proxySubclassKey before passing to the base class create()
+        '''Add the proxy_subclass_key before passing to the base class create()
         AccessSingleProxy needs to be first in the object inheritance to get
         super() to work properly'''
-        if cls.proxySubclassKey is not None:
-            subdoc[ cls.proxySubclassKeyName ] = cls.proxySubclassKey
+        if cls.proxy_subclass_key is not None:
+            subdoc[ cls.proxy_subclass_key_name ] = cls.proxy_subclass_key
         return super().create( parent, subdoc, key=key, autosave=autosave )
 
 
     @classmethod
-    def getProxy( cls, parent, key=None ):
+    def get_proxy( cls, parent, key=None ):
         '''Return a single proxy object. For PolymorphicMongoDictProxy,
         determine the correct subclass type and call __init__()'''
         # use an anonymous base-class proxy to get access to the subdocument
-        # so that getSubclassFromDoc can inspect the data and determine the
+        # so that get_subclass_from_doc can inspect the data and determine the
         # appropriate subclass.
         # Return a separate proxy object with that class
         if key is None:
-            key = cls.containerName
-        return cls.getSubclassFromDoc( cls( parent, key ) )( parent, key )
+            key = cls.container_name
+        return cls.get_subclass_from_doc( cls( parent, key ) )( parent, key )
```

### Comparing `mongo_objects-1.0.22/tests/test_MongoDictProxy.py` & `mongo_objects-1.0.26/tests/test_MongoDictProxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     '''Return a MongoUserDict configured for a per-class unique collection'''
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoDictProxyA( mongo_objects.MongoDictProxy ):
-        containerName = 'proxyA'
+        container_name = 'proxyA'
 
     class MyMongoDictProxyA1( mongo_objects.MongoDictProxy ):
-        containerName = 'proxyA1'
+        container_name = 'proxyA1'
 
     class MyMongoDictProxyB( mongo_objects.MongoDictProxy ):
-        containerName = 'proxyB'
+        container_name = 'proxyB'
 
     return {
         'base' : MyMongoUserDict,
         'A' : MyMongoDictProxyA,
         'A1' : MyMongoDictProxyA1,
         'B' : MyMongoDictProxyB
     }
@@ -78,108 +78,108 @@
     return classes['base'].find_one()
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent ):
     classes = getPopulatedMMUDClasses
     # return the first proxyA in the list
-    return classes['A'].getProxies( getSampleParent )[0]
+    return classes['A'].get_proxies( getSampleParent )[0]
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA1( getPopulatedMMUDClasses, getSampleProxyA ):
     classes = getPopulatedMMUDClasses
     # return the first proxyA1 in the list
-    return classes['A1'].getProxies( getSampleProxyA )[0]
+    return classes['A1'].get_proxies( getSampleProxyA )[0]
 
 
 
 
 class TestCreate:
     def test_create( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
 
         # create a new entry in a level one proxy
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
 
         # verify a new entry was created
-        assert len( proxyA.getSubdocContainer().keys() ) == count+1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container().keys() ) == count+1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
     def test_create_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
 
         # create a new entry in a level one proxy without saving the parent
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
 
         # verify a new entry was created
-        assert len( proxyA.getSubdocContainer().keys() ) == count+1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container().keys() ) == count+1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
     def test_create_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a new entry in a level two proxy
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 + 1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 + 1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
     def test_create_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a new entry in a level two proxy without saving the parent
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=None )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 + 1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 + 1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
@@ -187,103 +187,103 @@
     def test_delete( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy
         proxyA.delete()
 
         # verify the entry was deleted
-        assert key not in proxyA.getSubdocContainer().keys()
+        assert key not in proxyA.get_subdoc_container().keys()
         assert proxyA.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == count-1
+        assert len( proxyA.get_subdoc_container().keys() ) == count-1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestDelete_ProxyA_No_Save:
     def test_delete_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy without saving the parent
         proxyA.delete( autosave=False )
 
         # verify the entry was deleted
-        assert key not in proxyA.getSubdocContainer().keys()
+        assert key not in proxyA.get_subdoc_container().keys()
         assert proxyA.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == count-1
+        assert len( proxyA.get_subdoc_container().keys() ) == count-1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
 class TestDelete_ProxyA1:
     def test_delete_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete()
 
         # verify the entry was deleted
-        assert key not in proxyA1.getSubdocContainer().keys()
+        assert key not in proxyA1.get_subdoc_container().keys()
         assert proxyA1.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 - 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 - 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 
 
 class TestDelete_ProxyA1_No_Save:
     def test_delete_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete( autosave=False )
 
         # verify the entry was deleted
-        assert key not in proxyA1.getSubdocContainer().keys()
+        assert key not in proxyA1.get_subdoc_container().keys()
         assert proxyA1.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 - 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 - 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
@@ -326,15 +326,15 @@
         # verify that the key no longer exists
         assert 'nameA1' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimateParent['_id'] } )
+        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA1' not in doc['proxyA'][ proxy.parent.key ]['proxyA1'][ proxy.key ]
 
 
 
 class TestSetDefault:
@@ -439,15 +439,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimateParent['_id'] } )
+        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc['proxyA'][ proxy.parent.key ]['proxyA1'][ proxy.key ]
         assert doc['proxyA'][ proxy.parent.key ]['proxyA1'][ proxy.key ]['newKey'] == 'this is a new value'
 
 
 
@@ -503,33 +503,33 @@
         assert proxy['newKey2'] == 2
         assert len( proxy.keys() ) == count + 2
 
 
 
 
 class TestBasics:
-    def test_createKey( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_create_key( self, getPopulatedMMUDClasses, getSampleProxyA ):
         '''Test key creation for single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
         updated = parent['_updated']
 
         # create a proxyA key
-        keyA = classes['A'].createKey( parent )
+        keyA = classes['A'].create_key( parent )
         assert isinstance( keyA, str )
-        assert keyA == f"{parent['_lastUniqueInteger']:x}"
+        assert keyA == f"{parent['_last_unique_integer']:x}"
 
         # create a proxyA1 key
-        keyA1 = classes['A1'].createKey( proxyA )
+        keyA1 = classes['A1'].create_key( proxyA )
         assert isinstance( keyA1, str )
-        assert keyA1 == f"{parent['_lastUniqueInteger']:x}"
+        assert keyA1 == f"{parent['_last_unique_integer']:x}"
         assert keyA != keyA1
 
-        # verify that createKey doesn't save the parent object
+        # verify that create_key doesn't save the parent object
         doc = classes['base'].collection().find_one( { '_id' : parent['_id'] } )
         assert doc['_updated'] == updated
 
 
     def test_contains( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert 'nameA' in proxy
@@ -547,15 +547,15 @@
         # verify that the data references the same dictionary
         assert id( proxy.data() ) == id( proxy.parent['proxyA'][proxy.key] )
 
 
     def test_data_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         # verify that the data references the same dictionary
-        assert id( proxy.data() ) == id( proxy.ultimateParent['proxyA'][proxy.parent.key]['proxyA1'][proxy.key] )
+        assert id( proxy.data() ) == id( proxy.ultimate_parent['proxyA'][proxy.parent.key]['proxyA1'][proxy.key] )
 
 
     def test_get( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert proxy.get('nameA') is not None
         assert proxy.get('will-not-match') is None
 
@@ -576,134 +576,134 @@
     def test_getitem_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         assert proxy['nameA1'] is not None
         with pytest.raises( Exception ):
             assert proxy['will-not-match']
 
 
-    def test_getProxies( self, getPopulatedMMUDClasses, getSampleParent ):
+    def test_get_proxies( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test accessing both first-level and second-level proxy lists'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # get all keys in the proxy A container
-        keysA = list( parent[ classes['A'].containerName ].keys() )
+        keysA = list( parent[ classes['A'].container_name ].keys() )
 
         # get all first-level proxies
-        result = classes['A'].getProxies( parent )
+        result = classes['A'].get_proxies( parent )
 
         # verify type and length of the result
         assert isinstance( result, list )
         assert len( result ) == len( keysA )
 
         # verify all expected keys are present
         assert len( set( keysA ).symmetric_difference( [ x.key for x in result ] ) ) == 0
 
         # verify type matches
         for proxy in result:
             assert isinstance( proxy, classes['A'])
 
         # choose a proxyA to continue testing with
-        proxyA = classes['A'].getProxy( parent, keysA[0] )
+        proxyA = classes['A'].get_proxy( parent, keysA[0] )
 
         # get all keys in the proxy A1 container of the selected proxyA object
-        keysA1 = list( parent[ classes['A'].containerName ][ proxyA.key ][ classes['A1'].containerName ].keys() )
+        keysA1 = list( parent[ classes['A'].container_name ][ proxyA.key ][ classes['A1'].container_name ].keys() )
 
         # get all second-level proxies
-        result = classes['A1'].getProxies( proxyA )
+        result = classes['A1'].get_proxies( proxyA )
 
         # verify type and length of the result
         assert isinstance( result, list )
         assert len( result ) == len( keysA1 )
 
         # verify all expected keys are present
         assert len( set( keysA1 ).symmetric_difference( [ x.key for x in result ] ) ) == 0
 
         # verify type matches
         for proxy in result:
             assert isinstance( proxy, classes['A1'])
 
 
-    def test_getProxies_empty( self, getPopulatedMMUDClasses ):
+    def test_get_proxies_empty( self, getPopulatedMMUDClasses ):
         '''Test get proxies from an empty object'''
         classes = getPopulatedMMUDClasses
 
         # collect proxies from an empty object
-        result = classes['A'].getProxies( {} )
+        result = classes['A'].get_proxies( {} )
         assert len(result) == 0
 
 
-    def test_getProxy( self, getPopulatedMMUDClasses, getSampleParent ):
+    def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test accessing both first-level and second-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # locate the first key in the proxy A container
-        keyA = list( parent[ classes['A'].containerName ].keys() )[0]
+        keyA = list( parent[ classes['A'].container_name ].keys() )[0]
 
         # create a first-level proxy object
-        proxyA = classes['A'].getProxy( parent, keyA )
+        proxyA = classes['A'].get_proxy( parent, keyA )
 
         # verify dictionary and type matches
-        assert id( proxyA.data() ) == id( parent[ classes['A'].containerName ][ keyA ] )
+        assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ][ keyA ] )
         assert isinstance( proxyA, classes['A'])
 
         # locate the first key in the proxy A1 container
-        keyA1 = list( parent[ classes['A'].containerName ][ keyA ][ classes['A1'].containerName ].keys() )[0]
+        keyA1 = list( parent[ classes['A'].container_name ][ keyA ][ classes['A1'].container_name ].keys() )[0]
 
         # create a second-level proxy object
-        proxyA1 = classes['A1'].getProxy( proxyA, keyA1 )
+        proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
 
         # verify dictionary and type matches
-        assert id( proxyA1.data() ) == id( parent[ classes['A'].containerName ][ keyA ][ classes['A1'].containerName ][ keyA1 ] )
+        assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][ keyA ][ classes['A1'].container_name ][ keyA1 ] )
         assert isinstance( proxyA1, classes['A1'])
 
 
-    def test_getSubdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_get_subdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
-        assert id( proxyA.getSubdoc() ) == id( proxyA.parent[ classes['A'].containerName ][ proxyA.key ] )
+        assert id( proxyA.get_subdoc() ) == id( proxyA.parent[ classes['A'].container_name ][ proxyA.key ] )
 
 
-    def test_getSubdoc_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_get_subdoc_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # verify data location
-        assert id( proxyA1.getSubdoc() ) == id( proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA1.parent.key ][ classes['A1'].containerName ][ proxyA1.key ] )
+        assert id( proxyA1.get_subdoc() ) == id( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA1.parent.key ][ classes['A1'].container_name ][ proxyA1.key ] )
 
 
-    def test_getSubdocContainer( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_get_subdoc_container( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
-        assert id( proxyA.getSubdocContainer() ) == id( proxyA.parent[ classes['A'].containerName ] )
+        assert id( proxyA.get_subdoc_container() ) == id( proxyA.parent[ classes['A'].container_name ] )
 
 
-    def test_getSubdocContainer_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_get_subdoc_container_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # verify data location
-        assert id( proxyA1.getSubdocContainer() ) == id( proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA1.parent.key ][ classes['A1'].containerName ] )
+        assert id( proxyA1.get_subdoc_container() ) == id( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA1.parent.key ][ classes['A1'].container_name ] )
 
 
     def test_id( self, getSampleProxyA ):
         '''Test ID for single level proxy'''
         proxy = getSampleProxyA
-        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdocKeySep}{proxy.key}"
+        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
         '''Test ID for two-level proxy'''
         proxy = getSampleProxyA1
-        assert proxy.id() == f"{proxy.ultimateParent.id()}{proxy.ultimateParent.subdocKeySep}{proxy.parent.key}{proxy.ultimateParent.subdocKeySep}{proxy.key}"
+        assert proxy.id() == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_init( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test initialization of single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
@@ -745,23 +745,23 @@
 
 
 
     def test_items( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
-        assert proxy.items() == proxy.parent[ classes['A'].containerName ][ proxy.key ].items()
+        assert proxy.items() == proxy.parent[ classes['A'].container_name ][ proxy.key ].items()
 
 
     def test_items_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
-        assert proxyA1.items() == proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA.key ][ classes['A1'].containerName ][ proxyA1.key ].items()
+        assert proxyA1.items() == proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.key ][ classes['A1'].container_name ][ proxyA1.key ].items()
 
 
     def test_iter( self, getSampleProxyA ):
         proxy = getSampleProxyA
         # compare the keys
         assert set( [ key for key in proxy ] ) == set( proxy.parent['proxyA'][ proxy.key ].keys() )
 
@@ -772,23 +772,23 @@
         assert set( [ key for key in proxy ] ) == set( proxy.parent['proxyA1'][ proxy.key ].keys() )
 
 
     def test_keys( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
-        assert proxy.keys() == proxy.parent[ classes['A'].containerName ][ proxy.key ].keys()
+        assert proxy.keys() == proxy.parent[ classes['A'].container_name ][ proxy.key ].keys()
 
 
     def test_keys_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
-        assert proxyA1.keys() == proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA.key ][ classes['A1'].containerName ][ proxyA1.key ].keys()
+        assert proxyA1.keys() == proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.key ][ classes['A1'].container_name ][ proxyA1.key ].keys()
 
 
     def test_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # preserve original state
@@ -802,33 +802,33 @@
 
 
     def test_save_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # preserve original state
-        original = dict( proxyA1.ultimateParent )
+        original = dict( proxyA1.ultimate_parent )
 
         # save the object
         proxyA1.save()
 
         # verify the parent document was saved
-        assert proxyA1.ultimateParent['_updated'] > original['_updated']
+        assert proxyA1.ultimate_parent['_updated'] > original['_updated']
 
 
     def test_values( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
         # compare contents of values() as lists (dict_values objects don't compare properly)
-        assert list( proxy.values() ) == list( proxy.parent[ classes['A'].containerName ][ proxy.key ].values() )
+        assert list( proxy.values() ) == list( proxy.parent[ classes['A'].container_name ][ proxy.key ].values() )
 
 
     def test_values_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
         # compare contents of values() as lists (dict_values objects don't compare properly)
-        assert list( proxyA1.values() ) == list( proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA.key ][ classes['A1'].containerName ][ proxyA1.key ].values() )
+        assert list( proxyA1.values() ) == list( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.key ][ classes['A1'].container_name ][ proxyA1.key ].values() )
```

### Comparing `mongo_objects-1.0.22/tests/test_MongoListProxy.py` & `mongo_objects-1.0.26/tests/test_MongoListProxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     '''Return a MongoUserDict configured for a per-class unique collection'''
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoListProxyA( mongo_objects.MongoListProxy ):
-        containerName = 'proxyA'
+        container_name = 'proxyA'
 
     class MyMongoListProxyA1( mongo_objects.MongoListProxy ):
-        containerName = 'proxyA1'
+        container_name = 'proxyA1'
 
     class MyMongoListProxyB( mongo_objects.MongoListProxy ):
-        containerName = 'proxyB'
+        container_name = 'proxyB'
 
     return {
         'base' : MyMongoUserDict,
         'A' : MyMongoListProxyA,
         'A1' : MyMongoListProxyA1,
         'B' : MyMongoListProxyB
     }
@@ -78,136 +78,136 @@
     return classes['base'].find_one()
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent ):
     classes = getPopulatedMMUDClasses
     # return the first proxyA in the list
-    return classes['A'].getProxies( getSampleParent )[0]
+    return classes['A'].get_proxies( getSampleParent )[0]
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA1( getPopulatedMMUDClasses, getSampleProxyA ):
     classes = getPopulatedMMUDClasses
     # return the first proxyA1 in the list
-    return classes['A1'].getProxies( getSampleProxyA )[0]
+    return classes['A1'].get_proxies( getSampleProxyA )[0]
 
 
 # utility functions
-def getKeys( proxy ):
-    return [ proxy.getKey( doc ) for doc in proxy.getSubdocContainer() ]
+def get_keys( proxy ):
+    return [ proxy.get_key( doc ) for doc in proxy.get_subdoc_container() ]
 
 
 
 class TestCreate:
     def test_create( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer() )
+        count = len( proxyA.get_subdoc_container() )
 
         # create a new entry in a level one proxy
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
 
         # verify a key was added to the proxy
-        assert proxyA.subdocKeyName in newProxy
+        assert proxyA.subdoc_key_name in newProxy
 
         # verify new key exists in the list
-        assert newProxy.key in getKeys( proxyA )
+        assert newProxy.key in get_keys( proxyA )
 
         # verify a new entry was created
-        assert len( proxyA.getSubdocContainer() ) == count+1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container() ) == count+1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
     def test_create_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer() )
+        count = len( proxyA.get_subdoc_container() )
 
         # create a new entry in a level one proxy without saving the parent
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
 
         # verify a key was added to the proxy
-        assert proxyA.subdocKeyName in newProxy
+        assert proxyA.subdoc_key_name in newProxy
 
         # verify new key exists in the list
-        assert newProxy.key in getKeys( proxyA )
+        assert newProxy.key in get_keys( proxyA )
 
         # verify a new entry was created
-        assert len( proxyA.getSubdocContainer() ) == count+1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container() ) == count+1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
     def test_create_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer() )
-        countA1 = len( proxyA1.getSubdocContainer() )
+        countA = len( proxyA.get_subdoc_container() )
+        countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a new entry in a level two proxy
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
 
         # verify a key was added to the proxy
-        assert proxyA1.subdocKeyName in newProxy
+        assert proxyA1.subdoc_key_name in newProxy
 
         # verify new key exists in the list
-        assert newProxy.key in getKeys( proxyA1 )
+        assert newProxy.key in get_keys( proxyA1 )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.getSubdocContainer() ) == countA
-        assert len( proxyA1.getSubdocContainer() ) == countA1 + 1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container() ) == countA
+        assert len( proxyA1.get_subdoc_container() ) == countA1 + 1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
     def test_create_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer() )
-        countA1 = len( proxyA1.getSubdocContainer() )
+        countA = len( proxyA.get_subdoc_container() )
+        countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a new entry in a level two proxy without saving the parent
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=None )
 
         # verify a key was added to the proxy
-        assert proxyA1.subdocKeyName in newProxy
+        assert proxyA1.subdoc_key_name in newProxy
 
         # verify new key exists in the list
-        assert newProxy.key in getKeys( proxyA1 )
+        assert newProxy.key in get_keys( proxyA1 )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.getSubdocContainer() ) == countA
-        assert len( proxyA1.getSubdocContainer() ) == countA1 + 1
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 1
+        assert len( proxyA.get_subdoc_container() ) == countA
+        assert len( proxyA1.get_subdoc_container() ) == countA1 + 1
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
@@ -215,103 +215,103 @@
     def test_delete( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer() )
+        count = len( proxyA.get_subdoc_container() )
         key = proxyA.key
 
         # delete the level one proxy
         proxyA.delete()
 
         # verify the entry was deleted
-        assert key not in getKeys( proxyA )
+        assert key not in get_keys( proxyA )
         assert proxyA.key is None
-        assert len( proxyA.getSubdocContainer() ) == count-1
+        assert len( proxyA.get_subdoc_container() ) == count-1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestDelete_ProxyA_No_Save:
     def test_delete_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer() )
+        count = len( proxyA.get_subdoc_container() )
         key = proxyA.key
 
         # delete the level one proxy without saving the parent
         proxyA.delete( autosave=False )
 
         # verify the entry was deleted
-        assert key not in getKeys( proxyA )
+        assert key not in get_keys( proxyA )
         assert proxyA.key is None
-        assert len( proxyA.getSubdocContainer() ) == count-1
+        assert len( proxyA.get_subdoc_container() ) == count-1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
 class TestDelete_ProxyA1:
     def test_delete_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer() )
-        countA1 = len( proxyA1.getSubdocContainer() )
+        countA = len( proxyA.get_subdoc_container() )
+        countA1 = len( proxyA1.get_subdoc_container() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete()
 
         # verify the entry was deleted
-        assert key not in getKeys( proxyA1 )
+        assert key not in get_keys( proxyA1 )
         assert proxyA1.key is None
-        assert len( proxyA.getSubdocContainer() ) == countA
-        assert len( proxyA1.getSubdocContainer() ) == countA1 - 1
+        assert len( proxyA.get_subdoc_container() ) == countA
+        assert len( proxyA1.get_subdoc_container() ) == countA1 - 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 
 
 class TestDelete_ProxyA1_No_Save:
     def test_delete_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer() )
-        countA1 = len( proxyA1.getSubdocContainer() )
+        countA = len( proxyA.get_subdoc_container() )
+        countA1 = len( proxyA1.get_subdoc_container() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete( autosave=False )
 
         # verify the entry was deleted
-        assert key not in getKeys( proxyA )
+        assert key not in get_keys( proxyA )
         assert proxyA1.key is None
-        assert len( proxyA.getSubdocContainer() ) == countA
-        assert len( proxyA1.getSubdocContainer() ) == countA1 - 1
+        assert len( proxyA.get_subdoc_container() ) == countA
+        assert len( proxyA1.get_subdoc_container() ) == countA1 - 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
@@ -354,15 +354,15 @@
         # verify that the key no longer exists
         assert 'nameA1' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimateParent['_id'] } )
+        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA1' not in doc['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ]
 
 
 
 class TestSetDefault:
@@ -465,15 +465,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimateParent['_id'] } )
+        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ]
         assert doc['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ]['newKey'] == 'this is a new value'
 
 
 
@@ -529,33 +529,33 @@
         assert proxy['newKey2'] == 2
         assert len( proxy.keys() ) == count + 2
 
 
 
 
 class TestBasics:
-    def test_createKey( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_create_key( self, getPopulatedMMUDClasses, getSampleProxyA ):
         '''Test key creation for single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
         updated = parent['_updated']
 
         # create a proxyA key
-        keyA = classes['A'].createKey( parent )
+        keyA = classes['A'].create_key( parent )
         assert isinstance( keyA, str )
-        assert keyA == f"{parent['_lastUniqueInteger']:x}"
+        assert keyA == f"{parent['_last_unique_integer']:x}"
 
         # create a proxyA1 key
-        keyA1 = classes['A1'].createKey( proxyA )
+        keyA1 = classes['A1'].create_key( proxyA )
         assert isinstance( keyA1, str )
-        assert keyA1 == f"{parent['_lastUniqueInteger']:x}"
+        assert keyA1 == f"{parent['_last_unique_integer']:x}"
         assert keyA != keyA1
 
-        # verify that createKey doesn't save the parent object
+        # verify that create_key doesn't save the parent object
         doc = classes['base'].collection().find_one( { '_id' : parent['_id'] } )
         assert doc['_updated'] == updated
 
 
     def test_contains( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert 'nameA' in proxy
@@ -573,15 +573,15 @@
         # verify that the data references the same dictionary
         assert id( proxy.data() ) == id( proxy.parent['proxyA'][ proxy.seq ] )
 
 
     def test_data_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         # verify that the data references the same dictionary
-        assert id( proxy.data() ) == id( proxy.ultimateParent['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ] )
+        assert id( proxy.data() ) == id( proxy.ultimate_parent['proxyA'][ proxy.parent.seq ]['proxyA1'][ proxy.seq ] )
 
 
     def test_get( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert proxy.get('nameA') is not None
         assert proxy.get('will-not-match') is None
 
@@ -602,176 +602,176 @@
     def test_getitem_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         assert proxy['nameA1'] is not None
         with pytest.raises( Exception ):
             assert proxy['will-not-match']
 
 
-    def test_getKey( self, getMMUDClasses ):
+    def test_get_key( self, getMMUDClasses ):
         classes = getMMUDClasses
 
         sample = { '_sdkey' : 'proxy-key'}
 
-        assert classes['A'].getKey( sample ) == 'proxy-key'
+        assert classes['A'].get_key( sample ) == 'proxy-key'
 
 
-    def test_getKey_alt_name( self ):
+    def test_get_key_alt_name( self ):
         class MyAltListProxy( mongo_objects.MongoListProxy ):
-            subdocKeyName = 'alt-subdoc-key-name'
+            subdoc_key_name = 'alt-subdoc-key-name'
 
         sample = { 'alt-subdoc-key-name' : 'proxy-key'}
-        assert MyAltListProxy.getKey( sample ) == 'proxy-key'
+        assert MyAltListProxy.get_key( sample ) == 'proxy-key'
 
 
-    def test_getProxies( self, getPopulatedMMUDClasses, getSampleParent ):
+    def test_get_proxies( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test accessing both first-level and second-level proxy lists'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # get all first-level proxies
-        result = classes['A'].getProxies( parent )
+        result = classes['A'].get_proxies( parent )
 
         # verify type and length of the result
         assert isinstance( result, list )
-        assert len( result ) == len( parent[ classes['A'].containerName ] )
+        assert len( result ) == len( parent[ classes['A'].container_name ] )
 
         # verify type matches
         for proxy in result:
             assert isinstance( proxy, classes['A'])
 
         # choose a proxyA to continue testing with
-        proxyA = classes['A'].getProxy( parent, seq=0 )
+        proxyA = classes['A'].get_proxy( parent, seq=0 )
 
         # get all second-level proxies
-        result = classes['A1'].getProxies( proxyA )
+        result = classes['A1'].get_proxies( proxyA )
 
         # verify type and length of the result
         assert isinstance( result, list )
-        assert len( result ) == len( parent[ classes['A'].containerName ][ proxyA.seq ][ classes['A1'].containerName ] )
+        assert len( result ) == len( parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ] )
 
         # verify type matches
         for proxy in result:
             assert isinstance( proxy, classes['A1'])
 
 
-    def test_getProxies_empty( self, getPopulatedMMUDClasses ):
+    def test_get_proxies_empty( self, getPopulatedMMUDClasses ):
         '''Test get proxies from an empty object'''
         classes = getPopulatedMMUDClasses
 
         # collect proxies from an empty object
-        result = classes['A'].getProxies( {} )
+        result = classes['A'].get_proxies( {} )
         assert len(result) == 0
 
 
-    def test_getProxy( self, getPopulatedMMUDClasses, getSampleParent ):
+    def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test accessing both first-level and second-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # locate the key for the first entry in the proxy A container
-        keyA = parent[ classes['A'].containerName ][0][ classes['A'].subdocKeyName ]
+        keyA = parent[ classes['A'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create a first-level proxy object
-        proxyA = classes['A'].getProxy( parent, keyA )
+        proxyA = classes['A'].get_proxy( parent, keyA )
 
         # verify dictionary and type matches
-        assert id( proxyA.data() ) == id( parent[ classes['A'].containerName ][0] )
+        assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ][0] )
         assert isinstance( proxyA, classes['A'] )
 
         # locate the key for the first entry in the proxy A1 container
-        keyA1 = parent[ classes['A'].containerName ][0][ classes['A1'].containerName ][0][ classes['A'].subdocKeyName ]
+        keyA1 = parent[ classes['A'].container_name ][0][ classes['A1'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create a second-level proxy object
-        proxyA1 = classes['A1'].getProxy( proxyA, keyA1 )
+        proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
 
         # verify dictionary and type matches
-        assert id( proxyA1.data() ) == id( parent[ classes['A'].containerName ][0][ classes['A1'].containerName ][0] )
+        assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][0][ classes['A1'].container_name ][0] )
         assert isinstance( proxyA1, classes['A1'] )
 
 
-    def test_getProxy_by_sequence( self, getPopulatedMMUDClasses, getSampleParent ):
+    def test_get_proxy_by_sequence( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test accessing both first-level and second-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # create a first-level proxy object
-        proxyA = classes['A'].getProxy( parent, seq=0 )
+        proxyA = classes['A'].get_proxy( parent, seq=0 )
 
         # verify dictionary and type matches
-        assert id( proxyA.data() ) == id( parent[ classes['A'].containerName ][0] )
+        assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ][0] )
         assert isinstance( proxyA, classes['A'] )
 
         # create a second-level proxy object
-        proxyA1 = classes['A1'].getProxy( proxyA, seq=0 )
+        proxyA1 = classes['A1'].get_proxy( proxyA, seq=0 )
 
         # verify dictionary and type matches
-        assert id( proxyA1.data() ) == id( parent[ classes['A'].containerName ][0][ classes['A1'].containerName ][0] )
+        assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][0][ classes['A1'].container_name ][0] )
         assert isinstance( proxyA1, classes['A1'] )
 
 
-    def test_getSubdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_get_subdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
-        assert id( proxyA.getSubdoc() ) == id( proxyA.parent[ classes['A'].containerName ][ proxyA.seq ] )
+        assert id( proxyA.get_subdoc() ) == id( proxyA.parent[ classes['A'].container_name ][ proxyA.seq ] )
 
 
-    def test_getSubdoc_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_get_subdoc_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # verify data location
-        assert id( proxyA1.getSubdoc() ) == id( proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA1.parent.seq ][ classes['A1'].containerName ][ proxyA1.seq ] )
+        assert id( proxyA1.get_subdoc() ) == id( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA1.parent.seq ][ classes['A1'].container_name ][ proxyA1.seq ] )
 
 
-    def test_getSubdocContainer( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_get_subdoc_container( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
-        assert id( proxyA.getSubdocContainer() ) == id( proxyA.parent[ classes['A'].containerName ] )
+        assert id( proxyA.get_subdoc_container() ) == id( proxyA.parent[ classes['A'].container_name ] )
 
 
-    def test_getSubdocContainer_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_get_subdoc_container_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # verify data location
-        assert id( proxyA1.getSubdocContainer() ) == id( proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA1.parent.seq ][ classes['A1'].containerName ] )
+        assert id( proxyA1.get_subdoc_container() ) == id( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA1.parent.seq ][ classes['A1'].container_name ] )
 
 
     def test_id( self, getSampleProxyA ):
         '''Test ID for single level proxy'''
         proxy = getSampleProxyA
-        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdocKeySep}{proxy.key}"
+        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
         '''Test ID for two-level proxy'''
         proxy = getSampleProxyA1
-        assert proxy.id() == f"{proxy.ultimateParent.id()}{proxy.ultimateParent.subdocKeySep}{proxy.parent.key}{proxy.ultimateParent.subdocKeySep}{proxy.key}"
+        assert proxy.id() == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}{proxy.parent.key}{proxy.ultimate_parent.subdoc_key_sep}{proxy.key}"
 
 
     def test_init( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test initialization of single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # pick the first proxyA key
-        keyA = parent[ classes['A'].containerName ][0][ classes['A'].subdocKeyName ]
+        keyA = parent[ classes['A'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create the proxy
         proxyA = classes['A']( parent, keyA )
 
         # verify that the data references the same dictionary
         assert id( proxyA.data() ) == id( parent['proxyA'][0] )
 
         # pick the first proxyA1 key
-        keyA1 = parent[ classes['A'].containerName ][0][ classes['A1'].containerName ][0][ classes['A1'].subdocKeyName ]
+        keyA1 = parent[ classes['A'].container_name ][0][ classes['A1'].container_name ][0][ classes['A1'].subdoc_key_name ]
 
         # create the proxy
         proxyA1 = classes['A1']( proxyA, keyA1 )
 
         # verify that the data references the same dictionary
         assert id( proxyA1.data() ) == id( parent['proxyA'][0]['proxyA1'][0] )
 
@@ -801,24 +801,24 @@
     def test_init_bad_seq( self, getPopulatedMMUDClasses, getSampleParent ):
         '''Test initialization of single and two-level proxies with a bad sequence.
         Invalid sequence values are automatically corrected.'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # pick the first proxyA key
-        keyA = parent[ classes['A'].containerName ][0][ classes['A'].subdocKeyName ]
+        keyA = parent[ classes['A'].container_name ][0][ classes['A'].subdoc_key_name ]
 
         # create the proxy with a bad sequence
         proxyA = classes['A']( parent, keyA, seq=1.0 )
 
         # verify that the data references the same dictionary
         assert id( proxyA.data() ) == id( parent['proxyA'][0] )
 
         # pick the first proxyA1 key
-        keyA1 = parent[ classes['A'].containerName ][0][ classes['A1'].containerName ][0][ classes['A1'].subdocKeyName ]
+        keyA1 = parent[ classes['A'].container_name ][0][ classes['A1'].container_name ][0][ classes['A1'].subdoc_key_name ]
 
         # create the proxy
         proxyA1 = classes['A1']( proxyA, keyA1, seq=1.0 )
 
         # verify that the data references the same dictionary
         assert id( proxyA1.data() ) == id( parent['proxyA'][0]['proxyA1'][0] )
 
@@ -853,23 +853,23 @@
         assert set( [ key for key in proxy ] ) == set( proxy.parent['proxyA1'][ proxy.seq ].keys() )
 
 
     def test_keys( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
-        assert proxy.keys() == proxy.parent[ classes['A'].containerName ][ proxy.seq].keys()
+        assert proxy.keys() == proxy.parent[ classes['A'].container_name ][ proxy.seq].keys()
 
 
     def test_keys_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
-        assert proxyA1.keys() == proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA.seq ][ classes['A1'].containerName ][ proxyA1.seq ].keys()
+        assert proxyA1.keys() == proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ][ proxyA1.seq ].keys()
 
 
     def test_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # preserve original state
@@ -883,56 +883,56 @@
 
 
     def test_save_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # preserve original state
-        original = dict( proxyA1.ultimateParent )
+        original = dict( proxyA1.ultimate_parent )
 
         # save the object
         proxyA1.save()
 
         # verify the parent document was saved
-        assert proxyA1.ultimateParent['_updated'] > original['_updated']
+        assert proxyA1.ultimate_parent['_updated'] > original['_updated']
 
 
-    def test_setKey( self, getMMUDClasses ):
+    def test_set_key( self, getMMUDClasses ):
         classes = getMMUDClasses
 
         sample = {}
-        classes['A'].setKey( sample, 'proxy-key' )
+        classes['A'].set_key( sample, 'proxy-key' )
 
         assert sample['_sdkey'] == 'proxy-key'
 
 
-    def test_setKey_alt_name( self ):
+    def test_set_key_alt_name( self ):
         class MyAltListProxy( mongo_objects.MongoListProxy ):
-            subdocKeyName = 'alt-subdoc-key-name'
+            subdoc_key_name = 'alt-subdoc-key-name'
 
         sample = {}
-        MyAltListProxy.setKey( sample, 'proxy-key' )
+        MyAltListProxy.set_key( sample, 'proxy-key' )
 
         print( repr( sample ) )
         assert sample['alt-subdoc-key-name'] == 'proxy-key'
 
 
     def test_values( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
         # compare contents of values() as lists (dict_values objects don't compare properly)
-        assert list( proxy.values() ) == list( proxy.parent[ classes['A'].containerName ][ proxy.seq ].values() )
+        assert list( proxy.values() ) == list( proxy.parent[ classes['A'].container_name ][ proxy.seq ].values() )
 
 
     def test_values_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
         # compare contents of values() as lists (dict_values objects don't compare properly)
-        assert list( proxyA1.values() ) == list( proxyA1.ultimateParent[ classes['A'].containerName ][ proxyA.seq ][ classes['A1'].containerName ][ proxyA1.seq ].values() )
+        assert list( proxyA1.values() ) == list( proxyA1.ultimate_parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ][ proxyA1.seq ].values() )
```

### Comparing `mongo_objects-1.0.22/tests/test_MongoSingleProxy.py` & `mongo_objects-1.0.26/tests/test_MongoSingleProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 @pytest.fixture( scope='class' )
 def getMMUDClasses( mongo_db ):
     '''Return a MongoUserDict configured for a per-class unique collection
 
     Since the single proxy classes are used multiple times,
-    we don't provide a containerName. Otherwise, each instance
+    we don't provide a container_name. Otherwise, each instance
     would use the same location by default.'''
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyMongoSingleProxyA( mongo_objects.MongoSingleProxy ):
@@ -99,145 +99,145 @@
     '''Return a fixed sample key for first-level A proxy testing'''
     return 'proxyA-0'
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey ):
     classes = getPopulatedMMUDClasses
-    return classes['A'].getProxy( getSampleParent, getSampleProxyAKey )
+    return classes['A'].get_proxy( getSampleParent, getSampleProxyAKey )
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA1Key():
     '''Return a fixed sample key for second-level A1 proxy testing'''
     return 'proxyA1-0'
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA1( getPopulatedMMUDClasses, getSampleProxyA, getSampleProxyA1Key ):
     classes = getPopulatedMMUDClasses
-    return classes['A1'].getProxy( getSampleProxyA, getSampleProxyA1Key )
+    return classes['A1'].get_proxy( getSampleProxyA, getSampleProxyA1Key )
 
 
 
 
 class TestCreate:
     def test_create( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
 
         # create a new entry in a level one proxy
         newProxy = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry'},
             key='newProxyA'
         )
 
         # verify a new entry was created
-        assert len( proxyA.getSubdocContainer().keys() ) == count+1
+        assert len( proxyA.get_subdoc_container().keys() ) == count+1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestCreateNoSave:
     def test_create_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
 
         # create a new entry in a level one proxy without saving the parent
         newProxy = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry'},
             key='newProxyA',
             autosave=False
         )
 
         # verify a new entry was created
-        assert len( proxyA.getSubdocContainer().keys() ) == count+1
+        assert len( proxyA.get_subdoc_container().keys() ) == count+1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 class TestCreateA1:
     def test_create_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a new entry in a level two proxy
         newProxy = classes['A1'].create(
             proxyA,
             { 'name' : 'new proxyA1 entry'},
             key='newProxyA1'
         )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 + 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 + 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestCreateA1NoSave:
     def test_create_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a new entry in a level two proxy without saving the parent
         newProxy = classes['A1'].create(
             proxyA,
             { 'name' : 'new proxyA1 entry'},
             key='newProxyA1',
             autosave=None
         )
 
         # verify a new entry was created at the second (proxyA1) level
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 + 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 + 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
-class TestCreateContainerName:
+class TestCreatecontainer_name:
     def test_create_by_container( self, getMMUDClasses ):
         classes = getMMUDClasses
         parent = {}
 
         # adjust class to have a container name
-        classes['A'].containerName = 'proxyAByContainer'
-        classes['A1'].containerName = 'proxyA1ByContainer'
+        classes['A'].container_name = 'proxyAByContainer'
+        classes['A1'].container_name = 'proxyA1ByContainer'
 
         # create a new entry in a first level proxy
         newProxyA = classes['A'].create(
             parent,
             { 'name' : 'new proxyA entry by container'},
             autosave=False
         )
@@ -264,103 +264,103 @@
     def test_delete( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy
         proxyA.delete()
 
         # verify the entry was deleted
-        assert key not in proxyA.getSubdocContainer().keys()
+        assert key not in proxyA.get_subdoc_container().keys()
         assert proxyA.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == count-1
+        assert len( proxyA.get_subdoc_container().keys() ) == count-1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 class TestDelete_ProxyA_No_Save:
     def test_delete_no_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container().keys() )
         key = proxyA.key
 
         # delete the level one proxy without saving the parent
         proxyA.delete( autosave=False )
 
         # verify the entry was deleted
-        assert key not in proxyA.getSubdocContainer().keys()
+        assert key not in proxyA.get_subdoc_container().keys()
         assert proxyA.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == count-1
+        assert len( proxyA.get_subdoc_container().keys() ) == count-1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
 class TestDelete_ProxyA1:
     def test_delete_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete()
 
         # verify the entry was deleted
-        assert key not in proxyA1.getSubdocContainer().keys()
+        assert key not in proxyA1.get_subdoc_container().keys()
         assert proxyA1.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 - 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 - 1
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
 
 
 class TestDelete_ProxyA1_No_Save:
     def test_delete_A1_no_save( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
         key = proxyA1.key
 
         # delete the level one proxy
         proxyA1.delete( autosave=False )
 
         # verify the entry was deleted
-        assert key not in proxyA1.getSubdocContainer().keys()
+        assert key not in proxyA1.get_subdoc_container().keys()
         assert proxyA1.key is None
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1 - 1
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1 - 1
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 
@@ -403,15 +403,15 @@
         # verify that the key no longer exists
         assert 'nameA1' not in proxy
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimateParent['_id'] } )
+        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the key no longer exists in the database as well
         assert 'nameA1' not in doc[ proxy.parent.key ][ proxy.key ]
 
 
 
 class TestSetDefault:
@@ -514,15 +514,15 @@
         assert 'newKey' in proxy
         assert proxy['newKey'] == 'this is a new value'
 
         # save the data
         proxy.save()
 
         # locate the object on disk
-        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimateParent['_id'] } )
+        doc = classes['base'].collection().find_one( { '_id' : proxy.ultimate_parent['_id'] } )
 
         # verify that the new key exists in the database as well
         assert 'newKey' in doc[ proxy.parent.key ][ proxy.key ]
         assert doc[ proxy.parent.key ][ proxy.key ]['newKey'] == 'this is a new value'
 
 
 
@@ -578,33 +578,33 @@
         assert proxy['newKey2'] == 2
         assert len( proxy.keys() ) == count + 2
 
 
 
 
 class TestBasics:
-    def test_createKey( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_create_key( self, getPopulatedMMUDClasses, getSampleProxyA ):
         '''Test key creation for single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
         updated = parent['_updated']
 
         # create a proxyA key
-        keyA = classes['A'].createKey( parent )
+        keyA = classes['A'].create_key( parent )
         assert isinstance( keyA, str )
-        assert keyA == f"{parent['_lastUniqueInteger']:x}"
+        assert keyA == f"{parent['_last_unique_integer']:x}"
 
         # create a proxyA1 key
-        keyA1 = classes['A1'].createKey( proxyA )
+        keyA1 = classes['A1'].create_key( proxyA )
         assert isinstance( keyA1, str )
-        assert keyA1 == f"{parent['_lastUniqueInteger']:x}"
+        assert keyA1 == f"{parent['_last_unique_integer']:x}"
         assert keyA != keyA1
 
-        # verify that createKey doesn't save the parent object
+        # verify that create_key doesn't save the parent object
         doc = classes['base'].collection().find_one( { '_id' : parent['_id'] } )
         assert doc['_updated'] == updated
 
 
     def test_contains( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert 'nameA' in proxy
@@ -622,15 +622,15 @@
         # verify that the data references the same dictionary
         assert id( proxy.data() ) == id( proxy.parent[proxy.key] )
 
 
     def test_data_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         # verify that the data references the same dictionary
-        assert id( proxy.data() ) == id( proxy.ultimateParent[proxy.parent.key][proxy.key] )
+        assert id( proxy.data() ) == id( proxy.ultimate_parent[proxy.parent.key][proxy.key] )
 
 
     def test_get( self, getSampleProxyA ):
         proxy = getSampleProxyA
         assert proxy.get('nameA') is not None
         assert proxy.get('will-not-match') is None
 
@@ -651,91 +651,91 @@
     def test_getitem_A1( self, getSampleProxyA1 ):
         proxy = getSampleProxyA1
         assert proxy['nameA1'] is not None
         with pytest.raises( Exception ):
             assert proxy['will-not-match']
 
 
-    def test_getProxies( self, getPopulatedMMUDClasses, getSampleParent ):
-        '''single proxy objects don't support getProxies()'''
+    def test_get_proxies( self, getPopulatedMMUDClasses, getSampleParent ):
+        '''single proxy objects don't support get_proxies()'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         with pytest.raises( Exception ):
-            classes['A'].getProxies( parent )
+            classes['A'].get_proxies( parent )
 
 
-    def test_getProxy( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey ):
+    def test_get_proxy( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey ):
         '''Test accessing both first-level and second-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
 
         # locate the first key in the proxy A container
         keyA = getSampleProxyAKey
 
         # create a first-level proxy object
-        proxyA = classes['A'].getProxy( parent, keyA )
+        proxyA = classes['A'].get_proxy( parent, keyA )
 
         # verify dictionary and type matches
         assert id( proxyA.data() ) == id( parent[ keyA ] )
         assert isinstance( proxyA, classes['A'])
 
         # locate the first key in the proxy A1 container
         keyA1 = list( parent[ keyA ].keys() )[0]
 
         # create a second-level proxy object
-        proxyA1 = classes['A1'].getProxy( proxyA, keyA1 )
+        proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
 
         # verify dictionary and type matches
         assert id( proxyA1.data() ) == id( parent[ keyA ][ keyA1 ] )
         assert isinstance( proxyA1, classes['A1'])
 
 
-    def test_getSubdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_get_subdoc( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
-        assert id( proxyA.getSubdoc() ) == id( proxyA.parent[ proxyA.key ] )
+        assert id( proxyA.get_subdoc() ) == id( proxyA.parent[ proxyA.key ] )
 
 
-    def test_getSubdoc_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_get_subdoc_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # verify data location
-        assert id( proxyA1.getSubdoc() ) == id( proxyA1.ultimateParent[ proxyA1.parent.key ][ proxyA1.key ] )
+        assert id( proxyA1.get_subdoc() ) == id( proxyA1.ultimate_parent[ proxyA1.parent.key ][ proxyA1.key ] )
 
 
-    def test_getSubdocContainer( self, getPopulatedMMUDClasses, getSampleProxyA ):
+    def test_get_subdoc_container( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # verify data location
-        assert id( proxyA.getSubdocContainer() ) == id( proxyA.parent )
+        assert id( proxyA.get_subdoc_container() ) == id( proxyA.parent )
 
 
-    def test_getSubdocContainer_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
+    def test_get_subdoc_container_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # verify data location
-        assert id( proxyA1.getSubdocContainer() ) == id( proxyA1.parent )
+        assert id( proxyA1.get_subdoc_container() ) == id( proxyA1.parent )
 
 
     def test_id( self, getSampleProxyA ):
         '''Test ID for single level proxy'''
         proxy = getSampleProxyA
-        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdocKeySep}0"
+        assert proxy.id() == f"{proxy.parent.id()}{proxy.parent.subdoc_key_sep}0"
 
 
     def test_id_A1( self, getSampleProxyA1 ):
         '''Test ID for two-level proxy'''
         proxy = getSampleProxyA1
-        assert proxy.id() == f"{proxy.ultimateParent.id()}{proxy.ultimateParent.subdocKeySep}0{proxy.ultimateParent.subdocKeySep}0"
+        assert proxy.id() == f"{proxy.ultimate_parent.id()}{proxy.ultimate_parent.subdoc_key_sep}0{proxy.ultimate_parent.subdoc_key_sep}0"
 
 
     def test_init( self, getPopulatedMMUDClasses, getSampleParent, getSampleProxyAKey, getSampleProxyA1Key ):
         '''Test initialization of single and two-level proxies'''
         classes = getPopulatedMMUDClasses
         parent = getSampleParent
         keyA = getSampleProxyAKey
@@ -780,15 +780,15 @@
 
 
     def test_items_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
-        assert proxyA1.items() == proxyA1.ultimateParent[ proxyA.key ][ proxyA1.key ].items()
+        assert proxyA1.items() == proxyA1.ultimate_parent[ proxyA.key ][ proxyA1.key ].items()
 
 
     def test_iter( self, getSampleProxyA ):
         proxy = getSampleProxyA
         # compare the keys
         assert set( [ key for key in proxy ] ) == set( proxy.parent[ proxy.key ].keys() )
 
@@ -807,15 +807,15 @@
 
 
     def test_keys_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
-        assert proxyA1.keys() == proxyA1.ultimateParent[ proxyA.key ][ proxyA1.key ].keys()
+        assert proxyA1.keys() == proxyA1.ultimate_parent[ proxyA.key ][ proxyA1.key ].keys()
 
 
     def test_save( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxyA = getSampleProxyA
 
         # preserve original state
@@ -829,21 +829,21 @@
 
 
     def test_save_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
 
         # preserve original state
-        original = dict( proxyA1.ultimateParent )
+        original = dict( proxyA1.ultimate_parent )
 
         # save the object
         proxyA1.save()
 
         # verify the parent document was saved
-        assert proxyA1.ultimateParent['_updated'] > original['_updated']
+        assert proxyA1.ultimate_parent['_updated'] > original['_updated']
 
 
     def test_values( self, getPopulatedMMUDClasses, getSampleProxyA ):
         classes = getPopulatedMMUDClasses
         proxy = getSampleProxyA
 
         # compare contents of values() as lists (dict_values objects don't compare properly)
@@ -852,10 +852,10 @@
 
     def test_values_A1( self, getPopulatedMMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
 
         # compare contents of values() as lists (dict_values objects don't compare properly)
-        assert list( proxyA1.values() ) == list( proxyA1.ultimateParent[ proxyA.key ][ proxyA1.key ].values() )
+        assert list( proxyA1.values() ) == list( proxyA1.ultimate_parent[ proxyA.key ][ proxyA1.key ].values() )
```

### Comparing `mongo_objects-1.0.22/tests/test_MongoUserDict.py` & `mongo_objects-1.0.26/tests/test_MongoUserDict.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,23 +195,23 @@
         # any object with an _id is assumed to have been saved already
         # and to have a valid _updated timestamp
         obj = MMUD( sampleData[1] )
         obj['_id'] = ObjectId()
 
         # saving it should raise an exception as no existing object can be found
         # in this case _updated starts as None but it could be anything
-        originalUpdated = obj.get('_updated')
+        original_updated = obj.get('_updated')
         with pytest.raises( Exception ):
             obj.save()
 
         # verify that nothing was saved
         assert MMUD.collection().count_documents( {} ) == count
 
         # verify that _updated wasn't changed
-        assert obj.get('_updated') == originalUpdated
+        assert obj.get('_updated') == original_updated
 
         # force saving will work
         obj.save( force=True )
 
         # verify that something was saved
         assert MMUD.collection().count_documents( {} ) == count+1
 
@@ -236,32 +236,32 @@
         startTime = MMUD.utcnow()
 
         # save the third record
         obj = MMUD( sampleData[2] )
         obj.save()
 
         # reload the data into a new object
-        obj2 = MMUD.loadById( obj.id() )
+        obj2 = MMUD.load_by_id( obj.id() )
 
         # verify the timestamps are the same
         assert obj['_updated'] == obj2['_updated']
 
         # save the first object again
         obj.save()
 
         # verify a newer timestamp
         assert obj['_updated'] > obj2['_updated']
 
         # try to save second object; it won't work
-        originalUpdated = obj2.get('_updated')
+        original_updated = obj2.get('_updated')
         with pytest.raises( Exception ):
             obj2.save()
 
         # verify that obj2 _updated is the original value
-        assert obj2.get('_updated') == originalUpdated
+        assert obj2.get('_updated') == original_updated
 
         # locate object on disk and verify _updated matches obj (not obj2)
         doc = MMUD.collection().find_one( { '_id' : obj['_id'] } )
         assert doc['_updated'] == obj['_updated']
 
 
     def test_save_readonly( self, getPopulatedMMUDClass ):
@@ -581,21 +581,21 @@
         result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' } )
 
         # verify that we found nothing
         assert result is None
 
 
     def test_find_one_none_custom_return( self, getPopulatedMMUDClass ):
-        '''Verify a non-matching filter produces our custom "noMatch" result'''
+        '''Verify a non-matching filter produces our custom "no_match" result'''
         MMUD = getPopulatedMMUDClass
 
         class EmptyResponse( object ):
             pass
 
-        result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' }, noMatch=EmptyResponse() )
+        result = MMUD.find_one( { 'not-a-field' : 'wont-match-anything' }, no_match=EmptyResponse() )
 
         assert isinstance( result, EmptyResponse )
 
 
     def test_find_one_filter( self, getPopulatedMMUDClass, sampleData ):
         '''Use a filter to find a specific single record, in this case, the third sample by name'''
         MMUD = getPopulatedMMUDClass
@@ -688,109 +688,122 @@
                 return False
 
         # verify reading documents without read authorization produces an empty list
         result = LocalMMUD.find_one()
         assert result is None
 
 
-    def test_getUniqueInteger( self, getMMUDClass ):
+    def test_get_unique_integer( self, getMMUDClass ):
         MMUD = getMMUDClass
         obj = MMUD()
         startTime = MMUD.utcnow()
 
-        # verify new object doesn't have a _lastUniqueInteger
+        # verify new object doesn't have a _last_unique_integer
         # an _id, a created or an update time
         assert '_id' not in obj
         assert '_created' not in obj
         assert '_updated' not in obj
-        assert '_lastUniqueInteger' not in obj
+        assert '_last_unique_integer' not in obj
 
         # obtain the next unique integer
-        x = obj.getUniqueInteger()
+        x = obj.get_unique_integer()
         assert x == 1
-        assert x == obj['_lastUniqueInteger']
+        assert x == obj['_last_unique_integer']
 
         # object should have been saved
         assert '_id' in obj
         assert obj['_created'] >= startTime
         assert obj['_updated'] == obj['_created']
 
         # get 10 more integers
         for i in range(10):
-            x = obj.getUniqueInteger()
+            x = obj.get_unique_integer()
         assert x == 11
-        assert x == obj['_lastUniqueInteger']
+        assert x == obj['_last_unique_integer']
 
 
-    def test_getUniqueInteger_no_save( self, getMMUDClass ):
+    def test_get_unique_integer_no_save( self, getMMUDClass ):
         MMUD = getMMUDClass
         obj = MMUD()
 
-        # verify new object doesn't have a _lastUniqueInteger
+        # verify new object doesn't have a _last_unique_integer
         # an _id, a created or an update time
         assert '_id' not in obj
         assert '_created' not in obj
         assert '_updated' not in obj
-        assert '_lastUniqueInteger' not in obj
+        assert '_last_unique_integer' not in obj
 
         # obtain the next unique integer
-        x = obj.getUniqueInteger( autosave=False )
+        x = obj.get_unique_integer( autosave=False )
         assert x == 1
-        assert x == obj['_lastUniqueInteger']
+        assert x == obj['_last_unique_integer']
 
         # object should not have been saved
         assert '_id' not in obj
         assert '_created' not in obj
         assert '_updated' not in obj
 
 
-    def test_getUniqueKey( self, getMMUDClass ):
+    def test_get_unique_integer_migration( self, getMMUDClass ):
+        MMUD = getMMUDClass
+        obj = MMUD( { '_lastUniqueInteger' : 10 } )
+
+        # obtain the next unique integer
+        x = obj.get_unique_integer( autosave=False )
+        assert x == 11
+        assert x == obj['_last_unique_integer']
+
+        # verify that _lastUniqueInteger has been removed
+        assert '_lastUniqueInteger' not in obj
+
+
+    def test_get_unique_key( self, getMMUDClass ):
         MMUD = getMMUDClass
         obj = MMUD()
         startTime = MMUD.utcnow()
 
-        # verify new object doesn't have a _lastUniqueInteger
+        # verify new object doesn't have a _last_unique_integer
         # an _id, or an update time
         assert '_id' not in obj
         assert '_created' not in obj
         assert '_updated' not in obj
-        assert '_lastUniqueInteger' not in obj
+        assert '_last_unique_integer' not in obj
 
         # obtain the next unique key
-        x = obj.getUniqueKey()
+        x = obj.get_unique_key()
         assert x == '1'
-        assert x == str( obj['_lastUniqueInteger'] )
+        assert x == str( obj['_last_unique_integer'] )
 
         # object should have been saved
         assert '_id' in obj
         assert obj['_created'] >= startTime
         assert obj['_updated'] == obj['_created']
 
         # get 10 more keys
         for i in range(10):
-            x = obj.getUniqueKey()
+            x = obj.get_unique_key()
         assert x == 'b'   # 11 in hex
-        assert x == f"{obj['_lastUniqueInteger']:x}"
+        assert x == f"{obj['_last_unique_integer']:x}"
 
 
-    def test_getUniqueInteger_no_save( self, getMMUDClass ):
+    def test_get_unique_integer_no_save( self, getMMUDClass ):
         MMUD = getMMUDClass
         obj = MMUD()
 
-        # verify new object doesn't have a _lastUniqueInteger
+        # verify new object doesn't have a _last_unique_integer
         # an _id, or an update time
         assert '_id' not in obj
         assert '_created' not in obj
         assert '_updated' not in obj
-        assert '_lastUniqueInteger' not in obj
+        assert '_last_unique_integer' not in obj
 
         # obtain the next unique key
-        x = obj.getUniqueKey( autosave=False )
+        x = obj.get_unique_key( autosave=False )
         assert x == '1'
-        assert x == str(obj['_lastUniqueInteger'])
+        assert x == str(obj['_last_unique_integer'])
 
         # object should not have been saved
         assert '_id' not in obj
         assert '_created' not in obj
         assert '_updated' not in obj
 
 
@@ -808,106 +821,106 @@
         # new object don't have an _id value yet
         # so id() will raise an exception
         obj = MMUD( {} )
         with pytest.raises( Exception ):
             obj.id()
 
 
-    def test_loadById_bson( self, getPopulatedMMUDClass ):
+    def test_load_by_id_bson( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
 
         # load a random object
         source = MMUD.find_one()
 
         # locate it again by the MongoDB BSON id
-        result = MMUD.loadById( source['_id'] )
+        result = MMUD.load_by_id( source['_id'] )
 
         # verify the objects are the same
         assert source == result
 
         # since no flag was used, verify the object is not readonly
         assert source.readonly is False
 
 
-    def test_loadById_str( self, getPopulatedMMUDClass ):
+    def test_load_by_id_str( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
 
         # load a random object
         source = MMUD.find_one()
 
         # locate it again by the string id
-        result = MMUD.loadById( source.id() )
+        result = MMUD.load_by_id( source.id() )
 
         # verify the objects are the same
         assert source == result
 
         # since no flag was used, verify the object is not readonly
         assert result.readonly is False
 
 
-    def test_loadById_readonly( self, getPopulatedMMUDClass ):
+    def test_load_by_id_readonly( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
 
         # load a random object
         source = MMUD.find_one()
 
         # locate it again by the string id
-        result = MMUD.loadById( source.id(), readonly=True )
+        result = MMUD.load_by_id( source.id(), readonly=True )
 
         # verify the objects are the same
         assert source == result
 
         # verify the object is readonly
         assert result.readonly is True
 
 
-    def test_loadProxyById( self, getPopulatedMMUDClass ):
+    def test_load_proxy_by_id( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
 
         # load a random object
         source = MMUD.find_one()
 
         # load the same object with an empty proxy tree
-        result = MMUD.loadProxyById( source.id() )
+        result = MMUD.load_proxy_by_id( source.id() )
 
         # verify the objects are the same
         assert source == result
 
         # verify the object is readonly
         assert result.readonly is False
 
 
-    def test_loadProxyById_readonly( self, getPopulatedMMUDClass ):
+    def test_load_proxy_by_id_readonly( self, getPopulatedMMUDClass ):
         MMUD = getPopulatedMMUDClass
 
         # load a random object
         source = MMUD.find_one()
 
         # load the same object with an empty proxy tree
-        result = MMUD.loadProxyById( source.id(), readonly=True )
+        result = MMUD.load_proxy_by_id( source.id(), readonly=True )
 
         # verify the objects are the same
         assert source == result
 
         # verify the object is readonly
         assert result.readonly is True
 
 
-    def test_splitId( self, getMMUDClass ):
+    def test_split_id( self, getMMUDClass ):
         MMUD = getMMUDClass
 
         # verify that the subdocument key separator exists
-        assert hasattr( MMUD, 'subdocKeySep' )
+        assert hasattr( MMUD, 'subdoc_key_sep' )
 
         # construct a mock subdocument ID
         a = [ '123456', '78', '90']
-        id = MMUD.subdocKeySep.join( a )
+        id = MMUD.subdoc_key_sep.join( a )
 
         # split the ID back into components
-        assert MMUD.splitId( id ) == a
+        assert MMUD.split_id( id ) == a
 
 
     def test_utcnow( self, getMMUDClass ):
         MMUD = getMMUDClass
         startTime = datetime.utcnow()
         mongoNow = MMUD.utcnow()
         endTime = datetime.utcnow()
```

### Comparing `mongo_objects-1.0.22/tests/test_PolymorphicMongoDictProxy.py` & `mongo_objects-1.0.26/tests/test_PolymorphicMongoListProxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# test_PolymorphicMongoDictProxy
+# test_PolymorphicMongoListProxy
 #
-# Since MongoDictProxy has been thoroughly exercised elsewhere,
-# only test functionality unique to PolymorphicMongoDictProxy
+# Since MongoListProxy has been thoroughly exercised elsewhere,
+# only test functionality unique to PolymorphicMongoListProxy
 
 from bson import ObjectId
 from datetime import datetime
 import mongo_objects
 from pymongo.collection import Collection
 import pytest
 import secrets
@@ -16,68 +16,68 @@
 def getMPMUDClasses( mongo_db ):
     '''Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection'''
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
-    class MyMongoDictProxyA( mongo_objects.PolymorphicMongoDictProxy ):
-        containerName = 'proxyA'
-        proxySubclassMap = {}
+    class MyMongoListProxyA( mongo_objects.PolymorphicMongoListProxy ):
+        container_name = 'proxyA'
+        proxy_subclass_map = {}
 
-    class MyMongoDictProxyAa( MyMongoDictProxyA ):
-        proxySubclassKey = 'Aa'
+    class MyMongoListProxyAa( MyMongoListProxyA ):
+        proxy_subclass_key = 'Aa'
 
-    class MyMongoDictProxyAb( MyMongoDictProxyA ):
-        proxySubclassKey = 'Ab'
+    class MyMongoListProxyAb( MyMongoListProxyA ):
+        proxy_subclass_key = 'Ab'
 
-    class MyMongoDictProxyAc( MyMongoDictProxyA ):
-        proxySubclassKey = 'Ac'
+    class MyMongoListProxyAc( MyMongoListProxyA ):
+        proxy_subclass_key = 'Ac'
 
-    class MyMongoDictProxyA1( mongo_objects.PolymorphicMongoDictProxy ):
-        containerName = 'proxyA1'
-        proxySubclassMap = {}
+    class MyMongoListProxyA1( mongo_objects.PolymorphicMongoListProxy ):
+        container_name = 'proxyA1'
+        proxy_subclass_map = {}
 
-    class MyMongoDictProxyA1a( MyMongoDictProxyA1 ):
-        proxySubclassKey = 'A1a'
+    class MyMongoListProxyA1a( MyMongoListProxyA1 ):
+        proxy_subclass_key = 'A1a'
 
-    class MyMongoDictProxyA1b( MyMongoDictProxyA1 ):
-        proxySubclassKey = 'A1b'
+    class MyMongoListProxyA1b( MyMongoListProxyA1 ):
+        proxy_subclass_key = 'A1b'
 
-    class MyMongoDictProxyA1c( MyMongoDictProxyA1 ):
-        proxySubclassKey = 'A1c'
+    class MyMongoListProxyA1c( MyMongoListProxyA1 ):
+        proxy_subclass_key = 'A1c'
 
-    class MyMongoDictProxyB( mongo_objects.PolymorphicMongoDictProxy ):
-        containerName = 'proxyB'
-        proxySubclassMap = {}
+    class MyMongoListProxyB( mongo_objects.PolymorphicMongoListProxy ):
+        container_name = 'proxyB'
+        proxy_subclass_map = {}
 
-    class MyMongoDictProxyBa( MyMongoDictProxyB ):
-        proxySubclassKey = 'Ba'
+    class MyMongoListProxyBa( MyMongoListProxyB ):
+        proxy_subclass_key = 'Ba'
 
-    class MyMongoDictProxyBb( MyMongoDictProxyB ):
-        proxySubclassKey = 'Bb'
+    class MyMongoListProxyBb( MyMongoListProxyB ):
+        proxy_subclass_key = 'Bb'
 
-    class MyMongoDictProxyBc( MyMongoDictProxyB ):
-        proxySubclassKey = 'Bc'
+    class MyMongoListProxyBc( MyMongoListProxyB ):
+        proxy_subclass_key = 'Bc'
 
 
     return {
         'base' : MyMongoUserDict,
-        'A' : MyMongoDictProxyA,
-        'Aa' : MyMongoDictProxyAa,
-        'Ab' : MyMongoDictProxyAb,
-        'Ac' : MyMongoDictProxyAc,
-        'A1' : MyMongoDictProxyA1,
-        'A1a' : MyMongoDictProxyA1a,
-        'A1b' : MyMongoDictProxyA1b,
-        'A1c' : MyMongoDictProxyA1c,
-        'B' : MyMongoDictProxyB,
-        'Ba' : MyMongoDictProxyBa,
-        'Bb' : MyMongoDictProxyBb,
-        'Bc' : MyMongoDictProxyBc,
+        'A' : MyMongoListProxyA,
+        'Aa' : MyMongoListProxyAa,
+        'Ab' : MyMongoListProxyAb,
+        'Ac' : MyMongoListProxyAc,
+        'A1' : MyMongoListProxyA1,
+        'A1a' : MyMongoListProxyA1a,
+        'A1b' : MyMongoListProxyA1b,
+        'A1c' : MyMongoListProxyA1c,
+        'B' : MyMongoListProxyB,
+        'Ba' : MyMongoListProxyBa,
+        'Bb' : MyMongoListProxyBb,
+        'Bc' : MyMongoListProxyBc,
     }
 
 
 
 @pytest.fixture( scope='class' )
 def getPopulatedMPMUDClasses( getMPMUDClasses ):
 
@@ -88,32 +88,32 @@
     for i in range( itemMax ):
         parent = classes['base']( {
             'name' : f"Record {i}",
             'amount' : i * 10,
         } )
 
         # make "A" proxies include a base-class proxy
-        for (j, keyA) in enumerate( ['A', 'Aa', 'Ab', 'Ac'] ):
+        for keyA in ('A', 'Aa', 'Ab', 'Ac'):
             proxyA = classes[keyA].create( parent, {
                 'nameA' : f"Proxy A-{keyA}",
-                'amountA' : j * 100,
+                'amountA' : i * 100,
             } )
 
             # make second-level A1 proxies
-            for (k, keyA1) in enumerate( ['A1', 'A1a', 'A1b', 'A1c'] ):
+            for keyA1 in ('A1', 'A1a', 'A1b', 'A1c'):
                 proxyA1 = classes[keyA1].create( proxyA, {
                     'nameA1' : f"Proxy A1-{keyA}-{keyA1}",
-                    'amountA1' : k * 1000,
+                    'amountA1' : i * 1000,
                 } )
 
         # make "B" proxies
-        for (j, keyB) in enumerate( ['B', 'Ba', 'Bb', 'Bc'] ):
+        for keyB in ('B', 'Ba', 'Bb', 'Bc'):
             proxyB = classes[keyB].create( parent, {
                 'nameB' : f"Proxy B-{keyB}",
-                'amountB' : j * 100 + 1,
+                'amountB' : i * 100 + 1,
             } )
 
 
         # save data
         parent.save()
 
     return classes
@@ -126,252 +126,299 @@
     return classes['base'].find_one()
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA( getPopulatedMPMUDClasses, getSampleParent ):
     classes = getPopulatedMPMUDClasses
     # return the first proxyA in the list
-    return classes['A'].getProxies( getSampleParent )[0]
+    return classes['A'].get_proxies( getSampleParent )[0]
 
 
 @pytest.fixture( scope='class' )
 def getSampleProxyA1( getPopulatedMPMUDClasses, getSampleProxyA ):
     classes = getPopulatedMPMUDClasses
     # return the first proxyA1 in the list
-    return classes['A1'].getProxies( getSampleProxyA )[0]
+    return classes['A1'].get_proxies( getSampleProxyA )[0]
 
 
 
 class TestInitSubclass:
     '''Test __init_subclass__ permutations'''
 
     def test_init_subclass( self ):
-        class MyTestClassBase( mongo_objects.PolymorphicMongoDictProxy ):
+        class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
             # create our own local testing namespace
-            proxySubclassMap = {}
+            proxy_subclass_map = {}
 
         class MyTestSubclassA( MyTestClassBase ):
-            proxySubclassKey = 'A'
+            proxy_subclass_key = 'A'
 
         class MyTestSubclassB( MyTestClassBase ):
-            proxySubclassKey = 'B'
+            proxy_subclass_key = 'B'
 
         class MyTestSubclassC( MyTestClassBase ):
             pass
 
         # Verify that classes A and B were added to the map
-        # Class C should be skipped because it doesn't have a non-None subclassKey
-        assert MyTestClassBase.proxySubclassMap == {
+        # Class C should be skipped because it doesn't have a non-None subclass_key
+        assert MyTestClassBase.proxy_subclass_map == {
             'A' : MyTestSubclassA,
             'B' : MyTestSubclassB
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
-        assert len( mongo_objects.PolymorphicMongoBaseProxy.proxySubclassMap ) == 0
+        assert len( mongo_objects.PolymorphicMongoBaseProxy.proxy_subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
         with pytest.raises( Exception ):
 
-            class MyTestClassBase( mongo_objects.PolymorphicMongoDictProxy ):
+            class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
                 # create our own local testing namespace
-                proxySubclassMap = {}
+                proxy_subclass_map = {}
 
             class MyTestSubclassA( MyTestClassBase ):
-                proxySubclassKey = 'A'
+                proxy_subclass_key = 'A'
 
             class MyTestSubclassAnotherA( MyTestClassBase ):
-                proxySubclassKey = 'A'
+                proxy_subclass_key = 'A'
 
 
 
 
 class TestCreate:
     def test_create( self, getPopulatedMPMUDClasses, getSampleProxyA ):
         classes = getPopulatedMPMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container() )
 
         # create a base class proxy object
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A'] )
 
+        # verify key was added to the original data
+        assert '_sdkey' in newProxy
+
         # Now create new subclass objects
-        for key in ('Aa', 'Ab', 'Ac'):
-            newProxy = classes[key].create( parent, { 'name' : f"new proxy{key} entry" } )
-            assert newProxy['_psckey'] == key
-            assert isinstance( newProxy, classes[key] )
+        for proxy_subclass in ('Aa', 'Ab', 'Ac'):
+            newProxy = classes[proxy_subclass].create( parent, { 'name' : f"new proxy{proxy_subclass} entry" } )
+            assert newProxy['_psckey'] == proxy_subclass
+            assert isinstance( newProxy, classes[proxy_subclass] )
+            assert '_sdkey' in newProxy
 
         # verify four new entries created
-        assert len( proxyA.getSubdocContainer().keys() ) == count+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container() ) == count+4
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 4
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
     def test_create_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA ):
         classes = getPopulatedMPMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer().keys() )
+        count = len( proxyA.get_subdoc_container() )
 
         # create a base class proxy object
         newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A'] )
 
+        # verify key was added to the original data
+        assert '_sdkey' in newProxy
+
         # Now create new subclass objects
-        for key in ('Aa', 'Ab', 'Ac'):
-            newProxy = classes[key].create( parent, { 'name' : f"new proxy{key} entry" }, autosave=False )
-            assert newProxy['_psckey'] == key
-            assert isinstance( newProxy, classes[key] )
+        for proxy_subclass in ('Aa', 'Ab', 'Ac'):
+            newProxy = classes[proxy_subclass].create( parent, { 'name' : f"new proxy{proxy_subclass} entry" }, autosave=False )
+            assert newProxy['_psckey'] == proxy_subclass
+            assert isinstance( newProxy, classes[proxy_subclass] )
+            assert '_sdkey' in newProxy
 
         # verify four new entries created
-        assert len( proxyA.getSubdocContainer().keys() ) == count+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container() ) == count+4
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 4
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
     def test_create_A1( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMPMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container() )
+        countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a base class second-level proxy object
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A1'] )
 
         # Now create new second-level subclass objects
         for key in ('A1a', 'A1b', 'A1c'):
             newProxy = classes[key].create( proxyA, { 'name' : f"new proxy{key} entry" } )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
         # verify four new entries created at the second level
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container() ) == countA
+        assert len( proxyA1.get_subdoc_container() ) == countA1+4
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 4
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
     def test_create_A1_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMPMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer().keys() )
-        countA1 = len( proxyA1.getSubdocContainer().keys() )
+        countA = len( proxyA.get_subdoc_container() )
+        countA1 = len( proxyA1.get_subdoc_container() )
 
         # create a base class second-level proxy object
         newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=False )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A1'] )
 
         # Now create new second-level subclass objects
         for key in ('A1a', 'A1b', 'A1c'):
             newProxy = classes[key].create( proxyA, { 'name' : f"new proxy{key} entry" }, autosave=False )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
         # verify four new entries created at the second level
-        assert len( proxyA.getSubdocContainer().keys() ) == countA
-        assert len( proxyA1.getSubdocContainer().keys() ) == countA1+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container() ) == countA
+        assert len( proxyA1.get_subdoc_container() ) == countA1+4
+        assert parent['_last_unique_integer'] == original['_last_unique_integer'] + 4
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 class TestPolymorphicBasics:
-    def test_subclassMap( self , getPopulatedMPMUDClasses ):
-        '''getMPMUDClasses create a new proxySubclassMap namespace for each proxy base class
-        Verify the keys in the proxySubclass map
-        Verify the base class proxySubclass map is empty'''
+    def test_subclass_map( self , getPopulatedMPMUDClasses ):
+        '''getMPMUDClasses create a new proxy_subclass_map namespace for each proxy base class
+        Verify the keys in the proxy_subclass map
+        Verify the base class proxy_subclass map is empty'''
         classes = getPopulatedMPMUDClasses
-        assert len( mongo_objects.PolymorphicMongoDictProxy.proxySubclassMap ) == 0
-        assert sorted( classes['A'].proxySubclassMap ) == ['Aa', 'Ab', 'Ac']
-        assert sorted( classes['A1'].proxySubclassMap ) == ['A1a', 'A1b', 'A1c']
-        assert sorted( classes['B'].proxySubclassMap ) == ['Ba', 'Bb', 'Bc']
+        assert len( mongo_objects.PolymorphicMongoListProxy.proxy_subclass_map ) == 0
+        assert sorted( classes['A'].proxy_subclass_map ) == ['Aa', 'Ab', 'Ac']
+        assert sorted( classes['A1'].proxy_subclass_map ) == ['A1a', 'A1b', 'A1c']
+        assert sorted( classes['B'].proxy_subclass_map ) == ['Ba', 'Bb', 'Bc']
+
+
+    def test_get_proxy( self, getPopulatedMPMUDClasses, getSampleParent ):
+        '''Test accessing both first-level and second-level proxies
+
+        For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
+        match the proxy_subclass_key for each subclass'''
+        classes = getPopulatedMPMUDClasses
+        parent = getSampleParent
+
+        # loop through keys in the proxy A container
+        for keyA in [ entry['_sdkey'] for entry in parent[ classes['A'].container_name ] ]:
+
+            # create a first-level proxy object
+            proxyA = classes['A'].get_proxy( parent, keyA )
+
+            # verify dictionary
+            assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ][ proxyA.seq ] )
+
+            # the base class object won't have _psckey
+            if '_psckey' not in proxyA:
+                assert isinstance( proxyA, classes['A'] )
+            else:
+                assert isinstance( proxyA, classes[ proxyA['_psckey'] ] )
+
+            # loop through the keys of the second level proxy A1 container
+            for keyA1 in [ entry['_sdkey'] for entry in parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ] ]:
+
+                # create a second-level proxy object
+                proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
+
+                # verify dictionary
+                assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ][ proxyA1.seq ] )
+
+                # the base class object won't have _psckey
+                if '_psckey' not in proxyA1:
+                    assert isinstance( proxyA1, classes['A1'] )
+                else:
+                    assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
 
 
-    def test_getProxy( self, getPopulatedMPMUDClasses, getSampleParent ):
+    def test_get_proxy_by_sequence( self, getPopulatedMPMUDClasses, getSampleParent ):
         '''Test accessing both first-level and second-level proxies
 
         For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
-        match the proxySubclassKey for each subclass'''
+        match the proxy_subclass_key for each subclass'''
         classes = getPopulatedMPMUDClasses
         parent = getSampleParent
 
         # loop through keys in the proxy A container
-        for keyA in parent[ classes['A'].containerName ].keys():
+        for seqA in range( len( parent[ classes['A'].container_name ] ) ):
 
             # create a first-level proxy object
-            proxyA = classes['A'].getProxy( parent, keyA )
+            proxyA = classes['A'].get_proxy( parent, seq=seqA )
 
             # verify dictionary
-            assert id( proxyA.data() ) == id( parent[ classes['A'].containerName ][ keyA ] )
+            assert id( proxyA.data() ) == id( parent[ classes['A'].container_name ][ seqA ] )
 
             # the base class object won't have _psckey
             if '_psckey' not in proxyA:
                 assert isinstance( proxyA, classes['A'] )
             else:
                 assert isinstance( proxyA, classes[ proxyA['_psckey'] ] )
 
             # loop through the keys of the second level proxy A1 container
-            for keyA1 in parent[ classes['A'].containerName ][ keyA ][ classes['A1'].containerName ].keys():
+            for seqA1 in range( len( parent[ classes['A'].container_name ][ proxyA.seq ][ classes['A1'].container_name ] ) ):
 
                 # create a second-level proxy object
-                proxyA1 = classes['A1'].getProxy( proxyA, keyA1 )
+                proxyA1 = classes['A1'].get_proxy( proxyA, seq=seqA1 )
 
                 # verify dictionary
-                assert id( proxyA1.data() ) == id( parent[ classes['A'].containerName ][ keyA ][ classes['A1'].containerName ][ keyA1 ] )
+                assert id( proxyA1.data() ) == id( parent[ classes['A'].container_name ][ seqA ][ classes['A1'].container_name ][ seqA1 ] )
 
                 # the base class object won't have _psckey
                 if '_psckey' not in proxyA1:
                     assert isinstance( proxyA1, classes['A1'] )
                 else:
                     assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
 
 
-    def test_getSubclassByKey( self, getMPMUDClasses ):
+    def test_get_subclass_by_key( self, getMPMUDClasses ):
         classes = getMPMUDClasses
-        assert classes['A'].getSubclassByKey( 'Aa' ) == classes['Aa']
+        assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
 
 
-    def test_getSubclassFromDoc( self, getMPMUDClasses ):
+    def test_get_subclass_from_doc( self, getMPMUDClasses ):
         classes = getMPMUDClasses
-        assert classes['A'].getSubclassByKey( 'Aa' ) == classes['Aa']
-        assert classes['A'].getSubclassFromDoc( { classes['A'].proxySubclassKeyName : 'Aa' } ) == classes['Aa']
+        assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
+        assert classes['A'].get_subclass_from_doc( { classes['A'].proxy_subclass_key_name : 'Aa' } ) == classes['Aa']
```

### Comparing `mongo_objects-1.0.22/tests/test_PolymorphicMongoListProxy.py` & `mongo_objects-1.0.26/tests/test_PolymorphicMongoSingleProxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,94 @@
-# test_PolymorphicMongoListProxy
+# test_PolymorphicMongoSingleProxy
 #
-# Since MongoListProxy has been thoroughly exercised elsewhere,
-# only test functionality unique to PolymorphicMongoListProxy
+# Since MongoSingleProxy has been thoroughly exercised elsewhere,
+# only test functionality unique to PolymorphicMongoSingleProxy
 
 from bson import ObjectId
 from datetime import datetime
 import mongo_objects
 from pymongo.collection import Collection
 import pytest
 import secrets
 
 
 
 @pytest.fixture( scope='class' )
 def getMPMUDClasses( mongo_db ):
-    '''Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection'''
+    '''Return a set of polymorphic MongoUserDict classes configured for a per-test-class unique collection
+
+    Since each class is only used once per object, we can predefine the container_name'''
 
     class MyMongoUserDict( mongo_objects.MongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
-    class MyMongoListProxyA( mongo_objects.PolymorphicMongoListProxy ):
-        containerName = 'proxyA'
-        proxySubclassMap = {}
-
-    class MyMongoListProxyAa( MyMongoListProxyA ):
-        proxySubclassKey = 'Aa'
-
-    class MyMongoListProxyAb( MyMongoListProxyA ):
-        proxySubclassKey = 'Ab'
-
-    class MyMongoListProxyAc( MyMongoListProxyA ):
-        proxySubclassKey = 'Ac'
-
-    class MyMongoListProxyA1( mongo_objects.PolymorphicMongoListProxy ):
-        containerName = 'proxyA1'
-        proxySubclassMap = {}
-
-    class MyMongoListProxyA1a( MyMongoListProxyA1 ):
-        proxySubclassKey = 'A1a'
-
-    class MyMongoListProxyA1b( MyMongoListProxyA1 ):
-        proxySubclassKey = 'A1b'
-
-    class MyMongoListProxyA1c( MyMongoListProxyA1 ):
-        proxySubclassKey = 'A1c'
-
-    class MyMongoListProxyB( mongo_objects.PolymorphicMongoListProxy ):
-        containerName = 'proxyB'
-        proxySubclassMap = {}
-
-    class MyMongoListProxyBa( MyMongoListProxyB ):
-        proxySubclassKey = 'Ba'
-
-    class MyMongoListProxyBb( MyMongoListProxyB ):
-        proxySubclassKey = 'Bb'
-
-    class MyMongoListProxyBc( MyMongoListProxyB ):
-        proxySubclassKey = 'Bc'
+    class MyMongoSingleProxyA( mongo_objects.PolymorphicMongoSingleProxy ):
+        proxy_subclass_map = {}
+        container_name = "proxyA-0"
+
+    class MyMongoSingleProxyAa( MyMongoSingleProxyA ):
+        proxy_subclass_key = 'Aa'
+        container_name = "proxyA-1"
+
+    class MyMongoSingleProxyAb( MyMongoSingleProxyA ):
+        proxy_subclass_key = 'Ab'
+        container_name = "proxyA-2"
+
+    class MyMongoSingleProxyAc( MyMongoSingleProxyA ):
+        proxy_subclass_key = 'Ac'
+        container_name = "proxyA-3"
+
+    class MyMongoSingleProxyA1( mongo_objects.PolymorphicMongoSingleProxy ):
+        proxy_subclass_map = {}
+        container_name = "proxyA1-0"
+
+    class MyMongoSingleProxyA1a( MyMongoSingleProxyA1 ):
+        proxy_subclass_key = 'A1a'
+        container_name = "proxyA1-1"
+
+    class MyMongoSingleProxyA1b( MyMongoSingleProxyA1 ):
+        proxy_subclass_key = 'A1b'
+        container_name = "proxyA1-2"
+
+    class MyMongoSingleProxyA1c( MyMongoSingleProxyA1 ):
+        proxy_subclass_key = 'A1c'
+        container_name = "proxyA1-3"
+
+    class MyMongoSingleProxyB( mongo_objects.PolymorphicMongoSingleProxy ):
+        proxy_subclass_map = {}
+        container_name = "proxyB-0"
+
+    class MyMongoSingleProxyBa( MyMongoSingleProxyB ):
+        proxy_subclass_key = 'Ba'
+        container_name = "proxyB-1"
+
+    class MyMongoSingleProxyBb( MyMongoSingleProxyB ):
+        proxy_subclass_key = 'Bb'
+        container_name = "proxyB-2"
+
+    class MyMongoSingleProxyBc( MyMongoSingleProxyB ):
+        proxy_subclass_key = 'Bc'
+        container_name = "proxyB-3"
 
 
     return {
         'base' : MyMongoUserDict,
-        'A' : MyMongoListProxyA,
-        'Aa' : MyMongoListProxyAa,
-        'Ab' : MyMongoListProxyAb,
-        'Ac' : MyMongoListProxyAc,
-        'A1' : MyMongoListProxyA1,
-        'A1a' : MyMongoListProxyA1a,
-        'A1b' : MyMongoListProxyA1b,
-        'A1c' : MyMongoListProxyA1c,
-        'B' : MyMongoListProxyB,
-        'Ba' : MyMongoListProxyBa,
-        'Bb' : MyMongoListProxyBb,
-        'Bc' : MyMongoListProxyBc,
+        'A' : MyMongoSingleProxyA,
+        'Aa' : MyMongoSingleProxyAa,
+        'Ab' : MyMongoSingleProxyAb,
+        'Ac' : MyMongoSingleProxyAc,
+        'A1' : MyMongoSingleProxyA1,
+        'A1a' : MyMongoSingleProxyA1a,
+        'A1b' : MyMongoSingleProxyA1b,
+        'A1c' : MyMongoSingleProxyA1c,
+        'B' : MyMongoSingleProxyB,
+        'Ba' : MyMongoSingleProxyBa,
+        'Bb' : MyMongoSingleProxyBb,
+        'Bc' : MyMongoSingleProxyBc,
     }
 
 
 
 @pytest.fixture( scope='class' )
 def getPopulatedMPMUDClasses( getMPMUDClasses ):
 
@@ -88,33 +99,42 @@
     for i in range( itemMax ):
         parent = classes['base']( {
             'name' : f"Record {i}",
             'amount' : i * 10,
         } )
 
         # make "A" proxies include a base-class proxy
-        for keyA in ('A', 'Aa', 'Ab', 'Ac'):
-            proxyA = classes[keyA].create( parent, {
-                'nameA' : f"Proxy A-{keyA}",
-                'amountA' : i * 100,
-            } )
+        for (j, keyA) in enumerate( ['A', 'Aa', 'Ab', 'Ac'] ):
+            proxyA = classes[keyA].create(
+                parent,
+                {
+                    'nameA' : f"Proxy A-{j}",
+                    'amountA' : j * 100,
+                },
+            )
 
             # make second-level A1 proxies
-            for keyA1 in ('A1', 'A1a', 'A1b', 'A1c'):
-                proxyA1 = classes[keyA1].create( proxyA, {
-                    'nameA1' : f"Proxy A1-{keyA}-{keyA1}",
-                    'amountA1' : i * 1000,
-                } )
+            for (k, keyA1) in enumerate( ['A1', 'A1a', 'A1b', 'A1c'] ):
+                proxyA1 = classes[keyA1].create(
+                    proxyA,
+                    {
+                        'nameA1' : f"Proxy A1-{k}",
+                        'amountA1' : k * 1000,
+                    },
+                )
 
         # make "B" proxies
-        for keyB in ('B', 'Ba', 'Bb', 'Bc'):
-            proxyB = classes[keyB].create( parent, {
-                'nameB' : f"Proxy B-{keyB}",
-                'amountB' : i * 100 + 1,
-            } )
+        for (j, keyB) in enumerate( ['B', 'Ba', 'Bb', 'Bc'] ):
+            proxyB = classes[keyB].create(
+                parent,
+                {
+                    'nameB' : f"Proxy B-{j}",
+                    'amountB' : j * 100 + 1,
+                },
+            )
 
 
         # save data
         parent.save()
 
     return classes
 
@@ -123,302 +143,312 @@
 def getSampleParent( getPopulatedMPMUDClasses ):
     classes = getPopulatedMPMUDClasses
     # find a random entry of the base class
     return classes['base'].find_one()
 
 
 @pytest.fixture( scope='class' )
-def getSampleProxyA( getPopulatedMPMUDClasses, getSampleParent ):
+def getSampleProxyAKey():
+    '''Return a fixed sample key for first-level A proxy testing'''
+    return 'proxyA-0'
+
+
+@pytest.fixture( scope='class' )
+def getSampleProxyAKeys():
+    '''Return a fixed sample keys for first-level A proxy testing'''
+    return [ 'proxyA-0', 'proxyA-1', 'proxyA-2' ]
+
+
+@pytest.fixture( scope='class' )
+def getSampleProxyA( getPopulatedMPMUDClasses, getSampleParent, getSampleProxyAKey ):
     classes = getPopulatedMPMUDClasses
-    # return the first proxyA in the list
-    return classes['A'].getProxies( getSampleParent )[0]
+    return classes['A'].get_proxy( getSampleParent, getSampleProxyAKey )
+
+
+@pytest.fixture( scope='class' )
+def getSampleProxyA1Key():
+    '''Return a fixed sample key for second-level A1 proxy testing'''
+    return 'proxyA1-0'
+
+
+@pytest.fixture( scope='class' )
+def getSampleProxyA1Keys():
+    '''Return a fixed sample keys for first-level A proxy testing'''
+    return [ 'proxyA1-0', 'proxyA1-1', 'proxyA1-2' ]
 
 
 @pytest.fixture( scope='class' )
-def getSampleProxyA1( getPopulatedMPMUDClasses, getSampleProxyA ):
+def getSampleProxyA1( getPopulatedMPMUDClasses, getSampleProxyA, getSampleProxyA1Key ):
     classes = getPopulatedMPMUDClasses
-    # return the first proxyA1 in the list
-    return classes['A1'].getProxies( getSampleProxyA )[0]
+    return classes['A1'].get_proxy( getSampleProxyA, getSampleProxyA1Key )
 
 
 
 class TestInitSubclass:
     '''Test __init_subclass__ permutations'''
 
     def test_init_subclass( self ):
-        class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
+        class MyTestClassBase( mongo_objects.PolymorphicMongoSingleProxy ):
             # create our own local testing namespace
-            proxySubclassMap = {}
+            proxy_subclass_map = {}
 
         class MyTestSubclassA( MyTestClassBase ):
-            proxySubclassKey = 'A'
+            proxy_subclass_key = 'A'
 
         class MyTestSubclassB( MyTestClassBase ):
-            proxySubclassKey = 'B'
+            proxy_subclass_key = 'B'
 
         class MyTestSubclassC( MyTestClassBase ):
             pass
 
         # Verify that classes A and B were added to the map
-        # Class C should be skipped because it doesn't have a non-None subclassKey
-        assert MyTestClassBase.proxySubclassMap == {
+        # Class C should be skipped because it doesn't have a non-None subclass_key
+        assert MyTestClassBase.proxy_subclass_map == {
             'A' : MyTestSubclassA,
             'B' : MyTestSubclassB
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
-        assert len( mongo_objects.PolymorphicMongoBaseProxy.proxySubclassMap ) == 0
+        assert len( mongo_objects.PolymorphicMongoBaseProxy.proxy_subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
         with pytest.raises( Exception ):
 
-            class MyTestClassBase( mongo_objects.PolymorphicMongoListProxy ):
+            class MyTestClassBase( mongo_objects.PolymorphicMongoSingleProxy ):
                 # create our own local testing namespace
-                proxySubclassMap = {}
+                proxy_subclass_map = {}
 
             class MyTestSubclassA( MyTestClassBase ):
-                proxySubclassKey = 'A'
+                proxy_subclass_key = 'A'
 
             class MyTestSubclassAnotherA( MyTestClassBase ):
-                proxySubclassKey = 'A'
+                proxy_subclass_key = 'A'
 
 
 
 
 class TestCreate:
     def test_create( self, getPopulatedMPMUDClasses, getSampleProxyA ):
         classes = getPopulatedMPMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer() )
+        count = len( proxyA.get_subdoc_container().keys() )
 
         # create a base class proxy object
-        newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'} )
+        # Override the container name since there is already a proxyA at the default location
+        newProxy = classes['A'].create( 
+            parent,
+            { 'name' : 'new proxyA entry'},
+            key='newProxyA'
+        )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A'] )
 
-        # verify key was added to the original data
-        assert '_sdkey' in newProxy
-
         # Now create new subclass objects
-        for proxyClass in ('Aa', 'Ab', 'Ac'):
-            newProxy = classes[proxyClass].create( parent, { 'name' : f"new proxy{proxyClass} entry" } )
-            assert newProxy['_psckey'] == proxyClass
-            assert isinstance( newProxy, classes[proxyClass] )
-            assert '_sdkey' in newProxy
+        for key in ('Aa', 'Ab', 'Ac'):
+            newProxy = classes[key].create(
+                parent,
+                { 'name' : f"new proxy{key} entry" },
+                key=f"newProxy{key}" )
+            assert newProxy['_psckey'] == key
+            assert isinstance( newProxy, classes[key] )
 
         # verify four new entries created
-        assert len( proxyA.getSubdocContainer() ) == count+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container().keys() ) == count+4
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
+class TestCreateNoSave:
     def test_create_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA ):
         classes = getPopulatedMPMUDClasses
         proxyA = getSampleProxyA
         parent = proxyA.parent
 
         # record current state
         original = dict( parent )
-        count = len( proxyA.getSubdocContainer() )
+        count = len( proxyA.get_subdoc_container().keys() )
 
         # create a base class proxy object
-        newProxy = classes['A'].create( parent, { 'name' : 'new proxyA entry'}, autosave=False )
+        newProxy = classes['A'].create( 
+            parent,
+            { 'name' : 'new proxyA entry'},
+            key='newProxyA',
+            autosave=False
+        )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A'] )
 
-        # verify key was added to the original data
-        assert '_sdkey' in newProxy
-
         # Now create new subclass objects
-        for proxyClass in ('Aa', 'Ab', 'Ac'):
-            newProxy = classes[proxyClass].create( parent, { 'name' : f"new proxy{proxyClass} entry" }, autosave=False )
-            assert newProxy['_psckey'] == proxyClass
-            assert isinstance( newProxy, classes[proxyClass] )
-            assert '_sdkey' in newProxy
+        for key in ('Aa', 'Ab', 'Ac'):
+            newProxy = classes[key].create(
+                parent,
+                { 'name' : f"new proxy{key} entry" },
+                key=f"newProxy{key}",
+                autosave=False
+            )
+            assert newProxy['_psckey'] == key
+            assert isinstance( newProxy, classes[key] )
 
         # verify four new entries created
-        assert len( proxyA.getSubdocContainer() ) == count+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container().keys() ) == count+4
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
+class TestCreateA1:
     def test_create_A1( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMPMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer() )
-        countA1 = len( proxyA1.getSubdocContainer() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a base class second-level proxy object
-        newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'} )
+        newProxy = classes['A1'].create(
+            proxyA,
+            { 'name' : 'new proxyA1 entry'},
+            key='newProxyA1'
+        )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A1'] )
 
         # Now create new second-level subclass objects
         for key in ('A1a', 'A1b', 'A1c'):
-            newProxy = classes[key].create( proxyA, { 'name' : f"new proxy{key} entry" } )
+            newProxy = classes[key].create(
+                proxyA,
+                { 'name' : f"new proxy{key} entry" },
+                key=f"newProxy{key}",
+            )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
         # verify four new entries created at the second level
-        assert len( proxyA.getSubdocContainer() ) == countA
-        assert len( proxyA1.getSubdocContainer() ) == countA1+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1+4
 
         # confirm the parent document was saved
         assert parent['_updated'] > original['_updated']
 
 
+class TestCreateA1NoSave:
     def test_create_A1_no_save( self, getPopulatedMPMUDClasses, getSampleProxyA1 ):
         classes = getPopulatedMPMUDClasses
         proxyA1 = getSampleProxyA1
         proxyA = proxyA1.parent
-        parent = proxyA1.ultimateParent
+        parent = proxyA1.ultimate_parent
 
         # record current state
         original = dict( parent )
-        countA = len( proxyA.getSubdocContainer() )
-        countA1 = len( proxyA1.getSubdocContainer() )
+        countA = len( proxyA.get_subdoc_container().keys() )
+        countA1 = len( proxyA1.get_subdoc_container().keys() )
 
         # create a base class second-level proxy object
-        newProxy = classes['A1'].create( proxyA, { 'name' : 'new proxyA1 entry'}, autosave=False )
+        newProxy = classes['A1'].create(
+            proxyA,
+            { 'name' : 'new proxyA1 entry'},
+            key='newProxyA',
+            autosave=False
+        )
 
-        # Since the base class does not define a proxySubclassKey, verify none was added to the record
+        # Since the base class does not define a proxy_subclass_key, verify none was added to the record
         assert '_psckey' not in newProxy
         assert isinstance( newProxy, classes['A1'] )
 
         # Now create new second-level subclass objects
         for key in ('A1a', 'A1b', 'A1c'):
-            newProxy = classes[key].create( proxyA, { 'name' : f"new proxy{key} entry" }, autosave=False )
+            newProxy = classes[key].create(
+                proxyA,
+                { 'name' : f"new proxy{key} entry" },
+                key=f"newProxy{key}",
+                autosave=False
+            )
             assert newProxy['_psckey'] == key
             assert isinstance( newProxy, classes[key] )
 
         # verify four new entries created at the second level
-        assert len( proxyA.getSubdocContainer() ) == countA
-        assert len( proxyA1.getSubdocContainer() ) == countA1+4
-        assert parent['_lastUniqueInteger'] == original['_lastUniqueInteger'] + 4
+        assert len( proxyA.get_subdoc_container().keys() ) == countA
+        assert len( proxyA1.get_subdoc_container().keys() ) == countA1+4
 
         # confirm the parent document was not saved
         assert parent['_updated'] == original['_updated']
 
 
 
 class TestPolymorphicBasics:
-    def test_subclassMap( self , getPopulatedMPMUDClasses ):
-        '''getMPMUDClasses create a new proxySubclassMap namespace for each proxy base class
-        Verify the keys in the proxySubclass map
-        Verify the base class proxySubclass map is empty'''
+    def test_subclass_map( self , getPopulatedMPMUDClasses ):
+        '''getMPMUDClasses create a new proxy_subclass_map namespace for each proxy base class
+        Verify the keys in the proxy_subclass map
+        Verify the base class proxy_subclass map is empty'''
         classes = getPopulatedMPMUDClasses
-        assert len( mongo_objects.PolymorphicMongoListProxy.proxySubclassMap ) == 0
-        assert sorted( classes['A'].proxySubclassMap ) == ['Aa', 'Ab', 'Ac']
-        assert sorted( classes['A1'].proxySubclassMap ) == ['A1a', 'A1b', 'A1c']
-        assert sorted( classes['B'].proxySubclassMap ) == ['Ba', 'Bb', 'Bc']
-
-
-    def test_getProxy( self, getPopulatedMPMUDClasses, getSampleParent ):
-        '''Test accessing both first-level and second-level proxies
-
-        For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
-        match the proxySubclassKey for each subclass'''
-        classes = getPopulatedMPMUDClasses
-        parent = getSampleParent
-
-        # loop through keys in the proxy A container
-        for keyA in [ entry['_sdkey'] for entry in parent[ classes['A'].containerName ] ]:
-
-            # create a first-level proxy object
-            proxyA = classes['A'].getProxy( parent, keyA )
-
-            # verify dictionary
-            assert id( proxyA.data() ) == id( parent[ classes['A'].containerName ][ proxyA.seq ] )
-
-            # the base class object won't have _psckey
-            if '_psckey' not in proxyA:
-                assert isinstance( proxyA, classes['A'] )
-            else:
-                assert isinstance( proxyA, classes[ proxyA['_psckey'] ] )
-
-            # loop through the keys of the second level proxy A1 container
-            for keyA1 in [ entry['_sdkey'] for entry in parent[ classes['A'].containerName ][ proxyA.seq ][ classes['A1'].containerName ] ]:
-
-                # create a second-level proxy object
-                proxyA1 = classes['A1'].getProxy( proxyA, keyA1 )
-
-                # verify dictionary
-                assert id( proxyA1.data() ) == id( parent[ classes['A'].containerName ][ proxyA.seq ][ classes['A1'].containerName ][ proxyA1.seq ] )
-
-                # the base class object won't have _psckey
-                if '_psckey' not in proxyA1:
-                    assert isinstance( proxyA1, classes['A1'] )
-                else:
-                    assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
+        assert len( mongo_objects.PolymorphicMongoSingleProxy.proxy_subclass_map ) == 0
+        assert sorted( classes['A'].proxy_subclass_map ) == ['Aa', 'Ab', 'Ac']
+        assert sorted( classes['A1'].proxy_subclass_map ) == ['A1a', 'A1b', 'A1c']
+        assert sorted( classes['B'].proxy_subclass_map ) == ['Ba', 'Bb', 'Bc']
 
 
-    def test_getProxy_by_sequence( self, getPopulatedMPMUDClasses, getSampleParent ):
+    def test_get_proxy( self, getPopulatedMPMUDClasses, getSampleParent, getSampleProxyAKeys, getSampleProxyA1Keys ):
         '''Test accessing both first-level and second-level proxies
 
         For testing convenience, the keys of the getPopulatedMPMUDClasses dictionary
-        match the proxySubclassKey for each subclass'''
+        match the proxy_subclass_key for each subclass'''
         classes = getPopulatedMPMUDClasses
         parent = getSampleParent
 
         # loop through keys in the proxy A container
-        for seqA in range( len( parent[ classes['A'].containerName ] ) ):
+        for keyA in getSampleProxyAKeys:
 
             # create a first-level proxy object
-            proxyA = classes['A'].getProxy( parent, seq=seqA )
+            proxyA = classes['A'].get_proxy( parent, keyA )
 
             # verify dictionary
-            assert id( proxyA.data() ) == id( parent[ classes['A'].containerName ][ seqA ] )
+            assert id( proxyA.data() ) == id( parent[ keyA ] )
 
             # the base class object won't have _psckey
             if '_psckey' not in proxyA:
                 assert isinstance( proxyA, classes['A'] )
             else:
                 assert isinstance( proxyA, classes[ proxyA['_psckey'] ] )
 
             # loop through the keys of the second level proxy A1 container
-            for seqA1 in range( len( parent[ classes['A'].containerName ][ proxyA.seq ][ classes['A1'].containerName ] ) ):
+            for keyA1 in getSampleProxyA1Keys:
 
                 # create a second-level proxy object
-                proxyA1 = classes['A1'].getProxy( proxyA, seq=seqA1 )
+                proxyA1 = classes['A1'].get_proxy( proxyA, keyA1 )
 
                 # verify dictionary
-                assert id( proxyA1.data() ) == id( parent[ classes['A'].containerName ][ seqA ][ classes['A1'].containerName ][ seqA1 ] )
+                assert id( proxyA1.data() ) == id( parent[ keyA ][ keyA1 ] )
 
                 # the base class object won't have _psckey
                 if '_psckey' not in proxyA1:
                     assert isinstance( proxyA1, classes['A1'] )
                 else:
                     assert isinstance( proxyA1, classes[ proxyA1['_psckey'] ] )
 
 
-    def test_getSubclassByKey( self, getMPMUDClasses ):
+    def test_get_subclass_by_key( self, getMPMUDClasses ):
         classes = getMPMUDClasses
-        assert classes['A'].getSubclassByKey( 'Aa' ) == classes['Aa']
+        assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
 
 
-    def test_getSubclassFromDoc( self, getMPMUDClasses ):
+    def test_get_subclass_from_doc( self, getMPMUDClasses ):
         classes = getMPMUDClasses
-        assert classes['A'].getSubclassByKey( 'Aa' ) == classes['Aa']
-        assert classes['A'].getSubclassFromDoc( { classes['A'].proxySubclassKeyName : 'Aa' } ) == classes['Aa']
+        assert classes['A'].get_subclass_by_key( 'Aa' ) == classes['Aa']
+        assert classes['A'].get_subclass_from_doc( { classes['A'].proxy_subclass_key_name : 'Aa' } ) == classes['Aa']
```

### Comparing `mongo_objects-1.0.22/tests/test_PolymorphicMongoUserDict.py` & `mongo_objects-1.0.26/tests/test_PolymorphicMongoUserDict.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,21 @@
     '''Return a set of PolymorphicMongoUserDict classes configured for a per-test-class unique collection'''
 
     class MyPolymorphicMongoUserDictBase( mongo_objects.PolymorphicMongoUserDict ):
         collection_name = secrets.token_hex(6)
         database = mongo_db
 
     class MyPolymorphicMongoUserDictA( MyPolymorphicMongoUserDictBase ):
-        subclassKey = 'A'
+        subclass_key = 'A'
 
     class MyPolymorphicMongoUserDictB( MyPolymorphicMongoUserDictBase ):
-        subclassKey = 'B'
+        subclass_key = 'B'
 
     class MyPolymorphicMongoUserDictC( MyPolymorphicMongoUserDictBase ):
-        subclassKey = 'C'
+        subclass_key = 'C'
 
     return {
         'base' : MyPolymorphicMongoUserDictBase,
         'A' : MyPolymorphicMongoUserDictA,
         'B' : MyPolymorphicMongoUserDictB,
         'C' : MyPolymorphicMongoUserDictC
     }
@@ -73,58 +73,58 @@
 
 class TestInitSubclass:
     '''Test __init_subclass__ permutations'''
 
     def test_init_subclass( self ):
         class MyTestClassBase( mongo_objects.PolymorphicMongoUserDict ):
             # create our own local testing namespace
-            subclassMap = {}
+            subclass_map = {}
 
         class MyTestSubclassA( MyTestClassBase ):
-            subclassKey = 'A'
+            subclass_key = 'A'
 
         class MyTestSubclassB( MyTestClassBase ):
-            subclassKey = 'B'
+            subclass_key = 'B'
 
         class MyTestSubclassC( MyTestClassBase ):
             pass
 
         # Verify that classes A and B were added to the map
-        # Class C should be skipped because it doesn't have a non-None subclassKey
-        assert MyTestClassBase.subclassMap == {
+        # Class C should be skipped because it doesn't have a non-None subclass_key
+        assert MyTestClassBase.subclass_map == {
             'A' : MyTestSubclassA,
             'B' : MyTestSubclassB
         }
 
         # verify our local subclass map namespace didn't affect the module base class map
-        assert len( mongo_objects.PolymorphicMongoUserDict.subclassMap ) == 0
+        assert len( mongo_objects.PolymorphicMongoUserDict.subclass_map ) == 0
 
 
     def test_init_subclass_duplicate_key( self ):
         with pytest.raises( Exception ):
 
             class MyTestClassBase( mongo_objects.PolymorphicMongoUserDict ):
                 # create our own local testing namespace
-                subclassMap = {}
+                subclass_map = {}
 
             class MyTestSubclassA( MyTestClassBase ):
-                subclassKey = 'A'
+                subclass_key = 'A'
 
             class MyTestSubclassAnotherA( MyTestClassBase ):
-                subclassKey = 'A'
+                subclass_key = 'A'
 
 
 
 class TestPolymorphicBasics:
-    def test_subclassMap( self , getPopulatedMPMUDClasses ):
-        '''getMPMUDClasses doesn't create a new subclassMap namespace
-        Verify that our base class and the module base class subclassMaps are the same'''
+    def test_subclass_map( self , getPopulatedMPMUDClasses ):
+        '''getMPMUDClasses doesn't create a new subclass_map namespace
+        Verify that our base class and the module base class subclass_maps are the same'''
         classes = getPopulatedMPMUDClasses
-        assert len( classes['base'].subclassMap ) == 3
-        assert classes['base'].subclassMap == mongo_objects.PolymorphicMongoUserDict.subclassMap
+        assert len( classes['base'].subclass_map ) == 3
+        assert classes['base'].subclass_map == mongo_objects.PolymorphicMongoUserDict.subclass_map
 
 
     def test_find_all( self, getPopulatedMPMUDClasses ):
         '''Verify all sample data are returned with the correct class'''
         classes = getPopulatedMPMUDClasses
         for obj in classes['base'].find():
             # match the sample data to the expected classes
@@ -253,21 +253,21 @@
         '''Verify a non-matching filter produces a None result'''
         classes = getPopulatedMPMUDClasses
         obj = classes['base'].find_one( { 'not-a-match' : 'will not return data'} )
         assert obj is None
 
 
     def test_find_one_none_custom_return( self, getPopulatedMPMUDClasses ):
-        '''Verify a non-matching filter produces our custom "noMatch" result'''
+        '''Verify a non-matching filter produces our custom "no_match" result'''
         classes = getPopulatedMPMUDClasses
 
         class EmptyResponse( object ):
             pass
 
-        obj = classes['base'].find_one( { 'not-a-match' : 'will not return data'}, noMatch=EmptyResponse() )
+        obj = classes['base'].find_one( { 'not-a-match' : 'will not return data'}, no_match=EmptyResponse() )
 
         assert isinstance( obj, EmptyResponse )
 
 
     def test_find_one_projection_1( self, getPopulatedMPMUDClasses ):
         '''Verify "positive" projection works'''
         classes = getPopulatedMPMUDClasses
@@ -330,60 +330,60 @@
     def test_instantiate( self, getPopulatedMPMUDClasses ):
         classes = getPopulatedMPMUDClasses
         obj = classes['base'].instantiate( { '_sckey' : 'A' } )
         assert isinstance( obj, classes['A'] )
         assert obj.readonly is False
 
 
-    def test_getSubclassByKey( self, getMPMUDClasses ):
+    def test_get_subclass_by_key( self, getMPMUDClasses ):
         classes = getMPMUDClasses
-        assert classes['base'].getSubclassByKey( 'A' ) == classes['A']
+        assert classes['base'].get_subclass_by_key( 'A' ) == classes['A']
 
 
-    def test_getSubclassFromDoc( self, getMPMUDClasses ):
+    def test_get_subclass_from_doc( self, getMPMUDClasses ):
         classes = getMPMUDClasses
-        assert classes['base'].getSubclassFromDoc( { classes['base'].subclassKeyName : 'A' } ) == classes['A']
+        assert classes['base'].get_subclass_from_doc( { classes['base'].subclass_key_name : 'A' } ) == classes['A']
 
 
     def test_instantiate_readonly( self, getPopulatedMPMUDClasses ):
         classes = getPopulatedMPMUDClasses
         obj = classes['base'].instantiate( { '_sckey' : 'B' }, readonly=True )
         assert isinstance( obj, classes['B'] )
         assert obj.readonly is True
 
 
-    def test_loadProxyById( self, getPopulatedMPMUDClasses ):
+    def test_load_proxy_by_id( self, getPopulatedMPMUDClasses ):
         '''Verify find_one() readonly flag'''
         classes = getPopulatedMPMUDClasses
 
         # loop through sample objects
         for source in classes['base'].find():
 
             # load the same object with an empty proxy tree
-            result = classes['base'].loadProxyById( source.id() )
+            result = classes['base'].load_proxy_by_id( source.id() )
 
             # verify that the type of the object is correct
             assert type(source) == type(result)
 
             # verify the objects are the same
             assert source == result
 
             # verify the object is readonly
             assert result.readonly is False
 
 
-    def test_loadProxyById( self, getPopulatedMPMUDClasses ):
+    def test_load_proxy_by_id( self, getPopulatedMPMUDClasses ):
         '''Verify find_one() readonly flag'''
         classes = getPopulatedMPMUDClasses
 
         # loop through sample objects
         for source in classes['base'].find():
 
             # load the same object with an empty proxy tree
-            result = classes['base'].loadProxyById( source.id(), readonly=True )
+            result = classes['base'].load_proxy_by_id( source.id(), readonly=True )
 
             # verify that the type of the object is correct
             assert type(source) == type(result)
 
             # verify the objects are the same
             assert source == result
```

### Comparing `mongo_objects-1.0.22/tests/test_proxy_combo.py` & `mongo_objects-1.0.26/tests/test_proxy_combo.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,21 +27,21 @@
 
 class TestDictAsPrimary:
     def test_dict_proxy_as_primary( self, getMMUDBaseClass ):
         itemMax = 3     # make three of everything
 
         # create one class of each proxy type
         class MyMongoDictProxyA( mongo_objects.MongoDictProxy ):
-            containerName = 'proxyA'
+            container_name = 'proxyA'
 
         class MyMongoListProxyA1( mongo_objects.MongoListProxy ):
-            containerName = 'proxyA1'
+            container_name = 'proxyA1'
 
         class MyMongoSingleProxyA2( mongo_objects.MongoSingleProxy ):
-            containerName = 'proxyA2'
+            container_name = 'proxyA2'
 
         # create an empty object
         obj = getMMUDBaseClass()
 
         # populate three first-level dict proxies with
         # second-level list and single proxy objects
         for i in range( itemMax ):
@@ -64,41 +64,41 @@
                 { 'name' : f"proxyA2" },
             )
 
         # save the original object
         obj.save()
 
         # reload the data from the database into a new object
-        obj2 = getMMUDBaseClass.loadById( obj['_id'] )
+        obj2 = getMMUDBaseClass.load_by_id( obj['_id'] )
 
         # check that all first-level proxy entries are present
-        assert sorted( [ x['name'] for x in MyMongoDictProxyA.getProxies( obj2 ) ] ) == \
+        assert sorted( [ x['name'] for x in MyMongoDictProxyA.get_proxies( obj2 ) ] ) == \
                 [ 'proxyA-0', 'proxyA-1', 'proxyA-2' ]
 
         # loop through each first-level proxy and check the second-level entries
-        for proxyA in MyMongoDictProxyA.getProxies( obj2 ):
-            assert sorted( [ x['name'] for x in MyMongoListProxyA1.getProxies( proxyA ) ] ) == \
+        for proxyA in MyMongoDictProxyA.get_proxies( obj2 ):
+            assert sorted( [ x['name'] for x in MyMongoListProxyA1.get_proxies( proxyA ) ] ) == \
                     [ 'proxyA1-0', 'proxyA1-1', 'proxyA1-2' ]
-            assert MyMongoSingleProxyA2.getProxy( proxyA )['name'] == "proxyA2"
+            assert MyMongoSingleProxyA2.get_proxy( proxyA )['name'] == "proxyA2"
 
 
 
 class TestListAsPrimary:
     def test_list_proxy_as_primary( self, getMMUDBaseClass ):
         itemMax = 3     # make three of everything
 
         # create one class of each proxy type
         class MyMongoListProxyA( mongo_objects.MongoListProxy ):
-            containerName = 'proxyA'
+            container_name = 'proxyA'
 
         class MyMongoDictProxyA1( mongo_objects.MongoDictProxy ):
-            containerName = 'proxyA1'
+            container_name = 'proxyA1'
 
         class MyMongoSingleProxyA2( mongo_objects.MongoSingleProxy ):
-            containerName = 'proxyA2'
+            container_name = 'proxyA2'
 
         # create an empty object
         obj = getMMUDBaseClass()
 
         # populate three first-level list proxies with
         # second-level dict and single proxy objects
         for i in range( itemMax ):
@@ -121,41 +121,41 @@
                 { 'name' : f"proxyA2" },
             )
 
         # save the original object
         obj.save()
 
         # reload the data from the database into a new object
-        obj2 = getMMUDBaseClass.loadById( obj['_id'] )
+        obj2 = getMMUDBaseClass.load_by_id( obj['_id'] )
 
         # check that all first-level proxy entries are present
-        assert sorted( [ x['name'] for x in MyMongoListProxyA.getProxies( obj2 ) ] ) == \
+        assert sorted( [ x['name'] for x in MyMongoListProxyA.get_proxies( obj2 ) ] ) == \
                 [ 'proxyA-0', 'proxyA-1', 'proxyA-2' ]
 
         # loop through each first-level proxy and check the second-level entries
-        for proxyA in MyMongoListProxyA.getProxies( obj2 ):
-            assert sorted( [ x['name'] for x in MyMongoDictProxyA1.getProxies( proxyA ) ] ) == \
+        for proxyA in MyMongoListProxyA.get_proxies( obj2 ):
+            assert sorted( [ x['name'] for x in MyMongoDictProxyA1.get_proxies( proxyA ) ] ) == \
                     [ 'proxyA1-0', 'proxyA1-1', 'proxyA1-2' ]
-            assert MyMongoSingleProxyA2.getProxy( proxyA )['name'] == "proxyA2"
+            assert MyMongoSingleProxyA2.get_proxy( proxyA )['name'] == "proxyA2"
 
 
 
 class TestSingleAsPrimary:
     def test_dict_proxy_as_primary( self, getMMUDBaseClass ):
         itemMax = 3     # make three of everything
 
         # create one class of each proxy type
         class MyMongoSingleProxyA( mongo_objects.MongoSingleProxy ):
-            containerName = 'proxyA2'
+            container_name = 'proxyA2'
 
         class MyMongoDictProxyA1( mongo_objects.MongoDictProxy ):
-            containerName = 'proxyA1'
+            container_name = 'proxyA1'
 
         class MyMongoListProxyA2( mongo_objects.MongoListProxy ):
-            containerName = 'proxyA2'
+            container_name = 'proxyA2'
 
 
         # create an empty object
         obj = getMMUDBaseClass()
 
         # create only one single proxy object
         proxyA = MyMongoSingleProxyA.create(
@@ -177,21 +177,21 @@
                 { 'name' : f"proxyA2-{i}" },
                 autosave=False
             )
         # save the original object
         obj.save()
 
         # reload the data from the database into a new object
-        obj2 = getMMUDBaseClass.loadById( obj['_id'] )
+        obj2 = getMMUDBaseClass.load_by_id( obj['_id'] )
 
         # check that the first-level proxy entry is present
-        proxyA = MyMongoSingleProxyA.getProxy( obj2 )
+        proxyA = MyMongoSingleProxyA.get_proxy( obj2 )
         assert proxyA['name'] == "proxyA"
 
         # loop check the second-level entries
-        assert sorted( [ x['name'] for x in MyMongoDictProxyA1.getProxies( proxyA ) ] ) == \
+        assert sorted( [ x['name'] for x in MyMongoDictProxyA1.get_proxies( proxyA ) ] ) == \
                 [ 'proxyA1-0', 'proxyA1-1', 'proxyA1-2' ]
-        assert sorted( [ x['name'] for x in MyMongoListProxyA2.getProxies( proxyA ) ] ) == \
+        assert sorted( [ x['name'] for x in MyMongoListProxyA2.get_proxies( proxyA ) ] ) == \
                 [ 'proxyA2-0', 'proxyA2-1', 'proxyA2-2' ]
```

### Comparing `mongo_objects-1.0.22/tools/runTests` & `mongo_objects-1.0.26/tools/runTests`

 * *Files identical despite different names*

### Comparing `mongo_objects-1.0.22/tools/setupPythonVenv` & `mongo_objects-1.0.26/tools/setupPythonVenv`

 * *Files 9% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 PROJECT_DIR=$(pwd)
 PROJECT_NAME=$(basename ${PROJECT_DIR})
 VENV_DIR=${PROJECT_DIR}/venv
 
 # check the virtual environment version on MacOS
 if [[ "$(uname)" == "Darwin" ]]; then
 
-    # Make sure Homebrew Python 3.11 is installed
-    if [[ ! -e /usr/local/bin/python3.11 ]]; then
-        echo "Python 3.11 is not installed"
+    # Make sure Homebrew Python 3.12 is installed
+    if [[ ! -e /usr/local/bin/python3.12 ]]; then
+        echo "Python 3.12 is not installed"
         exit 1
     fi
 
-    # If the virtual environment exists, make sure the Python 3.11 version matches
-    if [[ -d ${VENV_DIR} && "$(/usr/local/bin/python3.11 -V)" != "$(${VENV_DIR}/bin/python3 -V)" ]]; then
+    # If the virtual environment exists, make sure the Python 3.12 version matches
+    if [[ -d ${VENV_DIR} && "$(/usr/local/bin/python3.12 -V)" != "$(${VENV_DIR}/bin/python3 -V)" ]]; then
         echo Removing obsolete $(${VENV_DIR}/bin/python3 -V) virtual environment
         rm -rf ${VENV_DIR}
     fi
 fi
 
 
 # create virtual environment if it doesn't exist
 if [[ ! -d ${VENV_DIR} ]]; then
     # only implemented for MacOS
     if [[ "$(uname)" == "Darwin" ]]; then
-        /usr/local/bin/python3.11 -m venv ${VENV_DIR} --prompt "${PROJECT_NAME}-dev"
+        /usr/local/bin/python3.12 -m venv ${VENV_DIR} --prompt "${PROJECT_NAME}-dev"
         echo initialized virtual environment ${VENV_DIR}
     fi
 fi
 
 # activate virtual environment
 if [[ ! "$(which python)" -ef "${VENV_DIR}/bin/python3" ]]; then
     source ${VENV_DIR}/bin/activate
```

