# Comparing `tmp/aswt-0.0.10-py3-none-any.whl.zip` & `tmp/aswt-0.0.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11458 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat    15135 b- defN 20-Sep-06 18:45 aswt.py
--rw-rw-rw-  2.0 fat       82 b- defN 24-Feb-15 08:08 aswt/__init__.py
--rw-rw-rw-  2.0 fat     1946 b- defN 24-Feb-12 08:10 aswt/__main__.py
--rw-rw-rw-  2.0 fat     1481 b- defN 24-Feb-15 08:07 aswt/flask.py
--rw-rw-rw-  2.0 fat     4428 b- defN 24-Feb-15 08:21 aswt/require.py
--rw-rw-rw-  2.0 fat     1709 b- defN 24-Feb-15 08:14 aswt/starlette.py
--rw-rw-rw-  2.0 fat     9395 b- defN 24-Feb-17 13:49 aswt/token.py
--rw-rw-rw-  2.0 fat       91 b- defN 24-Feb-17 13:58 aswt-0.0.10.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-17 13:58 aswt-0.0.10.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Feb-17 13:58 aswt-0.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      782 b- defN 24-Feb-17 13:58 aswt-0.0.10.dist-info/RECORD
-11 files, 35146 bytes uncompressed, 10166 bytes compressed:  71.1%
+Zip file size: 8352 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       82 b- defN 24-Apr-20 11:28 aswt/__init__.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-Apr-20 11:28 aswt/__main__.py
+-rw-r--r--  2.0 unx     1437 b- defN 24-Apr-20 11:28 aswt/flask.py
+-rw-r--r--  2.0 unx     4334 b- defN 24-Apr-20 11:28 aswt/require.py
+-rw-r--r--  2.0 unx     1663 b- defN 24-Apr-20 11:28 aswt/starlette.py
+-rw-r--r--  2.0 unx     9136 b- defN 24-Apr-20 11:28 aswt/token.py
+-rw-rw-rw-  2.0 unx     1115 b- defN 24-Apr-20 11:28 aswt-0.0.11.dist-info/LICENSE
+-rw-r--r--  2.0 unx      108 b- defN 24-Apr-20 11:28 aswt-0.0.11.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-20 11:28 aswt-0.0.11.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-20 11:28 aswt-0.0.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 24-Apr-20 11:28 aswt-0.0.11.dist-info/RECORD
+11 files, 20725 bytes uncompressed, 7016 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: aswt.py
-Comment: 
-
 Filename: aswt/__init__.py
 Comment: 
 
 Filename: aswt/__main__.py
 Comment: 
 
 Filename: aswt/flask.py
@@ -15,20 +12,23 @@
 
 Filename: aswt/starlette.py
 Comment: 
 
 Filename: aswt/token.py
 Comment: 
 
-Filename: aswt-0.0.10.dist-info/METADATA
+Filename: aswt-0.0.11.dist-info/LICENSE
+Comment: 
+
+Filename: aswt-0.0.11.dist-info/METADATA
 Comment: 
 
-Filename: aswt-0.0.10.dist-info/WHEEL
+Filename: aswt-0.0.11.dist-info/WHEEL
 Comment: 
 
-Filename: aswt-0.0.10.dist-info/top_level.txt
+Filename: aswt-0.0.11.dist-info/top_level.txt
 Comment: 
 
-Filename: aswt-0.0.10.dist-info/RECORD
+Filename: aswt-0.0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aswt/__main__.py

