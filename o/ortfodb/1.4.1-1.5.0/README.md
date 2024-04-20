# Comparing `tmp/ortfodb-1.4.1.tar.gz` & `tmp/ortfodb-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortfodb-1.4.1.tar", max compression
+gzip compressed data, was "ortfodb-1.5.0.tar", max compression
```

## Comparing `ortfodb-1.4.1.tar` & `ortfodb-1.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.4.1/README.md
--rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-1.4.1/ortfodb/__init__.py
--rw-r--r--   0        0        0     8179 2024-04-17 19:07:55.304880 ortfodb-1.4.1/ortfodb/configuration.py
--rw-r--r--   0        0        0    15476 2024-04-17 19:07:56.168247 ortfodb-1.4.1/ortfodb/database.py
--rw-r--r--   0        0        0     5270 2024-04-17 19:07:56.994944 ortfodb-1.4.1/ortfodb/exporter.py
--rw-r--r--   0        0        0     2791 2024-04-17 19:07:57.858311 ortfodb-1.4.1/ortfodb/tags.py
--rw-r--r--   0        0        0     2750 2024-04-17 19:07:58.668341 ortfodb-1.4.1/ortfodb/technologies.py
--rw-r--r--   0        0        0      301 2024-04-17 19:08:00.361739 ortfodb-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.5.0/README.md
+-rw-r--r--   0        0        0      917 2024-04-18 20:03:07.941753 ortfodb-1.5.0/ortfodb/__init__.py
+-rw-r--r--   0        0        0     9744 2024-04-20 11:25:50.063488 ortfodb-1.5.0/ortfodb/configuration.py
+-rw-r--r--   0        0        0    15626 2024-04-20 11:25:50.943522 ortfodb-1.5.0/ortfodb/database.py
+-rw-r--r--   0        0        0     5285 2024-04-20 11:25:51.776888 ortfodb-1.5.0/ortfodb/exporter.py
+-rw-r--r--   0        0        0     4485 2024-04-20 11:25:52.596919 ortfodb-1.5.0/ortfodb/tags.py
+-rw-r--r--   0        0        0     4389 2024-04-20 11:25:53.416951 ortfodb-1.5.0/ortfodb/technologies.py
+-rw-r--r--   0        0        0      301 2024-04-20 11:25:55.053680 ortfodb-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.5.0/PKG-INFO
```

### Comparing `ortfodb-1.4.1/ortfodb/database.py` & `ortfodb-1.5.0/ortfodb/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def from_int(x: Any) -> int:
     assert isinstance(x, int) and not isinstance(x, bool)
     return x
 
 
 def to_float(x: Any) -> float:
-    assert isinstance(x, float)
+    assert isinstance(x, (int, float))
     return x
 
 
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
@@ -40,15 +40,15 @@
 
 
 def from_dict(f: Callable[[Any], T], x: Any) -> Dict[str, T]:
     assert isinstance(x, dict)
     return { k: f(v) for (k, v) in x.items() }
 
 
-class Attributes:
+class MediaAttributes:
     """MediaAttributes stores which HTML attributes should be added to the media."""
 
     autoplay: bool
     """Controlled with attribute character > (adds)"""
 
     controls: bool
     """Controlled with attribute character = (removes)"""
@@ -66,62 +66,62 @@
         self.autoplay = autoplay
         self.controls = controls
         self.loop = loop
         self.muted = muted
         self.playsinline = playsinline
 
     @staticmethod
-    def from_dict(obj: Any) -> 'Attributes':
+    def from_dict(obj: Any) -> 'MediaAttributes':
         assert isinstance(obj, dict)
         autoplay = from_bool(obj.get("autoplay"))
         controls = from_bool(obj.get("controls"))
         loop = from_bool(obj.get("loop"))
         muted = from_bool(obj.get("muted"))
         playsinline = from_bool(obj.get("playsinline"))
