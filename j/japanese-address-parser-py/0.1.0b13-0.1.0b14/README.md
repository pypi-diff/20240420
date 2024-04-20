# Comparing `tmp/japanese_address_parser_py-0.1.0b13.tar.gz` & `tmp/japanese_address_parser_py-0.1.0b14.tar.gz`

## Comparing `japanese_address_parser_py-0.1.0b13.tar` & `japanese_address_parser_py-0.1.0b14.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0     1001      127      729 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/Cargo.toml
--rw-r--r--   0     1001      127     1065 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/LICENSE
--rw-r--r--   0     1001      127     4410 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/api/city_master_api.rs
--rw-r--r--   0     1001      127     4915 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/api/prefecture_master_api.rs
--rw-r--r--   0     1001      127     2775 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/api.rs
--rw-r--r--   0     1001      127     1794 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/entity.rs
--rw-r--r--   0     1001      127     1326 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/err.rs
--rw-r--r--   0     1001      127       64 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/lib.rs
--rw-r--r--   0     1001      127     3131 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/adapter/orthographical_variant_adapter.rs
--rw-r--r--   0     1001      127       40 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/adapter.rs
--rw-r--r--   0     1001      127      570 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/filter/fullwidth_character.rs
--rw-r--r--   0     1001      127     7292 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/filter/invalid_town_name_format.rs
--rw-r--r--   0     1001      127     3393 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/filter/non_kanji_block_number.rs
--rw-r--r--   0     1001      127      162 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/filter.rs
--rw-r--r--   0     1001      127     3078 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/read_city.rs
--rw-r--r--   0     1001      127     2293 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/read_house_number.rs
--rw-r--r--   0     1001      127     1739 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/read_prefecture.rs
--rw-r--r--   0     1001      127     7124 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser/read_town.rs
--rw-r--r--   0     1001      127     9275 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/parser.rs
--rw-r--r--   0     1001      127     3695 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/util/converter.rs
--rw-r--r--   0     1001      127       19 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/core/src/util.rs
--rw-r--r--   0     1001      127     2826 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/README.md
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b13/python/Cargo.toml
--rw-r--r--   0     1001      127     3282 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/python/README.md
--rw-r--r--   0     1001      127      823 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/python/japanese_address_parser_py.pyi
--rw-r--r--   0     1001      127     1426 2024-04-10 14:46:27.000000 japanese_address_parser_py-0.1.0b13/python/src/lib.rs
--rw-r--r--   0     1001      127    35483 2024-04-10 14:46:31.000000 japanese_address_parser_py-0.1.0b13/Cargo.lock
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b13/Cargo.toml
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b13/pyproject.toml
--rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b13/PKG-INFO
+-rw-r--r--   0     1001      127      749 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/Cargo.toml
+-rw-r--r--   0     1001      127     1065 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/LICENSE
+-rw-r--r--   0     1001      127     4410 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/api/city_master_api.rs
+-rw-r--r--   0     1001      127     4915 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/api/prefecture_master_api.rs
+-rw-r--r--   0     1001      127     2775 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/api.rs
+-rw-r--r--   0     1001      127     1794 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/entity.rs
+-rw-r--r--   0     1001      127     1326 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/err.rs
+-rw-r--r--   0     1001      127       64 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/lib.rs
+-rw-r--r--   0     1001      127     3131 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/orthographical_variant_adapter.rs
+-rw-r--r--   0     1001      127     2794 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/vague_expression_adapter.rs
+-rw-r--r--   0     1001      127       74 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/adapter.rs
+-rw-r--r--   0     1001      127      570 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter/fullwidth_character.rs
+-rw-r--r--   0     1001      127     7292 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter/invalid_town_name_format.rs
+-rw-r--r--   0     1001      127     3393 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter/non_kanji_block_number.rs
+-rw-r--r--   0     1001      127      162 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/filter.rs
+-rw-r--r--   0     1001      127     3769 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_city.rs
+-rw-r--r--   0     1001      127     2293 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_house_number.rs
+-rw-r--r--   0     1001      127     1739 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_prefecture.rs
+-rw-r--r--   0     1001      127     7124 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser/read_town.rs
+-rw-r--r--   0     1001      127     9275 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/parser.rs
+-rw-r--r--   0     1001      127     3695 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/util/converter.rs
+-rw-r--r--   0     1001      127     7165 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/util/sequence_matcher.rs
+-rw-r--r--   0     1001      127       45 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/core/src/util.rs
+-rw-r--r--   0     1001      127     2826 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/README.md
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/python/Cargo.toml
+-rw-r--r--   0     1001      127     3282 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/python/README.md
+-rw-r--r--   0     1001      127      823 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/python/japanese_address_parser_py.pyi
+-rw-r--r--   0     1001      127     1426 2024-04-20 11:50:24.000000 japanese_address_parser_py-0.1.0b14/python/src/lib.rs
+-rw-r--r--   0     1001      127    35920 2024-04-20 11:50:29.000000 japanese_address_parser_py-0.1.0b14/Cargo.lock
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/Cargo.toml
+-rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/pyproject.toml
+-rw-r--r--   0        0        0     3813 1970-01-01 00:00:00.000000 japanese_address_parser_py-0.1.0b14/PKG-INFO
```

### Comparing `japanese_address_parser_py-0.1.0b13/core/Cargo.toml` & `japanese_address_parser_py-0.1.0b14/core/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 [lib]
 crate-type = ["rlib", "cdylib"]
 
 [dependencies]
 itertools = "0.12.0"
 js-sys = "0.3.67"
 nom = "7.1.3"