```diff
@@ -1,59 +1,60 @@
-import json, os.path
-import logging
-import argparse, sys
-
-logger = logging.getLogger(__name__)
-
-print(repr(sys.argv))
-parser = argparse.ArgumentParser()
-parser.add_argument('--new-key',action="store_true")
-parser.add_argument('--new-token',action="store_true")
-parser.add_argument("--keyid",default=None)
-parser.add_argument('--verify-token',action="store_true")
-parser.add_argument('--claim',action="append")
-parser.add_argument('--age',type=int,default=None)
-parser.add_argument('config_file',nargs='?')
-args = parser.parse_args()
-
-if args.config_file and os.path.exists(args.config_file):
-    with open(args.config_file,"r") as fo:
-        rawconfig = fo.read()
-    config = json.loads(rawconfig)
-else:
-    config = {'keys':[]}
-    rawconfig = None
-dirty = False
-if args.new_key:
-    keydata = new_key(args.age)
-    # insert the new key at the beginning (so it becomes the default signing key)
-    config['keys'].insert(0,keydata)
-    dirty = True
-elif args.new_token:
-    if rawconfig is None:
-        raise ValueError("Missing config file with keys!")
-    load_config(rawconfig)
-    if GLOBAL_CONFIG['default_key'] is None:
-        raise ValueError("No signing key found!")
-    t = Token(key=args.keyid,age=args.age)
-    for claim in args.claim:
-        key,value = claim.split('=',1)
-        key = key.strip()
-        value = value.strip()
-        if value[0:1] in ['[','{']:
-            sys.stderr.write("converting %s to json\n"%(value))
-            value = json.loads(value)
-        t[key]=value
-    print(t.dumps())
-elif args.verify_token:
-    if rawconfig is None:
-        raise ValueError("Missing config file with keys!")
-    load_config(rawconfig)
-    TOKEN = sys.stdin.read()
-    t = Token.load(TOKEN)
-    print("valid!")
-
-if dirty:
-    print(json.dumps(config))
-    with open(args.config_file,"w") as fobj:
-        fobj.write(json.dumps(config))
-        fobj.write("\n")
+import json, os.path
+import logging
+import argparse, sys
+from .token import Token, new_key, load_config, GLOBAL_CONFIG
+
+logger = logging.getLogger(__name__)
+
+print(repr(sys.argv))
+parser = argparse.ArgumentParser()
+parser.add_argument('--new-key',action="store_true")
+parser.add_argument('--new-token',action="store_true")
+parser.add_argument("--keyid",default=None)
+parser.add_argument('--verify-token',action="store_true")
+parser.add_argument('--claim',action="append")
+parser.add_argument('--age',type=int,default=None)
+parser.add_argument('config_file',nargs='?')
+args = parser.parse_args()
+
+if args.config_file and os.path.exists(args.config_file):
+    with open(args.config_file,"r") as fo:
+        rawconfig = fo.read()
+    config = json.loads(rawconfig)
+else:
+    config = {'keys':[]}
+    rawconfig = None
+dirty = False
+if args.new_key:
+    keydata = new_key(args.age)
+    # insert the new key at the beginning (so it becomes the default signing key)
+    config['keys'].insert(0,keydata)
+    dirty = True
+elif args.new_token:
+    if rawconfig is None:
+        raise ValueError("Missing config file with keys!")
+    load_config(rawconfig)
+    if GLOBAL_CONFIG['default_key'] is None:
+        raise ValueError("No signing key found!")
+    t = Token(key=args.keyid,age=args.age)
+    for claim in args.claim:
+        key,value = claim.split('=',1)
+        key = key.strip()
+        value = value.strip()
+        if value[0:1] in ['[','{']:
+            sys.stderr.write("converting %s to json\n"%(value))
+            value = json.loads(value)
+        t[key]=value
+    print(t.dumps())
+elif args.verify_token:
+    if rawconfig is None:
+        raise ValueError("Missing config file with keys!")
+    load_config(rawconfig)
+    TOKEN = sys.stdin.read()
+    t = Token.load(TOKEN)
+    print("valid!")
+
+if dirty:
+    print(json.dumps(config))
+    with open(args.config_file,"w") as fobj:
+        fobj.write(json.dumps(config))
+        fobj.write("\n")
```

## aswt/flask.py

 * *Ordering differences only*

```diff
@@ -1,44 +1,44 @@
-import json, struct, os
-import logging
-from .token import Token, is_key_set
-from .require import require_aswt
-
-logger = logging.getLogger(__name__)
-
-import flask
-
-def FlaskCookie(name):
-    def get_cookie():
-        return flask.request.cookies.get(name)
-    return get_cookie
-
-def FlaskForm(name):
-    def get_value():
-        return flask.request.form.get(name)
-    return get_value
-
-def FlaskAuthorization():
-    def get_token():
-        authheader = flask.request.headers.get('Authorization')
-        if authheader is not None:
-            tokentype,tokenraw = authheader.split(' ')
-            if tokentype == "Bearer":
-                return tokenraw
-            elif tokentype == "Basic":
-                username, _, token = base64.b64decode(tokenraw).decode('ascii').partition(':')
-                # ignore the username
-                return token
-        return None
-    return get_token
-
-def FlaskUnauthorized():
-    return "Unauthorized", 403
-def FlaskMissingToken():
-    return "Missing Token",401
-def FlaskMissingClaim(claim):
-    return "Missing Claim %s"%(claim), 403
-
-def require(token_sources, required_claims=None, authz=None, pass_token=False, token_required=True):
-    return require_aswt(token_sources, required_claims=required_claims, authz=authz, pass_token=pass_token, token_required=token_required,
-            missing_claim=FlaskMissingClaim, missing_token=FlaskMissingToken, unauthorized=FlaskUnauthorized)
-
+import json, struct, os
+import logging
+from .token import Token, is_key_set
+from .require import require_aswt
+
+logger = logging.getLogger(__name__)
+
+import flask
+
+def FlaskCookie(name):
+    def get_cookie():
+        return flask.request.cookies.get(name)
+    return get_cookie
+
+def FlaskForm(name):
+    def get_value():
+        return flask.request.form.get(name)
+    return get_value
+
+def FlaskAuthorization():
+    def get_token():
+        authheader = flask.request.headers.get('Authorization')
+        if authheader is not None:
+            tokentype,tokenraw = authheader.split(' ')
+            if tokentype == "Bearer":
+                return tokenraw
+            elif tokentype == "Basic":
+                username, _, token = base64.b64decode(tokenraw).decode('ascii').partition(':')
+                # ignore the username
+                return token
+        return None
+    return get_token
+
+def FlaskUnauthorized():
+    return "Unauthorized", 403
+def FlaskMissingToken():
+    return "Missing Token",401
+def FlaskMissingClaim(claim):
+    return "Missing Claim %s"%(claim), 403
+
+def require(token_sources, required_claims=None, authz=None, pass_token=False, token_required=True):
+    return require_aswt(token_sources, required_claims=required_claims, authz=authz, pass_token=pass_token, token_required=token_required,
+            missing_claim=FlaskMissingClaim, missing_token=FlaskMissingToken, unauthorized=FlaskUnauthorized)
+
```

## aswt/require.py

 * *Ordering differences only*