-        return Attributes(autoplay, controls, loop, muted, playsinline)
+        return MediaAttributes(autoplay, controls, loop, muted, playsinline)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["autoplay"] = from_bool(self.autoplay)
         result["controls"] = from_bool(self.controls)
         result["loop"] = from_bool(self.loop)
         result["muted"] = from_bool(self.muted)
         result["playsinline"] = from_bool(self.playsinline)
         return result
 
 
-class Colors:
+class ColorPalette:
     """ColorPalette reprensents the object in a Work's metadata.colors."""
 
     primary: str
     secondary: str
     tertiary: str
 
     def __init__(self, primary: str, secondary: str, tertiary: str) -> None:
         self.primary = primary
         self.secondary = secondary
         self.tertiary = tertiary
 
     @staticmethod
-    def from_dict(obj: Any) -> 'Colors':
+    def from_dict(obj: Any) -> 'ColorPalette':
         assert isinstance(obj, dict)
         primary = from_str(obj.get("primary"))
         secondary = from_str(obj.get("secondary"))
         tertiary = from_str(obj.get("tertiary"))
-        return Colors(primary, secondary, tertiary)
+        return ColorPalette(primary, secondary, tertiary)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["primary"] = from_str(self.primary)
         result["secondary"] = from_str(self.secondary)
         result["tertiary"] = from_str(self.tertiary)
         return result
 
 
-class Dimensions:
+class ImageDimensions:
     """ImageDimensions represents metadata about a media as it's extracted from its file."""
 
     aspect_ratio: float
     """width / height"""
 
     height: int
     """Height in pixels"""
@@ -131,79 +131,79 @@
 
     def __init__(self, aspect_ratio: float, height: int, width: int) -> None:
         self.aspect_ratio = aspect_ratio
         self.height = height
         self.width = width
 
     @staticmethod
-    def from_dict(obj: Any) -> 'Dimensions':
+    def from_dict(obj: Any) -> 'ImageDimensions':
         assert isinstance(obj, dict)
         aspect_ratio = from_float(obj.get("aspectRatio"))
         height = from_int(obj.get("height"))
         width = from_int(obj.get("width"))
-        return Dimensions(aspect_ratio, height, width)
+        return ImageDimensions(aspect_ratio, height, width)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["aspectRatio"] = to_float(self.aspect_ratio)
         result["height"] = from_int(self.height)
         result["width"] = from_int(self.width)
         return result
 
 
-class Thumbnails:
+class ThumbnailsMap:
     pass
 
     def __init__(self, ) -> None:
         pass
 
     @staticmethod
-    def from_dict(obj: Any) -> 'Thumbnails':
+    def from_dict(obj: Any) -> 'ThumbnailsMap':
         assert isinstance(obj, dict)
-        return Thumbnails()
+        return ThumbnailsMap()
 
     def to_dict(self) -> dict:
         result: dict = {}
         return result
 
 
-class BlockElement:
+class ContentBlock:
     alt: str
     analyzed: bool
     """whether the media has been analyzed"""
 
     anchor: str
-    attributes: Attributes
+    attributes: MediaAttributes
     caption: str
-    colors: Colors
+    colors: ColorPalette
     content: str
     """html"""
 
     content_type: str
-    dimensions: Dimensions
+    dimensions: ImageDimensions
     dist_source: str
     duration: float
     """in seconds"""
 
     has_sound: bool
     id: str
     index: int
     online: bool
     relative_source: str
     size: int
     """in bytes"""
 
     text: str
-    thumbnails: Thumbnails
+    thumbnails: ThumbnailsMap
     thumbnails_built_at: str
     title: str
     type: str
     url: str
 
