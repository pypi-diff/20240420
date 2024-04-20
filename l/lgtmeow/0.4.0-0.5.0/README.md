# Comparing `tmp/lgtmeow-0.4.0.tar.gz` & `tmp/lgtmeow-0.5.0.tar.gz`

## Comparing `lgtmeow-0.4.0.tar` & `lgtmeow-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 lgtmeow-0.4.0/Cargo.toml
--rw-r--r--   0     1001      127      244 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.editorconfig
--rw-r--r--   0     1001      127      107 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.github/renovate.json5
--rw-r--r--   0     1001      127     5449 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.github/workflows/build-and-release.yml
--rw-r--r--   0     1001      127      945 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.github/workflows/lint-and-fmt.yml
--rw-r--r--   0     1001      127      929 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127       67 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.gitignore
--rw-r--r--   0     1001      127      140 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/.vscode/settings.json
--rw-r--r--   0     1001      127    52528 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/Cargo.lock
--rw-r--r--   0     1001      127     1080 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/LICENSE
--rw-r--r--   0     1001      127     1146 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/README.md
--rw-r--r--   0     1001      127     7358 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/build.rs
--rw-r--r--   0     1001      127      633 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/cli/args.rs
--rw-r--r--   0     1001      127     1895 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/cli/choose.rs
--rw-r--r--   0     1001      127       45 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/cli/mod.rs
--rw-r--r--   0     1001      127     5940 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/cli/setup.rs
--rw-r--r--   0     1001      127      279 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/clipboard.rs
--rw-r--r--   0     1001      127     1215 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/config.rs
--rw-r--r--   0     1001      127      848 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/kitchen/combinate.rs
--rw-r--r--   0     1001      127      932 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/kitchen/metadata.rs
--rw-r--r--   0     1001      127       79 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/kitchen/mod.rs
--rw-r--r--   0     1001      127     3299 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/kitchen/partial_data.rs
--rw-r--r--   0     1001      127      994 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/kitchen/recommands.rs
--rw-r--r--   0     1001      127      651 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/main.rs
--rw-r--r--   0     1001      127     1065 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/reply.rs
--rw-r--r--   0     1001      127      546 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/src/storage.rs
--rw-r--r--   0     1001      127      676 2024-03-05 02:59:27.000000 lgtmeow-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 lgtmeow-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 lgtmeow-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      127      244 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.editorconfig
+-rw-r--r--   0     1001      127      107 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.github/renovate.json5
+-rw-r--r--   0     1001      127     5309 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.github/workflows/build-and-release.yml
+-rw-r--r--   0     1001      127      945 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.github/workflows/lint-and-fmt.yml
+-rw-r--r--   0     1001      127      929 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127       67 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.gitignore
+-rw-r--r--   0     1001      127      140 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/.vscode/settings.json
+-rw-r--r--   0     1001      127    54256 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/Cargo.lock
+-rw-r--r--   0     1001      127     1080 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/LICENSE
+-rw-r--r--   0     1001      127     1146 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/README.md
+-rw-r--r--   0     1001      127     7358 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/build.rs
+-rw-r--r--   0     1001      127      633 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/cli/args.rs
+-rw-r--r--   0     1001      127     1895 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/cli/choose.rs
+-rw-r--r--   0     1001      127       45 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/cli/mod.rs
+-rw-r--r--   0     1001      127     5940 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/cli/setup.rs
+-rw-r--r--   0     1001      127      279 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/clipboard.rs
+-rw-r--r--   0     1001      127     1215 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/config.rs
+-rw-r--r--   0     1001      127      848 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/kitchen/combinate.rs
+-rw-r--r--   0     1001      127      932 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/kitchen/metadata.rs
+-rw-r--r--   0     1001      127       79 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/kitchen/mod.rs
+-rw-r--r--   0     1001      127     3299 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/kitchen/partial_data.rs
+-rw-r--r--   0     1001      127     1389 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/kitchen/recommands.rs
+-rw-r--r--   0     1001      127      651 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/main.rs
+-rw-r--r--   0     1001      127     1065 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/reply.rs
+-rw-r--r--   0     1001      127      546 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/src/storage.rs
+-rw-r--r--   0     1001      127      676 2024-04-20 13:12:16.000000 lgtmeow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 lgtmeow-0.5.0/PKG-INFO
```

### Comparing `lgtmeow-0.4.0/Cargo.toml` & `lgtmeow-0.5.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lgtmeow"
-version = "0.4.0"
+version = "0.5.0"
 edition = "2021"
 authors = ["Nyakku Shigure <sigure.qaq@gmail.com>"]
 description = "LGTMeow 🐾 —— 「本喵觉得很不错～」"
 license = "MIT"
 homepage = "https://github.com/moefyit/lgtmeow"
 repository = "https://github.com/moefyit/lgtmeow"
 readme = "README.md"