```diff
@@ -1,94 +1,94 @@
-"""
-It's unfortunate that we have to have multiple critical paths. One for synchronous code
-and one for asynchronous code. They are side-by-side here so it's easier to visually
-inspect that they're both correct. If one needs a fix or change, make sure to do the same
-to the other.
-
-"""
-from .token import Token, is_key_set
-from functools import wraps
-import logging
-
-logger = logging.getLogger(__name__)
-
-def require_aswt(token_sources, required_claims=None, authz=None, pass_token=False, token_required=True,
-        missing_claim=None, missing_token=None, unauthorized=None):
-    def makewrapper(func):
-        @wraps(func)
-        def mywrapper(*args,**kwargs):
-            if not is_key_set(): raise Exception("default key isn't set!")
-            token = None
-            logger.debug("checking for valid token")
-            try:
-                tokenraw = None
-                for ts in token_sources:
-                    tokenraw = ts()
-                    if tokenraw is not None:
-                        token = Token.load(tokenraw)
-                        break
-            except (KeyError,ValueError):
-                logger.exception("error parsing token!")
-                token = None
-            if token is not None:
-                logger.info("request_aswt - valid token found with digest=%s", token.digest)
-                if required_claims is not None:
-                    for claim in required_claims:
-                        if claim not in token:
-                            logger.warning("request_aswt - missing claim %s on token with digest=%s", claim, token.digest)
-                            return missing_claim(claim)
-            elif token_required:
-                logger.info("request_aswt - no valid token found!")
-                return missing_token()
-
-            if authz is not None:
-                if not authz(token,**kwargs):
-                    logger.warning("request_aswt - failed authz for token with digest=%s", token.digest if token else "(no token)")
-                    return unauthorized()
-            if pass_token:
-                kwargs = kwargs.copy()
-                kwargs['token'] = token
-            logger.info("request_aswt - access allowed for token with digest=%s", token.digest if token else "(no token)")
-            return func(*args,**kwargs)
-
-        return mywrapper
-    return makewrapper
-
-def require_aswt_async(token_sources, required_claims=None, authz=None, pass_token=False, missing_claim=None, missing_token=None, unauthorized=None):
-    def makewrapper(func):
-        @wraps(func)
-        async def mywrapper(request,*args,**kwargs):
-            if not is_key_set(): raise Exception("default key isn't set!")
-            token = None
-            logger.debug("checking for valid token")
-            try:
-                tokenraw = None
-                for ts in token_sources:
-                    tokenraw = await ts(request)
-                    if tokenraw is not None:
-                        token = Token.load(tokenraw)
-                        break
-            except (KeyError,ValueError):
-                logger.exception("error parsing token!")
-                token = None
-            if token is None:
-                logger.info("request_aswt_async - no valid token found!")
-                return missing_token()
-            else:
-                logger.info("request_aswt_async - valid token found with digest=%s", token.digest)
-                if required_claims is not None:
-                    for claim in required_claims:
-                        if claim not in token:
-                            logger.warning("request_aswt_async - missing claim %s on token with digest=%s", claim, token.digest)
-                            return missing_claim(claim)
-                if authz is not None:
-                    if not authz(token,**kwargs):
-                        logger.warning("request_aswt_async - failed authz for token with digest=%s", token.digest)
-                        return unauthorized()
-                if pass_token:
-                    kwargs = kwargs.copy()
-                    kwargs['token'] = token
-                logger.info("request_aswt_async - access allowed for token with digest=%s", token.digest)
-                return await func(request,*args,**kwargs)
-        return mywrapper
-    return makewrapper
-
+"""
+It's unfortunate that we have to have multiple critical paths. One for synchronous code
+and one for asynchronous code. They are side-by-side here so it's easier to visually
+inspect that they're both correct. If one needs a fix or change, make sure to do the same
+to the other.
+
+"""
+from .token import Token, is_key_set
+from functools import wraps
+import logging
+
+logger = logging.getLogger(__name__)
+
+def require_aswt(token_sources, required_claims=None, authz=None, pass_token=False, token_required=True,
+        missing_claim=None, missing_token=None, unauthorized=None):
+    def makewrapper(func):
+        @wraps(func)
+        def mywrapper(*args,**kwargs):
+            if not is_key_set(): raise Exception("default key isn't set!")
+            token = None
+            logger.debug("checking for valid token")
+            try:
+                tokenraw = None
+                for ts in token_sources:
+                    tokenraw = ts()
+                    if tokenraw is not None:
+                        token = Token.load(tokenraw)
+                        break
+            except (KeyError,ValueError):
+                logger.exception("error parsing token!")
+                token = None
+            if token is not None:
+                logger.info("request_aswt - valid token found with digest=%s", token.digest)
+                if required_claims is not None:
+                    for claim in required_claims:
+                        if claim not in token:
+                            logger.warning("request_aswt - missing claim %s on token with digest=%s", claim, token.digest)
+                            return missing_claim(claim)
+            elif token_required:
+                logger.info("request_aswt - no valid token found!")
+                return missing_token()
+
+            if authz is not None:
+                if not authz(token,**kwargs):
+                    logger.warning("request_aswt - failed authz for token with digest=%s", token.digest if token else "(no token)")
+                    return unauthorized()
+            if pass_token:
+                kwargs = kwargs.copy()
+                kwargs['token'] = token
+            logger.info("request_aswt - access allowed for token with digest=%s", token.digest if token else "(no token)")
+            return func(*args,**kwargs)
+
+        return mywrapper
+    return makewrapper
+
+def require_aswt_async(token_sources, required_claims=None, authz=None, pass_token=False, missing_claim=None, missing_token=None, unauthorized=None):
+    def makewrapper(func):
+        @wraps(func)
+        async def mywrapper(request,*args,**kwargs):
+            if not is_key_set(): raise Exception("default key isn't set!")
+            token = None
+            logger.debug("checking for valid token")
+            try:
+                tokenraw = None
+                for ts in token_sources:
+                    tokenraw = await ts(request)
+                    if tokenraw is not None:
+                        token = Token.load(tokenraw)
+                        break
+            except (KeyError,ValueError):
+                logger.exception("error parsing token!")
+                token = None
+            if token is None:
+                logger.info("request_aswt_async - no valid token found!")
+                return missing_token()
+            else:
+                logger.info("request_aswt_async - valid token found with digest=%s", token.digest)
+                if required_claims is not None:
+                    for claim in required_claims:
+                        if claim not in token:
+                            logger.warning("request_aswt_async - missing claim %s on token with digest=%s", claim, token.digest)
+                            return missing_claim(claim)
+                if authz is not None:
+                    if not authz(token,**kwargs):
+                        logger.warning("request_aswt_async - failed authz for token with digest=%s", token.digest)
+                        return unauthorized()
+                if pass_token:
+                    kwargs = kwargs.copy()
+                    kwargs['token'] = token
+                logger.info("request_aswt_async - access allowed for token with digest=%s", token.digest)
+                return await func(request,*args,**kwargs)
+        return mywrapper
+    return makewrapper
+
```