-    def __init__(self, alt: str, analyzed: bool, anchor: str, attributes: Attributes, caption: str, colors: Colors, content: str, content_type: str, dimensions: Dimensions, dist_source: str, duration: float, has_sound: bool, id: str, index: int, online: bool, relative_source: str, size: int, text: str, thumbnails: Thumbnails, thumbnails_built_at: str, title: str, type: str, url: str) -> None:
+    def __init__(self, alt: str, analyzed: bool, anchor: str, attributes: MediaAttributes, caption: str, colors: ColorPalette, content: str, content_type: str, dimensions: ImageDimensions, dist_source: str, duration: float, has_sound: bool, id: str, index: int, online: bool, relative_source: str, size: int, text: str, thumbnails: ThumbnailsMap, thumbnails_built_at: str, title: str, type: str, url: str) -> None:
         self.alt = alt
         self.analyzed = analyzed
         self.anchor = anchor
         self.attributes = attributes
         self.caption = caption
         self.colors = colors
         self.content = content
@@ -221,134 +221,134 @@
         self.thumbnails = thumbnails
         self.thumbnails_built_at = thumbnails_built_at
         self.title = title
         self.type = type
         self.url = url
 
     @staticmethod
-    def from_dict(obj: Any) -> 'BlockElement':
+    def from_dict(obj: Any) -> 'ContentBlock':
         assert isinstance(obj, dict)
         alt = from_str(obj.get("alt"))
         analyzed = from_bool(obj.get("analyzed"))
         anchor = from_str(obj.get("anchor"))
-        attributes = Attributes.from_dict(obj.get("attributes"))
+        attributes = MediaAttributes.from_dict(obj.get("attributes"))
         caption = from_str(obj.get("caption"))
-        colors = Colors.from_dict(obj.get("colors"))
+        colors = ColorPalette.from_dict(obj.get("colors"))
         content = from_str(obj.get("content"))
         content_type = from_str(obj.get("contentType"))
-        dimensions = Dimensions.from_dict(obj.get("dimensions"))
+        dimensions = ImageDimensions.from_dict(obj.get("dimensions"))
         dist_source = from_str(obj.get("distSource"))
         duration = from_float(obj.get("duration"))
         has_sound = from_bool(obj.get("hasSound"))
         id = from_str(obj.get("id"))
         index = from_int(obj.get("index"))
         online = from_bool(obj.get("online"))
         relative_source = from_str(obj.get("relativeSource"))
         size = from_int(obj.get("size"))
         text = from_str(obj.get("text"))
-        thumbnails = Thumbnails.from_dict(obj.get("thumbnails"))
+        thumbnails = ThumbnailsMap.from_dict(obj.get("thumbnails"))
         thumbnails_built_at = from_str(obj.get("thumbnailsBuiltAt"))
         title = from_str(obj.get("title"))
         type = from_str(obj.get("type"))
         url = from_str(obj.get("url"))
-        return BlockElement(alt, analyzed, anchor, attributes, caption, colors, content, content_type, dimensions, dist_source, duration, has_sound, id, index, online, relative_source, size, text, thumbnails, thumbnails_built_at, title, type, url)
+        return ContentBlock(alt, analyzed, anchor, attributes, caption, colors, content, content_type, dimensions, dist_source, duration, has_sound, id, index, online, relative_source, size, text, thumbnails, thumbnails_built_at, title, type, url)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["alt"] = from_str(self.alt)
         result["analyzed"] = from_bool(self.analyzed)
         result["anchor"] = from_str(self.anchor)
-        result["attributes"] = to_class(Attributes, self.attributes)
+        result["attributes"] = to_class(MediaAttributes, self.attributes)
         result["caption"] = from_str(self.caption)
-        result["colors"] = to_class(Colors, self.colors)
+        result["colors"] = to_class(ColorPalette, self.colors)
         result["content"] = from_str(self.content)
         result["contentType"] = from_str(self.content_type)
-        result["dimensions"] = to_class(Dimensions, self.dimensions)
+        result["dimensions"] = to_class(ImageDimensions, self.dimensions)
         result["distSource"] = from_str(self.dist_source)
         result["duration"] = to_float(self.duration)
         result["hasSound"] = from_bool(self.has_sound)
         result["id"] = from_str(self.id)
         result["index"] = from_int(self.index)
         result["online"] = from_bool(self.online)
         result["relativeSource"] = from_str(self.relative_source)
         result["size"] = from_int(self.size)
         result["text"] = from_str(self.text)