+rapidfuzz = "0.5.0"
 regex = "1.10.2"
 reqwest = { version = "0.12.3", default-features = false, features = ["json", "rustls-tls", "blocking"] }
 serde = { version = "1.0.192", features = ["derive"] }
 
 [dev-dependencies]
 test-case = "3.3.1"
 tokio = { version = "1.37.0", features = ["rt", "macros"] }
```

### Comparing `japanese_address_parser_py-0.1.0b13/core/LICENSE` & `japanese_address_parser_py-0.1.0b14/core/LICENSE`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/api/city_master_api.rs` & `japanese_address_parser_py-0.1.0b14/core/src/api/city_master_api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/api/prefecture_master_api.rs` & `japanese_address_parser_py-0.1.0b14/core/src/api/prefecture_master_api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/api.rs` & `japanese_address_parser_py-0.1.0b14/core/src/api.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/entity.rs` & `japanese_address_parser_py-0.1.0b14/core/src/entity.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/err.rs` & `japanese_address_parser_py-0.1.0b14/core/src/err.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/adapter/orthographical_variant_adapter.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/adapter/orthographical_variant_adapter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/filter/fullwidth_character.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/filter/fullwidth_character.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/filter/invalid_town_name_format.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/filter/invalid_town_name_format.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/filter/non_kanji_block_number.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/filter/non_kanji_block_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/read_city.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/read_city.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 use crate::entity::Prefecture;
 use crate::parser::adapter::orthographical_variant_adapter::{
     OrthographicalVariantAdapter, OrthographicalVariants, Variant,
 };
+use crate::parser::adapter::vague_expression_adapter::VagueExpressionAdapter;
 use nom::bytes::complete::tag;
 use nom::error::VerboseError;
 use nom::Parser;
 
 pub fn read_city(input: &str, prefecture: Prefecture) -> Option<(String, String)> {
-    for city_name in prefecture.cities {
-        if let Ok((rest, city_name)) =
-            tag::<&str, &str, VerboseError<&str>>(&city_name).parse(input)
+    for city_name in &prefecture.cities {
+        if let Ok((rest, city_name)) = tag::<&str, &str, VerboseError<&str>>(city_name).parse(input)
         {
             return Some((rest.to_string(), city_name.to_string()));
         }
         let mut variant_list = vec![Variant::ケ];
         match prefecture.name.as_str() {
             "宮城県" => {
                 variant_list.push(Variant::竈);
@@ -24,18 +24,25 @@
             }
             "東京都" => {
                 variant_list.push(Variant::檜);
             }
             _ => {}
         }
         let adapter = OrthographicalVariantAdapter { variant_list };
-        if let Some(result) = adapter.apply(input, &city_name) {
+        if let Some(result) = adapter.apply(input, city_name) {
             return Some(result);
         }
     }
+
+    // ここまでで市町村名の特定ができない場合はVagueExpressionAdapterを使用して市町村名を推測する
+    let vague_expression_adapter = VagueExpressionAdapter {};
+    if let Some(result) = vague_expression_adapter.apply(input, &prefecture.cities) {
+        return Some(result);
+    }
+
     None
 }
 
 #[cfg(all(test, not(target_arch = "wasm32")))]
 mod tests {
     use crate::api::{BlockingApi, BlockingApiImpl};
     use crate::parser::read_city::read_city;
@@ -48,14 +55,16 @@
     #[test_case("神奈川県", "横浜市保土ヶ谷区川辺町2番地9", "横浜市保土ケ谷区"; "success_横浜市保土ヶ谷区_表記ゆれ")]
     #[test_case("岐阜県", "不破郡関ケ原町大字関ケ原894番地の58", "不破郡関ケ原町"; "success_不破郡関ケ原町")]
     #[test_case("岐阜県", "不破郡関が原町大字関ケ原894番地の58", "不破郡関ケ原町"; "success_不破郡関が原町_表記ゆれ")]
     #[test_case("茨城県", "龍ヶ崎市佐貫町647", "龍ヶ崎市"; "success_龍ヶ崎市")]
     #[test_case("茨城県", "龍ケ崎市佐貫町647", "龍ヶ崎市"; "success_龍ケ崎市_表記ゆれ")]
     #[test_case("茨城県", "竜ヶ崎市佐貫町647", "龍ヶ崎市"; "success_竜ヶ崎市_表記ゆれ")]
     #[test_case("茨城県", "竜ケ崎市佐貫町647", "龍ヶ崎市"; "success_竜ケ崎市_表記ゆれ")]
+    #[test_case("群馬県", "みなかみ町後閑318", "利根郡みなかみ町"; "success_利根郡みなかみ町_郡名が省略されている")]
+    #[test_case("埼玉県", "東秩父村大字御堂634番地", "秩父郡東秩父村"; "success_秩父郡東秩父村_郡名が省略されている")]
     fn test_read_city(prefecture_name: &str, input: &str, expected: &str) {
         let api = BlockingApiImpl::new();
         let prefecture = api.get_prefecture_master(prefecture_name).unwrap();
         let (_, city_name) = read_city(input, prefecture).unwrap();
         assert_eq!(city_name, expected);
     }
 }
```

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/read_house_number.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/read_house_number.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/read_prefecture.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/read_prefecture.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser/read_town.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser/read_town.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/parser.rs` & `japanese_address_parser_py-0.1.0b14/core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/core/src/util/converter.rs` & `japanese_address_parser_py-0.1.0b14/core/src/util/converter.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/README.md` & `japanese_address_parser_py-0.1.0b14/README.md`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/python/README.md` & `japanese_address_parser_py-0.1.0b14/python/README.md`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/python/japanese_address_parser_py.pyi` & `japanese_address_parser_py-0.1.0b14/python/japanese_address_parser_py.pyi`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/python/src/lib.rs` & `japanese_address_parser_py-0.1.0b14/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `japanese_address_parser_py-0.1.0b13/Cargo.lock` & `japanese_address_parser_py-0.1.0b14/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -112,17 +112,17 @@
 checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
