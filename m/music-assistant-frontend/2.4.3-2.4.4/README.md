# Comparing `tmp/music-assistant-frontend-2.4.3.tar.gz` & `tmp/music-assistant-frontend-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-assistant-frontend-2.4.3.tar", last modified: Fri Apr 19 10:43:12 2024, max compression
+gzip compressed data, was "music-assistant-frontend-2.4.4.tar", last modified: Sat Apr 20 10:48:40 2024, max compression
```

## Comparing `music-assistant-frontend-2.4.3.tar` & `music-assistant-frontend-2.4.4.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.245503 music-assistant-frontend-2.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 10:42:17.000000 music-assistant-frontend-2.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 10:42:17.000000 music-assistant-frontend-2.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 10:43:12.245503 music-assistant-frontend-2.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-19 10:42:17.000000 music-assistant-frontend-2.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.217503 music-assistant-frontend-2.4.3/music_assistant_frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.245503 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddGroupPlayer-8a4f0893.js
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddProvider-f756ebc3.js
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AlbumDetails-0b4de4f6.js
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Alert-19e36349.js
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Alert-3971d760.css
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ArtistDetails-53ff83d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/BrowseView-a95cb7cc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-127b1d7c.css
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-dc894acd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-75569bfe.css
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-f0329745.js
--rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-2157b447.css
--rw-r--r--   0 runner    (1001) docker     (127)    64005 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-c7088a94.js
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig-f2bca5b1.css
--rw-r--r--   0 runner    (1001) docker     (127)    47426 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditCoreConfig-d27a9b35.js
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditPlayer-6e04043d.js
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditProvider-e046ee5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-8f9e6181.js
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-f9b96eef.css
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing-5372ff4e.css
--rw-r--r--   0 runner    (1001) docker     (127)    23624 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js
--rw-r--r--   0 runner    (1001) docker     (127)    93824 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryAlbums-7cfa0763.js
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryArtists-9924ed14.js
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryPlaylists-95e35cdd.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryRadios-4a033696.js
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryTracks-eeccb967.js
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ListviewItem-20f54197.css
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ListviewItem-8b992256.js
--rw-r--r--   0 runner    (1001) docker     (127)   160576 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
--rw-r--r--   0 runner    (1001) docker     (127)   347588 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   125116 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   143452 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PanelviewItem-cbf7c595.css
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlayerQueue-9f89c917.js
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Players-0e31a251.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlaylistDetails-2fe134b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails-2713c080.css
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Providers-58a591e0.js
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Providers-e2f60749.css
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/RadioDetails-54e9e340.js
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Search-00ee9dd8.js
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Settings-bbdb2168.js
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/TrackDetails-72029d5e.js
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-1c823677.css
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-56af8987.js
--rw-r--r--   0 runner    (1001) docker     (127)    30407 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-84e3406b.js
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-8b8b8a6d.css
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-257d0eab.css
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-b98fe47e.js
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCardText-6774ea5e.js
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-5309eac2.css
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-d7e50927.js
--rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-58c5fe02.js
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VForm-fc99b4aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VGrid-37b0738d.css
--rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-5b197ccd.js
--rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-b16e222c.css
--rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-a46f5e7a.css
--rw-r--r--   0 runner    (1001) docker     (127)    45661 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-b634019c.js
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-7df244e0.css
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-d10e917f.js
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-b576aa37.js
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-11e16be1.css
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-8ad24bfd.js
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-0c2ec62d.js
--rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-d31117f3.css
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-78a5e824.css
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-b7f10b15.js
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3a8fb95f.css
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3ef94159.js
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-84259ceb.js
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/contextmenu-521b5304.js
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_dark-75402cd0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_light-b832ae9e.png
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/fallback-d0ff2800.png
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/folder-6b5595ac.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40039 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-7be90dc2.js
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-e5b3781d.css
--rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/hires-438c7046.png
--rw-r--r--   0 runner    (1001) docker     (127)   699901 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-52c10419.css
--rw-r--r--   0 runner    (1001) docker     (127)   703850 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-b687f95a.js
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index.browser-342e672c.js
--rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/layout-42b7d22e.js
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/logo-9391b78c.svg
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/m4a-45331b05.png
--rw-r--r--   0 runner    (1001) docker     (127)   155276 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  1307880 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot
--rw-r--r--   0 runner    (1001) docker     (127)  1307660 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   403216 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   587984 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-19 10:43:06.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 10:43:04.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-19 10:43:08.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/sw.js
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-19 10:43:08.000000 music-assistant-frontend-2.4.3/music_assistant_frontend/workbox-27b29e6f.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:43:12.217503 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-19 10:43:11.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-19 10:43:12.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:43:11.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:43:10.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 10:43:12.000000 music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-19 10:42:38.000000 music-assistant-frontend-2.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:43:12.249503 music-assistant-frontend-2.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:48:40.443080 music-assistant-frontend-2.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 10:47:45.000000 music-assistant-frontend-2.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 10:47:45.000000 music-assistant-frontend-2.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-20 10:48:40.443080 music-assistant-frontend-2.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-20 10:47:45.000000 music-assistant-frontend-2.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:48:40.415080 music-assistant-frontend-2.4.4/music_assistant_frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:48:40.443080 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/AddGroupPlayer-ee16256c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/AddProvider-ac9c5e72.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/AlbumDetails-2e6fc4ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Alert-3971d760.css
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Alert-f8f9596c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ArtistDetails-c7f91dbb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/BrowseView-b98345de.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Container-127b1d7c.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Container-235383e5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/CoreConfigs-75569bfe.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/CoreConfigs-f5c6bb00.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Default-2157b447.css
+-rw-r--r--   0 runner    (1001) docker     (127)    64005 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Default-9d744187.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditConfig-f2bca5b1.css
+-rw-r--r--   0 runner    (1001) docker     (127)    47426 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditCoreConfig-72a12486.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditPlayer-e8fd1918.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditProvider-63f3a683.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/HomeView-9a92e516.js
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/HomeView-f9b96eef.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ItemsListing-5372ff4e.css
+-rw-r--r--   0 runner    (1001) docker     (127)    23624 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    93824 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14688 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15920 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14968 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14684 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15744 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15344 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryAlbums-20b785fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryArtists-af4c276c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryPlaylists-b8198cb0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryRadios-2aa75500.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryTracks-4227e977.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ListviewItem-04c2a02f.js
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ListviewItem-20f54197.css
+-rw-r--r--   0 runner    (1001) docker     (127)   160576 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   347588 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   125116 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   143452 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PanelviewItem-cbf7c595.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PlayerQueue-0a9bc504.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Players-23776fba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PlaylistDetails-59d16a22.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ProviderDetails-2713c080.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Providers-c5daf86a.js
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Providers-e2f60749.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/RadioDetails-5f7de0e3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Search-d1673cac.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Settings-34342ef5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/TrackDetails-40ca37ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VAlert-1c823677.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VAlert-ed4cb12a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VBadge-8b8b8a6d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    30407 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VBadge-e60e80c3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VCard-257d0eab.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VCard-4532b814.js
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VCardText-35ed9014.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VDialog-5309eac2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VDialog-7155dc5f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21125 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VExpansionPanel-8b2da313.js
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VForm-7178cd98.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VGrid-37b0738d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VInput-8a0f3c4b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22645 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VInput-b16e222c.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VMenu-a46f5e7a.css
+-rw-r--r--   0 runner    (1001) docker     (127)    45661 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VMenu-ec95eec6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSelect-7df244e0.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSelect-da46c348.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSlideGroup-c7be05c1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTabs-11e16be1.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTabs-9b65d90e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTextField-95a689ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTextField-d31117f3.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VToolbar-78a5e824.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VToolbar-c9911418.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTooltip-3a8fb95f.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTooltip-ebb61ea6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VVirtualScroll-acb73766.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/contextmenu-c35de49a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/cover_dark-75402cd0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/cover_light-b832ae9e.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/fallback-d0ff2800.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/folder-6b5595ac.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40039 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/forwardRefs-708ed339.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/forwardRefs-e5b3781d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/hires-438c7046.png
+-rw-r--r--   0 runner    (1001) docker     (127)   699901 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/index-52c10419.css
+-rw-r--r--   0 runner    (1001) docker     (127)   703850 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/index-e734c256.js
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/index.browser-342e672c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28226 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/layout-f1bc9409.js
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/logo-9391b78c.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/m4a-45331b05.png
+-rw-r--r--   0 runner    (1001) docker     (127)   155276 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  1307880 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  1307660 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   403216 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   587984 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-20 10:48:34.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/pwa-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/pwa-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 10:48:32.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-20 10:48:35.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/sw.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-20 10:48:35.000000 music-assistant-frontend-2.4.4/music_assistant_frontend/workbox-27b29e6f.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:48:40.415080 music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-20 10:48:39.000000 music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-20 10:48:40.000000 music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:48:39.000000 music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:48:38.000000 music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 10:48:40.000000 music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-20 10:48:07.000000 music-assistant-frontend-2.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 10:48:40.443080 music-assistant-frontend-2.4.4/setup.cfg
```

### Comparing `music-assistant-frontend-2.4.3/LICENSE` & `music-assistant-frontend-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/PKG-INFO` & `music-assistant-frontend-2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.4.3
+Version: 2.4.4
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.4.3/README.md` & `music-assistant-frontend-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/apple-touch-icon.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddGroupPlayer-8a4f0893.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/AddGroupPlayer-ee16256c.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -10,36 +10,36 @@
     l as a,
     A as o,
     x as v,
     Q as c,
     N as p,
     I as N,
     B as s
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     a as U,
     V as w
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     k as P,
     l as b
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as T
-} from "./VForm-fc99b4aa.js";
+} from "./VForm-7178cd98.js";
 import {
     V as S
-} from "./VTextField-0c2ec62d.js";
+} from "./VTextField-95a689ca.js";
 import {
     V as q
-} from "./VSelect-d10e917f.js";
-import "./VMenu-b634019c.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./VSelect-da46c348.js";
+import "./VMenu-ec95eec6.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VVirtualScroll-acb73766.js";
 const A = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AddProvider-f756ebc3.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/AddProvider-ac9c5e72.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -16,41 +16,41 @@
     A as l,
     x as a,
     Q as p,
     N as d,
     z as y,
     B as r,
     I as v
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     _ as T
-} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js";
 import {
     a as $,
     V as A
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     a as _
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     k as j,
     x as I
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     f as U
-} from "./VMenu-b634019c.js";
-import "./VExpansionPanel-58c5fe02.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VForm-fc99b4aa.js"; /* empty css              */
-import "./VDialog-d7e50927.js";
-import "./VAlert-56af8987.js";
-import "./VTextField-0c2ec62d.js";
-import "./VSelect-d10e917f.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./VMenu-ec95eec6.js";
+import "./VExpansionPanel-8b2da313.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VForm-7178cd98.js"; /* empty css              */
+import "./VDialog-7155dc5f.js";
+import "./VAlert-ed4cb12a.js";
+import "./VTextField-95a689ca.js";
+import "./VSelect-da46c348.js";
+import "./VVirtualScroll-acb73766.js";
 const z = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/AlbumDetails-0b4de4f6.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/AlbumDetails-2e6fc4ee.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as v
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     _ as h,
     a as w
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js";
 import {
     v as A,
     r as d,
     c as g,
     ap as c,
     w as I,
     o as D,
@@ -17,34 +17,34 @@
     b as E,
     y as l,
     E as M,
     l as V,
     z as n,
     I as u,
     B as f
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-import "./layout-42b7d22e.js";
-import "./VDialog-d7e50927.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+import "./layout-f1bc9409.js";
+import "./VDialog-7155dc5f.js";
 const T = f("br", null, null, -1),
     $ = f("br", null, null, -1),
     te = A({
         __name: "AlbumDetails",
         props: {
             itemId: {},
             provider: {},
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ArtistDetails-53ff83d9.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ArtistDetails-c7f91dbb.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as b
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     _ as A,
     a as h
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js";
 import {
     v as g,
     r as p,
     w as I,
     o as D,
     L as l,
     an as F,
@@ -17,34 +17,34 @@
     ap as v,
     y as o,
     E as B,
     l as E,
     z as m,
     I as d,
     B as _
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-import "./layout-42b7d22e.js";
-import "./VDialog-d7e50927.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+import "./layout-f1bc9409.js";
+import "./VDialog-7155dc5f.js";
 const $ = _("br", null, null, -1),
     N = _("br", null, null, -1),
     re = g({
         __name: "ArtistDetails",
         props: {
             itemId: {},
             provider: {}
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/BrowseView-a95cb7cc.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/BrowseView-b98345de.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -4,35 +4,35 @@
     aa as c,
     c as u,
     K as a,
     y as h,
     E as f,
     l as w,
     L as b
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     _ as d
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
 const A = n({
     __name: "BrowseView",
     props: {
         path: {}
     },
     setup(s) {
         const t = s,
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-127b1d7c.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Container-127b1d7c.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Container-dc894acd.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Container-235383e5.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,70 +1,70 @@
 import {
-    c as o,
-    y as r,
+    c as l,
+    y as i,
     z as p,
     Y as M,
     G as $,
     A as d,
     _ as k,
     n as h,
-    v as z,
-    L as i,
+    v as C,
+    L as r,
+    x as o,
     E as m,
-    x as l,
     D as g,
+    I as z,
     R as V,
     l as f,
-    F as C,
-    I as P,
+    F as P,
     a6 as L,
     p as w,
     g as B,
     u as A
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     l as x,
     n as b,
     a as D,
     d as S,
     i as T
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     e as H,
     b as R,
     d as F,
     V as E
-} from "./VMenu-b634019c.js"; /* empty css              */
+} from "./VMenu-ec95eec6.js"; /* empty css              */
 const N = {
     props: {
         variant: {
             type: String,
             default: "default",
             validator: t => ["plain", "default", "responsive", "icon", "list"].includes(t)
         }
     },
     setup(t, a) {
         const e = {},
-            n = o(() => ({
+            n = l(() => ({
                 ...e,
                 class: "v-btn--variant-responsive",
                 ripple: !0,
                 icon: !0,
                 style: "height: min(calc(100vw - 40px), calc(100vh - 340px)); width: min(calc(100vw - 40px), calc(100vh - 340px));"
             })),
-            u = o(() => ({
+            u = l(() => ({
                 ...e,
                 ripple: !1
             })),
-            v = o(() => ({
+            v = l(() => ({
                 ...e,
                 density: "comfortable"
             }));
         return {
-            btnProps: o(() => {
+            btnProps: l(() => {
                 switch (t.variant) {
                     case "default":
                         return e;
                     case "plain":
                         return e;
                     case "responsive":
                         return n.value;
@@ -82,134 +82,135 @@
 const I = (t, a) => {
     const e = t.__vccOpts || t;
     for (const [n, u] of a) e[n] = u;
     return e
 };
 
 function G(t, a, e, n, u, v) {
-    return r(), p(x, h(n.btnProps, {
+    return i(), p(x, h(n.btnProps, {
         variant: "plain"
     }), M({
         _: 2
     }, [$(t.$slots, (_, c) => ({
         name: c,
         fn: d(() => [k(t.$slots, c)])
     }))]), 1040)
 }
 const O = I(N, [
         ["render", G]
     ]),
     Y = ["title", "innerHTML"],
     j = ["title", "innerHTML"],
-    se = z({
+    se = C({
         __name: "ProviderIcon",
         props: {
             domain: {},
             size: {},
             dark: {
                 type: Boolean
             }
         },
         setup(t) {
             const a = t,
-                e = o(() => a.domain in i.providers ? i.providers[a.domain].domain : a.domain);
-            return (n, u) => (r(), m("div", {
+                e = l(() => a.domain in r.providers ? r.providers[a.domain].domain : a.domain);
+            return (n, u) => o(r).providerManifests[e.value] ? (i(), m("div", {
+                key: 0,
                 style: g(`width:${n.size}px;margin-left:10px;margin-right:10px`)
-            }, [e.value == "library" ? (r(), p(b, {
+            }, [e.value == "library" ? (i(), p(b, {
                 key: 0,
                 size: n.size,
                 icon: "mdi-bookshelf",
                 title: n.$t("item_in_library")
-            }, null, 8, ["size", "title"])) : n.$vuetify.theme.current.dark && l(i).providerManifests[e.value].icon_svg_dark ? (r(), m("div", {
+            }, null, 8, ["size", "title"])) : n.$vuetify.theme.current.dark && o(r).providerManifests[e.value].icon_svg_dark ? (i(), m("div", {
                 key: 1,
                 style: g(`width: ${n.size}px`),
-                title: l(i).providerManifests[e.value].name,
-                innerHTML: l(i).providerManifests[e.value].icon_svg_dark
-            }, null, 12, Y)) : l(i).providerManifests[e.value].icon_svg ? (r(), m("div", {
+                title: o(r).providerManifests[e.value].name,
+                innerHTML: o(r).providerManifests[e.value].icon_svg_dark
+            }, null, 12, Y)) : o(r).providerManifests[e.value].icon_svg ? (i(), m("div", {
                 key: 2,
                 style: g(`width: ${n.size}px;height: ${n.size}px`),
-                title: l(i).providerManifests[e.value].name,
-                innerHTML: l(i).providerManifests[e.value].icon_svg
-            }, null, 12, j)) : l(i).providerManifests[e.value].icon ? (r(), p(b, {
+                title: o(r).providerManifests[e.value].name,
+                innerHTML: o(r).providerManifests[e.value].icon_svg
+            }, null, 12, j)) : o(r).providerManifests[e.value].icon ? (i(), p(b, {
                 key: 3,
                 size: n.size,
-                icon: "mdi-" + l(i).providerManifests[e.value].icon,
-                title: l(i).providerManifests[e.value].name,
+                icon: "mdi-" + o(r).providerManifests[e.value].icon,
+                title: o(r).providerManifests[e.value].name,
                 dark: n.$vuetify.theme.current.dark
-            }, null, 8, ["size", "icon", "title", "dark"])) : (r(), p(b, {
+            }, null, 8, ["size", "icon", "title", "dark"])) : (i(), p(b, {
                 key: 4,
                 size: n.size,
                 dark: n.$vuetify.theme.current.dark,
                 icon: "mdi-playlist-play"
-            }, null, 8, ["size", "dark"]))], 4))
+            }, null, 8, ["size", "dark"]))], 4)) : z("", !0)
         }
     }),
     q = {
         components: {
             MAButton: O
         },
         props: {
             contextMenuItems: {
                 type: Array,
                 default: []
             }
         },
         setup(t, a) {
-            const e = o(() => ({}));
+            const e = l(() => ({}));
             return {
-                listItemProps: o(() => ({
+                listItemProps: l(() => ({
                     ...e.value,
                     ...a.attrs
                 }))
             }
         }
     };
 const J = {
     key: 0,
     class: "contextmenubtn"
 };
 
 function K(t, a, e, n, u, v) {
     const _ = V("MAButton"),
         c = V("ListItem", !0);
-    return r(), p(E, h(n.listItemProps, {
+    return i(), p(E, h(n.listItemProps, {
         class: "list-item-main",
         onInput: a[0] || (a[0] = s => t.$emit("input", s))
     }), M({
         _: 2
     }, [$(t.$slots, (s, y) => ({
         name: y,
         fn: d(() => [k(t.$slots, y)])
     })), t.$slots.append ? {
         name: "append",
-        fn: d(() => [k(t.$slots, "append"), e.contextMenuItems.length > 0 ? (r(), m("div", J, [f(H, {
+        fn: d(() => [k(t.$slots, "append"), e.contextMenuItems.length > 0 ? (i(), m("div", J, [f(H, {
             location: "bottom end"
         }, {
             activator: d(({
                 props: s
             }) => [f(_, h(s, {
                 variant: "list",
                 icon: "mdi-dots-vertical"
             }), null, 16)]),
             default: d(() => [f(R, null, {
-                default: d(() => [(r(!0), m(C, null, $(e.contextMenuItems.filter(s => s.hide != !0), (s, y) => (r(), p(c, {
+                default: d(() => [(i(!0), m(P, null, $(e.contextMenuItems.filter(s => s.hide != !0), (s, y) => (i(), p(c, {
                     key: y,
                     title: t.$t(s.label, s.labelArgs),
                     disabled: s.disabled == !0,
                     onClick: Z => s.action ? s.action() : ""
                 }, {
                     prepend: d(() => [f(F, {
                         icon: s.icon
                     }, null, 8, ["icon"])]),
                     _: 2
                 }, 1032, ["title", "disabled", "onClick"]))), 128))]),
                 _: 1
             })]),
             _: 1
-        })])) : P("", !0)]),
+        })])) : z("", !0)]),
         key: "0"
     } : void 0]), 1040)
 }
 const re = I(q, [
         ["render", K]
     ]),
     Q = {
@@ -217,22 +218,22 @@
             variant: {
                 type: String,
                 default: "default",
                 validator: t => ["default", "panel"].includes(t)
             }
         },
         setup(t, a) {
-            const e = o(() => ({
+            const e = l(() => ({
                     class: "container-default"
                 })),
-                n = o(() => ({
+                n = l(() => ({
                     class: L.theme.current.value.dark ? "container-default container-panels-dark" : "container-default container-panels-light"
                 }));
             return {
-                btnProps: o(() => {
+                btnProps: l(() => {
                     switch (t.variant) {
                         case "default":
                             return e.value;
                         case "panel":
                             return n.value;
                         default:
                             return e.value
@@ -265,15 +266,15 @@
                 }, n.value, t.class],
                 style: t.style
             }, e)), {}
         }
     });
 
 function X(t, a, e, n, u, v) {
-    return r(), p(W, h(n.btnProps, {
+    return i(), p(W, h(n.btnProps, {
         variant: "default",
         fluid: ""
     }), M({
         _: 2
     }, [$(t.$slots, (_, c) => ({
         name: c,
         fn: d(() => [k(t.$slots, c)])
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-75569bfe.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/CoreConfigs-75569bfe.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/CoreConfigs-f0329745.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/CoreConfigs-f5c6bb00.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -20,32 +20,32 @@
     N as t,
     F as w,
     G,
     x as s,
     I as T,
     af as Q,
     z as V
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     C as B,
     L as j,
     _ as J
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     V as I
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     a as K,
     o as O,
     d as W,
     q as X,
     i as Y,
     n as A
-} from "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
+} from "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
 const Z = D({
         fixedHeader: Boolean,
         fixedFooter: Boolean,
         height: [Number, String],
         hover: Boolean,
         ...K(),
         ...O(),
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-2157b447.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Default-2157b447.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Default-c7088a94.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Default-9d744187.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -69,32 +69,32 @@
     ad as ke,
     ae as al,
     af as ut,
     ag as ct,
     ah as ol,
     ai as wt,
     aj as il
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     B as Y,
     L as X,
     _ as ze,
     a as xe,
     C as sl
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     u as qe,
     a as nl,
     V as dt,
     b as ie,
     c as rl,
     d as mt,
     e as Pt,
     f as ul
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     m as Ue,
     a as he,
     b as Fe,
     c as Oe,
     d as Qe,
     u as Ye,
@@ -113,70 +113,70 @@
     p as pl,
     q as yl,
     r as fl,
     s as hl,
     v as _l,
     w as gl,
     x as bl
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     m as Xe,
     u as Ke,
     a as kl,
     b as wl,
     c as Pl
-} from "./layout-42b7d22e.js";
+} from "./layout-f1bc9409.js";
 import {
     M as Ze,
     V as Vt,
     i as re,
     a as ce,
     _ as Cl,
     g as vt
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     e as Ve,
     g as Vl,
     a as $l
-} from "./contextmenu-521b5304.js";
+} from "./contextmenu-c35de49a.js";
 import {
     V as Je,
     a as $t
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     V as Ee,
     a as Il
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     V as Se,
     a as xl
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     V as et
-} from "./VDialog-d7e50927.js";
+} from "./VDialog-7155dc5f.js";
 import {
     V as Ql
-} from "./VSelect-d10e917f.js";
+} from "./VSelect-da46c348.js";
 import {
     V as Sl,
     a as Tl
-} from "./VTabs-8ad24bfd.js";
+} from "./VTabs-9b65d90e.js";
 import {
     V as It,
     a as Bl,
     b as Ml,
     c as zl,
     d as Dl
-} from "./VExpansionPanel-58c5fe02.js";
+} from "./VExpansionPanel-8b2da313.js";
 import {
     V as Nl
-} from "./VInput-5b197ccd.js"; /* empty css              */
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-import "./VSlideGroup-b576aa37.js";
+} from "./VInput-8a0f3c4b.js"; /* empty css              */
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+import "./VSlideGroup-c7be05c1.js";
 const El = "" + new URL("logo-9391b78c.svg", import.meta.url).href;
 
 function Ll(a) {
     let {
         rootEl: l,
         isSticky: u,
         layoutItemStyles: o
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig-f2bca5b1.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditConfig-f2bca5b1.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -37,66 +37,66 @@
     G as Ee,
     Q as H,
     N as O,
     x as f,
     I as ae,
     B as I,
     $ as T
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     a as ot,
     b as ut,
     c as ct,
     d as pt,
     V as ht
-} from "./VExpansionPanel-58c5fe02.js";
+} from "./VExpansionPanel-8b2da313.js";
 import {
     P as dt,
     i as gt,
     j as kt,
     Q as ft,
     n as mt,
     R as bt,
     x as xt,
     l as X,
     k as wt
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as vt
-} from "./VForm-fc99b4aa.js";
+} from "./VForm-7178cd98.js";
 import {
     V as $t,
     b as yt
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     V as Ae
-} from "./VCardText-6774ea5e.js"; /* empty css              */
+} from "./VCardText-35ed9014.js"; /* empty css              */
 import {
     h as Tt
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     V as Vt
-} from "./VDialog-d7e50927.js";
+} from "./VDialog-7155dc5f.js";
 import {
     m as Rt,
     d as zt,
     u as Ct,
     b as Le,
     e as qe,
     f as Pe
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 import {
     V as St
-} from "./VAlert-56af8987.js";
+} from "./VAlert-ed4cb12a.js";
 import {
     V as W
-} from "./VTextField-0c2ec62d.js";
+} from "./VTextField-95a689ca.js";
 import {
     V as It
-} from "./VSelect-d10e917f.js";
+} from "./VSelect-da46c348.js";
 const Et = Tt("v-spacer", "div", "VSpacer");
 const At = tt({
         indeterminate: Boolean,
         inset: Boolean,
         flat: Boolean,
         loading: {
             type: [Boolean, String],
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditCoreConfig-d27a9b35.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditCoreConfig-72a12486.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -10,44 +10,44 @@
     Q as c,
     N as u,
     x as d,
     z as p,
     B as i,
     I as f,
     L as n
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     _ as $
-} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js";
 import {
     n as j
 } from "./index.browser-342e672c.js";
 import {
     a as E,
     V as O
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     a as v
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     k as h,
     x as S
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     f as T
-} from "./VMenu-b634019c.js";
-import "./VExpansionPanel-58c5fe02.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VForm-fc99b4aa.js"; /* empty css              */
-import "./VDialog-d7e50927.js";
-import "./VAlert-56af8987.js";
-import "./VTextField-0c2ec62d.js";
-import "./VSelect-d10e917f.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./VMenu-ec95eec6.js";
+import "./VExpansionPanel-8b2da313.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VForm-7178cd98.js"; /* empty css              */
+import "./VDialog-7155dc5f.js";
+import "./VAlert-ed4cb12a.js";
+import "./VTextField-95a689ca.js";
+import "./VSelect-da46c348.js";
+import "./VVirtualScroll-acb73766.js";
 const z = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditPlayer-6e04043d.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditPlayer-e8fd1918.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -10,41 +10,41 @@
     x as t,
     Q as p,
     N as r,
     B as i,
     I as d,
     z as m,
     L as l
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     V as I,
     _ as S
-} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js";
 import {
     a as T,
     V as E
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     a as v
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     k
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as D
-} from "./VTextField-0c2ec62d.js";
-import "./VExpansionPanel-58c5fe02.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VMenu-b634019c.js";
-import "./VForm-fc99b4aa.js"; /* empty css              */
-import "./VDialog-d7e50927.js";
-import "./VAlert-56af8987.js";
-import "./VSelect-d10e917f.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./VTextField-95a689ca.js";
+import "./VExpansionPanel-8b2da313.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VMenu-ec95eec6.js";
+import "./VForm-7178cd98.js"; /* empty css              */
+import "./VDialog-7155dc5f.js";
+import "./VAlert-ed4cb12a.js";
+import "./VSelect-da46c348.js";
+import "./VVirtualScroll-acb73766.js";
 const U = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/EditProvider-e046ee5d.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/EditProvider-63f3a683.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -13,47 +13,47 @@
     A as d,
     x as i,
     Q as f,
     N as m,
     z as p,
     B as u,
     I as v
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     V as x,
     _ as I
-} from "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js";
 import {
     n as P
 } from "./index.browser-342e672c.js";
 import {
     a as U,
     V as O
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     a as _
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     k as h,
     x as A
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as z
-} from "./VTextField-0c2ec62d.js";
+} from "./VTextField-95a689ca.js";
 import {
     f as D
-} from "./VMenu-b634019c.js";
-import "./VExpansionPanel-58c5fe02.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VForm-fc99b4aa.js"; /* empty css              */
-import "./VDialog-d7e50927.js";
-import "./VAlert-56af8987.js";
-import "./VSelect-d10e917f.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./VMenu-ec95eec6.js";
+import "./VExpansionPanel-8b2da313.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VForm-7178cd98.js"; /* empty css              */
+import "./VDialog-7155dc5f.js";
+import "./VAlert-ed4cb12a.js";
+import "./VSelect-da46c348.js";
+import "./VVirtualScroll-acb73766.js";
 const F = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-8f9e6181.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/HomeView-9a92e516.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     L as J,
     a as K,
     C as U
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     v as h,
     o as Z,
     R as I,
     y as a,
     z as v,
     A as r,
@@ -30,43 +30,43 @@
     Q as C,
     ab as ie,
     J as k,
     a2 as q,
     Z as ae,
     c as se,
     am as re
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     _ as oe
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
 import {
     i as ne,
     e as le
-} from "./contextmenu-521b5304.js";
+} from "./contextmenu-c35de49a.js";
 import {
     n as R,
     l as ue,
     x as de
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as me,
     M as _e,
     i as ce
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     V as Y
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     V as pe
-} from "./VCard-b98fe47e.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VTooltip-3ef94159.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCardText-6774ea5e.js";
+} from "./VCard-4532b814.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VTooltip-ebb61ea6.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCardText-35ed9014.js";
 const j = h({
         __name: "Carousel",
         setup(b) {
             return Z(() => {
                 document.documentElement.style.setProperty("--swiper-navigation-color", "primary")
             }), (e, t) => {
                 const i = I("swiper");
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/HomeView-f9b96eef.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/HomeView-f9b96eef.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing-5372ff4e.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ItemsListing-5372ff4e.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -40,44 +40,44 @@
     x as T,
     F as W,
     G as Q,
     M as yt,
     K as H,
     Z as ht,
     ak as gt
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     L as bt
-} from "./ListviewItem-8b992256.js";
+} from "./ListviewItem-04c2a02f.js";
 import {
     C as kt,
     B as E,
     _ as $e,
     L as te
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     _ as wt
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
 import {
     e as St,
     i as Ct,
     a as Bt
-} from "./contextmenu-521b5304.js";
+} from "./contextmenu-c35de49a.js";
 import {
     A as _e
-} from "./Alert-19e36349.js";
+} from "./Alert-f8f9596c.js";
 import {
     V as Vt
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     V as $t
-} from "./VTextField-0c2ec62d.js";
+} from "./VTextField-95a689ca.js";
 import {
     V as ae
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     a as Ee,
     d as Me,
     y as _t,
     z as It,
     c as Ft,
     A as At,
@@ -89,29 +89,29 @@
     E as Mt,
     v as Te,
     j as Tt,
     F as jt,
     n as P,
     k as le,
     l as oe
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as Ie
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     m as Rt,
     a as Dt,
     f as Fe,
     b as ne,
     e as se,
     d as Kt
-} from "./VMenu-b634019c.js"; /* empty css              */
+} from "./VMenu-ec95eec6.js"; /* empty css              */
 import {
     V as Ut
-} from "./VVirtualScroll-84259ceb.js";
+} from "./VVirtualScroll-acb73766.js";
 const je = (() => Y.reduce((t, r) => (t[r] = {
         type: [Boolean, String, Number],
         default: !1
     }, t), {}))(),
     Re = (() => Y.reduce((t, r) => {
         const a = "offset" + ie(r);
         return t[a] = {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryAlbums-7cfa0763.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryAlbums-20b785fa.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,41 +1,41 @@
 import {
     _ as p
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     v as u,
     r as c,
     o as y,
     L as e,
     an as s,
     b as _,
     y as f,
     z as d,
     x as b,
     M as n,
     ao as o,
     K as v
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
 const P = u({
     __name: "LibraryAlbums",
     setup(E) {
         const r = c(!1),
             i = {
                 name: "sort_name",
                 recent: "timestamp_added DESC",
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryArtists-9924ed14.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryPlaylists-b8198cb0.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,75 +1,91 @@
 import {
-    _ as c
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+    _
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
-    v as f,
-    r as n,
-    o as y,
-    L as e,
-    an as i,
-    b as _,
-    y as d,
-    z as b,
-    x as v,
-    M as m,
-    ao as r,
-    K as h
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-const F = f({
-    __name: "LibraryArtists",
-    setup(E) {
-        const p = n([]),
-            s = n(!1),
-            o = {
-                name: "sort_name",
-                recent: "timestamp_added DESC"
-            },
-            u = async function(t) {
-                if (t.refresh && !s.value) {
-                    for (e.startSync([m.ARTIST]), await r(250); e.syncTasks.value.length > 0 && e.syncTasks.value.filter(a => a.media_types.includes(m.ARTIST)).length != 0;) await r(500);
-                    await r(500)
-                }
-                return s.value = !1, await e.getLibraryArtists(t.favoritesOnly || void 0, t.search, t.limit, t.offset, o[t.sortBy], t.albumArtistsFilter)
-            };
-        return y(() => {
-            const t = e.subscribe_multi([i.MEDIA_ITEM_ADDED, i.MEDIA_ITEM_UPDATED, i.MEDIA_ITEM_DELETED], a => {
-                var l;
-                (l = a.object_id) != null && l.startsWith("library://artist") && (s.value = !0)
+    v as d,
+    O as v,
+    r as o,
+    o as b,
+    L as s,
+    P as h,
+    an as r,
+    b as E,
+    y as w,
+    z as T,
+    x as I,
+    M as u,
+    ao as l,
+    K as k
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+const q = d({
+    __name: "LibraryPlaylists",
+    setup(A) {
+        const {
+            t: c
+        } = v(), m = o([]), i = o(!1), n = o([]), p = {
+            name: "sort_name",
+            recent: "timestamp_added DESC"
+        }, y = async function(t) {
+            if (t.refresh && !i.value) {
+                for (s.startSync([u.PLAYLIST]), await l(250); s.syncTasks.value.length > 0 && s.syncTasks.value.filter(e => e.media_types.includes(u.PLAYLIST)).length != 0;) await l(500);
+                await l(500)
+            }
+            return i.value = !1, await s.getLibraryPlaylists(t.favoritesOnly || void 0, t.search, t.limit, t.offset, p[t.sortBy])
+        };
+        b(() => {
+            for (const e of Object.values(s.providers).filter(a => a.available && a.supported_features.includes(h.PLAYLIST_CREATE))) n.value.push({
+                label: "create_playlist_on",
+                labelArgs: [e.name],
+                action: () => {
+                    f(e.instance_id)
+                },
+                icon: "mdi-playlist-plus"
             });
-            _(t)
-        }), (t, a) => (d(), b(c, {
-            itemtype: "artists",
-            items: p.value,
-            "show-provider": !1,
+            const t = s.subscribe_multi([r.MEDIA_ITEM_ADDED, r.MEDIA_ITEM_UPDATED, r.MEDIA_ITEM_DELETED], e => {
+                var a;
+                (a = e.object_id) != null && a.startsWith("library://playlist") && (i.value = !0)
+            });
+            E(t)
+        });
+        const f = async function(t) {
+            const e = prompt(c("new_playlist_name"));
+            e && await s.createPlaylist(e, t).then(() => location.reload()).catch(a => alert(a))
+        };
+        return (t, e) => (w(), T(_, {
+            itemtype: "playlists",
+            items: m.value,
+            "show-duration": !1,
+            "show-provider": !0,
             "show-favorites-only-filter": !0,
-            "load-paged-data": u,
-            "show-album-artists-only-filter": !0,
-            "update-available": s.value,
-            title: v(h)("bp4") ? t.$t("artists") : "",
+            "load-paged-data": y,
+            "show-library": !0,
+            "sort-keys": Object.keys(p),
+            "update-available": i.value,
+            title: I(k)("bp4") ? t.$t("playlists") : "",
             "allow-key-hooks": !0,
             "show-search-button": !0,
-            "sort-keys": Object.keys(o)
-        }, null, 8, ["items", "update-available", "title", "sort-keys"]))
+            "context-menu-items": n.value
+        }, null, 8, ["items", "sort-keys", "update-available", "title", "context-menu-items"]))
     }
 });
 export {
-    F as
+    q as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryPlaylists-95e35cdd.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryTracks-4227e977.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,91 +1,96 @@
 import {
     _
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
-    v as d,
-    O as v,
-    r as o,
+    v as f,
+    O as y,
+    r as m,
     o as b,
-    L as s,
-    P as h,
-    an as r,
-    b as E,
-    y as w,
-    z as T,
-    x as I,
-    M as u,
-    ao as l,
-    K as k
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-const q = d({
-    __name: "LibraryPlaylists",
-    setup(A) {
+    L as a,
+    an as s,
+    b as k,
+    y as v,
+    z as h,
+    x as T,
+    M as i,
+    ao as n,
+    K as E
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+const q = f({
+    __name: "LibraryTracks",
+    setup(D) {
         const {
-            t: c
-        } = v(), m = o([]), i = o(!1), n = o([]), p = {
+            t: l
+        } = y(), c = m([]), r = m(!1), u = {
             name: "sort_name",
-            recent: "timestamp_added DESC"
-        }, y = async function(t) {
-            if (t.refresh && !i.value) {
-                for (s.startSync([u.PLAYLIST]), await l(250); s.syncTasks.value.length > 0 && s.syncTasks.value.filter(e => e.media_types.includes(u.PLAYLIST)).length != 0;) await l(500);
-                await l(500)
-            }
-            return i.value = !1, await s.getLibraryPlaylists(t.favoritesOnly || void 0, t.search, t.limit, t.offset, p[t.sortBy])
+            recent: "timestamp_added DESC",
+            artist: "sort_artist, sort_name",
+            album: "albums.sort_name, tracks.sort_name",
+            duration: "duration",
+            duration_desc: "duration DESC"
         };
         b(() => {
-            for (const e of Object.values(s.providers).filter(a => a.available && a.supported_features.includes(h.PLAYLIST_CREATE))) n.value.push({
-                label: "create_playlist_on",
-                labelArgs: [e.name],
-                action: () => {
-                    f(e.instance_id)
-                },
-                icon: "mdi-playlist-plus"
+            const t = a.subscribe_multi([s.MEDIA_ITEM_ADDED, s.MEDIA_ITEM_UPDATED, s.MEDIA_ITEM_DELETED], e => {
+                var o;
+                (o = e.object_id) != null && o.startsWith("library://track") && (r.value = !0)
             });
-            const t = s.subscribe_multi([r.MEDIA_ITEM_ADDED, r.MEDIA_ITEM_UPDATED, r.MEDIA_ITEM_DELETED], e => {
-                var a;
-                (a = e.object_id) != null && a.startsWith("library://playlist") && (i.value = !0)
-            });
-            E(t)
+            k(t)
         });
-        const f = async function(t) {
-            const e = prompt(c("new_playlist_name"));
-            e && await s.createPlaylist(e, t).then(() => location.reload()).catch(a => alert(a))
+        const p = async function(t) {
+            if (t.favoritesOnly = t.favoritesOnly || void 0, t.refresh && !r.value) {
+                for (a.startSync([i.TRACK]), await n(250); a.syncTasks.value.length > 0 && a.syncTasks.value.filter(e => e.media_types.includes(i.TRACK)).length != 0;) await n(500);
+                await n(500)
+            }
+            return r.value = !1, await a.getLibraryTracks(t.favoritesOnly, t.search, t.limit, t.offset, u[t.sortBy])
+        }, d = async function() {
+            const t = prompt(l("enter_url"));
+            t && a.getItem(i.TRACK, t, "builtin").then(e => {
+                const o = prompt(l("enter_name"), e.name);
+                e.name = o || e.name, a.addItemToLibrary(e).then(() => r.value = !0)
+            }).catch(e => alert(e))
         };
-        return (t, e) => (w(), T(_, {
-            itemtype: "playlists",
-            items: m.value,
-            "show-duration": !1,
-            "show-provider": !0,
+        return (t, e) => (v(), h(_, {
+            itemtype: "tracks",
+            items: c.value,
+            "show-provider": !1,
             "show-favorites-only-filter": !0,
-            "load-paged-data": y,
-            "show-library": !0,
-            "sort-keys": Object.keys(p),
-            "update-available": i.value,
-            title: I(k)("bp4") ? t.$t("playlists") : "",
-            "allow-key-hooks": !0,
+            "show-track-number": !1,
+            "load-paged-data": p,
+            "sort-keys": Object.keys(u),
+            "show-album": !0,
+            "update-available": r.value,
+            title: T(E)("bp4") ? t.$t("tracks") : "",
             "show-search-button": !0,
-            "context-menu-items": n.value
+            "allow-key-hooks": !0,
+            "context-menu-items": [{
+                label: "add_url_item",
+                labelArgs: [],
+                action: () => {
+                    d()
+                },
+                icon: "mdi-link-plus"
+            }]
         }, null, 8, ["items", "sort-keys", "update-available", "title", "context-menu-items"]))
     }
 });
 export {
     q as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryRadios-4a033696.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryRadios-2aa75500.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     _ as y
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     v as b,
     O as h,
     r as c,
     o as v,
     L as a,
     an as s,
@@ -13,32 +13,32 @@
     z as I,
     x as E,
     M as n,
     ao as l,
     ag as k,
     V as T,
     K as w
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
 const J = b({
     __name: "LibraryRadios",
     setup(A) {
         const {
             t: o
         } = h(), d = c([]), r = c(!1), m = {
             name: "sort_name",
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/LibraryTracks-eeccb967.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/LibraryArtists-af4c276c.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,96 +1,75 @@
 import {
-    _
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+    _ as c
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     v as f,
-    O as y,
-    r as m,
-    o as b,
-    L as a,
-    an as s,
-    b as k,
-    y as v,
-    z as h,
-    x as T,
-    M as i,
-    ao as n,
-    K as E
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-const q = f({
-    __name: "LibraryTracks",
-    setup(D) {
-        const {
-            t: l
-        } = y(), c = m([]), r = m(!1), u = {
-            name: "sort_name",
-            recent: "timestamp_added DESC",
-            artist: "sort_artist, sort_name",
-            album: "albums.sort_name, tracks.sort_name",
-            duration: "duration",
-            duration_desc: "duration DESC"
-        };
-        b(() => {
-            const t = a.subscribe_multi([s.MEDIA_ITEM_ADDED, s.MEDIA_ITEM_UPDATED, s.MEDIA_ITEM_DELETED], e => {
-                var o;
-                (o = e.object_id) != null && o.startsWith("library://track") && (r.value = !0)
+    r as n,
+    o as y,
+    L as e,
+    an as i,
+    b as _,
+    y as d,
+    z as b,
+    x as v,
+    M as m,
+    ao as r,
+    K as h
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+const F = f({
+    __name: "LibraryArtists",
+    setup(E) {
+        const p = n([]),
+            s = n(!1),
+            o = {
+                name: "sort_name",
+                recent: "timestamp_added DESC"
+            },
+            u = async function(t) {
+                if (t.refresh && !s.value) {
+                    for (e.startSync([m.ARTIST]), await r(250); e.syncTasks.value.length > 0 && e.syncTasks.value.filter(a => a.media_types.includes(m.ARTIST)).length != 0;) await r(500);
+                    await r(500)
+                }
+                return s.value = !1, await e.getLibraryArtists(t.favoritesOnly || void 0, t.search, t.limit, t.offset, o[t.sortBy], t.albumArtistsFilter)
+            };
+        return y(() => {
+            const t = e.subscribe_multi([i.MEDIA_ITEM_ADDED, i.MEDIA_ITEM_UPDATED, i.MEDIA_ITEM_DELETED], a => {
+                var l;
+                (l = a.object_id) != null && l.startsWith("library://artist") && (s.value = !0)
             });
-            k(t)
-        });
-        const p = async function(t) {
-            if (t.favoritesOnly = t.favoritesOnly || void 0, t.refresh && !r.value) {
-                for (a.startSync([i.TRACK]), await n(250); a.syncTasks.value.length > 0 && a.syncTasks.value.filter(e => e.media_types.includes(i.TRACK)).length != 0;) await n(500);
-                await n(500)
-            }
-            return r.value = !1, await a.getLibraryTracks(t.favoritesOnly, t.search, t.limit, t.offset, u[t.sortBy])
-        }, d = async function() {
-            const t = prompt(l("enter_url"));
-            t && a.getItem(i.TRACK, t, "builtin").then(e => {
-                const o = prompt(l("enter_name"), e.name);
-                e.name = o || e.name, a.addItemToLibrary(e).then(() => r.value = !0)
-            }).catch(e => alert(e))
-        };
-        return (t, e) => (v(), h(_, {
-            itemtype: "tracks",
-            items: c.value,
+            _(t)
+        }), (t, a) => (d(), b(c, {
+            itemtype: "artists",
+            items: p.value,
             "show-provider": !1,
             "show-favorites-only-filter": !0,
-            "show-track-number": !1,
-            "load-paged-data": p,
-            "sort-keys": Object.keys(u),
-            "show-album": !0,
-            "update-available": r.value,
-            title: T(E)("bp4") ? t.$t("tracks") : "",
-            "show-search-button": !0,
+            "load-paged-data": u,
+            "show-album-artists-only-filter": !0,
+            "update-available": s.value,
+            title: v(h)("bp4") ? t.$t("artists") : "",
             "allow-key-hooks": !0,
-            "context-menu-items": [{
-                label: "add_url_item",
-                labelArgs: [],
-                action: () => {
-                    d()
-                },
-                icon: "mdi-link-plus"
-            }]
-        }, null, 8, ["items", "sort-keys", "update-available", "title", "context-menu-items"]))
+            "show-search-button": !0,
+            "sort-keys": Object.keys(o)
+        }, null, 8, ["items", "update-available", "title", "sort-keys"]))
     }
 });
 export {
-    q as
+    F as
     default
 };
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ListviewItem-8b992256.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ListviewItem-04c2a02f.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -21,35 +21,35 @@
     M as d,
     L as P,
     aI as S,
     aq as H,
     ab as k,
     K as B,
     W as z
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     M as E,
     b as O
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     _ as K,
     L as U,
     a as W
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     a as q,
     c as y,
     b as G,
     _ as Q,
     V as _
-} from "./VTooltip-3ef94159.js";
+} from "./VTooltip-ebb61ea6.js";
 import {
     n as w,
     V as Y
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 const Z = {
         key: 0,
         class: "media-thumb listitem-media-thumb"
     },
     j = {
         key: 1,
         class: "media-thumb listitem-media-thumb"
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -18,40 +18,40 @@
     aI as M,
     Q as r,
     ab as N,
     aq as S,
     Z as D,
     K as L,
     H as z
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     M as A,
     b as H
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     L as E
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     a as R,
     b as O,
     c as u,
     V as P,
     _ as q
-} from "./VTooltip-3ef94159.js";
+} from "./VTooltip-ebb61ea6.js";
 import {
     f as G,
     g as K,
     c as v
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     n as k
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as Q
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 const W = {
         key: 0
     },
     Z = {
         key: 1
     },
     j = {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlayerQueue-9f89c917.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PlayerQueue-0a9bc504.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -23,63 +23,63 @@
     F as ie,
     G as ne,
     B as k,
     H as h,
     K as B,
     a3 as oe,
     M as re
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     L as se
-} from "./ListviewItem-8b992256.js";
+} from "./ListviewItem-04c2a02f.js";
 import {
     B as de,
     L as _,
     C as me
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     A as z
-} from "./Alert-19e36349.js";
+} from "./Alert-f8f9596c.js";
 import {
     V as D
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     a as G,
     V as pe
-} from "./VTabs-8ad24bfd.js";
+} from "./VTabs-9b65d90e.js";
 import {
     n as g,
     l as I,
     k as P
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     b as H,
     e as ve,
     d as b
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     V as J,
     a as O
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     V as ce
-} from "./VVirtualScroll-84259ceb.js";
+} from "./VVirtualScroll-acb73766.js";
 import {
     V as fe
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     V as _e
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     V as ye
-} from "./VDialog-d7e50927.js";
-import "./VTooltip-3ef94159.js";
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js"; /* empty css              */
-import "./VAlert-56af8987.js";
+} from "./VDialog-7155dc5f.js";
+import "./VTooltip-ebb61ea6.js";
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js"; /* empty css              */
+import "./VAlert-ed4cb12a.js";
 const ge = k("br", null, null, -1),
     be = {
         key: 0
     },
     Se = Y({
         __name: "PlayerQueue",
         setup(qe) {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Players-0e31a251.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Players-23776fba.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -19,35 +19,35 @@
     n as O,
     F as C,
     G as h,
     I as k,
     af as S,
     x as d,
     B as V
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     C as j,
     L as A,
     _ as E,
     B
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     l as Q,
     n as N
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as W
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     e as q
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     V as H
-} from "./VToolbar-b7f10b15.js"; /* empty css              */
-import "./VCardText-6774ea5e.js";
+} from "./VToolbar-c9911418.js"; /* empty css              */
+import "./VCardText-35ed9014.js";
 const J = {
         style: {
             "margin-bottom": "10px"
         }
     },
     K = {
         class: "line-clamp-1"
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/PlaylistDetails-2fe134b1.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/PlaylistDetails-59d16a22.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,48 @@
 import {
     _ as v
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     _ as y,
     a as _
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js";
 import {
     v as k,
     r as n,
     w as b,
     o as h,
     L as r,
     an as w,
     b as I,
     y as l,
     E as D,
     l as E,
     z as p,
     I as u,
     ao as T
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-import "./layout-42b7d22e.js";
-import "./VDialog-d7e50927.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+import "./layout-f1bc9409.js";
+import "./VDialog-7155dc5f.js";
 const S = k({
     __name: "PlaylistDetails",
     props: {
         itemId: {},
         provider: {}
     },
     setup(c) {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails-2713c080.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ProviderDetails-2713c080.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,179 +1,180 @@
 import {
     p as W,
     g as Z,
     l as t,
-    v as G,
-    r as P,
+    v as Y,
+    r as H,
     f as X,
     aa as M,
     O as ee,
     w as te,
     c as z,
     y as i,
     E as p,
     A as a,
     z as u,
     I as d,
-    x as y,
+    x as c,
     H as T,
     B as v,
     Q as w,
     N as r,
     n as N,
     F as I,
     G as B,
     ag as F,
     J as U,
-    M as R,
+    M as D,
     aq as ie,
-    L as A,
+    L as P,
     ar as ae,
     Z as oe,
     K as le
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     B as x,
-    _ as Y,
+    _ as G,
     L as q,
     C as se
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     M as S,
     g as j,
     b as ne
-} from "./VBadge-84e3406b.js";
+} from "./VBadge-e60e80c3.js";
 import {
     e as re,
     a as me
-} from "./contextmenu-521b5304.js";
+} from "./contextmenu-c35de49a.js";
 import {
     a as de,
     i as ue,
     V as J,
     n as $,
-    l as D,
+    l as A,
     v as pe,
     k as ce
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     d as E,
     e as ye,
     b as O
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     a as fe,
     V as ge
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 import {
     a as V,
     V as K,
     b as ve
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     V as be
-} from "./VTooltip-3ef94159.js";
+} from "./VTooltip-ebb61ea6.js";
 import {
     b as he,
     c as ke
-} from "./layout-42b7d22e.js";
-import {
-    V as Ce
-} from "./VDialog-d7e50927.js";
+} from "./layout-f1bc9409.js";
 import {
     V as _e
-} from "./VInput-5b197ccd.js";
+} from "./VDialog-7155dc5f.js";
+import {
+    V as Ce
+} from "./VInput-8a0f3c4b.js";
 import {
     V as $e
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 const Ve = W({
         ...de(),
         ...he()
     }, "VLayout"),
     we = Z()({
         name: "VLayout",
         props: Ve(),
         setup(h, m) {
             let {
-                slots: c
+                slots: y
             } = m;
             const {
                 layoutClasses: k,
                 layoutStyles: L,
                 getLayoutItem: n,
                 items: f,
                 layoutRef: g
             } = ke(h);
             return ue(() => {
                 var o;
                 return t("div", {
                     ref: g,
                     class: [k.value, h.class],
                     style: [L.value, h.style]
-                }, [(o = c.default) == null ? void 0 : o.call(c)])
+                }, [(o = y.default) == null ? void 0 : o.call(y)])
             }), {
                 getLayoutItem: n,
                 items: f
             }
         }
     }),
     Le = {
         key: 0,
         xs5: "",
         "pa-5": "",
         style: {
-            width: "230px",
-            height: "230px",
+            height: "100%",
+            "min-width": "230px",
             "margin-top": "15px",
             "margin-bottom": "15px",
-            "margin-right": "24px"
+            "margin-right": "24px",
+            "align-content": "center"
         }
     },
     Te = {
         key: 0
     },
     Ie = {
         key: 1
     },
     Be = {
         style: {
             "padding-bottom": "10px"
         }
     },
-    De = ["onClick"],
-    Re = {
+    Ae = ["onClick"],
+    De = {
         style: {
             color: "primary"
         }
     },
-    Ae = {
+    Pe = {
         style: {
             display: "flex",
             "margin-left": "14px",
             "padding-bottom": "10px"
         }
     },
-    He = ["innerHTML"],
-    Pe = {
+    Re = ["innerHTML"],
+    He = {
         key: 1,
         class: "justify-center",
         style: {
             "margin-left": "15px",
             "padding-bottom": "20px"
         }
     },
-    Xe = G({
+    Xe = Y({
         __name: "InfoHeader",
         props: {
             item: {}
         },
         setup(h) {
             const m = h,
-                c = P(!1),
-                k = P(),
+                y = H(!1),
+                k = H(),
                 {
                     mobile: L
                 } = X(),
                 n = new URL("" + new URL("info_gradient-a4aefd1d.jpg", import.meta.url).href, self.location).href,
                 f = M();
             ee(), te(() => m.item, async e => {
                 e && (k.value = j(m.item, F.FANART) || j(m.item, F.THUMB))
@@ -194,29 +195,29 @@
                         name: "artist",
                         params: {
                             itemId: e.item_id,
                             provider: e.provider
                         }
                     })
                 },
-                C = z(() => {
+                _ = z(() => {
                     let e = "";
                     return m.item ? (m.item.metadata && m.item.metadata.description ? e = m.item.metadata.description : m.item.metadata && m.item.metadata.copyright ? e = m.item.metadata.copyright : "artists" in m.item && m.item.artists.forEach(function(l) {
                         "metadata" in l && l.metadata.description && (e = l.metadata.description)
                     }), e = e.replace(`\r
 `, "<br /><br /><br />"), e = e.replace("\r", "<br /><br />"), e = e.replace(`
 `, "<br /><br />"), e) : ""
                 }),
-                H = z(() => {
+                R = z(() => {
                     const e = L.value ? 160 : 260;
-                    return C.value.length > e ? C.value.substring(0, e) + "..." : C.value
+                    return _.value.length > e ? _.value.substring(0, e) + "..." : _.value
                 });
             return (e, l) => (i(), p("div", null, [t(K, {
                 variant: "flat",
-                img: y(n),
+                img: c(n),
                 style: {
                     "margin-top": "-10px",
                     "z-index": "0"
                 },
                 height: "30vh",
                 "max-height": "500px",
                 "min-height": "340px"
@@ -227,66 +228,66 @@
                 })), t(J, {
                     width: "100%",
                     height: "100%",
                     cover: "",
                     class: "background-image",
                     src: k.value,
                     gradient: e.$vuetify.theme.current.dark ? "to bottom, rgba(0,0,0,.90), rgba(0,0,0,.75)" : "to bottom, rgba(255,255,255,.90), rgba(255,255,255,.75)"
-                }, null, 8, ["src", "gradient"]), y(U).prevScrollName ? (i(), u(x, {
+                }, null, 8, ["src", "gradient"]), c(U).prevScrollName ? (i(), u(x, {
                     key: 1,
                     "xx-large": "",
                     style: {
                         position: "absolute",
                         width: "40px, height:40px",
-                        right: "4px",
+                        left: "4px",
                         top: "10px"
                     },
                     icon: "mdi-arrow-left",
                     title: e.$t("tooltip.back"),
-                    onClick: l[0] || (l[0] = T(_ => y(f).go(-1), ["stop"]))
+                    onClick: l[0] || (l[0] = T(C => c(f).go(-1), ["stop"]))
                 }, null, 8, ["title"])) : d("", !0), e.item ? (i(), u(we, {
                     key: 2,
                     style: {
                         margin: "0",
                         position: "absolute",
                         top: "50%",
                         "-ms-transform": "translateY(-50%)",
                         transform: "translateY(-50%)",
                         "padding-left": "15px",
                         "align-items": "center",
                         "padding-right": "15px"
                     }
                 }, {
                     default: a(() => {
-                        var _;
-                        return [e.$vuetify.display.mobile ? d("", !0) : (i(), p("div", Le, [e.item.media_type && (e.item.media_type == y(R).ARTIST || "owner" in e.item) ? (i(), p("div", Te, [t(E, {
+                        var C;
+                        return [e.$vuetify.display.mobile ? d("", !0) : (i(), p("div", Le, [e.item.media_type && [c(D).ARTIST, c(D).PLAYLIST].includes(e.item.media_type) ? (i(), p("div", Te, [t(E, {
                             size: "192"
                         }, {
                             default: a(() => [t(S, {
                                 item: e.item,
-                                height: 230,
-                                width: 230
+                                height: 300,
+                                width: 300
                             }, null, 8, ["item"])]),
                             _: 1
                         })])) : (i(), p("div", Ie, [t(S, {
-                            width: 230,
+                            width: 300,
                             item: e.item
                         }, null, 8, ["item"])]))])), v("div", null, [t(fe, null, {
                             default: a(() => [w(r(e.item.name), 1)]),
                             _: 1
                         }), v("div", Be, ["version" in e.item && e.item.version ? (i(), u(V, {
                             key: 0,
                             class: "caption"
                         }, {
                             default: a(() => [w(r(e.item.version) + " ", 1), t(be, {
                                 location: "bottom"
                             }, {
                                 activator: a(({
                                     props: s
-                                }) => [y(ie)(e.item.metadata.explicit || !1) ? (i(), u($, N({
+                                }) => [c(ie)(e.item.metadata.explicit || !1) ? (i(), u($, N({
                                     key: 0
                                 }, s, {
                                     icon: "mdi-alpha-e-box",
                                     width: "35"
                                 }), null, 16)) : d("", !0)]),
                                 default: a(() => [v("span", null, r(e.$t("tooltip.explicit")), 1)]),
                                 _: 1
@@ -307,15 +308,15 @@
                             }), (i(!0), p(I, null, B(e.item.artists, (s, b) => (i(), p("span", {
                                 key: s.item_id
                             }, [v("a", {
                                 style: {
                                     color: "accent"
                                 },
                                 onClick: Q => o(s)
-                            }, r(s.name), 9, De), b + 1 < e.item.artists.length ? (i(), p("span", {
+                            }, r(s.name), 9, Ae), b + 1 < e.item.artists.length ? (i(), p("span", {
                                 key: b,
                                 style: {
                                     color: "accent"
                                 }
                             }, r(" / "))) : d("", !0)]))), 128))]),
                             _: 1
                         })) : d("", !0), "artist" in e.item && e.item.artist ? (i(), u(V, {
@@ -342,15 +343,15 @@
                                 color: "primary",
                                 style: {
                                     "margin-left": "-3px",
                                     "margin-right": "3px"
                                 },
                                 small: "",
                                 icon: "mdi-account-music"
-                            }), v("a", Re, r(e.item.owner), 1)]),
+                            }), v("a", De, r(e.item.owner), 1)]),
                             _: 1
                         })) : d("", !0), "album" in e.item && e.item.album ? (i(), u(V, {
                             key: 4
                         }, {
                             default: a(() => [t($, {
                                 color: "primary",
                                 style: {
@@ -365,19 +366,19 @@
                                 },
                                 onClick: l[2] || (l[2] = s => {
                                     var b;
                                     return g((b = e.item) == null ? void 0 : b.album)
                                 })
                             }, r(e.item.album.name), 1)]),
                             _: 1
-                        })) : d("", !0)]), v("div", Ae, [t(D, {
+                        })) : d("", !0)]), v("div", Pe, [t(A, {
                             color: "primary",
                             "prepend-icon": "mdi-play-circle",
-                            disabled: !((_ = y(U).selectedPlayer) != null && _.available),
-                            onClick: l[3] || (l[3] = s => y(re).emit("playdialog", {
+                            disabled: !((C = c(U).selectedPlayer) != null && C.available),
+                            onClick: l[3] || (l[3] = s => c(re).emit("playdialog", {
                                 items: [e.item],
                                 parentItem: e.item,
                                 showContextMenuItems: !1
                             }))
                         }, {
                             default: a(() => [w(r(e.$t("play")), 1)]),
                             _: 1
@@ -392,59 +393,59 @@
                             }, s), {
                                 default: a(() => [t($, {
                                     icon: "mdi-dots-vertical"
                                 })]),
                                 _: 2
                             }, 1040)]),
                             default: a(() => [t(O, null, {
-                                default: a(() => [(i(!0), p(I, null, B(y(me)([e.item], e.item).filter(s => s.hide != !0), (s, b) => (i(), u(q, {
+                                default: a(() => [(i(!0), p(I, null, B(c(me)([e.item], e.item).filter(s => s.hide != !0), (s, b) => (i(), u(q, {
                                     key: b,
                                     title: e.$t(s.label, s.labelArgs),
                                     disabled: s.disabled == !0,
                                     onClick: Q => s.action ? s.action() : ""
                                 }, {
                                     prepend: a(() => [t(E, {
                                         icon: s.icon
                                     }, null, 8, ["icon"])]),
                                     _: 2
                                 }, 1032, ["title", "disabled", "onClick"]))), 128))]),
                                 _: 1
                             })]),
                             _: 1
-                        }), t(D, {
+                        }), t(A, {
                             variant: "plain",
                             ripple: "",
                             icon: e.item.favorite ? "mdi-heart" : "mdi-heart-outline",
                             size: "x-large",
                             style: {
                                 "margin-top": "-14px"
                             },
                             title: e.$t("tooltip.favorite"),
-                            onClick: [l[4] || (l[4] = s => y(A).toggleFavorite(e.item)), l[5] || (l[5] = T(() => {}, ["prevent"])), l[6] || (l[6] = T(() => {}, ["stop"]))]
-                        }, null, 8, ["icon", "title"]), t(Y, {
+                            onClick: [l[4] || (l[4] = s => c(P).toggleFavorite(e.item)), l[5] || (l[5] = T(() => {}, ["prevent"])), l[6] || (l[6] = T(() => {}, ["stop"]))]
+                        }, null, 8, ["icon", "title"]), t(G, {
                             domain: e.item.provider,
                             size: 25,
                             style: {
                                 "margin-top": "4px"
                             }
-                        }, null, 8, ["domain"])]), H.value ? (i(), u(V, {
+                        }, null, 8, ["domain"])]), R.value ? (i(), u(V, {
                             key: 0,
                             class: "body-2 justify-left",
                             style: {
                                 "padding-bottom": "10px",
                                 "white-space": "pre-line",
                                 cursor: "pointer"
                             },
-                            onClick: l[7] || (l[7] = s => c.value = !c.value)
+                            onClick: l[7] || (l[7] = s => y.value = !y.value)
                         }, {
                             default: a(() => [v("div", {
-                                innerHTML: H.value
-                            }, null, 8, He)]),
+                                innerHTML: R.value
+                            }, null, 8, Re)]),
                             _: 1
-                        })) : d("", !0), e.item && e.item.metadata.genres ? (i(), p("div", Pe, [(i(!0), p(I, null, B(e.item.metadata.genres.slice(0, e.$vuetify.display.mobile ? 15 : 25), s => (i(), u(_e, {
+                        })) : d("", !0), e.item && e.item.metadata.genres ? (i(), p("div", He, [(i(!0), p(I, null, B(e.item.metadata.genres.slice(0, e.$vuetify.display.mobile ? 15 : 25), s => (i(), u(Ce, {
                             key: s,
                             color: "blue-grey lighten-1",
                             style: {
                                 "margin-right": "5px",
                                 "margin-bottom": "5px"
                             },
                             small: "",
@@ -453,28 +454,28 @@
                             default: a(() => [w(r(s), 1)]),
                             _: 2
                         }, 1024))), 128))])) : d("", !0)])]
                     }),
                     _: 1
                 })) : d("", !0)]),
                 _: 1
-            }, 8, ["img"]), t(Ce, {
-                modelValue: c.value,
-                "onUpdate:modelValue": l[9] || (l[9] = _ => c.value = _),
+            }, 8, ["img"]), t(_e, {
+                modelValue: y.value,
+                "onUpdate:modelValue": l[9] || (l[9] = C => y.value = C),
                 "max-width": "975",
                 width: "auto"
             }, {
                 default: a(() => [t(K, null, {
                     default: a(() => [t(ge, {
-                        innerHTML: C.value
+                        innerHTML: _.value
                     }, null, 8, ["innerHTML"]), t(ve, null, {
-                        default: a(() => [t(D, {
+                        default: a(() => [t(A, {
                             color: "primary",
                             block: "",
-                            onClick: l[8] || (l[8] = _ => c.value = !1)
+                            onClick: l[8] || (l[8] = C => y.value = !1)
                         }, {
                             default: a(() => [w(r(e.$t("close")), 1)]),
                             _: 1
                         })]),
                         _: 1
                     })]),
                     _: 1
@@ -489,81 +490,81 @@
         }
     },
     Ne = {
         key: 0
     },
     Fe = ["title", "onClick"],
     Ue = ["title"],
-    Me = G({
+    Me = Y({
         __name: "ProviderDetails",
         props: {
             itemDetails: {}
         },
         setup(h) {
             const m = function(n) {
                     window.open(n, "_blank")
                 },
-                c = ae({}),
+                y = ae({}),
                 k = function(n) {
                     const f = `${n.provider_instance}.${n.item_id}`,
-                        g = c[f];
-                    if (g) g.load(), delete c[f];
+                        g = y[f];
+                    if (g) g.load(), delete y[f];
                     else {
                         const o = new Audio(L(n.provider_instance, n.item_id));
-                        c[f] = o, o.play()
+                        y[f] = o, o.play()
                     }
                 },
                 L = function(n, f) {
-                    return `${A.baseUrl}/preview?item_id=${encodeURIComponent(f)}&provider=${n}`
+                    return `${P.baseUrl}/preview?item_id=${encodeURIComponent(f)}&provider=${n}`
                 };
             return (n, f) => (i(), p("section", ze, [t($e, {
                 color: "transparent",
                 title: n.$t("mapped_providers"),
                 style: {
                     height: "55px"
                 }
             }, null, 8, ["title"]), t(ce), t(se, null, {
                 default: a(() => [t(O, null, {
                     default: a(() => {
                         var g;
                         return [(i(!0), p(I, null, B((g = n.itemDetails) == null ? void 0 : g.provider_mappings, o => (i(), u(q, {
                             key: o.provider_instance
                         }, {
-                            prepend: a(() => [t(Y, {
+                            prepend: a(() => [t(G, {
                                 domain: o.provider_domain,
                                 size: 30
                             }, null, 8, ["domain"])]),
-                            title: a(() => [w(r(y(A).providerManifests[o.provider_domain].name), 1)]),
-                            subtitle: a(() => [n.itemDetails.media_type == y(R).TRACK && o.audio_format ? (i(), p("span", Ne, r(o.audio_format.content_type) + " | " + r(o.audio_format.sample_rate / 1e3) + "kHz/" + r(o.audio_format.bit_depth) + " bits | ", 1)) : d("", !0), o.url && !o.provider_domain.startsWith("file") ? (i(), p("a", {
+                            title: a(() => [w(r(c(P).providerManifests[o.provider_domain].name), 1)]),
+                            subtitle: a(() => [n.itemDetails.media_type == c(D).TRACK && o.audio_format ? (i(), p("span", Ne, r(o.audio_format.content_type) + " | " + r(o.audio_format.sample_rate / 1e3) + "kHz/" + r(o.audio_format.bit_depth) + " bits | ", 1)) : d("", !0), o.url && !o.provider_domain.startsWith("file") ? (i(), p("a", {
                                 key: 1,
                                 style: {
                                     opacity: "0.4"
                                 },
                                 title: n.$t("tooltip.open_provider_link"),
-                                onClick: T(C => m(o.url), ["prevent"])
+                                onClick: T(_ => m(o.url), ["prevent"])
                             }, r(o.url), 9, Fe)) : (i(), p("span", {
                                 key: 2,
                                 style: {
                                     opacity: "0.4"
                                 },
                                 title: o.item_id
                             }, r(o.item_id), 9, Ue))]),
                             append: a(() => [o.audio_format && o.audio_format.bit_depth > 16 ? (i(), u(J, {
                                 key: 0,
-                                src: y(ne),
+                                src: c(ne),
                                 width: "30",
                                 class: oe(n.$vuetify.theme.current.dark ? "hiresicondark" : "hiresicon"),
                                 style: {
                                     "margin-right": "15px"
                                 }
-                            }, null, 8, ["src", "class"])) : d("", !0), y(le)("bp1") && n.itemDetails.media_type == y(R).TRACK ? (i(), u(D, {
+                            }, null, 8, ["src", "class"])) : d("", !0), c(le)("bp1") && n.itemDetails.media_type == c(D).TRACK ? (i(), u(A, {
                                 key: 1,
-                                icon: c[`${o.provider_instance}.${o.item_id}`] ? "mdi-pause" : "mdi-play-circle",
+                                icon: y[`${o.provider_instance}.${o.item_id}`] ? "mdi-pause" : "mdi-play-circle",
                                 title: n.$t("tooltip.play_sample"),
-                                onClick: C => k(o)
+                                onClick: _ => k(o)
                             }, null, 8, ["icon", "title", "onClick"])) : d("", !0)]),
                             _: 2
                         }, 1024))), 128))]
                     }),
                     _: 1
                 })]),
                 _: 1
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Providers-58a591e0.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Providers-c5daf86a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,40 +22,40 @@
     n as J,
     I as v,
     aQ as b,
     B as h,
     af as K,
     a8 as T,
     a9 as W
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     L as B,
     _ as S,
     B as g,
     C as X,
     a as Y
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     A as Z
-} from "./Alert-19e36349.js";
+} from "./Alert-f8f9596c.js";
 import {
     e as ee
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     l as ne,
     n as y
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as te
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 import {
     V as ae
-} from "./VToolbar-b7f10b15.js"; /* empty css              */
-import "./VAlert-56af8987.js";
-import "./VCardText-6774ea5e.js";
+} from "./VToolbar-c9911418.js"; /* empty css              */
+import "./VAlert-ed4cb12a.js";
+import "./VCardText-35ed9014.js";
 const ie = p => (T("data-v-15cfe784"), p = p(), W(), p),
     se = ie(() => h("br", null, null, -1)),
     oe = {
         class: "line-clamp-1"
     },
     de = {
         class: "line-clamp-1"
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/RadioDetails-54e9e340.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/RadioDetails-5f7de0e3.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,46 +1,46 @@
 import {
     _ as u
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     _ as f,
     a as v
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js";
 import {
     v as _,
     r as h,
     w as y,
     y as a,
     E as w,
     l as V,
     z as m,
     I as n,
     B as k,
     L as s,
     ap as g
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-import "./layout-42b7d22e.js";
-import "./VDialog-d7e50927.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+import "./layout-f1bc9409.js";
+import "./VDialog-7155dc5f.js";
 const I = k("br", null, null, -1),
     T = _({
         __name: "RadioDetails",
         props: {
             itemId: {},
             provider: {}
         },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Search-00ee9dd8.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Search-d1673cac.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     V as $,
     _ as B,
     a as I
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     v as F,
     r as o,
     w as L,
     o as _,
     b as C,
     y as i,
@@ -16,38 +16,38 @@
     Q as E,
     N,
     F as b,
     G as V,
     L as R,
     z as g,
     I as x
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     V as D
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     k as P
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as U
-} from "./VTextField-0c2ec62d.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VVirtualScroll-84259ceb.js";
+} from "./VTextField-95a689ca.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VVirtualScroll-acb73766.js";
 const le = F({
     __name: "Search",
     props: {
         initSearch: {}
     },
     setup(w) {
         const p = w,
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/Settings-bbdb2168.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/Settings-34342ef5.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -10,26 +10,26 @@
     Q as o,
     N as s,
     x as _,
     z as V,
     S as y,
     B as h,
     K as b
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     V as B,
     a as n
-} from "./VTabs-8ad24bfd.js";
+} from "./VTabs-9b65d90e.js";
 import {
     V as k
-} from "./VToolbar-b7f10b15.js";
+} from "./VToolbar-c9911418.js";
 import {
     k as S
-} from "./forwardRefs-7be90dc2.js";
-import "./VSlideGroup-b576aa37.js";
+} from "./forwardRefs-708ed339.js";
+import "./VSlideGroup-c7be05c1.js";
 const T = h("div", {
         style: {
             height: "15px"
         }
     }, null, -1),
     x = d({
         __name: "Settings",
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/TrackDetails-72029d5e.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/TrackDetails-40ca37ef.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     _ as d
-} from "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js";
+} from "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js";
 import {
     _ as w,
     a as I
-} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js";
+} from "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js";
 import {
     v as T,
     r as n,
     c as g,
     ap as c,
     w as D,
     o as A,
@@ -17,34 +17,34 @@
     b as E,
     y as l,
     E as M,
     l as V,
     z as u,
     I as p,
     B as f
-} from "./index-b687f95a.js";
-import "./ListviewItem-8b992256.js";
-import "./VBadge-84e3406b.js";
-import "./Container-dc894acd.js";
-import "./forwardRefs-7be90dc2.js";
-import "./VMenu-b634019c.js"; /* empty css              */
-import "./VInput-5b197ccd.js";
-import "./VSlideGroup-b576aa37.js";
-import "./VCard-b98fe47e.js";
-import "./VCardText-6774ea5e.js";
-import "./VTooltip-3ef94159.js";
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js";
-import "./contextmenu-521b5304.js";
-import "./Alert-19e36349.js";
-import "./VAlert-56af8987.js";
-import "./VToolbar-b7f10b15.js";
-import "./VTextField-0c2ec62d.js";
-import "./VVirtualScroll-84259ceb.js";
-import "./layout-42b7d22e.js";
-import "./VDialog-d7e50927.js";
+} from "./index-e734c256.js";
+import "./ListviewItem-04c2a02f.js";
+import "./VBadge-e60e80c3.js";
+import "./Container-235383e5.js";
+import "./forwardRefs-708ed339.js";
+import "./VMenu-ec95eec6.js"; /* empty css              */
+import "./VInput-8a0f3c4b.js";
+import "./VSlideGroup-c7be05c1.js";
+import "./VCard-4532b814.js";
+import "./VCardText-35ed9014.js";
+import "./VTooltip-ebb61ea6.js";
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js";
+import "./contextmenu-c35de49a.js";
+import "./Alert-f8f9596c.js";
+import "./VAlert-ed4cb12a.js";
+import "./VToolbar-c9911418.js";
+import "./VTextField-95a689ca.js";
+import "./VVirtualScroll-acb73766.js";
+import "./layout-f1bc9409.js";
+import "./VDialog-7155dc5f.js";
 const $ = f("br", null, null, -1),
     F = f("br", null, null, -1),
     te = T({
         __name: "TrackDetails",
         props: {
             itemId: {},
             provider: {},
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-1c823677.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VAlert-1c823677.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VAlert-56af8987.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VAlert-ed4cb12a.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     h as I
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     a as L,
     o as $,
     T as z,
     b as E,
     y as F,
     z as R,
@@ -19,28 +19,28 @@
     C as U,
     g as G,
     J as H,
     E as K,
     n as Q,
     j as d,
     l as W
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as X,
     aL as Y,
     d as Z,
     g as ee,
     h as te,
     c as o,
     e as ae,
     t as le,
     aM as ne,
     l as a,
     n as se
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 const oe = I("v-alert-title"),
     re = ["success", "info", "warning", "error"],
     ie = X({
         border: {
             type: [Boolean, String],
             validator: e => typeof e == "boolean" || ["top", "end", "bottom", "start"].includes(e)
         },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-84e3406b.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VBadge-e60e80c3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -27,46 +27,46 @@
     d as G,
     g as K,
     t as H,
     aM as Q,
     aN as W,
     af as j,
     aO as q
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     _,
     a as $
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     V as ee
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 import {
     b as te,
     V as ae,
     g as ie,
     e as ne
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     k as Ae,
     a as se,
     y as oe,
     c as re,
     d as le,
     I as ce,
     e as ue,
     g as ge,
     J as me,
     B as fe,
     i as de,
     M as he,
     n as be
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     V as ke
-} from "./VCard-b98fe47e.js";
+} from "./VCard-4532b814.js";
 const Re = "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACQAAAAkCAYAAADhAJiYAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QAAAAAAAD5Q7t/AAAACXBIWXMAAABgAAAAYADwa0LPAAAAnElEQVRYw+2UwQ6AMAhDwfjh+OXzZrgslqxjW8K7GWdtRqlIUYyh/qG1Zt8LVYuKzTDUnCGNy41zrfhpGRrhZgn5/HmiWdzuhsrQH7QMicjDENmuGKEbQjaotiwLaGSZeUIzZB2jhnwfAdqyzFAze+gXxPSZxcgaB6JDa+rUDLG2DNFJ3TLkzDlN3bveGWc83ZFlctTIKOVWFCt5AYSDaENMYFhMAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIyLTA0LTE1VDEzOjExOjE0KzAwOjAwADepDgAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMi0wNC0xNVQxMzoxMToxNCswMDowMHFqEbIAAAAASUVORK5CYII=",
     Be = {
         class: "d-flex justify-center",
         style: {
             width: "100%"
         }
     },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VBadge-8b8b8a6d.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VBadge-8b8b8a6d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-257d0eab.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VCard-257d0eab.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VCard-b98fe47e.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VCard-4532b814.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,36 +24,36 @@
     B as ie,
     C as le,
     g as se,
     Y as ce,
     V as re,
     R as ue,
     E as oe
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     g as f,
     k as ve,
     l as n,
     p as S,
     aL as u,
     F as A,
     d as me,
     e as ye,
     c as p,
     af as ke,
     ae as ge
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     h as be,
     d as h
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     a as fe,
     V as Ce
-} from "./VCardText-6774ea5e.js";
+} from "./VCardText-35ed9014.js";
 const Ie = f()({
         name: "VCardActions",
         props: g(),
         setup(e, i) {
             let {
                 slots: t
             } = i;
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-5309eac2.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VDialog-5309eac2.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VDialog-d7e50927.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VDialog-7155dc5f.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 import {
     m as b,
     k as y,
     a as D,
     f
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     i as h,
     j as S,
     F as w
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as x,
     g as F,
     h as B,
     r as I,
     aX as R,
     w as v,
     q as T,
     c as k,
     n as m,
     l as g,
     aY as L
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 const O = x({
         fullscreen: Boolean,
         retainFocus: {
             type: Boolean,
             default: !0
         },
         scrollable: Boolean,
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VExpansionPanel-58c5fe02.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VExpansionPanel-8b2da313.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     h as Be,
     F as Le,
     n as ze,
     d as Me,
     e as Re,
     k as be,
     aL as ue
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     c as pe,
     b as ye,
     a as G,
     S as he,
     f as ke,
     J as Ne,
@@ -39,26 +39,26 @@
     p as $e,
     d as Se,
     r as De,
     O as Oe,
     n as je,
     G as qe,
     H as Ke
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     g as Ge,
     m as Ue,
     u as We,
     b as ce,
     f as Xe
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 import {
     i as ge,
     j as Ye
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 const se = Symbol.for("vuetify:v-slider");
 
 function He(e, a, l) {
     const t = l === "vertical",
         i = a.getBoundingClientRect(),
         m = "touches" in e ? e.touches[0] : e;
     return t ? m.clientY - (i.top + i.height / 2) : m.clientX - (i.left + i.width / 2)
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VForm-fc99b4aa.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VForm-7178cd98.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 import {
     a as p,
     i as v,
     F as b
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     h as F,
     i as V
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 import {
     p as h,
     g as y,
     r as R,
     l as P
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 const k = h({
         ...p(),
         ...F()
     }, "VForm"),
     S = y()({
         name: "VForm",
         props: k(),
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VGrid-37b0738d.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VGrid-37b0738d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-5b197ccd.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VInput-8a0f3c4b.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -32,15 +32,15 @@
     w as j,
     x as Ae,
     j as Me,
     b as $e,
     o as _e,
     i as ae,
     u as De
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     a as E,
     p as Fe,
     d as me,
     A as ye,
     r as we,
     i as z,
@@ -65,22 +65,22 @@
     n as L,
     j as q,
     J as be,
     e as Je,
     I as Ze,
     Z as Qe,
     M as We
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     m as ea,
     V as le
-} from "./VSlideGroup-b576aa37.js";
+} from "./VSlideGroup-c7be05c1.js";
 import {
     d as te
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 const Ve = Symbol.for("vuetify:v-chip-group"),
     aa = x({
         column: Boolean,
         filter: Boolean,
         valueComparator: {
             type: Function,
             default: se
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VInput-b16e222c.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VInput-b16e222c.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-a46f5e7a.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VMenu-a46f5e7a.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VMenu-b634019c.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VMenu-ec95eec6.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -53,15 +53,15 @@
     f as mn,
     ar as xt,
     u as yn,
     bk as gn,
     bl as hn,
     aY as at,
     bm as bn
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     a as ae,
     L as ue,
     a4 as Sn,
     N as Ie,
     a5 as wn,
     a6 as Ot,
@@ -101,15 +101,15 @@
     ab as Ee,
     ac as it,
     ad as rt,
     I as Ln,
     h as In,
     ae as Bn,
     F as Tn
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 const ye = new WeakMap;
 
 function Mn(e, n) {
     Object.keys(n).forEach(t => {
         if (St(t)) {
             const a = wt(t),
                 o = ye.get(e);
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-7df244e0.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSelect-7df244e0.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSelect-d10e917f.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSelect-da46c348.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     m as re,
     V as N
-} from "./VTextField-0c2ec62d.js";
+} from "./VTextField-95a689ca.js";
 import {
     s as Q,
     w as E,
     p as X,
     aL as ce,
     aC as de,
     g as fe,
@@ -18,39 +18,39 @@
     F as O,
     n as x,
     aZ as pe,
     Q as he,
     a_ as ye,
     q as ge,
     a$ as j
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     j as Ve,
     c as ke,
     V as we
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 import {
     I as be,
     i as Ce,
     n as z,
     j as Pe,
     F as xe
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     l as Se,
     k as De,
     n as Te,
     e as Ie,
     b as Ae,
     V as W,
     d as Fe
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 import {
     V as Le
-} from "./VVirtualScroll-84259ceb.js";
+} from "./VVirtualScroll-acb73766.js";
 
 function Re(e, B) {
     const n = Q(!1);
     let y;
 
     function m(i) {
         cancelAnimationFrame(y), n.value = !0, y = requestAnimationFrame(() => {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-b576aa37.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSlideGroup-c7be05c1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,30 +3,30 @@
     d as ee,
     p as te,
     r as le,
     w as H,
     i as ae,
     a3 as G,
     n as L
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as ne,
     aL as $,
     m as se,
     g as ue,
     u as oe,
     f as ie,
     s as x,
     c as S,
     aX as ce,
     w as re,
     l as h,
     aY as ve,
     aV as fe
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 
 function X(a) {
     const s = Math.abs(a);
     return Math.sign(a) * (s / ((1 / .501 - 2) * (1 - s) + 1))
 }
 
 function Y(a) {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VSlideGroup-c5ba1538.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-11e16be1.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTabs-11e16be1.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTabs-8ad24bfd.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTabs-9b65d90e.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -6,34 +6,34 @@
     F as X,
     L as Y,
     N as j,
     o as J,
     d as K,
     q as L,
     e as W
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as R,
     aC as p,
     g as F,
     r as E,
     c as V,
     l as f,
     F as Q,
     n as T,
     h as Z,
     t as n,
     k as ee,
     a as te,
     aP as ae
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     m as se,
     V as M
-} from "./VSlideGroup-b576aa37.js";
+} from "./VSlideGroup-c7be05c1.js";
 const G = Symbol.for("vuetify:v-tabs"),
     oe = R({
         fixed: Boolean,
         sliderColor: String,
         hideSlider: Boolean,
         direction: {
             type: String,
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-0c2ec62d.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTextField-95a689ca.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
     b2 as be,
     h as xe,
     aK as Ce,
     ae as ke,
     b3 as Ve,
     q as p,
     b4 as he
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     a as H,
     I as _e,
     Z as Ie,
     i as K,
     M as Pe,
     W as Fe,
@@ -42,23 +42,23 @@
     L as $e,
     R as Ae,
     $ as De,
     j as Ee,
     N as Me,
     a0 as Ne,
     F as Oe
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     f as Ue,
     g as Ke,
     u as te,
     k as je,
     m as We,
     b as ee
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 const qe = O({
         active: Boolean,
         max: [Number, String],
         value: {
             type: [Number, String],
             default: 0
         },
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTextField-d31117f3.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTextField-d31117f3.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-78a5e824.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VToolbar-78a5e824.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VToolbar-b7f10b15.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VToolbar-c9911418.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,28 +8,28 @@
     e as D,
     u as w,
     f as $,
     g as j,
     V as F,
     j as u,
     O
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as V,
     g as k,
     l as a,
     d as U,
     t as q,
     e as z,
     u as A,
     s as G,
     c as h,
     k as J,
     a as o
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 const K = V({
         text: String,
         ...x(),
         ...y()
     }, "VToolbarTitle"),
     L = k()({
         name: "VToolbarTitle",
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3a8fb95f.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTooltip-3a8fb95f.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VTooltip-3ef94159.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VTooltip-ebb61ea6.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     m as w,
     a as H,
     u as R,
     b as h,
     c as C
-} from "./VInput-5b197ccd.js";
+} from "./VInput-8a0f3c4b.js";
 import {
     p as y,
     aC as G,
     g,
     h as S,
     at as B,
     c as v,
@@ -20,33 +20,33 @@
     z as K,
     x as L,
     H as I,
     L as N,
     d as W,
     e as j,
     r as q
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     i as T,
     a as E,
     p as J,
     d as Q,
     r as X,
     G as Y,
     H as Z,
     F as _
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     B as ee
-} from "./Container-dc894acd.js";
+} from "./Container-235383e5.js";
 import {
     m as te,
     a as oe,
     f as x
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 const ae = y({
         ...w(),
         ...G(H(), ["inline"])
     }, "VCheckbox"),
     de = g()({
         name: "VCheckbox",
         inheritAttrs: !1,
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VVirtualScroll-29c92c23.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/VVirtualScroll-84259ceb.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/VVirtualScroll-acb73766.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as L,
     w as W,
     i as X,
     T as re,
     U as oe
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as D,
     g as $,
     w as O,
     l as S,
     F as j,
     n as se,
@@ -23,18 +23,18 @@
     q as ie,
     aX as ve,
     au as fe,
     t as de,
     i as me,
     a as F,
     o as he
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 import {
     o as ge
-} from "./VMenu-b634019c.js";
+} from "./VMenu-ec95eec6.js";
 const pe = D({
         renderless: Boolean,
         ...L()
     }, "VVirtualScrollItem"),
     Se = $()({
         name: "VVirtualScrollItem",
         inheritAttrs: !1,
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/contextmenu-521b5304.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/contextmenu-c35de49a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     aJ as p,
     M as n,
     L as e,
     V as u,
     $ as c,
     P as t
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 
 function f(i) {
     return {
         all: i = i || new Map,
         on: function(l, r) {
             var a = i.get(l);
             a ? a.push(r) : i.set(l, [r])
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_dark-75402cd0.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/cover_dark-75402cd0.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/cover_light-b832ae9e.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/cover_light-b832ae9e.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/fallback-d0ff2800.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/fallback-d0ff2800.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/folder-6b5595ac.svg` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/folder-6b5595ac.svg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-7be90dc2.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/forwardRefs-708ed339.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -54,15 +54,15 @@
     af as he,
     ae as qe,
     bz as Ue,
     aB as pe,
     ba as Dt,
     j as Ft,
     aO as Ht
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 const Xe = ["top", "bottom"],
     Mt = ["start", "end", "left", "right"];
 
 function jt(e, n) {
     let [a, t] = e.split(" ");
     return t || (t = se(Xe, a) ? "start" : se(Mt, a) ? "top" : "center"), {
         side: $e(a, n),
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/forwardRefs-e5b3781d.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/forwardRefs-e5b3781d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/hires-438c7046.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/hires-438c7046.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-52c10419.css` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/index-52c10419.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/index-b687f95a.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/index-e734c256.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -11670,153 +11670,153 @@
             condition: "gt",
             offset: le.navigationMenuSize
         }) ? 9 : 0
     },
     j0 = ["artists", "albums", "tracks", "playlists", "browse"],
     U0 = [{
         path: "/",
-        component: () => Se(() => import("./Default-c7088a94.js"), ["./Default-c7088a94.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./layout-42b7d22e.js", "./VBadge-84e3406b.js", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./contextmenu-521b5304.js", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VSelect-d10e917f.js", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./VTabs-8ad24bfd.js", "./VTabs-11e16be1.css", "./VExpansionPanel-58c5fe02.js", "./VExpansionPanel-00a7e4f4.css", "./Default-2157b447.css"], import.meta.url),
+        component: () => Se(() => import("./Default-9d744187.js"), ["./Default-9d744187.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./layout-f1bc9409.js", "./VBadge-e60e80c3.js", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./contextmenu-c35de49a.js", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./VSelect-da46c348.js", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./VTabs-9b65d90e.js", "./VTabs-11e16be1.css", "./VExpansionPanel-8b2da313.js", "./VExpansionPanel-00a7e4f4.css", "./Default-2157b447.css"], import.meta.url),
         children: [{
             path: "",
             redirect: "/home",
             name: "homeredirect"
         }, {
             path: "/home",
             name: "home",
-            component: () => Se(() => import("./HomeView-8f9e6181.js"), ["./HomeView-8f9e6181.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./VBadge-84e3406b.js", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./HomeView-f9b96eef.css"], import.meta.url),
+            component: () => Se(() => import("./HomeView-9a92e516.js"), ["./HomeView-9a92e516.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./VBadge-e60e80c3.js", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./HomeView-f9b96eef.css"], import.meta.url),
             props: !0
         }, {
             path: "/search",
             name: "search",
-            component: () => Se(() => import("./Search-00ee9dd8.js"), ["./Search-00ee9dd8.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+            component: () => Se(() => import("./Search-d1673cac.js"), ["./Search-d1673cac.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
             props: !0
         }, {
             path: "/browse",
             name: "browse",
-            component: () => Se(() => import("./BrowseView-a95cb7cc.js"), ["./BrowseView-a95cb7cc.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+            component: () => Se(() => import("./BrowseView-b98345de.js"), ["./BrowseView-b98345de.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
             props: e => ({
                 ...e.query
             })
         }, {
             path: "/artists",
             children: [{
                 path: "",
                 name: "artists",
-                component: () => Se(() => import("./LibraryArtists-9924ed14.js"), ["./LibraryArtists-9924ed14.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryArtists-af4c276c.js"), ["./LibraryArtists-af4c276c.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "artist",
-                component: () => Se(() => import("./ArtistDetails-53ff83d9.js"), ["./ArtistDetails-53ff83d9.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./ArtistDetails-c7f91dbb.js"), ["./ArtistDetails-c7f91dbb.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js", "./layout-f1bc9409.js", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/albums",
             children: [{
                 path: "",
                 name: "albums",
-                component: () => Se(() => import("./LibraryAlbums-7cfa0763.js"), ["./LibraryAlbums-7cfa0763.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryAlbums-20b785fa.js"), ["./LibraryAlbums-20b785fa.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "album",
-                component: () => Se(() => import("./AlbumDetails-0b4de4f6.js"), ["./AlbumDetails-0b4de4f6.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./AlbumDetails-2e6fc4ee.js"), ["./AlbumDetails-2e6fc4ee.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js", "./layout-f1bc9409.js", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/tracks",
             children: [{
                 path: "",
                 name: "tracks",
-                component: () => Se(() => import("./LibraryTracks-eeccb967.js"), ["./LibraryTracks-eeccb967.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryTracks-4227e977.js"), ["./LibraryTracks-4227e977.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "track",
-                component: () => Se(() => import("./TrackDetails-72029d5e.js"), ["./TrackDetails-72029d5e.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./TrackDetails-40ca37ef.js"), ["./TrackDetails-40ca37ef.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js", "./layout-f1bc9409.js", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: e => ({
                     ...e.params,
                     ...e.query
                 })
             }]
         }, {
             path: "/playlists",
             children: [{
                 path: "",
                 name: "playlists",
-                component: () => Se(() => import("./LibraryPlaylists-95e35cdd.js"), ["./LibraryPlaylists-95e35cdd.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryPlaylists-b8198cb0.js"), ["./LibraryPlaylists-b8198cb0.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "playlist",
-                component: () => Se(() => import("./PlaylistDetails-2fe134b1.js"), ["./PlaylistDetails-2fe134b1.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./PlaylistDetails-59d16a22.js"), ["./PlaylistDetails-59d16a22.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js", "./layout-f1bc9409.js", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/radios",
             children: [{
                 path: "",
                 name: "radios",
-                component: () => Se(() => import("./LibraryRadios-4a033696.js"), ["./LibraryRadios-4a033696.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
+                component: () => Se(() => import("./LibraryRadios-2aa75500.js"), ["./LibraryRadios-2aa75500.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css"], import.meta.url),
                 props: !0
             }, {
                 path: ":provider/:itemId",
                 name: "radio",
-                component: () => Se(() => import("./RadioDetails-54e9e340.js"), ["./RadioDetails-54e9e340.js", "./ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-521b5304.js", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js", "./layout-42b7d22e.js", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
+                component: () => Se(() => import("./RadioDetails-5f7de0e3.js"), ["./RadioDetails-5f7de0e3.js", "./ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js", "./PanelviewItem-cbf7c595.css", "./contextmenu-c35de49a.js", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./ItemsListing-5372ff4e.css", "./ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js", "./layout-f1bc9409.js", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./ProviderDetails-2713c080.css"], import.meta.url),
                 props: !0
             }]
         }, {
             path: "/playerqueue",
             name: "playerqueue",
-            component: () => Se(() => import("./PlayerQueue-9f89c917.js"), ["./PlayerQueue-9f89c917.js", "./ListviewItem-8b992256.js", "./VBadge-84e3406b.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-3ef94159.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VTabs-8ad24bfd.js", "./VTabs-11e16be1.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css"], import.meta.url),
+            component: () => Se(() => import("./PlayerQueue-0a9bc504.js"), ["./PlayerQueue-0a9bc504.js", "./ListviewItem-04c2a02f.js", "./VBadge-e60e80c3.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VBadge-8b8b8a6d.css", "./VTooltip-ebb61ea6.js", "./VTooltip-3a8fb95f.css", "./ListviewItem-20f54197.css", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VTabs-9b65d90e.js", "./VTabs-11e16be1.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css"], import.meta.url),
             props: !0
         }, {
             path: "/settings",
             name: "settings",
-            component: () => Se(() => import("./Settings-bbdb2168.js"), ["./Settings-bbdb2168.js", "./VTabs-8ad24bfd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VTabs-11e16be1.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css"], import.meta.url),
+            component: () => Se(() => import("./Settings-34342ef5.js"), ["./Settings-34342ef5.js", "./VTabs-9b65d90e.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VTabs-11e16be1.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css"], import.meta.url),
             props: !0,
             children: [{
                 path: "providers",
                 name: "providersettings",
-                component: () => Se(() => import("./Providers-58a591e0.js"), ["./Providers-58a591e0.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./Alert-19e36349.js", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./Providers-e2f60749.css"], import.meta.url),
+                component: () => Se(() => import("./Providers-c5daf86a.js"), ["./Providers-c5daf86a.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./Alert-f8f9596c.js", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./Alert-3971d760.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./Providers-e2f60749.css"], import.meta.url),
                 props: !0
             }, {
                 path: "players",
                 name: "playersettings",
-                component: () => Se(() => import("./Players-0e31a251.js"), ["./Players-0e31a251.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css"], import.meta.url),
+                component: () => Se(() => import("./Players-23776fba.js"), ["./Players-23776fba.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css"], import.meta.url),
                 props: !0
             }, {
                 path: "core",
                 name: "coresettings",
-                component: () => Se(() => import("./CoreConfigs-f0329745.js"), ["./CoreConfigs-f0329745.js", "./Container-dc894acd.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VToolbar-b7f10b15.js", "./VToolbar-78a5e824.css", "./CoreConfigs-75569bfe.css"], import.meta.url),
+                component: () => Se(() => import("./CoreConfigs-f5c6bb00.js"), ["./CoreConfigs-f5c6bb00.js", "./Container-235383e5.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./Container-127b1d7c.css", "./VGrid-37b0738d.css", "./VToolbar-c9911418.js", "./VToolbar-78a5e824.css", "./CoreConfigs-75569bfe.css"], import.meta.url),
                 props: !0
             }, {
                 path: "addprovider/:domain",
                 name: "addprovider",
-                component: () => Se(() => import("./AddProvider-f756ebc3.js"), ["./AddProvider-f756ebc3.js", "./index.browser-342e672c.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
+                component: () => Se(() => import("./AddProvider-ac9c5e72.js"), ["./AddProvider-ac9c5e72.js", "./index.browser-342e672c.js", "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js", "./VExpansionPanel-8b2da313.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-7178cd98.js", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VSelect-da46c348.js", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editprovider/:instanceId",
                 name: "editprovider",
-                component: () => Se(() => import("./EditProvider-e046ee5d.js"), ["./EditProvider-e046ee5d.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
+                component: () => Se(() => import("./EditProvider-63f3a683.js"), ["./EditProvider-63f3a683.js", "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js", "./VExpansionPanel-8b2da313.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-7178cd98.js", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VSelect-da46c348.js", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
                 props: !0
             }, {
                 path: "editplayer/:playerId",
                 name: "editplayer",
-                component: () => Se(() => import("./EditPlayer-6e04043d.js"), ["./EditPlayer-6e04043d.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
+                component: () => Se(() => import("./EditPlayer-e8fd1918.js"), ["./EditPlayer-e8fd1918.js", "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js", "./VExpansionPanel-8b2da313.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-7178cd98.js", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VSelect-da46c348.js", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editcore/:domain",
                 name: "editcore",
-                component: () => Se(() => import("./EditCoreConfig-d27a9b35.js"), ["./EditCoreConfig-d27a9b35.js", "./EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js", "./VExpansionPanel-58c5fe02.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VMenu-b634019c.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-fc99b4aa.js", "./VCard-b98fe47e.js", "./VCardText-6774ea5e.js", "./VCard-257d0eab.css", "./VDialog-d7e50927.js", "./VDialog-5309eac2.css", "./VAlert-56af8987.js", "./VAlert-1c823677.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
+                component: () => Se(() => import("./EditCoreConfig-72a12486.js"), ["./EditCoreConfig-72a12486.js", "./EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js", "./VExpansionPanel-8b2da313.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VMenu-ec95eec6.js", "./VMenu-a46f5e7a.css", "./VInput-b16e222c.css", "./VExpansionPanel-00a7e4f4.css", "./VForm-7178cd98.js", "./VCard-4532b814.js", "./VCardText-35ed9014.js", "./VCard-257d0eab.css", "./VDialog-7155dc5f.js", "./VDialog-5309eac2.css", "./VAlert-ed4cb12a.js", "./VAlert-1c823677.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VSelect-da46c348.js", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css", "./EditConfig-f2bca5b1.css", "./VGrid-37b0738d.css", "./index.browser-342e672c.js"], import.meta.url),
                 props: !0
             }, {
                 path: "addgroup/:provider",
                 name: "addgroup",
-                component: () => Se(() => import("./AddGroupPlayer-8a4f0893.js"), ["./AddGroupPlayer-8a4f0893.js", "./VCardText-6774ea5e.js", "./VMenu-b634019c.js", "./forwardRefs-7be90dc2.js", "./forwardRefs-e5b3781d.css", "./VMenu-a46f5e7a.css", "./VForm-fc99b4aa.js", "./VInput-5b197ccd.js", "./VSlideGroup-b576aa37.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VTextField-0c2ec62d.js", "./VTextField-d31117f3.css", "./VSelect-d10e917f.js", "./VVirtualScroll-84259ceb.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css"], import.meta.url),
+                component: () => Se(() => import("./AddGroupPlayer-ee16256c.js"), ["./AddGroupPlayer-ee16256c.js", "./VCardText-35ed9014.js", "./VMenu-ec95eec6.js", "./forwardRefs-708ed339.js", "./forwardRefs-e5b3781d.css", "./VMenu-a46f5e7a.css", "./VForm-7178cd98.js", "./VInput-8a0f3c4b.js", "./VSlideGroup-c7be05c1.js", "./VSlideGroup-c5ba1538.css", "./VInput-b16e222c.css", "./VTextField-95a689ca.js", "./VTextField-d31117f3.css", "./VSelect-da46c348.js", "./VVirtualScroll-acb73766.js", "./VVirtualScroll-29c92c23.css", "./VSelect-7df244e0.css"], import.meta.url),
                 props: !0
             }, {
                 path: "",
                 redirect: "/settings/providers",
                 name: "settingsredirect"
             }]
         }]
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/layout-42b7d22e.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/layout-f1bc9409.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     w as ee
-} from "./forwardRefs-7be90dc2.js";
+} from "./forwardRefs-708ed339.js";
 import {
     p as U,
     as as E,
     at as te,
     au as Z,
     av as k,
     s as D,
@@ -13,15 +13,15 @@
     c as s,
     b as ae,
     r as se,
     ar as $,
     a as R,
     o as ue,
     ay as le
-} from "./index-b687f95a.js";
+} from "./index-e734c256.js";
 const M = Symbol.for("vuetify:layout"),
     X = Symbol.for("vuetify:layout-item"),
     N = 1e3,
     de = U({
         overlaps: {
             type: Array,
             default: () => []
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/logo-9391b78c.svg` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/logo-9391b78c.svg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/m4a-45331b05.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/m4a-45331b05.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/favicon.ico` & `music-assistant-frontend-2.4.4/music_assistant_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/index.html` & `music-assistant-frontend-2.4.4/music_assistant_frontend/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link rel="mask-icon" href="favicon.svg" color="#FFFFFF">
     <link rel="manifest" href="manifest.webmanifest">
     <meta name="theme-color" media="(prefers-color-scheme: light)" content="#ffffff">
     <meta name="theme-color" media="(prefers-color-scheme: dark)"  content="#121212">
     <link rel="icon" href="favicon.ico" />
     <title>Music Assistant</title>
     <meta name="description" content="Music Assistant - Music library manager for Home Assistant">
-    <script type="module" crossorigin src="./assets/index-b687f95a.js"></script>
+    <script type="module" crossorigin src="./assets/index-e734c256.js"></script>
     <link rel="stylesheet" href="./assets/index-52c10419.css">
   <link rel="manifest" href="./manifest.webmanifest"><style>@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2) format('woff2');unicode-range:U+0370-0377,U+037A-037F,U+0384-038A,U+038C,U+038E-03A1,U+03A3-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20C0,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}</style></head>
   <body>
     <noscript>
       <strong
         >We're sorry but musicassistant-frontend doesn't work properly without
         JavaScript enabled. Please enable it to continue.</strong
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/manifest.webmanifest` & `music-assistant-frontend-2.4.4/music_assistant_frontend/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-192x192.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/pwa-192x192.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/pwa-512x512.png` & `music-assistant-frontend-2.4.4/music_assistant_frontend/pwa-512x512.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/sw.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/sw.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -26,259 +26,259 @@
     }
 }
 define(["./workbox-27b29e6f"], (function(s) {
     "use strict";
     self.addEventListener("message", (s => {
         s.data && "SKIP_WAITING" === s.data.type && self.skipWaiting()
     })), s.precacheAndRoute([{
-        url: "assets/AddGroupPlayer-8a4f0893.js",
+        url: "assets/AddGroupPlayer-ee16256c.js",
         revision: null
     }, {
-        url: "assets/AddProvider-f756ebc3.js",
+        url: "assets/AddProvider-ac9c5e72.js",
         revision: null
     }, {
-        url: "assets/AlbumDetails-0b4de4f6.js",
+        url: "assets/AlbumDetails-2e6fc4ee.js",
         revision: null
     }, {
-        url: "assets/Alert-19e36349.js",
+        url: "assets/Alert-3971d760.css",
         revision: null
     }, {
-        url: "assets/Alert-3971d760.css",
+        url: "assets/Alert-f8f9596c.js",
         revision: null
     }, {
-        url: "assets/ArtistDetails-53ff83d9.js",
+        url: "assets/ArtistDetails-c7f91dbb.js",
         revision: null
     }, {
-        url: "assets/BrowseView-a95cb7cc.js",
+        url: "assets/BrowseView-b98345de.js",
         revision: null
     }, {
         url: "assets/Container-127b1d7c.css",
         revision: null
     }, {
-        url: "assets/Container-dc894acd.js",
+        url: "assets/Container-235383e5.js",
         revision: null
     }, {
-        url: "assets/contextmenu-521b5304.js",
+        url: "assets/contextmenu-c35de49a.js",
         revision: null
     }, {
         url: "assets/CoreConfigs-75569bfe.css",
         revision: null
     }, {
-        url: "assets/CoreConfigs-f0329745.js",
+        url: "assets/CoreConfigs-f5c6bb00.js",
         revision: null
     }, {
         url: "assets/Default-2157b447.css",
         revision: null
     }, {
-        url: "assets/Default-c7088a94.js",
+        url: "assets/Default-9d744187.js",
         revision: null
     }, {
         url: "assets/EditConfig-f2bca5b1.css",
         revision: null
     }, {
-        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js",
+        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js",
         revision: null
     }, {
-        url: "assets/EditCoreConfig-d27a9b35.js",
+        url: "assets/EditCoreConfig-72a12486.js",
         revision: null
     }, {
-        url: "assets/EditPlayer-6e04043d.js",
+        url: "assets/EditPlayer-e8fd1918.js",
         revision: null
     }, {
-        url: "assets/EditProvider-e046ee5d.js",
+        url: "assets/EditProvider-63f3a683.js",
         revision: null
     }, {
-        url: "assets/forwardRefs-7be90dc2.js",
+        url: "assets/forwardRefs-708ed339.js",
         revision: null
     }, {
         url: "assets/forwardRefs-e5b3781d.css",
         revision: null
     }, {
-        url: "assets/HomeView-8f9e6181.js",
+        url: "assets/HomeView-9a92e516.js",
         revision: null
     }, {
         url: "assets/HomeView-f9b96eef.css",
         revision: null
     }, {
         url: "assets/index-52c10419.css",
         revision: null
     }, {
-        url: "assets/index-b687f95a.js",
+        url: "assets/index-e734c256.js",
         revision: null
     }, {
         url: "assets/index.browser-342e672c.js",
         revision: null
     }, {
         url: "assets/ItemsListing-5372ff4e.css",
         revision: null
     }, {
-        url: "assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js",
+        url: "assets/ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js",
         revision: null
     }, {
-        url: "assets/layout-42b7d22e.js",
+        url: "assets/layout-f1bc9409.js",
         revision: null
     }, {
-        url: "assets/LibraryAlbums-7cfa0763.js",
+        url: "assets/LibraryAlbums-20b785fa.js",
         revision: null
     }, {
-        url: "assets/LibraryArtists-9924ed14.js",
+        url: "assets/LibraryArtists-af4c276c.js",
         revision: null
     }, {
-        url: "assets/LibraryPlaylists-95e35cdd.js",
+        url: "assets/LibraryPlaylists-b8198cb0.js",
         revision: null
     }, {
-        url: "assets/LibraryRadios-4a033696.js",
+        url: "assets/LibraryRadios-2aa75500.js",
         revision: null
     }, {
-        url: "assets/LibraryTracks-eeccb967.js",
+        url: "assets/LibraryTracks-4227e977.js",
         revision: null
     }, {
-        url: "assets/ListviewItem-20f54197.css",
+        url: "assets/ListviewItem-04c2a02f.js",
         revision: null
     }, {
-        url: "assets/ListviewItem-8b992256.js",
+        url: "assets/ListviewItem-20f54197.css",
         revision: null
     }, {
         url: "assets/PanelviewItem-cbf7c595.css",
         revision: null
     }, {
-        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js",
+        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js",
         revision: null
     }, {
-        url: "assets/PlayerQueue-9f89c917.js",
+        url: "assets/PlayerQueue-0a9bc504.js",
         revision: null
     }, {
-        url: "assets/Players-0e31a251.js",
+        url: "assets/Players-23776fba.js",
         revision: null
     }, {
-        url: "assets/PlaylistDetails-2fe134b1.js",
+        url: "assets/PlaylistDetails-59d16a22.js",
         revision: null
     }, {
         url: "assets/ProviderDetails-2713c080.css",
         revision: null
     }, {
-        url: "assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js",
+        url: "assets/ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js",
         revision: null
     }, {
-        url: "assets/Providers-58a591e0.js",
+        url: "assets/Providers-c5daf86a.js",
         revision: null
     }, {
         url: "assets/Providers-e2f60749.css",
         revision: null
     }, {
-        url: "assets/RadioDetails-54e9e340.js",
+        url: "assets/RadioDetails-5f7de0e3.js",
         revision: null
     }, {
-        url: "assets/Search-00ee9dd8.js",
+        url: "assets/Search-d1673cac.js",
         revision: null
     }, {
-        url: "assets/Settings-bbdb2168.js",
+        url: "assets/Settings-34342ef5.js",
         revision: null
     }, {
-        url: "assets/TrackDetails-72029d5e.js",
+        url: "assets/TrackDetails-40ca37ef.js",
         revision: null
     }, {
         url: "assets/VAlert-1c823677.css",
         revision: null
     }, {
-        url: "assets/VAlert-56af8987.js",
+        url: "assets/VAlert-ed4cb12a.js",
         revision: null
     }, {
-        url: "assets/VBadge-84e3406b.js",
+        url: "assets/VBadge-8b8b8a6d.css",
         revision: null
     }, {
-        url: "assets/VBadge-8b8b8a6d.css",
+        url: "assets/VBadge-e60e80c3.js",
         revision: null
     }, {
         url: "assets/VCard-257d0eab.css",
         revision: null
     }, {
-        url: "assets/VCard-b98fe47e.js",
+        url: "assets/VCard-4532b814.js",
         revision: null
     }, {
-        url: "assets/VCardText-6774ea5e.js",
+        url: "assets/VCardText-35ed9014.js",
         revision: null
     }, {
         url: "assets/VDialog-5309eac2.css",
         revision: null
     }, {
-        url: "assets/VDialog-d7e50927.js",
+        url: "assets/VDialog-7155dc5f.js",
         revision: null
     }, {
         url: "assets/VExpansionPanel-00a7e4f4.css",
         revision: null
     }, {
-        url: "assets/VExpansionPanel-58c5fe02.js",
+        url: "assets/VExpansionPanel-8b2da313.js",
         revision: null
     }, {
-        url: "assets/VForm-fc99b4aa.js",
+        url: "assets/VForm-7178cd98.js",
         revision: null
     }, {
         url: "assets/VGrid-37b0738d.css",
         revision: null
     }, {
-        url: "assets/VInput-5b197ccd.js",
+        url: "assets/VInput-8a0f3c4b.js",
         revision: null
     }, {
         url: "assets/VInput-b16e222c.css",
         revision: null
     }, {
         url: "assets/VMenu-a46f5e7a.css",
         revision: null
     }, {
-        url: "assets/VMenu-b634019c.js",
+        url: "assets/VMenu-ec95eec6.js",
         revision: null
     }, {
         url: "assets/VSelect-7df244e0.css",
         revision: null
     }, {
-        url: "assets/VSelect-d10e917f.js",
+        url: "assets/VSelect-da46c348.js",
         revision: null
     }, {
-        url: "assets/VSlideGroup-b576aa37.js",
+        url: "assets/VSlideGroup-c5ba1538.css",
         revision: null
     }, {
-        url: "assets/VSlideGroup-c5ba1538.css",
+        url: "assets/VSlideGroup-c7be05c1.js",
         revision: null
     }, {
         url: "assets/VTabs-11e16be1.css",
         revision: null
     }, {
-        url: "assets/VTabs-8ad24bfd.js",
+        url: "assets/VTabs-9b65d90e.js",
         revision: null
     }, {
-        url: "assets/VTextField-0c2ec62d.js",
+        url: "assets/VTextField-95a689ca.js",
         revision: null
     }, {
         url: "assets/VTextField-d31117f3.css",
         revision: null
     }, {
         url: "assets/VToolbar-78a5e824.css",
         revision: null
     }, {
-        url: "assets/VToolbar-b7f10b15.js",
+        url: "assets/VToolbar-c9911418.js",
         revision: null
     }, {
         url: "assets/VTooltip-3a8fb95f.css",
         revision: null
     }, {
-        url: "assets/VTooltip-3ef94159.js",
+        url: "assets/VTooltip-ebb61ea6.js",
         revision: null
     }, {
         url: "assets/VVirtualScroll-29c92c23.css",
         revision: null
     }, {
-        url: "assets/VVirtualScroll-84259ceb.js",
+        url: "assets/VVirtualScroll-acb73766.js",
         revision: null
     }, {
         url: "assets/workbox-window.prod.es5-a7b12eab.js",
         revision: null
     }, {
         url: "index.html",
-        revision: "9316d7db7067601d034630c21a631d4d"
+        revision: "f9b1421247b3bb62b1bf4de44a275e54"
     }, {
         url: "favicon.ico",
         revision: "60d77c1713c2255be3f6de69c4de24d9"
     }, {
         url: "robots.txt",
         revision: "5e0bd1c281a62a380d7a948085bfe2d1"
     }, {
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend/workbox-27b29e6f.js` & `music-assistant-frontend-2.4.4/music_assistant_frontend/workbox-27b29e6f.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/PKG-INFO` & `music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.4.3
+Version: 2.4.4
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.4.3/music_assistant_frontend.egg-info/SOURCES.txt` & `music-assistant-frontend-2.4.4/music_assistant_frontend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 music_assistant_frontend/sw.js
 music_assistant_frontend/workbox-27b29e6f.js
 music_assistant_frontend.egg-info/PKG-INFO
 music_assistant_frontend.egg-info/SOURCES.txt
 music_assistant_frontend.egg-info/dependency_links.txt
 music_assistant_frontend.egg-info/not-zip-safe
 music_assistant_frontend.egg-info/top_level.txt
-music_assistant_frontend/assets/AddGroupPlayer-8a4f0893.js
-music_assistant_frontend/assets/AddProvider-f756ebc3.js
-music_assistant_frontend/assets/AlbumDetails-0b4de4f6.js
-music_assistant_frontend/assets/Alert-19e36349.js
+music_assistant_frontend/assets/AddGroupPlayer-ee16256c.js
+music_assistant_frontend/assets/AddProvider-ac9c5e72.js
+music_assistant_frontend/assets/AlbumDetails-2e6fc4ee.js
 music_assistant_frontend/assets/Alert-3971d760.css
-music_assistant_frontend/assets/ArtistDetails-53ff83d9.js
-music_assistant_frontend/assets/BrowseView-a95cb7cc.js
+music_assistant_frontend/assets/Alert-f8f9596c.js
+music_assistant_frontend/assets/ArtistDetails-c7f91dbb.js
+music_assistant_frontend/assets/BrowseView-b98345de.js
 music_assistant_frontend/assets/Container-127b1d7c.css
-music_assistant_frontend/assets/Container-dc894acd.js
+music_assistant_frontend/assets/Container-235383e5.js
 music_assistant_frontend/assets/CoreConfigs-75569bfe.css
-music_assistant_frontend/assets/CoreConfigs-f0329745.js
+music_assistant_frontend/assets/CoreConfigs-f5c6bb00.js
 music_assistant_frontend/assets/Default-2157b447.css
-music_assistant_frontend/assets/Default-c7088a94.js
+music_assistant_frontend/assets/Default-9d744187.js
 music_assistant_frontend/assets/EditConfig-f2bca5b1.css
-music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-807fdd8e.js
-music_assistant_frontend/assets/EditCoreConfig-d27a9b35.js
-music_assistant_frontend/assets/EditPlayer-6e04043d.js
-music_assistant_frontend/assets/EditProvider-e046ee5d.js
-music_assistant_frontend/assets/HomeView-8f9e6181.js
+music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-e4cfec5b.js
+music_assistant_frontend/assets/EditCoreConfig-72a12486.js
+music_assistant_frontend/assets/EditPlayer-e8fd1918.js
+music_assistant_frontend/assets/EditProvider-63f3a683.js
+music_assistant_frontend/assets/HomeView-9a92e516.js
 music_assistant_frontend/assets/HomeView-f9b96eef.css
 music_assistant_frontend/assets/ItemsListing-5372ff4e.css
-music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-74e3dc20.js
+music_assistant_frontend/assets/ItemsListing.vue_vue_type_style_index_0_lang-ab18972e.js
 music_assistant_frontend/assets/JetBrainsMono-Medium-086c48df.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
@@ -80,82 +80,82 @@
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
-music_assistant_frontend/assets/LibraryAlbums-7cfa0763.js
-music_assistant_frontend/assets/LibraryArtists-9924ed14.js
-music_assistant_frontend/assets/LibraryPlaylists-95e35cdd.js
-music_assistant_frontend/assets/LibraryRadios-4a033696.js
-music_assistant_frontend/assets/LibraryTracks-eeccb967.js
+music_assistant_frontend/assets/LibraryAlbums-20b785fa.js
+music_assistant_frontend/assets/LibraryArtists-af4c276c.js
+music_assistant_frontend/assets/LibraryPlaylists-b8198cb0.js
+music_assistant_frontend/assets/LibraryRadios-2aa75500.js
+music_assistant_frontend/assets/LibraryTracks-4227e977.js
+music_assistant_frontend/assets/ListviewItem-04c2a02f.js
 music_assistant_frontend/assets/ListviewItem-20f54197.css
-music_assistant_frontend/assets/ListviewItem-8b992256.js
 music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
 music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
 music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
 music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
 music_assistant_frontend/assets/PanelviewItem-cbf7c595.css
-music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-a3a9dd78.js
-music_assistant_frontend/assets/PlayerQueue-9f89c917.js
-music_assistant_frontend/assets/Players-0e31a251.js
-music_assistant_frontend/assets/PlaylistDetails-2fe134b1.js
+music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-1aec1346.js
+music_assistant_frontend/assets/PlayerQueue-0a9bc504.js
+music_assistant_frontend/assets/Players-23776fba.js
+music_assistant_frontend/assets/PlaylistDetails-59d16a22.js
 music_assistant_frontend/assets/ProviderDetails-2713c080.css
-music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-a372fabe.js
-music_assistant_frontend/assets/Providers-58a591e0.js
+music_assistant_frontend/assets/ProviderDetails.vue_vue_type_script_setup_true_lang-bb35ff48.js
+music_assistant_frontend/assets/Providers-c5daf86a.js
 music_assistant_frontend/assets/Providers-e2f60749.css
-music_assistant_frontend/assets/RadioDetails-54e9e340.js
-music_assistant_frontend/assets/Search-00ee9dd8.js
-music_assistant_frontend/assets/Settings-bbdb2168.js
-music_assistant_frontend/assets/TrackDetails-72029d5e.js
+music_assistant_frontend/assets/RadioDetails-5f7de0e3.js
+music_assistant_frontend/assets/Search-d1673cac.js
+music_assistant_frontend/assets/Settings-34342ef5.js
+music_assistant_frontend/assets/TrackDetails-40ca37ef.js
 music_assistant_frontend/assets/VAlert-1c823677.css
-music_assistant_frontend/assets/VAlert-56af8987.js
-music_assistant_frontend/assets/VBadge-84e3406b.js
+music_assistant_frontend/assets/VAlert-ed4cb12a.js
 music_assistant_frontend/assets/VBadge-8b8b8a6d.css
+music_assistant_frontend/assets/VBadge-e60e80c3.js
 music_assistant_frontend/assets/VCard-257d0eab.css
-music_assistant_frontend/assets/VCard-b98fe47e.js
-music_assistant_frontend/assets/VCardText-6774ea5e.js
+music_assistant_frontend/assets/VCard-4532b814.js
+music_assistant_frontend/assets/VCardText-35ed9014.js
 music_assistant_frontend/assets/VDialog-5309eac2.css
-music_assistant_frontend/assets/VDialog-d7e50927.js
+music_assistant_frontend/assets/VDialog-7155dc5f.js
 music_assistant_frontend/assets/VExpansionPanel-00a7e4f4.css
-music_assistant_frontend/assets/VExpansionPanel-58c5fe02.js
-music_assistant_frontend/assets/VForm-fc99b4aa.js
+music_assistant_frontend/assets/VExpansionPanel-8b2da313.js
+music_assistant_frontend/assets/VForm-7178cd98.js
 music_assistant_frontend/assets/VGrid-37b0738d.css
-music_assistant_frontend/assets/VInput-5b197ccd.js
+music_assistant_frontend/assets/VInput-8a0f3c4b.js
 music_assistant_frontend/assets/VInput-b16e222c.css
 music_assistant_frontend/assets/VMenu-a46f5e7a.css
-music_assistant_frontend/assets/VMenu-b634019c.js
+music_assistant_frontend/assets/VMenu-ec95eec6.js
 music_assistant_frontend/assets/VSelect-7df244e0.css
-music_assistant_frontend/assets/VSelect-d10e917f.js
-music_assistant_frontend/assets/VSlideGroup-b576aa37.js
+music_assistant_frontend/assets/VSelect-da46c348.js
 music_assistant_frontend/assets/VSlideGroup-c5ba1538.css
+music_assistant_frontend/assets/VSlideGroup-c7be05c1.js
 music_assistant_frontend/assets/VTabs-11e16be1.css
-music_assistant_frontend/assets/VTabs-8ad24bfd.js
-music_assistant_frontend/assets/VTextField-0c2ec62d.js
+music_assistant_frontend/assets/VTabs-9b65d90e.js
+music_assistant_frontend/assets/VTextField-95a689ca.js
 music_assistant_frontend/assets/VTextField-d31117f3.css
 music_assistant_frontend/assets/VToolbar-78a5e824.css
-music_assistant_frontend/assets/VToolbar-b7f10b15.js
+music_assistant_frontend/assets/VToolbar-c9911418.js
 music_assistant_frontend/assets/VTooltip-3a8fb95f.css
-music_assistant_frontend/assets/VTooltip-3ef94159.js
+music_assistant_frontend/assets/VTooltip-ebb61ea6.js
 music_assistant_frontend/assets/VVirtualScroll-29c92c23.css
-music_assistant_frontend/assets/VVirtualScroll-84259ceb.js
-music_assistant_frontend/assets/contextmenu-521b5304.js
+music_assistant_frontend/assets/VVirtualScroll-acb73766.js
+music_assistant_frontend/assets/contextmenu-c35de49a.js
 music_assistant_frontend/assets/cover_dark-75402cd0.png
 music_assistant_frontend/assets/cover_light-b832ae9e.png
 music_assistant_frontend/assets/fallback-d0ff2800.png
 music_assistant_frontend/assets/folder-6b5595ac.svg
-music_assistant_frontend/assets/forwardRefs-7be90dc2.js
+music_assistant_frontend/assets/forwardRefs-708ed339.js
 music_assistant_frontend/assets/forwardRefs-e5b3781d.css
 music_assistant_frontend/assets/hires-438c7046.png
 music_assistant_frontend/assets/index-52c10419.css
-music_assistant_frontend/assets/index-b687f95a.js
+music_assistant_frontend/assets/index-e734c256.js
 music_assistant_frontend/assets/index.browser-342e672c.js
 music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
-music_assistant_frontend/assets/layout-42b7d22e.js
+music_assistant_frontend/assets/layout-f1bc9409.js
 music_assistant_frontend/assets/logo-9391b78c.svg
 music_assistant_frontend/assets/m4a-45331b05.png
 music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
 music_assistant_frontend/assets/materialdesignicons-webfont-0b183104.eot
 music_assistant_frontend/assets/materialdesignicons-webfont-61e8aba5.ttf
 music_assistant_frontend/assets/materialdesignicons-webfont-662fefa8.woff2
 music_assistant_frontend/assets/materialdesignicons-webfont-a5928a0d.woff
```

### Comparing `music-assistant-frontend-2.4.3/pyproject.toml` & `music-assistant-frontend-2.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "music-assistant-frontend"
-version = "2.4.3"
+version = "2.4.4"
 description = "The Music Assistant frontend"
 readme = "README.md"
 authors = [
     { name = "The Music Assistant Authors", email = "m.vanderveldt@outlook.com" },
 ]
 requires-python = ">=3.9.0"
```