-        result["thumbnails"] = to_class(Thumbnails, self.thumbnails)
+        result["thumbnails"] = to_class(ThumbnailsMap, self.thumbnails)
         result["thumbnailsBuiltAt"] = from_str(self.thumbnails_built_at)
         result["title"] = from_str(self.title)
         result["type"] = from_str(self.type)
         result["url"] = from_str(self.url)
         return result
 
 
-class ContentValue:
-    blocks: List[BlockElement]
+class LocalizedContent:
+    blocks: List[ContentBlock]
     footnotes: Dict[str, str]
     layout: List[List[str]]
     title: str
 
-    def __init__(self, blocks: List[BlockElement], footnotes: Dict[str, str], layout: List[List[str]], title: str) -> None:
+    def __init__(self, blocks: List[ContentBlock], footnotes: Dict[str, str], layout: List[List[str]], title: str) -> None:
         self.blocks = blocks
         self.footnotes = footnotes
         self.layout = layout
         self.title = title
 
     @staticmethod
-    def from_dict(obj: Any) -> 'ContentValue':
+    def from_dict(obj: Any) -> 'LocalizedContent':
         assert isinstance(obj, dict)
-        blocks = from_list(BlockElement.from_dict, obj.get("blocks"))
+        blocks = from_list(ContentBlock.from_dict, obj.get("blocks"))
         footnotes = from_dict(from_str, obj.get("footnotes"))
         layout = from_list(lambda x: from_list(from_str, x), obj.get("layout"))
         title = from_str(obj.get("title"))
-        return ContentValue(blocks, footnotes, layout, title)
+        return LocalizedContent(blocks, footnotes, layout, title)
 
     def to_dict(self) -> dict:
         result: dict = {}
-        result["blocks"] = from_list(lambda x: to_class(BlockElement, x), self.blocks)
+        result["blocks"] = from_list(lambda x: to_class(ContentBlock, x), self.blocks)
         result["footnotes"] = from_dict(from_str, self.footnotes)
         result["layout"] = from_list(lambda x: from_list(from_str, x), self.layout)
         result["title"] = from_str(self.title)
         return result
 
 
-class DatabaseMetadataClass:
+class DatabaseMeta:
     partial: bool
     """Partial is true if the database was not fully built."""
 
     def __init__(self, partial: bool) -> None:
         self.partial = partial
 
     @staticmethod
-    def from_dict(obj: Any) -> 'DatabaseMetadataClass':
+    def from_dict(obj: Any) -> 'DatabaseMeta':
         assert isinstance(obj, dict)
         partial = from_bool(obj.get("Partial"))
-        return DatabaseMetadataClass(partial)
+        return DatabaseMeta(partial)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["Partial"] = from_bool(self.partial)
         return result
 
 
-class Metadata:
+class WorkMetadata:
     additional_metadata: Dict[str, Any]
     aliases: List[str]
-    colors: Colors
-    database_metadata: DatabaseMetadataClass
+    colors: ColorPalette
+    database_metadata: DatabaseMeta
     finished: str
     made_with: List[str]
     page_background: str
     private: bool
     started: str
     tags: List[str]
     thumbnail: str
     title_style: str
     wip: bool
 
-    def __init__(self, additional_metadata: Dict[str, Any], aliases: List[str], colors: Colors, database_metadata: DatabaseMetadataClass, finished: str, made_with: List[str], page_background: str, private: bool, started: str, tags: List[str], thumbnail: str, title_style: str, wip: bool) -> None:
+    def __init__(self, additional_metadata: Dict[str, Any], aliases: List[str], colors: ColorPalette, database_metadata: DatabaseMeta, finished: str, made_with: List[str], page_background: str, private: bool, started: str, tags: List[str], thumbnail: str, title_style: str, wip: bool) -> None:
         self.additional_metadata = additional_metadata
         self.aliases = aliases
         self.colors = colors
         self.database_metadata = database_metadata
         self.finished = finished
         self.made_with = made_with
         self.page_background = page_background