@@ -252,17 +252,17 @@
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "hyper"
-version = "1.2.0"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
+checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "http",
  "http-body",
  "httparse",
@@ -345,19 +345,20 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "japanese-address-parser"
-version = "0.1.0-beta.13"
+version = "0.1.0-beta.14"
 dependencies = [
  "itertools",
  "js-sys",
  "nom",
+ "rapidfuzz",
  "regex",
  "reqwest",
  "serde",
  "test-case",
  "tokio",
  "wasm-bindgen-test",
 ]
@@ -540,26 +541,26 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -567,60 +568,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python"
-version = "0.1.0-beta.13"
+version = "0.1.0-beta.14"
 dependencies = [
  "japanese-address-parser",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -628,14 +629,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rapidfuzz"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "270e04e5ea61d40841942bb15e451c29ee1618637bcf97fc7ede5dd4a9b1601b"
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
@@ -667,17 +674,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "base64",
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "http",
@@ -730,17 +737,17 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki",
  "subtle",
  "zeroize",
@@ -789,17 +796,17 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.6.5"
@@ -809,28 +816,28 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -880,17 +887,17 @@
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -936,15 +943,15 @@
  "quote",
  "syn",
  "test-case-core",
 ]
 
 [[package]]
 name = "tests"
-version = "0.1.0-beta.13"
+version = "0.1.0-beta.14"
 dependencies = [
  "csv",
  "japanese-address-parser",
  "serde",
  "tokio",
 ]
 
@@ -1113,15 +1120,15 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm"
-version = "0.1.0-beta.13"
+version = "0.1.0-beta.14"
 dependencies = [
  "console_error_panic_hook",
  "japanese-address-parser",
  "serde-wasm-bindgen",
  "wasm-bindgen",
  "wasm-bindgen-futures",
 ]
@@ -1247,15 +1254,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1267,110 +1274,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
```

### Comparing `japanese_address_parser_py-0.1.0b13/PKG-INFO` & `japanese_address_parser_py-0.1.0b14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: japanese-address-parser-py
-Version: 0.1.0b13
+Version: 0.1.0b14
 Classifier: Topic :: Text Processing
 Classifier: Programming Language :: Rust
 Classifier: Typing :: Typed
 Summary: A Rust Library to parse japanese addresses.
 Keywords: converter,utility,geo,rust
 Author: Yuuki Toriyama <github@toriyama.dev>
 Author-email: Yuuki Toriyama <github@toriyama.dev>
```