## aswt/starlette.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-import json, struct, os
-import logging
-from .token import Token, is_key_set
-from .require import require_aswt_async
-
-logger = logging.getLogger(__name__)
-
-from functools import wraps
-
-import starlette.responses
-
-def StarletteCookie(name):
-    async def get_cookie(request):
-        return request.cookies.get(name)
-    return get_cookie
-
-def StartletteForm(name):
-    async def get_value():
-        f = await request.form()
-        return f.get(name)
-    return get_value
-
-def StarletteAuthorization():
-    async def get_token(request):
-        authheader = request.headers.get('Authorization')
-        if authheader is not None:
-            tokentype,tokenraw = authheader.split(' ')
-            if tokentype == "Bearer":
-                return tokenraw
-            elif tokentype == "Basic":
-                username, _, token = base64.b64decode(tokenraw).decode('ascii').partition(':')
-                # ignore the username
-                return token
-        return None
-    return get_token
-
-def StarletteUnauthorized():
-    return starlette.responses.Response("Unauthorized",status_code=403)
-def StarletteMissingToken():
-    return starlette.responses.Response("Missing Token",status_code=401, headers={"WWW-Authenticate":"Basic"})
-def StarletteMissingClaim(claim):
-    return starlette.responses.Response("Missing Claim %s"%(claim),status_code=403)
-
-def require(token_sources, required_claims=None, authz=None, pass_token=False):
-    return require_aswt_async(token_sources, required_claims=required_claims, authz=authz, pass_token=pass_token, missing_claim=StarletteMissingClaim, missing_token=StarletteMissingToken, unauthorized=StarletteUnauthorized)
-
+import json, struct, os
+import logging
+from .token import Token, is_key_set
+from .require import require_aswt_async
+
+logger = logging.getLogger(__name__)
+
+from functools import wraps
+
+import starlette.responses
+
+def StarletteCookie(name):
+    async def get_cookie(request):
+        return request.cookies.get(name)
+    return get_cookie
+
+def StartletteForm(name):
+    async def get_value():
+        f = await request.form()
+        return f.get(name)
+    return get_value
+
+def StarletteAuthorization():
+    async def get_token(request):
+        authheader = request.headers.get('Authorization')
+        if authheader is not None:
+            tokentype,tokenraw = authheader.split(' ')
+            if tokentype == "Bearer":
+                return tokenraw
+            elif tokentype == "Basic":
+                username, _, token = base64.b64decode(tokenraw).decode('ascii').partition(':')
+                # ignore the username
+                return token
+        return None
+    return get_token
+
+def StarletteUnauthorized():
+    return starlette.responses.Response("Unauthorized",status_code=403)
+def StarletteMissingToken():
+    return starlette.responses.Response("Missing Token",status_code=401, headers={"WWW-Authenticate":"Basic"})
+def StarletteMissingClaim(claim):
+    return starlette.responses.Response("Missing Claim %s"%(claim),status_code=403)
+
+def require(token_sources, required_claims=None, authz=None, pass_token=False):
+    return require_aswt_async(token_sources, required_claims=required_claims, authz=authz, pass_token=pass_token, missing_claim=StarletteMissingClaim, missing_token=StarletteMissingToken, unauthorized=StarletteUnauthorized)
+
```

## aswt/token.py

 * *Ordering differences only*

```diff
@@ -1,259 +1,259 @@
-import json, struct, os
-import base64
-import binascii
-import time
-import logging
-from Crypto import Random
-from Crypto.Cipher import AES
-from Crypto.Hash import SHA256, HMAC
-
-logger = logging.getLogger(__name__)
-
-# Default age of a signed token
-DEFAULT_AGE=3600  # 1 hour
-
-# give 60 seconds of grace on expiration/not-before times
-DEFAULT_GRACE=60
-
-GLOBAL_CONFIG = None
-
-class HMACKey(object):
-    digestmod = SHA256
-    header = b"HS"
-    def __init__(self, key, keyid, default_age=None):
-        if isinstance(key,str): key = key.encode('utf-8')
-        self.key = key
-        self.id = keyid
-        self.default_age = default_age
-
-    def verify(self, mac, content):
-        if len(mac) != (self.digestmod.digest_size*2):
-            raise ValueError("digest not right length")
-
-        h = HMAC.new(self.key, digestmod=self.digestmod)
-        h.update(content)
-
-        try:
-            h.hexverify(mac) # this throws an error if the signature is wrong
-        except:
-            logger.exception("verify error on keyid %s mac %s",self.id,mac)
-            raise
-
-    def sign(self, content):
-        h = HMAC.new(self.key, digestmod=self.digestmod)
-        h.update(content)
-        return h.hexdigest()
-
-        
-class Token(object):
-    MAX_STRING = 1024
-    def __init__(self, tokenstring=None, key=None, age=None, notnew=False, grace=DEFAULT_GRACE):
-        global GLOBAL_CONFIG
-        self._dict = {}
-        self.dirty = False
-        self.digest = None
-
-        if isinstance(key,HMACKey):
-            self.key = key
-        elif key is not None:
-            self.key = GLOBAL_CONFIG['keys'][key]
-        elif GLOBAL_CONFIG['default_key'] is not None:
-            self.key = GLOBAL_CONFIG['default_key']
-        else:
-            self.key = None
-
-        if tokenstring is not None:
-            if len(tokenstring)>self.MAX_STRING:
-                raise ValueError("token too long!")
-            self._load(tokenstring,key,grace=grace)
-        elif not notnew:
-            # initialize a new token
-            now = int(time.time())
-            if age is None:
-                if self.key is not None and self.key.default_age is not None:
-                    age = self.key.default_age
-                else:
-                    age = DEFAULT_AGE
-            if age is not None and age!=0: # age of 0 means unlimited
-                self['exp'] = now+age
-            self['nbf'] = now
-        else:
-            raise ValueError("token not passed! can't be None")
-
-    @classmethod
-    def load(cls, tokenstring, key=None, grace=DEFAULT_GRACE):
-        """
-        Load an existing token and validate (fail if the token is not valid)
-        """
-        return cls(tokenstring,key=key,notnew=True,grace=grace)
-
-    def _load(self, tokenstring, key=None, grace=DEFAULT_GRACE):
-        global GLOBAL_CONFIG
-        if isinstance(tokenstring,str): tokenstring = tokenstring.encode('utf-8')
-        header, keyid, digest, jsoncontent = tokenstring.split(b'.')
-        while jsoncontent[-1] in b"\n \r\t":
-            jsoncontent = jsoncontent[:-1]
-        
-        if header != b"HS":
-            raise ValueError("incorrect header")
-        
-        keyid = keyid.decode('utf-8')
-
-        if key is not None:
-            # a key was specified! make sure it matches what key is in the token
-            if isinstance(key,HMACKey):
-                if key.id!=keyid:
-                    raise KeyError("key mismatch", key.id, keyid)
-                self.key = key
-            elif isinstance(key,str):
-                if key != keyid:
-                    raise KeyError("key mismatch", key, keyid)
-                if key not in GLOBAL_CONFIG['keys']:
-                    raise KeyError("can't find keyid in keys!",keyid)
-                self.key = GLOBAL_CONFIG['keys'][keyid]
-
-        else: # key is None
-            key = self.key
-            if key.id != keyid: # no key was specified so we can lookup the key if it's in our config
-                if keyid not in GLOBAL_CONFIG['keys']:
-                    raise KeyError("can't find keyid in keys!",keyid)
-                self.key = GLOBAL_CONFIG['keys'][keyid]
-
-        assert self.key is not None
-        self.key.verify(digest, jsoncontent)
-        self.digest = digest.decode('utf-8')
-
-        self._dict = json.loads(base64.b64decode(jsoncontent).decode('utf-8'))
-
-        # now enforce any time limits in the token        
-        if 'exp' not in self or 'nbf' not in self:
-            logger.warning("token missing exp and nbf claims - digest=%s",self.digest)
-            raise ValueError("must have an expiration and not before set in token")
-        now = time.time()
-        # give (by default) 60 seconds grace
-        if (self['nbf']-grace) > now:
-            logger.warning("token not yet valid digest=%s nbf=%d",self.digest,self['nbf'])
-            raise ValueError("token not yet valid!")
-        if (self['exp']+grace) < now:
-            logger.warning("token expired digest=%s exp=%d",self.digest,self['exp'])
-            raise ValueError("token expired!")
-
-    def dump(self, key=None):
-        """
-        Sign Token and return as bytes
-        """
-        if key is None:
-            key = self.key
-        if key is None:
-            raise ValueError("no key specified and no default key setup! Set ASWT_CONFIG environment variable")
-
-        # encode our token
-        # use of separators generates more compact JSON
-        data = json.dumps(self._dict,separators=(',',':')).encode('utf-8')
-        data = base64.b64encode(data)
-
-        # now sign it
-        hashfordata = key.sign(data)
-        self.digest = hashfordata
-
-        if '.' in key.id:
-            raise ValueError("Key id can't contain a period!",key.id)
-
-        #logger.debug("dumps - hashfordata = %s",h.hexdigest())
-        data = b'HS.'+(key.id.encode('utf-8'))+b'.'+hashfordata.encode('utf-8')+b'.'+data
-
-        return data
-
-    def dumps(self,key=None):
-        """
-        Sign Token and return as str
-        """
-        return self.dump(key).decode('utf-8')
-
-    def __setitem__(self, name, value):
-        # FIXME: we can't go dirty on changes in child objects because only
-        # __getitem__ is called in those cases... :(
-        if name in self._dict:
-            oldvalue = self._dict[name]
-            self._dict[name] = value
-            # only mark dirty if we changed the value
-            if value != oldvalue: self.dirty = True
-        else:
-            # it's a new value, we are dirty
-            self.dirty = True
-            self._dict[name] = value
-
-    def __delitem__(self, name):
-        del self._dict[name]
-        self.dirty = True
-
-    def __getitem__(self, name):
-        return self._dict[name]
-
-    def __contains__(self,name):
-        return name in self._dict
-
-    def items(self):
-        return self._dict.items()
-
-    def get(self, name, default=None):
-        if name in self._dict: return self._dict[name]
-        else: return default
-
-def new_key(age=None):
-    r = Random.new()
-    key = r.read(SHA256.digest_size)
-    keyid = binascii.hexlify(r.read(4)).decode('utf-8')
-    keydata = {'key':binascii.hexlify(key).decode('utf-8'),'keyid':keyid}
-    if age is not None:
-        keydata['age'] = age
-    return keydata
-
-# FINISHME
-# 1. pull config/key location from environment
-# 2. if gsutil URL, then go to google cloud storage for the file
-# 3. Load keys into an array (or dict by keyid?) and automatically use with the wrappers above
-def download_gcs_to_string(bucket,filename):
-    global GOOGLE_CLOUD_STORAGE_CLIENT
-    import google.cloud.storage
-    GOOGLE_CLOUD_STORAGE_CLIENT = google.cloud.storage.Client()
-    return GOOGLE_CLOUD_STORAGE_CLIENT.bucket(bucket).blob(filename).download_as_string()
-
-def load_config(config=None):
-    global GLOBAL_CONFIG
-    GLOBAL_CONFIG = {'keys':{},'default_key':None}
-    if config is not None:
-        config = json.loads(config)
-
-        keys = [HMACKey(key=binascii.unhexlify(keyconfig['key']), keyid=keyconfig['keyid'], default_age=(keyconfig['age'] if 'age' in keyconfig else None)) for keyconfig in config['keys']]
-        for key in keys:
-            GLOBAL_CONFIG['keys'][key.id] = key
-        
-        # choose a default key
-        if 'default_key' in config and config['default_key'] in GLOBAL_CONFIG['keys']:
-            GLOBAL_CONFIG['default_key'] = GLOBAL_CONFIG['keys'][config['default_key']]
-        elif len(keys):
-            GLOBAL_CONFIG['default_key'] = keys[0]
-
-def get_config(configpath):
-    if configpath is not None:
-        if configpath.startswith("{"):
-            # it's JSON, try to consume as config
-            return configpath
-        if configpath.startswith('gs://'):
-            bucket, blob = configpath[5:].split('/',1)
-            config = download_gcs_to_string(bucket,blob)
-        else:
-            with open(configpath,"r") as fo:
-                config = fo.read()
-        return config
-    else:
-        return None
-
-def is_key_set():
-    global GLOBAL_CONFIG
-    return GLOBAL_CONFIG['default_key'] is not None
-
-def reload_config():
-    load_config(get_config(os.environ['ASWT_CONFIG'] if 'ASWT_CONFIG' in os.environ else None))
-reload_config()
+import json, struct, os
+import base64
+import binascii
+import time
+import logging
+from Crypto import Random
+from Crypto.Cipher import AES
+from Crypto.Hash import SHA256, HMAC
+
+logger = logging.getLogger(__name__)
+
+# Default age of a signed token
+DEFAULT_AGE=3600  # 1 hour
+
+# give 60 seconds of grace on expiration/not-before times
+DEFAULT_GRACE=60
+
+GLOBAL_CONFIG = None
+
+class HMACKey(object):
+    digestmod = SHA256
+    header = b"HS"
+    def __init__(self, key, keyid, default_age=None):
+        if isinstance(key,str): key = key.encode('utf-8')
+        self.key = key
+        self.id = keyid
+        self.default_age = default_age
+
+    def verify(self, mac, content):
+        if len(mac) != (self.digestmod.digest_size*2):
+            raise ValueError("digest not right length")
+
+        h = HMAC.new(self.key, digestmod=self.digestmod)
+        h.update(content)
+
+        try:
+            h.hexverify(mac) # this throws an error if the signature is wrong
+        except:
+            logger.exception("verify error on keyid %s mac %s",self.id,mac)
+            raise
+
+    def sign(self, content):
+        h = HMAC.new(self.key, digestmod=self.digestmod)
+        h.update(content)
+        return h.hexdigest()
+
+        
+class Token(object):
+    MAX_STRING = 1024
+    def __init__(self, tokenstring=None, key=None, age=None, notnew=False, grace=DEFAULT_GRACE):
+        global GLOBAL_CONFIG
+        self._dict = {}
+        self.dirty = False
+        self.digest = None
+
+        if isinstance(key,HMACKey):
+            self.key = key
+        elif key is not None:
+            self.key = GLOBAL_CONFIG['keys'][key]
+        elif GLOBAL_CONFIG['default_key'] is not None:
+            self.key = GLOBAL_CONFIG['default_key']
+        else:
+            self.key = None
+
+        if tokenstring is not None:
+            if len(tokenstring)>self.MAX_STRING:
+                raise ValueError("token too long!")
+            self._load(tokenstring,key,grace=grace)
+        elif not notnew:
+            # initialize a new token
+            now = int(time.time())
+            if age is None:
+                if self.key is not None and self.key.default_age is not None:
+                    age = self.key.default_age
+                else:
+                    age = DEFAULT_AGE
+            if age is not None and age!=0: # age of 0 means unlimited
+                self['exp'] = now+age
+            self['nbf'] = now
+        else:
+            raise ValueError("token not passed! can't be None")
+
+    @classmethod
+    def load(cls, tokenstring, key=None, grace=DEFAULT_GRACE):
+        """
+        Load an existing token and validate (fail if the token is not valid)
+        """
+        return cls(tokenstring,key=key,notnew=True,grace=grace)
+
+    def _load(self, tokenstring, key=None, grace=DEFAULT_GRACE):
+        global GLOBAL_CONFIG
+        if isinstance(tokenstring,str): tokenstring = tokenstring.encode('utf-8')
+        header, keyid, digest, jsoncontent = tokenstring.split(b'.')
+        while jsoncontent[-1] in b"\n \r\t":
+            jsoncontent = jsoncontent[:-1]
+        
+        if header != b"HS":
+            raise ValueError("incorrect header")
+        
+        keyid = keyid.decode('utf-8')
+
+        if key is not None:
+            # a key was specified! make sure it matches what key is in the token
+            if isinstance(key,HMACKey):
+                if key.id!=keyid:
+                    raise KeyError("key mismatch", key.id, keyid)
+                self.key = key
+            elif isinstance(key,str):
+                if key != keyid:
+                    raise KeyError("key mismatch", key, keyid)
+                if key not in GLOBAL_CONFIG['keys']:
+                    raise KeyError("can't find keyid in keys!",keyid)
+                self.key = GLOBAL_CONFIG['keys'][keyid]
+
+        else: # key is None
+            key = self.key
+            if key.id != keyid: # no key was specified so we can lookup the key if it's in our config
+                if keyid not in GLOBAL_CONFIG['keys']:
+                    raise KeyError("can't find keyid in keys!",keyid)
+                self.key = GLOBAL_CONFIG['keys'][keyid]
+
+        assert self.key is not None
+        self.key.verify(digest, jsoncontent)
+        self.digest = digest.decode('utf-8')
+
+        self._dict = json.loads(base64.b64decode(jsoncontent).decode('utf-8'))
+
+        # now enforce any time limits in the token        
+        if 'exp' not in self or 'nbf' not in self:
+            logger.warning("token missing exp and nbf claims - digest=%s",self.digest)
+            raise ValueError("must have an expiration and not before set in token")
+        now = time.time()
+        # give (by default) 60 seconds grace
+        if (self['nbf']-grace) > now:
+            logger.warning("token not yet valid digest=%s nbf=%d",self.digest,self['nbf'])
+            raise ValueError("token not yet valid!")
+        if (self['exp']+grace) < now:
+            logger.warning("token expired digest=%s exp=%d",self.digest,self['exp'])
+            raise ValueError("token expired!")
+
+    def dump(self, key=None):
+        """
+        Sign Token and return as bytes
+        """
+        if key is None:
+            key = self.key
+        if key is None:
+            raise ValueError("no key specified and no default key setup! Set ASWT_CONFIG environment variable")
+
+        # encode our token
+        # use of separators generates more compact JSON
+        data = json.dumps(self._dict,separators=(',',':')).encode('utf-8')
+        data = base64.b64encode(data)
+
+        # now sign it
+        hashfordata = key.sign(data)
+        self.digest = hashfordata
+
+        if '.' in key.id:
+            raise ValueError("Key id can't contain a period!",key.id)
+
+        #logger.debug("dumps - hashfordata = %s",h.hexdigest())
+        data = b'HS.'+(key.id.encode('utf-8'))+b'.'+hashfordata.encode('utf-8')+b'.'+data
+
+        return data
+
+    def dumps(self,key=None):
+        """
+        Sign Token and return as str
+        """
+        return self.dump(key).decode('utf-8')
+
+    def __setitem__(self, name, value):
+        # FIXME: we can't go dirty on changes in child objects because only
+        # __getitem__ is called in those cases... :(
+        if name in self._dict:
+            oldvalue = self._dict[name]
+            self._dict[name] = value
+            # only mark dirty if we changed the value
+            if value != oldvalue: self.dirty = True
+        else:
+            # it's a new value, we are dirty
+            self.dirty = True
+            self._dict[name] = value
+
+    def __delitem__(self, name):
+        del self._dict[name]
+        self.dirty = True
+
+    def __getitem__(self, name):
+        return self._dict[name]
+
+    def __contains__(self,name):
+        return name in self._dict
+
+    def items(self):
+        return self._dict.items()
+
+    def get(self, name, default=None):
+        if name in self._dict: return self._dict[name]
+        else: return default
+
+def new_key(age=None):
+    r = Random.new()
+    key = r.read(SHA256.digest_size)
+    keyid = binascii.hexlify(r.read(4)).decode('utf-8')
+    keydata = {'key':binascii.hexlify(key).decode('utf-8'),'keyid':keyid}
+    if age is not None:
+        keydata['age'] = age
+    return keydata
+
+# FINISHME
+# 1. pull config/key location from environment
+# 2. if gsutil URL, then go to google cloud storage for the file
+# 3. Load keys into an array (or dict by keyid?) and automatically use with the wrappers above
+def download_gcs_to_string(bucket,filename):
+    global GOOGLE_CLOUD_STORAGE_CLIENT
+    import google.cloud.storage
+    GOOGLE_CLOUD_STORAGE_CLIENT = google.cloud.storage.Client()
+    return GOOGLE_CLOUD_STORAGE_CLIENT.bucket(bucket).blob(filename).download_as_string()
+
+def load_config(config=None):
+    global GLOBAL_CONFIG
+    GLOBAL_CONFIG = {'keys':{},'default_key':None}
+    if config is not None:
+        config = json.loads(config)
+
+        keys = [HMACKey(key=binascii.unhexlify(keyconfig['key']), keyid=keyconfig['keyid'], default_age=(keyconfig['age'] if 'age' in keyconfig else None)) for keyconfig in config['keys']]
+        for key in keys:
+            GLOBAL_CONFIG['keys'][key.id] = key
+        
+        # choose a default key
+        if 'default_key' in config and config['default_key'] in GLOBAL_CONFIG['keys']:
+            GLOBAL_CONFIG['default_key'] = GLOBAL_CONFIG['keys'][config['default_key']]
+        elif len(keys):
+            GLOBAL_CONFIG['default_key'] = keys[0]
+
+def get_config(configpath):
+    if configpath is not None:
+        if configpath.startswith("{"):
+            # it's JSON, try to consume as config
+            return configpath
+        if configpath.startswith('gs://'):
+            bucket, blob = configpath[5:].split('/',1)
+            config = download_gcs_to_string(bucket,blob)
+        else:
+            with open(configpath,"r") as fo:
+                config = fo.read()
+        return config
+    else:
+        return None
+
+def is_key_set():
+    global GLOBAL_CONFIG
+    return GLOBAL_CONFIG['default_key'] is not None
+
+def reload_config():
+    load_config(get_config(os.environ['ASWT_CONFIG'] if 'ASWT_CONFIG' in os.environ else None))
+reload_config()
```

## Comparing `aswt-0.0.10.dist-info/RECORD` & `aswt-0.0.11.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-aswt.py,sha256=2Shvb6rYFpUSbXL6dxRohgLjNJbSQLrwm4njuufobPM,15135
 aswt/__init__.py,sha256=A8DWSk3VSs_M8gPN8875uu_ZOX89dIVaiHAExGxQCIA,82