@@ -356,88 +356,88 @@
         self.started = started
         self.tags = tags
         self.thumbnail = thumbnail
         self.title_style = title_style
         self.wip = wip
 
     @staticmethod
-    def from_dict(obj: Any) -> 'Metadata':
+    def from_dict(obj: Any) -> 'WorkMetadata':
         assert isinstance(obj, dict)
         additional_metadata = from_dict(lambda x: x, obj.get("additionalMetadata"))
         aliases = from_list(from_str, obj.get("aliases"))
-        colors = Colors.from_dict(obj.get("colors"))
-        database_metadata = DatabaseMetadataClass.from_dict(obj.get("databaseMetadata"))
+        colors = ColorPalette.from_dict(obj.get("colors"))
+        database_metadata = DatabaseMeta.from_dict(obj.get("databaseMetadata"))
         finished = from_str(obj.get("finished"))
         made_with = from_list(from_str, obj.get("madeWith"))
         page_background = from_str(obj.get("pageBackground"))
         private = from_bool(obj.get("private"))
         started = from_str(obj.get("started"))
         tags = from_list(from_str, obj.get("tags"))
         thumbnail = from_str(obj.get("thumbnail"))
         title_style = from_str(obj.get("titleStyle"))
         wip = from_bool(obj.get("wip"))
-        return Metadata(additional_metadata, aliases, colors, database_metadata, finished, made_with, page_background, private, started, tags, thumbnail, title_style, wip)
+        return WorkMetadata(additional_metadata, aliases, colors, database_metadata, finished, made_with, page_background, private, started, tags, thumbnail, title_style, wip)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["additionalMetadata"] = from_dict(lambda x: x, self.additional_metadata)
         result["aliases"] = from_list(from_str, self.aliases)
-        result["colors"] = to_class(Colors, self.colors)
-        result["databaseMetadata"] = to_class(DatabaseMetadataClass, self.database_metadata)
+        result["colors"] = to_class(ColorPalette, self.colors)
+        result["databaseMetadata"] = to_class(DatabaseMeta, self.database_metadata)
         result["finished"] = from_str(self.finished)
         result["madeWith"] = from_list(from_str, self.made_with)
         result["pageBackground"] = from_str(self.page_background)
         result["private"] = from_bool(self.private)
         result["started"] = from_str(self.started)
         result["tags"] = from_list(from_str, self.tags)
         result["thumbnail"] = from_str(self.thumbnail)
         result["titleStyle"] = from_str(self.title_style)
         result["wip"] = from_bool(self.wip)
         return result
 
 
-class DatabaseValue:
+class AnalyzedWork:
     """AnalyzedWork represents a complete work, with analyzed mediae."""
 
     built_at: str
-    content: Dict[str, ContentValue]
+    content: Dict[str, LocalizedContent]
     description_hash: str
     id: str
-    metadata: Metadata
+    metadata: WorkMetadata
     partial: bool
 
-    def __init__(self, built_at: str, content: Dict[str, ContentValue], description_hash: str, id: str, metadata: Metadata, partial: bool) -> None:
+    def __init__(self, built_at: str, content: Dict[str, LocalizedContent], description_hash: str, id: str, metadata: WorkMetadata, partial: bool) -> None:
         self.built_at = built_at
         self.content = content
         self.description_hash = description_hash
         self.id = id
         self.metadata = metadata
         self.partial = partial
 
     @staticmethod
-    def from_dict(obj: Any) -> 'DatabaseValue':
+    def from_dict(obj: Any) -> 'AnalyzedWork':
         assert isinstance(obj, dict)
         built_at = from_str(obj.get("builtAt"))