@@ -14,34 +14,34 @@
 default = ["emoji-paw-prints"]
 emojis-all = ["emoji-paw-prints", "emoji-cat"]
 emoji-paw-prints = []
 emoji-cat = []
 copy = ["copypasta"]
 
 [build-dependencies]
-reqwest = { version = "0.11.24", features = ["json", "stream"] }
-tokio = { version = "1.36.0", features = ["full"] }
+reqwest = { version = "0.12.3", features = ["json", "stream"] }
+tokio = { version = "1.37.0", features = ["full"] }
 tokio-stream = "0.1"
 indicatif = "0.17.8"
 serde = { version = "1.0.197", features = ["derive"] }
-serde_json = "1.0.114"
+serde_json = "1.0.115"
 
 [target.'cfg(target_os = "linux")'.build-dependencies]
 openssl = { version = "0.10", features = ["vendored"] }
 
 [dependencies]
-clap = { version = "4.5.1", features = ["derive"] }
+clap = { version = "4.5.4", features = ["derive"] }
 lazy_static = "1.4.0"
 rand = "0.8.5"
 serde = { version = "1.0.197", features = ["derive"] }
-serde_json = "1.0.114"
+serde_json = "1.0.115"
 dirs = "5.0"
-cliclack = "0.1.13"
+cliclack = "0.2.5"
 console = "0.15.8"
-toml = "0.8.10"
+toml = "0.8.12"
 copypasta = { version = "0.10.1", optional = true }
 
 [profile.release]
 opt-level = "z"
 lto = true
 codegen-units = 1
 panic = "abort"
```

### Comparing `lgtmeow-0.4.0/.github/workflows/build-and-release.yml` & `lgtmeow-0.5.0/.github/workflows/build-and-release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,14 @@
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: "true"
           manylinux: auto
-          maturin-version: "1.4.0"
           # Refer to https://github.com/sfackler/rust-openssl/issues/2036#issuecomment-1724324145
           before-script-linux: |
             # If we're running on rhel centos, install needed packages.
             if command -v yum &> /dev/null; then
                 yum update -y && yum install -y perl-core openssl openssl-devel pkgconfig libatomic
 
                 # If we're running on i686 we need to symlink libatomic
@@ -68,15 +67,14 @@
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: "true"
-          maturin-version: "1.4.0"
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-windows-${{ matrix.target }}-${{ matrix.python-version }}
           path: dist
 
   macos:
@@ -93,15 +91,14 @@
           python-version: ${{ matrix.python-version }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: "true"
-          maturin-version: "1.4.0"
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.target }}-${{ matrix.python-version }}
           path: dist
 
   sdist:
@@ -109,15 +106,14 @@
     steps:
       - uses: actions/checkout@v4
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           args: --out dist
-          maturin-version: "1.4.0"
       - name: Upload sdist
         uses: actions/upload-artifact@v4
         with:
           name: wheels-sdist
           path: dist
 
   publish-pypi:
@@ -150,15 +146,15 @@
         with:
           pattern: wheels-*
           merge-multiple: true
           path: dist
       - name: Get tag name
         run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
       - name: Publish to GitHub
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
           draft: true
           files: dist/*
           tag_name: ${{ env.RELEASE_VERSION }}
 
   publish-crates-io:
     runs-on: ubuntu-latest
```

### Comparing `lgtmeow-0.4.0/.github/workflows/lint-and-fmt.yml` & `lgtmeow-0.5.0/.github/workflows/lint-and-fmt.yml`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/.github/workflows/test.yml` & `lgtmeow-0.5.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/Cargo.lock` & `lgtmeow-0.5.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,17 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.7"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -158,39 +158,39 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.5.1"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.1"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.0"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "307bc0538d5f0f83b8248db3087aa92fe504e4691294d0c96c0eabc33f47ba47"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "syn",
 ]
 
@@ -198,17 +198,17 @@
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "cliclack"
-version = "0.1.13"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be29210ca32b96e4f67fe9a520d2eeacc078d94ff4027100dc6b7262fdfec5c4"
+checksum = "4febf49beeedc40528e4956995631f1bbdb4d8804ef940b44351f393a996c739"
 dependencies = [
  "console",
  "indicatif",
  "once_cell",
  "textwrap",
  "zeroize",
 ]
@@ -482,17 +482,17 @@
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "h2"
-version = "0.3.24"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+checksum = "51ee2dd2e4f378392eeff5d51618cd9a63166a2513846bbc55f21cfacd9199d4"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -507,93 +507,118 @@
 name = "hashbrown"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "hermit-abi"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0c62115964e08cb8039170eb33c1d0e2388a256930279edca206fff675f82c3"
 
 [[package]]
 name = "http"
-version = "0.2.11"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.6"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
+checksum = "1cac85db508abc24a2e48553ba12a996e87244a0395ce011e62b37158745d643"
 dependencies = [
  "bytes",
  "http",
+]
+
+[[package]]
+name = "http-body-util"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0475f8b2ac86659c21b64320d5d653f9efe42acd2a4e560073ec61a155a34f1d"
+dependencies = [
+ "bytes",
+ "futures-core",
+ "http",
+ "http-body",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
-name = "httpdate"
-version = "1.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
-
-[[package]]
 name = "hyper"
-version = "0.14.28"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
+checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
 dependencies = [
  "bytes",
  "futures-channel",
- "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
- "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2",
+ "smallvec",
  "tokio",
- "tower-service",
- "tracing",
  "want",
 ]
 
 [[package]]
 name = "hyper-tls"
-version = "0.5.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6183ddfa99b85da61a140bea0efc93fdf56ceaa041b37d553518030827f9905"
+checksum = "70206fc6890eaca9fde8a0bf71caa2ddfc9fe045ac9e5c70df101a7dbde866e0"
 dependencies = [
  "bytes",
+ "http-body-util",
  "hyper",
+ "hyper-util",
  "native-tls",
  "tokio",
  "tokio-native-tls",
+ "tower-service",
+]
+
+[[package]]
+name = "hyper-util"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-util",
+ "http",
+ "http-body",
+ "hyper",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower",
+ "tower-service",
+ "tracing",
 ]
 
 [[package]]
 name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
@@ -665,15 +690,15 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "lgtmeow"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "clap",
  "cliclack",
  "console",
  "copypasta",
  "dirs",
  "indicatif",
@@ -951,14 +976,34 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
+name = "pin-project"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
+dependencies = [
+ "pin-project-internal",
+]
+
+[[package]]
+name = "pin-project-internal"
+version = "1.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
 
 [[package]]
 name = "pin-utils"
@@ -1073,28 +1118,30 @@
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.24"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
+checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
+ "http-body-util",
  "hyper",
  "hyper-tls",
+ "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
@@ -1134,22 +1181,29 @@
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.4"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
  "base64",
+ "rustls-pki-types",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+
+[[package]]
 name = "ryu"
 version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
 name = "schannel"
@@ -1213,17 +1267,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1423,17 +1477,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -1488,17 +1542,17 @@
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "toml"
-version = "0.8.10"
+version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a9aad4a3066010876e8dcf5a8a06e70a558751117a145c6ce2b82c2e2054290"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
@@ -1509,37 +1563,60 @@
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.5"
+version = "0.22.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99e68c159e8f5ba8a28c4eb7b0c0c190d77bb479047ca713270048145a9ad28a"
+checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
+name = "tower"
+version = "0.4.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
+dependencies = [
+ "futures-core",
+ "futures-util",
+ "pin-project",
+ "pin-project-lite",
+ "tokio",
+ "tower-layer",
+ "tower-service",
+ "tracing",
+]
+
+[[package]]
+name = "tower-layer"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
+
+[[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
+ "log",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
@@ -1972,17 +2049,17 @@
 checksum = "6b1dbce9e90e5404c5a52ed82b1d13fc8cfbdad85033b6f57546ffd1265f8451"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
-version = "0.50.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "x11-clipboard"
```

### Comparing `lgtmeow-0.4.0/LICENSE` & `lgtmeow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/README.md` & `lgtmeow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/build.rs` & `lgtmeow-0.5.0/build.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/cli/args.rs` & `lgtmeow-0.5.0/src/cli/args.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/cli/choose.rs` & `lgtmeow-0.5.0/src/cli/choose.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/cli/setup.rs` & `lgtmeow-0.5.0/src/cli/setup.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/config.rs` & `lgtmeow-0.5.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/kitchen/combinate.rs` & `lgtmeow-0.5.0/src/kitchen/combinate.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/kitchen/metadata.rs` & `lgtmeow-0.5.0/src/kitchen/metadata.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/kitchen/partial_data.rs` & `lgtmeow-0.5.0/src/kitchen/partial_data.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/kitchen/recommands.rs` & `lgtmeow-0.5.0/src/kitchen/recommands.rs`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,29 @@
     "1f525",      // 🔥
     "1f52e",      // 🔮
     "1f5ef-fe0f", // 🗯️
     "1f6f8",      // 🛸
     "1f947",      // 🥇
     "1f9ca",      // 🧊
     "1faa4",      // 🪤
+    "1f48c",      // 💌
+    "1fa82",      // 🪂
+    "1f32a-fe0f", // 🌪️
+    "1f30b",      // 🌋
+    "1f304",      // 🌄
+    "1f34c",      // 🍌
+    "1f3a3",      // 🎣
+    "1f3b3",      // 🎳
+    "1f9e9",      // 🧩
+    "1f58d-fe0f", // 🖍️
+    "1f3ac",      // 🎬
+    "1f4e0",      // 📠
+    "1f4be",      // 💾
+    "2757",       // ❗
+    "1f4ac",      // 💬
 ];
 
 /// A list of recommended combinations of 🐱
 #[cfg(feature = "emoji-cat")]
 pub static RECOMMAND_EMOJI_CODEPOINTS_COMBINATE_WITH_CAT: &[&str] = &[
     "1f4df", // 📟
 ];
```

### Comparing `lgtmeow-0.4.0/src/main.rs` & `lgtmeow-0.5.0/src/main.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/reply.rs` & `lgtmeow-0.5.0/src/reply.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/src/storage.rs` & `lgtmeow-0.5.0/src/storage.rs`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/pyproject.toml` & `lgtmeow-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lgtmeow-0.4.0/PKG-INFO` & `lgtmeow-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lgtmeow
-Version: 0.4.0
+Version: 0.5.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: LGTMeow 🐾 —— 「本喵觉得很不错～」
 Keywords: LGTM,meow,LGTMeow,cli,emoji-kitchen
```