-aswt/__main__.py,sha256=tSzxISi1u0qYVjaPYzMJfyRZ_jF_q-it0BIav7udQ40,1946
-aswt/flask.py,sha256=2ZKQgXF_aBebdCz62-ufdy7iuil6eTLbXH4bKO-UFQA,1481
-aswt/require.py,sha256=Wvj-cXTOIBl3G1TGJb3vMXVnL7yMME_Kzrw9OiDaznM,4428
-aswt/starlette.py,sha256=nqOSGC-T8eqKR4Zz1zltJBxmHA4pjQHhon_6f2MgLds,1709
-aswt/token.py,sha256=DxbkFx5gp5r-4ldmFeQOObHU8RsGyi3bYbkvbUJdWUE,9395
-aswt-0.0.10.dist-info/METADATA,sha256=cW09NwKj69Dx2afPFibjo4NOwq5OQaY3sP9IGLtFvHg,91
-aswt-0.0.10.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-aswt-0.0.10.dist-info/top_level.txt,sha256=jF9JEf-5K7yjVjPtv-l82iaOBjX7i857JFcEtc8Kicc,5
-aswt-0.0.10.dist-info/RECORD,,
+aswt/__main__.py,sha256=bprVHlwVjsel9Ry-bUDKgum_0SdM-FEksnlCM3nilVY,1949
+aswt/flask.py,sha256=dRnaai-rUy_-3J2vqpaFisjvOVjrljV5RG7uz61JEwM,1437
+aswt/require.py,sha256=kDWgaVnjkxSGGResV1adBZdyYnhyxkLiHUVztQyBYvY,4334
+aswt/starlette.py,sha256=d2z2pMJ3sVesHZBpSXlKXe4-dVPn9OhnhFe86g_0fHo,1663
+aswt/token.py,sha256=_SVBmdO0MkZM5KNJT0Zbu9icwmoB5ykMaFT1CswA_Sg,9136
+aswt-0.0.11.dist-info/LICENSE,sha256=py-UogKT4vpm7osGOdAZ5KWbghi1FPvoCD2rIgOC3OI,1115
+aswt-0.0.11.dist-info/METADATA,sha256=nKy0Lr5yihw5sbCA6RG90FSdrppngR3Qod-sD241XXQ,108
+aswt-0.0.11.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+aswt-0.0.11.dist-info/top_level.txt,sha256=jF9JEf-5K7yjVjPtv-l82iaOBjX7i857JFcEtc8Kicc,5
+aswt-0.0.11.dist-info/RECORD,,
```