-        content = from_dict(ContentValue.from_dict, obj.get("content"))
+        content = from_dict(LocalizedContent.from_dict, obj.get("content"))
         description_hash = from_str(obj.get("descriptionHash"))
         id = from_str(obj.get("id"))
-        metadata = Metadata.from_dict(obj.get("metadata"))
+        metadata = WorkMetadata.from_dict(obj.get("metadata"))
         partial = from_bool(obj.get("Partial"))
-        return DatabaseValue(built_at, content, description_hash, id, metadata, partial)
+        return AnalyzedWork(built_at, content, description_hash, id, metadata, partial)
 
     def to_dict(self) -> dict:
         result: dict = {}
         result["builtAt"] = from_str(self.built_at)
-        result["content"] = from_dict(lambda x: to_class(ContentValue, x), self.content)
+        result["content"] = from_dict(lambda x: to_class(LocalizedContent, x), self.content)
         result["descriptionHash"] = from_str(self.description_hash)
         result["id"] = from_str(self.id)
-        result["metadata"] = to_class(Metadata, self.metadata)
+        result["metadata"] = to_class(WorkMetadata, self.metadata)
         result["Partial"] = from_bool(self.partial)
         return result
 
 
-def database_from_dict(s: Any) -> Dict[str, DatabaseValue]:
-    return from_dict(DatabaseValue.from_dict, s)
+def database_from_dict(s: Any) -> Dict[str, AnalyzedWork]:
+    return from_dict(AnalyzedWork.from_dict, s)
 
 
-def database_to_dict(x: Dict[str, DatabaseValue]) -> Any:
-    return from_dict(lambda x: to_class(DatabaseValue, x), x)
+def database_to_dict(x: Dict[str, AnalyzedWork]) -> Any:
+    return from_dict(lambda x: to_class(AnalyzedWork, x), x)
```

### Comparing `ortfodb-1.4.1/ortfodb/exporter.py` & `ortfodb-1.5.0/ortfodb/exporter.py`

 * *Files 24% similar despite different names*

```diff
@@ -39,48 +39,48 @@
 
 
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
 
-class ExporterSchema:
+class ExporterCommand:
     log: Optional[List[str]]
     """Log a message. The first argument is the verb, the second is the color, the third is the
     message.
     """
     run: Optional[str]
     """Run a command in a shell"""
 
     def __init__(self, log: Optional[List[str]], run: Optional[str]) -> None:
         self.log = log
         self.run = run
 
     @staticmethod
-    def from_dict(obj: Any) -> 'ExporterSchema':
+    def from_dict(obj: Any) -> 'ExporterCommand':
         assert isinstance(obj, dict)
         log = from_union([lambda x: from_list(from_str, x), from_none], obj.get("log"))
         run = from_union([from_str, from_none], obj.get("run"))
-        return ExporterSchema(log, run)
+        return ExporterCommand(log, run)
 
     def to_dict(self) -> dict:
         result: dict = {}
         if self.log is not None:
             result["log"] = from_union([lambda x: from_list(from_str, x), from_none], self.log)
         if self.run is not None:
             result["run"] = from_union([from_str, from_none], self.run)
         return result
 
 
 class Exporter:
-    after: Optional[List[ExporterSchema]]
+    after: Optional[List[ExporterCommand]]
     """Commands to run after the build finishes. Go text template that receives .Data and
     .Database, the built database.
     """
-    before: Optional[List[ExporterSchema]]
+    before: Optional[List[ExporterCommand]]
     """Commands to run before the build starts. Go text template that receives .Data"""
 
     data: Optional[Dict[str, Any]]
     """Initial data"""
 
     description: str
     """Some documentation about the exporter"""
@@ -90,58 +90,58 @@
 
     requires: Optional[List[str]]
     """List of programs that are required to be available in the PATH for the exporter to run."""
 
     verbose: Optional[bool]
     """If true, will show every command that is run"""
 
-    work: Optional[List[ExporterSchema]]
+    work: Optional[List[ExporterCommand]]
     """Commands to run during the build, for each work. Go text template that receives .Data and
     .Work, the current work.
     """
 
-    def __init__(self, after: Optional[List[ExporterSchema]], before: Optional[List[ExporterSchema]], data: Optional[Dict[str, Any]], description: str, name: str, requires: Optional[List[str]], verbose: Optional[bool], work: Optional[List[ExporterSchema]]) -> None:
+    def __init__(self, after: Optional[List[ExporterCommand]], before: Optional[List[ExporterCommand]], data: Optional[Dict[str, Any]], description: str, name: str, requires: Optional[List[str]], verbose: Optional[bool], work: Optional[List[ExporterCommand]]) -> None:
         self.after = after
         self.before = before
         self.data = data
         self.description = description
         self.name = name
         self.requires = requires
         self.verbose = verbose
         self.work = work
 
     @staticmethod
     def from_dict(obj: Any) -> 'Exporter':
         assert isinstance(obj, dict)
-        after = from_union([lambda x: from_list(ExporterSchema.from_dict, x), from_none], obj.get("after"))
-        before = from_union([lambda x: from_list(ExporterSchema.from_dict, x), from_none], obj.get("before"))
+        after = from_union([lambda x: from_list(ExporterCommand.from_dict, x), from_none], obj.get("after"))
+        before = from_union([lambda x: from_list(ExporterCommand.from_dict, x), from_none], obj.get("before"))
         data = from_union([lambda x: from_dict(lambda x: x, x), from_none], obj.get("data"))
         description = from_str(obj.get("description"))
         name = from_str(obj.get("name"))
         requires = from_union([lambda x: from_list(from_str, x), from_none], obj.get("requires"))
         verbose = from_union([from_bool, from_none], obj.get("verbose"))
-        work = from_union([lambda x: from_list(ExporterSchema.from_dict, x), from_none], obj.get("work"))
+        work = from_union([lambda x: from_list(ExporterCommand.from_dict, x), from_none], obj.get("work"))
         return Exporter(after, before, data, description, name, requires, verbose, work)
 
     def to_dict(self) -> dict:
         result: dict = {}
         if self.after is not None:
-            result["after"] = from_union([lambda x: from_list(lambda x: to_class(ExporterSchema, x), x), from_none], self.after)
+            result["after"] = from_union([lambda x: from_list(lambda x: to_class(ExporterCommand, x), x), from_none], self.after)
         if self.before is not None:
-            result["before"] = from_union([lambda x: from_list(lambda x: to_class(ExporterSchema, x), x), from_none], self.before)
+            result["before"] = from_union([lambda x: from_list(lambda x: to_class(ExporterCommand, x), x), from_none], self.before)
         if self.data is not None:
             result["data"] = from_union([lambda x: from_dict(lambda x: x, x), from_none], self.data)
         result["description"] = from_str(self.description)
         result["name"] = from_str(self.name)
         if self.requires is not None:
             result["requires"] = from_union([lambda x: from_list(from_str, x), from_none], self.requires)
         if self.verbose is not None:
             result["verbose"] = from_union([from_bool, from_none], self.verbose)
         if self.work is not None:
-            result["work"] = from_union([lambda x: from_list(lambda x: to_class(ExporterSchema, x), x), from_none], self.work)
+            result["work"] = from_union([lambda x: from_list(lambda x: to_class(ExporterCommand, x), x), from_none], self.work)
         return result
 
 
 def exporter_from_dict(s: Any) -> Exporter:
     return Exporter.from_dict(s)
```

### Comparing `ortfodb-1.4.1/PKG-INFO` & `ortfodb-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortfodb
-Version: 1.4.1
+Version: 1.5.0
 Summary: ortfodb client library
 License: MIT
 Author: Ewen Le Bihan
 Author-email: hey@ewen.works
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

