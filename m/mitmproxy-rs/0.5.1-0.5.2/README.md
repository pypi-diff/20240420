# Comparing `tmp/mitmproxy_rs-0.5.1.tar.gz` & `tmp/mitmproxy_rs-0.5.2.tar.gz`

## Comparing `mitmproxy_rs-0.5.1.tar` & `mitmproxy_rs-0.5.2.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0     1001      127      316 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.cargo/config.toml
--rw-r--r--   0     1001      127       28 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/FUNDING.yml
--rw-r--r--   0     1001      127      337 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/dependabot.yml
--rw-r--r--   0     1001      127        5 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/python-version.txt
--rwxr-xr-x   0     1001      127     2231 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/scripts/build-macos-redirector.sh
--rw-r--r--   0     1001      127      454 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/scripts/pin-versions.py
--rw-r--r--   0     1001      127     1528 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/workflows/autofix.yml
--rw-r--r--   0     1001      127     7201 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     1755 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.github/workflows/docs.yml
--rw-r--r--   0     1001      127       87 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/.gitignore
--rw-r--r--   0     1001      127     6348 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/CHANGELOG.md
--rwxr-xr-x   0     1001      127     1958 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/CONTRIBUTING.md
--rw-r--r--   0     1001      127     1080 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/LICENSE
--rw-r--r--   0     1001      127     4014 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/README.md
--rw-r--r--   0     1001      127   293989 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/architecture.png
--rw-r--r--   0     1001      127       22 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/.gitignore
--rw-r--r--   0     1001      127      220 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/local.conf
--rw-r--r--   0     1001      127      214 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/nonlocal.conf
--rw-r--r--   0     1001      127    67352 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/openvpnserv.exe
--rw-r--r--   0     1001      127    10121 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/plot.py
--rwxr-xr-x   0     1001      127     1730 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/process.rs
--rw-r--r--   0     1001      127     2375 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/py_echo_client.py
--rw-r--r--   0     1001      127     1246 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/py_echo_server.py
--rw-r--r--   0     1001      127     2346 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/wg_echo_client.py
--rw-r--r--   0     1001      127     2036 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/benches/wg_echo_server.py
--rw-r--r--   0     1001      127       70 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/.swift-format
--rw-r--r--   0     1001      127      201 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/.swiftlint.yml
--rw-r--r--   0     1001      127      306 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/README.md
--rw-r--r--   0     1001      127        0 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/mitmproxy_macos/__init__.py
--rw-r--r--   0     1001      127      957 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Info.plist
--rw-r--r--   0     1001      127   154566 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Resources/mitmproxy.icns
--rw-r--r--   0     1001      127      725 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/pyproject.toml
--rw-r--r--   0     1001      127       18 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/.gitignore
--rw-r--r--   0     1001      127      729 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/ExportOptions.plist
--rw-r--r--   0     1001      127     1357 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/README.md
--rw-r--r--   0     1001      127    30743 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/ipc/mitmproxy_ipc.pb.swift
--rw-r--r--   0     1001      127     4062 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/ipc/utils.swift
--rw-r--r--   0     1001      127     1321 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0     1001      127   310258 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-1024.png
--rw-r--r--   0     1001      127    27567 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-128.png
--rw-r--r--   0     1001      127     1998 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-16.png
--rw-r--r--   0     1001      127    62133 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-256.png
--rw-r--r--   0     1001      127     4949 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-32.png
--rw-r--r--   0     1001      127   139022 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-512.png
--rw-r--r--   0     1001      127    11972 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-64.png
--rw-r--r--   0     1001      127       63 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/Contents.json
--rw-r--r--   0     1001      127     4343 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/app.swift
--rw-r--r--   0     1001      127      387 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/macos_redirector.entitlements
--rw-r--r--   0     1001      127    26440 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.pbxproj
--rw-r--r--   0     1001      127      135 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.xcworkspace/contents.xcworkspacedata
--rw-r--r--   0     1001      127      238 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-r--r--   0     1001      127      311 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
--rw-r--r--   0     1001      127     3996 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/xcshareddata/xcschemes/macos-redirector.xcscheme
--rw-r--r--   0     1001      127     5453 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/FlowExtensions.swift
--rw-r--r--   0     1001      127      497 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/Info.plist
--rw-r--r--   0     1001      127     1174 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/InterceptConf.swift
--rw-r--r--   0     1001      127     1352 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/ProcessInfoCache.swift
--rw-r--r--   0     1001      127     7451 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/TransparentProxyProvider.swift
--rw-r--r--   0     1001      127       79 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/libproc-Bridging-Header.h
--rw-r--r--   0     1001      127      391 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/main.swift
--rw-r--r--   0     1001      127      321 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/network_extension.entitlements
--rw-r--r--   0     1001      127     2327 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-macos/version-info.toml
--rw-r--r--   0     1001      127      555 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/README.md
--rw-r--r--   0     1001      127    61349 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/LICENSE
--rw-r--r--   0     1001      127        6 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WINDIVERT_VERSION
--rw-r--r--   0     1001      127    47616 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WinDivert.dll
--rw-r--r--   0     1001      127    25422 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WinDivert.lib
--rw-r--r--   0     1001      127    94144 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WinDivert64.sys
--rw-r--r--   0     1001      127     1221 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/__init__.py
--rw-r--r--   0     1001      127      596 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-windows/pyproject.toml
--rwxr-xr-x   0     1001      127     4293 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/intercept_conf.rs
--rw-r--r--   0     1001      127     1337 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/ipc/mitmproxy_ipc.proto
--rw-r--r--   0     1001      127     4070 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/ipc/mitmproxy_ipc.rs
--rw-r--r--   0     1001      127     1085 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/ipc/mod.rs
--rwxr-xr-x   0     1001      127      258 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/lib.rs
--rw-r--r--   0     1001      127     1420 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/macos.rs
--rwxr-xr-x   0     1001      127     5673 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/messages.rs
--rw-r--r--   0     1001      127     4157 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/core.rs
--rw-r--r--   0     1001      127     3778 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/icmp.rs
--rwxr-xr-x   0     1001      127      208 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/mod.rs
--rwxr-xr-x   0     1001      127     5300 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/task.rs
--rw-r--r--   0     1001      127    12839 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/tcp.rs
--rwxr-xr-x   0     1001      127    24478 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/tests.rs
--rw-r--r--   0     1001      127    11635 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/udp.rs
--rwxr-xr-x   0     1001      127     2711 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/network/virtual_device.rs
--rw-r--r--   0     1001      127    14378 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/packet_sources/macos.rs
--rwxr-xr-x   0     1001      127      761 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/packet_sources/mod.rs
--rw-r--r--   0     1001      127     4156 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/packet_sources/udp.rs
--rwxr-xr-x   0     1001      127     8333 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/packet_sources/windows.rs
--rwxr-xr-x   0     1001      127    14238 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/packet_sources/wireguard.rs
--rw-r--r--   0     1001      127      243 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/processes.rs
--rwxr-xr-x   0     1001      127      796 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/shutdown.rs
--rwxr-xr-x   0     1001      127        1 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/util.rs
--rw-r--r--   0     1001      127     5264 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/windows/icons.rs
--rw-r--r--   0     1001      127       51 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/windows/mod.rs
--rw-r--r--   0     1001      127     6552 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/windows/network.rs
--rw-r--r--   0     1001      127    10853 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/src/windows/processes.rs
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/Cargo.toml
--rw-r--r--   0     1001      127      116 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/.gitignore
--rw-r--r--   0     1001      127      235 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/README.md
--rw-r--r--   0     1001      127      132 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/__init__.py
--rw-r--r--   0     1001      127     3483 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/__init__.pyi
--rw-r--r--   0     1001      127      121 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/_pyinstaller/__init__.py
--rw-r--r--   0     1001      127      102 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/_pyinstaller/hook-mitmproxy_macos.py
--rw-r--r--   0     1001      127      280 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
--rw-r--r--   0     1001      127      104 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/_pyinstaller/hook-mitmproxy_windows.py
--rw-r--r--   0     1001      127        0 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/py.typed
--rw-r--r--   0     1001      127     2222 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/lib.rs
--rw-r--r--   0     1001      127     2054 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/process_info.rs
--rw-r--r--   0     1001      127     2870 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/base.rs
--rw-r--r--   0     1001      127     4269 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/local_redirector.rs
--rw-r--r--   0     1001      127      232 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/mod.rs
--rw-r--r--   0     1001      127     2210 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/udp.rs
--rw-r--r--   0     1001      127     3059 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/wireguard.rs
--rw-r--r--   0     1001      127     7610 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/stream.rs
--rw-r--r--   0     1001      127     5840 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/task.rs
--rw-r--r--   0     1001      127     6704 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/udp_client.rs
--rw-r--r--   0     1001      127     3621 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/src/util.rs
--rw-r--r--   0     1001      127      180 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy-rs/stubtest-allowlist.txt
--rw-r--r--   0     1001      127    70760 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/Cargo.lock
--rw-r--r--   0        0        0     2203 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.1/Cargo.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.1/pyproject.toml
--rw-r--r--   0     1001      127      102 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/_pyinstaller/hook-mitmproxy_macos.py
--rw-r--r--   0     1001      127      121 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/_pyinstaller/__init__.py
--rw-r--r--   0     1001      127      104 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/_pyinstaller/hook-mitmproxy_windows.py
--rw-r--r--   0     1001      127      280 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
--rw-r--r--   0     1001      127     3483 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/__init__.pyi
--rw-r--r--   0     1001      127      132 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/__init__.py
--rw-r--r--   0     1001      127        0 2023-12-19 14:09:51.000000 mitmproxy_rs-0.5.1/mitmproxy_rs/py.typed
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.1/PKG-INFO
+-rw-r--r--   0     1001      127      316 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.cargo/config.toml
+-rw-r--r--   0     1001      127       28 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/FUNDING.yml
+-rw-r--r--   0     1001      127      337 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/dependabot.yml
+-rw-r--r--   0     1001      127        5 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/python-version.txt
+-rwxr-xr-x   0     1001      127     2231 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/scripts/build-macos-redirector.sh
+-rw-r--r--   0     1001      127      454 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/scripts/pin-versions.py
+-rw-r--r--   0     1001      127     1528 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/workflows/autofix.yml
+-rw-r--r--   0     1001      127     7312 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     1755 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127       87 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/.gitignore
+-rw-r--r--   0     1001      127     6381 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/CHANGELOG.md
+-rwxr-xr-x   0     1001      127     1958 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0     1001      127     1080 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/LICENSE
+-rw-r--r--   0     1001      127     4014 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/README.md
+-rw-r--r--   0     1001      127   293989 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/architecture.png
+-rw-r--r--   0     1001      127       22 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/.gitignore
+-rw-r--r--   0     1001      127      220 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/local.conf
+-rw-r--r--   0     1001      127      214 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/nonlocal.conf
+-rw-r--r--   0     1001      127    67352 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/openvpnserv.exe
+-rw-r--r--   0     1001      127    10121 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/plot.py
+-rwxr-xr-x   0     1001      127     1730 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/process.rs
+-rw-r--r--   0     1001      127     2375 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/py_echo_client.py
+-rw-r--r--   0     1001      127     1246 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/py_echo_server.py
+-rw-r--r--   0     1001      127     2346 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/wg_echo_client.py
+-rw-r--r--   0     1001      127     2036 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/benches/wg_echo_server.py
+-rw-r--r--   0     1001      127       70 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/.swift-format
+-rw-r--r--   0     1001      127      201 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/.swiftlint.yml
+-rw-r--r--   0     1001      127      306 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/README.md
+-rw-r--r--   0     1001      127        0 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/mitmproxy_macos/__init__.py
+-rw-r--r--   0     1001      127      957 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Info.plist
+-rw-r--r--   0     1001      127   154566 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Resources/mitmproxy.icns
+-rw-r--r--   0     1001      127      725 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/pyproject.toml
+-rw-r--r--   0     1001      127       18 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/.gitignore
+-rw-r--r--   0     1001      127      729 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/ExportOptions.plist
+-rw-r--r--   0     1001      127     1357 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/README.md
+-rw-r--r--   0     1001      127    30743 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/ipc/mitmproxy_ipc.pb.swift
+-rw-r--r--   0     1001      127     4062 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/ipc/utils.swift
+-rw-r--r--   0     1001      127     1321 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0     1001      127   310258 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-1024.png
+-rw-r--r--   0     1001      127    27567 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-128.png
+-rw-r--r--   0     1001      127     1998 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-16.png
+-rw-r--r--   0     1001      127    62133 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-256.png
+-rw-r--r--   0     1001      127     4949 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-32.png
+-rw-r--r--   0     1001      127   139022 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-512.png
+-rw-r--r--   0     1001      127    11972 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-64.png
+-rw-r--r--   0     1001      127       63 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/Contents.json
+-rw-r--r--   0     1001      127     4343 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/app.swift
+-rw-r--r--   0     1001      127      387 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/macos_redirector.entitlements
+-rw-r--r--   0     1001      127    26440 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.pbxproj
+-rw-r--r--   0     1001      127      135 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+-rw-r--r--   0     1001      127      238 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0     1001      127      311 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
+-rw-r--r--   0     1001      127     3996 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/xcshareddata/xcschemes/macos-redirector.xcscheme
+-rw-r--r--   0     1001      127     5453 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/FlowExtensions.swift
+-rw-r--r--   0     1001      127      497 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/Info.plist
+-rw-r--r--   0     1001      127     1174 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/InterceptConf.swift
+-rw-r--r--   0     1001      127     1352 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/ProcessInfoCache.swift
+-rw-r--r--   0     1001      127     7451 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/TransparentProxyProvider.swift
+-rw-r--r--   0     1001      127       79 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/libproc-Bridging-Header.h
+-rw-r--r--   0     1001      127      391 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/main.swift
+-rw-r--r--   0     1001      127      321 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/network_extension.entitlements
+-rw-r--r--   0     1001      127     2335 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-macos/version-info.toml
+-rw-r--r--   0     1001      127      555 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/README.md
+-rw-r--r--   0     1001      127    61349 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/LICENSE
+-rw-r--r--   0     1001      127        6 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WINDIVERT_VERSION
+-rw-r--r--   0     1001      127    47616 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WinDivert.dll
+-rw-r--r--   0     1001      127    25422 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WinDivert.lib
+-rw-r--r--   0     1001      127    94144 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WinDivert64.sys
+-rw-r--r--   0     1001      127     1221 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/__init__.py
+-rw-r--r--   0     1001      127      596 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-windows/pyproject.toml
+-rwxr-xr-x   0     1001      127     4293 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/intercept_conf.rs
+-rw-r--r--   0     1001      127     1337 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/ipc/mitmproxy_ipc.proto
+-rw-r--r--   0     1001      127     4070 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/ipc/mitmproxy_ipc.rs
+-rw-r--r--   0     1001      127     1085 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/ipc/mod.rs
+-rwxr-xr-x   0     1001      127      258 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/lib.rs
+-rw-r--r--   0     1001      127     1420 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/macos.rs
+-rwxr-xr-x   0     1001      127     5673 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/messages.rs
+-rw-r--r--   0     1001      127     4157 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/core.rs
+-rw-r--r--   0     1001      127     3778 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/icmp.rs
+-rwxr-xr-x   0     1001      127      208 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/mod.rs
+-rwxr-xr-x   0     1001      127     5300 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/task.rs
+-rw-r--r--   0     1001      127    12839 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/tcp.rs
+-rwxr-xr-x   0     1001      127    24478 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/tests.rs
+-rw-r--r--   0     1001      127    11635 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/udp.rs
+-rwxr-xr-x   0     1001      127     2711 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/network/virtual_device.rs
+-rw-r--r--   0     1001      127    14378 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/packet_sources/macos.rs
+-rwxr-xr-x   0     1001      127      761 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/packet_sources/mod.rs
+-rw-r--r--   0     1001      127     4156 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/packet_sources/udp.rs
+-rwxr-xr-x   0     1001      127     8333 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/packet_sources/windows.rs
+-rwxr-xr-x   0     1001      127    14238 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/packet_sources/wireguard.rs
+-rw-r--r--   0     1001      127      243 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/processes.rs
+-rwxr-xr-x   0     1001      127      796 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/shutdown.rs
+-rwxr-xr-x   0     1001      127        1 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/util.rs
+-rw-r--r--   0     1001      127     5264 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/windows/icons.rs
+-rw-r--r--   0     1001      127       51 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/windows/mod.rs
+-rw-r--r--   0     1001      127     6552 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/windows/network.rs
+-rw-r--r--   0     1001      127    10853 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/src/windows/processes.rs
+-rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/Cargo.toml
+-rw-r--r--   0     1001      127      116 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/.gitignore
+-rw-r--r--   0     1001      127      235 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/README.md
+-rw-r--r--   0     1001      127      132 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/__init__.py
+-rw-r--r--   0     1001      127     3483 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/__init__.pyi
+-rw-r--r--   0     1001      127      121 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/_pyinstaller/__init__.py
+-rw-r--r--   0     1001      127      102 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/_pyinstaller/hook-mitmproxy_macos.py
+-rw-r--r--   0     1001      127      280 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
+-rw-r--r--   0     1001      127      104 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/_pyinstaller/hook-mitmproxy_windows.py
+-rw-r--r--   0     1001      127        0 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/py.typed
+-rw-r--r--   0     1001      127     2222 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/lib.rs
+-rw-r--r--   0     1001      127     2054 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/process_info.rs
+-rw-r--r--   0     1001      127     2871 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/base.rs
+-rw-r--r--   0     1001      127     4269 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/local_redirector.rs
+-rw-r--r--   0     1001      127      232 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/mod.rs
+-rw-r--r--   0     1001      127     2210 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/udp.rs
+-rw-r--r--   0     1001      127     3059 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/wireguard.rs
+-rw-r--r--   0     1001      127     7610 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/stream.rs
+-rw-r--r--   0     1001      127     5840 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/task.rs
+-rw-r--r--   0     1001      127     6746 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/udp_client.rs
+-rw-r--r--   0     1001      127     3621 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/src/util.rs
+-rw-r--r--   0     1001      127      180 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy-rs/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127    71051 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/Cargo.lock
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.2/Cargo.toml
+-rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.2/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/py.typed
+-rw-r--r--   0     1001      127      132 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/__init__.py
+-rw-r--r--   0     1001      127     3483 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/__init__.pyi
+-rw-r--r--   0     1001      127      104 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/_pyinstaller/hook-mitmproxy_windows.py
+-rw-r--r--   0     1001      127      280 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
+-rw-r--r--   0     1001      127      102 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/_pyinstaller/hook-mitmproxy_macos.py
+-rw-r--r--   0     1001      127      121 2024-04-20 01:33:45.000000 mitmproxy_rs-0.5.2/mitmproxy_rs/_pyinstaller/__init__.py
+-rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 mitmproxy_rs-0.5.2/PKG-INFO
```

### Comparing `mitmproxy_rs-0.5.1/.github/scripts/build-macos-redirector.sh` & `mitmproxy_rs-0.5.2/.github/scripts/build-macos-redirector.sh`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/.github/workflows/autofix.yml` & `mitmproxy_rs-0.5.2/.github/workflows/autofix.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   contents: read
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 env:
-  rust_clippy: "1.70"  # MSRV
+  rust_clippy: "1.74"  # MSRV
 
 jobs:
   protobuf:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v4
       - run: brew install swift-protobuf
@@ -34,19 +34,19 @@
           - os: windows-latest
           - os: macos-latest
           - os: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - run: rustup toolchain install ${{ env.rust_clippy }} --profile minimal --component rustfmt --component clippy
       - run: rustup default ${{ env.rust_clippy }}
-      - uses: Swatinem/rust-cache@3cf7f8cc28d1b4e7d01e3783be10a97d55d483c8  # v2.7.1
+      - uses: Swatinem/rust-cache@23bce251a8cd2ffc3c1075eaa2367cf899916d84  # v2.7.3
         timeout-minutes: 2
         continue-on-error: true
       # PyO3 wants recent Python on Windows.
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: .github/python-version.txt
 
       - run: cargo clippy --fix --allow-dirty --workspace
       - run: cargo fmt --all
       - run: git checkout src/ipc/mitmproxy_ipc.rs
```

### Comparing `mitmproxy_rs-0.5.1/.github/workflows/ci.yml` & `mitmproxy_rs-0.5.2/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         include:
           - os: windows-latest
-            rust: "1.70"  # MSRV
+            rust: "1.74"  # MSRV
             args: --exclude macos-certificate-truster
           - os: macos-latest
-            rust: "1.70"
+            rust: "1.74"
             args: --exclude windows-redirector
           - os: ubuntu-latest
             rust: stable
             args: --exclude windows-redirector --exclude macos-certificate-truster
     steps:
       - uses: actions/checkout@v4
       - name: Set up Rust toolchain
         run: rustup toolchain install ${{ matrix.rust }} --profile minimal
-      - uses: Swatinem/rust-cache@3cf7f8cc28d1b4e7d01e3783be10a97d55d483c8  # v2.7.1
+      - uses: Swatinem/rust-cache@23bce251a8cd2ffc3c1075eaa2367cf899916d84  # v2.7.3
         timeout-minutes: 2
         continue-on-error: true
       # PyO3 wants recent Python on Windows.
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: .github/python-version.txt
 
       - name: Run "cargo check"
         # the action-rs/cargo action adds inline annotations for "cargo check" output
         uses: actions-rs/cargo@9e120dd99b0fbad1c065f686657e914e76bd7b72
         with:
@@ -75,64 +75,64 @@
     steps:
       - uses: actions/checkout@v4
       - run: rustup toolchain install stable --profile minimal
       - run: rustup default stable
       - if: matrix.target
         run: rustup target add ${{ matrix.target }}
       - run: rustup show
-      - uses: Swatinem/rust-cache@3cf7f8cc28d1b4e7d01e3783be10a97d55d483c8  # v2.7.1
+      - uses: Swatinem/rust-cache@23bce251a8cd2ffc3c1075eaa2367cf899916d84  # v2.7.3
         timeout-minutes: 2
         continue-on-error: true
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: .github/python-version.txt
 
       - if: runner.os == 'Linux'
         name: Install maturin[zig] from PyPI
-        uses: install-pinned/maturin-with-zig@1c81abaaee669d7c37cd893e1037216ecf5df7e0
+        uses: install-pinned/maturin-with-zig@7dc6082180bb4d3acd615d58c00156b7d444c772
       - if: runner.os != 'Linux'
         name: Install maturin from PyPI
-        uses: install-pinned/maturin@63688f9ac50926e464a1968e2383270d2d18c07c
+        uses: install-pinned/maturin@dfebcaa782a69944b584ec164e97fbbd09885352
 
       - if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         run: python .github/scripts/pin-versions.py
 
       - run: maturin build --release ${{ matrix.args }}
         working-directory: ./mitmproxy-rs
 
       # ensure that sdist is building.
       # We do this here instead of a separate job because we don't want to wait for the entire matrix.
       - if: contains(matrix.args, 'sdist')
         run: pip install target/wheels/*.tar.gz
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-${{ runner.os }}-${{ matrix.target || 'x64' }}
           path: target/wheels
 
   build-macos-app:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         id: cache-app
         with:
           path: mitmproxy-macos/redirector/dist/
           key: macos-${{ hashFiles('mitmproxy-macos/redirector/**', '.github/scripts/build-macos-redirector.sh') }}
       - if: steps.cache-app.outputs.cache-hit != 'true' || hashFiles('mitmproxy-macos/redirector/dist/Mitmproxy Redirector.app.tar') == ''
         run: $GITHUB_WORKSPACE/.github/scripts/build-macos-redirector.sh
         working-directory: mitmproxy-macos/redirector
         env:
           APPLE_ID: ${{ secrets.APPLE_ID }}
           APPLE_APP_PASSWORD: ${{ secrets.APPLE_APP_PASSWORD }}
           APPLE_PROVISIONING_PROFILE_APP: ${{ secrets.APPLE_PROVISIONING_PROFILE_APP }}
           APPLE_PROVISIONING_PROFILE_EXT: ${{ secrets.APPLE_PROVISIONING_PROFILE_EXT }}
           APPLE_CERTIFICATE: ${{ secrets.APPLE_CERTIFICATE }}
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           name: macos-app
           path: mitmproxy-macos/redirector/dist/
 
   build-os-wheels:
     needs: build-macos-app
     strategy:
@@ -144,15 +144,15 @@
             build-rust: --package macos-certificate-truster
     runs-on: ${{ matrix.os }}-latest
     name: build mitmproxy-${{ matrix.os }}
     steps:
       - uses: actions/checkout@v4
 
       # Build Rust
-      - uses: Swatinem/rust-cache@3cf7f8cc28d1b4e7d01e3783be10a97d55d483c8  # v2.7.1
+      - uses: Swatinem/rust-cache@23bce251a8cd2ffc3c1075eaa2367cf899916d84  # v2.7.3
         timeout-minutes: 2
         continue-on-error: true
       - run: rustup toolchain install stable --profile minimal
       - run: rustup default stable
       - if: runner.os == 'macOS'
         run: rustup target add aarch64-apple-darwin
       - if: runner.os == 'macOS'
@@ -162,44 +162,45 @@
           lipo -create -output target/release/macos-certificate-truster target/x86_64-apple-darwin/release/macos-certificate-truster target/aarch64-apple-darwin/release/macos-certificate-truster
       - if: runner.os != 'macOS'
         run: cargo build --release ${{ matrix.build-rust }}
 
 
       # Download macOS app
       - if: runner.os == 'macOS'
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: macos-app
           path: mitmproxy-macos/redirector/dist/
 
       # Build & upload wheel
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version-file: .github/python-version.txt
       - name: Install build from PyPI
-        uses: install-pinned/build@8abfe6b59c77f639a26f11c0ce295f9940f7865f
+        uses: install-pinned/build@6921a57b43fbb0fd3bcc42465ec9b4f3630e0032
       - run: python -m build --wheel ./mitmproxy-${{ matrix.os }} --outdir target/wheels/
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-os-${{ runner.os }}
           path: target/wheels
 
   check:
     if: always()
     needs:
       - test
       - build
       - build-os-wheels
     uses: mhils/workflows/.github/workflows/alls-green.yml@main
     with:
       jobs: ${{ toJSON(needs) }}
 
   deploy:
-    uses: mhils/workflows/.github/workflows/python-deploy.yml@main
+    uses: mhils/workflows/.github/workflows/python-deploy.yml@v5
     needs: check
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     with:
-      artifact: wheels
+      artifact-pattern: wheels-*
+      artifact-merge-multiple: true
       # repository: testpypi
       # environment: deploy-testpypi
     secrets:
       password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `mitmproxy_rs-0.5.1/.github/workflows/docs.yml` & `mitmproxy_rs-0.5.2/.github/workflows/docs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 
 jobs:
   # Build the documentation and upload the static HTML files as an artifact.
   build:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
-      - uses: Swatinem/rust-cache@3cf7f8cc28d1b4e7d01e3783be10a97d55d483c8  # v2.7.1
+      - uses: Swatinem/rust-cache@23bce251a8cd2ffc3c1075eaa2367cf899916d84  # v2.7.3
         timeout-minutes: 2
         continue-on-error: true
       - name: Install maturin[zig] from PyPI
-        uses: install-pinned/maturin-with-zig@1c81abaaee669d7c37cd893e1037216ecf5df7e0
+        uses: install-pinned/maturin-with-zig@7dc6082180bb4d3acd615d58c00156b7d444c772
       - name: Install mypy from PyPI
-        uses: install-pinned/mypy@5257e4e0636763f6fb849c6354a2ff13d645d3a9
+        uses: install-pinned/mypy@c2223951641cbb406fa8526d08f0690899f130e4
       - name: Install pdoc from PyPI
-        uses: install-pinned/pdoc@1e3e54521769cb06a10c2c4479c682551d4c9dce
+        uses: install-pinned/pdoc@0e6f61cda677884443a526256e42093789b1e9eb
 
       - run: maturin build
         working-directory: ./mitmproxy-rs
       - run: pip install --no-index --find-links target/wheels/ mitmproxy_rs
 
       - run: stubtest --allowlist mitmproxy-rs/stubtest-allowlist.txt --mypy-config-file mitmproxy-rs/pyproject.toml mitmproxy_rs
 
       - run: pdoc -o docs/ mitmproxy_rs
 
-      - uses: actions/upload-pages-artifact@v2
+      - uses: actions/upload-pages-artifact@v3
         with:
           path: docs/
 
   # Deploy the artifact to GitHub pages.
   # This is a separate job so that only actions/deploy-pages has the necessary permissions.
   deploy:
     if: github.ref == 'refs/heads/main'
@@ -52,8 +52,8 @@
       pages: write
       id-token: write
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     steps:
       - id: deployment
-        uses: actions/deploy-pages@v2
+        uses: actions/deploy-pages@v4
```

### Comparing `mitmproxy_rs-0.5.1/CHANGELOG.md` & `mitmproxy_rs-0.5.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## 0.5.1
 
+- Dependency updates.
+
+## 0.5.1
+
 - Make server shutdown more robust.
 
 ## 0.5.0
 
 - UDP connections are now modeled as streams.
 
 ## 0.4.0
```

### Comparing `mitmproxy_rs-0.5.1/CONTRIBUTING.md` & `mitmproxy_rs-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/LICENSE` & `mitmproxy_rs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/README.md` & `mitmproxy_rs-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/architecture.png` & `mitmproxy_rs-0.5.2/architecture.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/openvpnserv.exe` & `mitmproxy_rs-0.5.2/benches/openvpnserv.exe`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/plot.py` & `mitmproxy_rs-0.5.2/benches/plot.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/process.rs` & `mitmproxy_rs-0.5.2/benches/process.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/py_echo_client.py` & `mitmproxy_rs-0.5.2/benches/py_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/py_echo_server.py` & `mitmproxy_rs-0.5.2/benches/py_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/wg_echo_client.py` & `mitmproxy_rs-0.5.2/benches/wg_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/benches/wg_echo_server.py` & `mitmproxy_rs-0.5.2/benches/wg_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Info.plist` & `mitmproxy_rs-0.5.2/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Resources/mitmproxy.icns` & `mitmproxy_rs-0.5.2/mitmproxy-macos/mitmproxy_macos/macos-certificate-truster.app/Contents/Resources/mitmproxy.icns`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/pyproject.toml` & `mitmproxy_rs-0.5.2/mitmproxy-macos/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/ExportOptions.plist` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/ExportOptions.plist`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/README.md` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/ipc/mitmproxy_ipc.pb.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/ipc/mitmproxy_ipc.pb.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/ipc/utils.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/ipc/utils.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/Contents.json` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-1024.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-1024.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-128.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-128.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-16.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-16.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-256.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-256.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-32.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-32.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-512.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-512.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-64.png` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/Assets.xcassets/AppIcon.appiconset/logo-circle-64.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector/app.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector/app.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.pbxproj` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/macos-redirector.xcodeproj/xcshareddata/xcschemes/macos-redirector.xcscheme` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/macos-redirector.xcodeproj/xcshareddata/xcschemes/macos-redirector.xcscheme`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/FlowExtensions.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/FlowExtensions.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/InterceptConf.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/InterceptConf.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/ProcessInfoCache.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/ProcessInfoCache.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/redirector/network-extension/TransparentProxyProvider.swift` & `mitmproxy_rs-0.5.2/mitmproxy-macos/redirector/network-extension/TransparentProxyProvider.swift`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-macos/version-info.toml` & `mitmproxy_rs-0.5.2/mitmproxy-macos/version-info.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,46 +8,46 @@
 ]
 
 [workspace.package]
 authors = [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version = "0.5.1"
+version = "0.5.2"
 publish = false
 repository = "https://github.com/mitmproxy/mitmproxy-rs"
 edition = "2021"
-rust-version = "1.70"
+rust-version = "1.74"  # MSRV
 
 [package]
 name = "mitmproxy"
 license = "MIT"
 authors.workspace = true
 version.workspace = true
 repository.workspace = true
 edition.workspace = true
 rust-version.workspace = true
 publish.workspace = true
 
 [dependencies]
-anyhow = { version = "1.0.75", features = ["backtrace"] }
+anyhow = { version = "1.0.79", features = ["backtrace"] }
 log = "0.4.18"
 once_cell = "1"
-pretty-hex = "0.4.0"
+pretty-hex = "0.4.1"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
 smoltcp = "0.10"
-tokio = { version = "1.34.0", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util", "process"] }
+tokio = { version = "1.35.1", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util", "process"] }
 boringtun = { version = "0.6", default-features = false }
 x25519-dalek = "=2.0.0-rc.3"
-async-trait = "0.1.74"
+async-trait = "0.1.77"
 console-subscriber = { version = "0.2.0", optional = true }
-image = "0.24.6"
+image = "0.24.8"
 prost = "0.12.3"
 tokio-util = { version = "0.7.10", features = ["codec"] }
-futures-util = { version = "0.3.29", features = ["sink"] }
+futures-util = { version = "0.3.30", features = ["sink"] }
 lru_time_cache = "0.11.11"
 internet-packet = { version = "0.2.0", features = ["smoltcp"] }
 
 # [patch.crates-io]
 # tokio = { path = "../tokio/tokio" }
 # smoltcp = { git = 'https://github.com/mhils/smoltcp', rev = 'f65351adfa92db5193f368368cb668bac721fe43' }
```

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/README.md` & `mitmproxy_rs-0.5.2/mitmproxy-windows/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/LICENSE` & `mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/LICENSE`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WinDivert.dll` & `mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WinDivert.dll`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WinDivert.lib` & `mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WinDivert.lib`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/WinDivert64.sys` & `mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/WinDivert64.sys`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/mitmproxy_windows/__init__.py` & `mitmproxy_rs-0.5.2/mitmproxy-windows/mitmproxy_windows/__init__.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-windows/pyproject.toml` & `mitmproxy_rs-0.5.2/mitmproxy-windows/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/intercept_conf.rs` & `mitmproxy_rs-0.5.2/src/intercept_conf.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/ipc/mitmproxy_ipc.proto` & `mitmproxy_rs-0.5.2/src/ipc/mitmproxy_ipc.proto`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/ipc/mitmproxy_ipc.rs` & `mitmproxy_rs-0.5.2/src/ipc/mitmproxy_ipc.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/ipc/mod.rs` & `mitmproxy_rs-0.5.2/src/ipc/mod.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/macos.rs` & `mitmproxy_rs-0.5.2/src/macos.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/messages.rs` & `mitmproxy_rs-0.5.2/src/messages.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/core.rs` & `mitmproxy_rs-0.5.2/src/network/core.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/icmp.rs` & `mitmproxy_rs-0.5.2/src/network/icmp.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/task.rs` & `mitmproxy_rs-0.5.2/src/network/task.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/tcp.rs` & `mitmproxy_rs-0.5.2/src/network/tcp.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/tests.rs` & `mitmproxy_rs-0.5.2/src/network/tests.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/udp.rs` & `mitmproxy_rs-0.5.2/src/network/udp.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/network/virtual_device.rs` & `mitmproxy_rs-0.5.2/src/network/virtual_device.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/packet_sources/macos.rs` & `mitmproxy_rs-0.5.2/src/packet_sources/macos.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/packet_sources/mod.rs` & `mitmproxy_rs-0.5.2/src/packet_sources/mod.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/packet_sources/udp.rs` & `mitmproxy_rs-0.5.2/src/packet_sources/udp.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/packet_sources/windows.rs` & `mitmproxy_rs-0.5.2/src/packet_sources/windows.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/packet_sources/wireguard.rs` & `mitmproxy_rs-0.5.2/src/packet_sources/wireguard.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/shutdown.rs` & `mitmproxy_rs-0.5.2/src/shutdown.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/windows/icons.rs` & `mitmproxy_rs-0.5.2/src/windows/icons.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/windows/network.rs` & `mitmproxy_rs-0.5.2/src/windows/network.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/src/windows/processes.rs` & `mitmproxy_rs-0.5.2/src/windows/processes.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/Cargo.toml` & `mitmproxy_rs-0.5.2/mitmproxy-rs/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 [lib]
 name = "mitmproxy_rs"
 crate-type = ["cdylib"]
 
 [dependencies]
 mitmproxy = { path = "../" }
-anyhow = { version = "1.0.75", features = ["backtrace"] }
+anyhow = { version = "1.0.79", features = ["backtrace"] }
 data-encoding = "2.5.0"
 log = "0.4.18"
 once_cell = "1"
-pyo3 = { version = "0.19.2", features = ["abi3", "abi3-py310", "extension-module", "anyhow"] }
-pyo3-asyncio = { version = "0.19.0", features = ["tokio-runtime"] }
+pyo3 = { version = "0.20.3", features = ["abi3", "abi3-py310", "extension-module", "anyhow"] }
+pyo3-asyncio = { version = "0.20", features = ["tokio-runtime"] }
 pyo3-log = "0.9.0"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
-tokio = { version = "1.34", features = ["macros", "net", "rt-multi-thread", "sync"] }
+tokio = { version = "1.35", features = ["macros", "net", "rt-multi-thread", "sync"] }
 boringtun = "0.6"
 tar = "0.4.40"
 console-subscriber = { version = "0.2.0", optional = true }
 
 
 [dev-dependencies]
 env_logger = "0.10"
```

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/mitmproxy_rs/__init__.pyi` & `mitmproxy_rs-0.5.2/mitmproxy-rs/mitmproxy_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/lib.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/process_info.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/process_info.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/base.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/base.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     shutdown_done: broadcast::Receiver<()>,
     start_shutdown: Option<broadcast::Sender<()>>,
 }
 
 impl Server {
     pub fn close(&mut self) {
         if let Some(trigger) = self.start_shutdown.take() {
-            log::info!("Shutting down.");
+            log::debug!("Shutting down.");
             trigger.send(()).ok();
         }
     }
 
     pub fn wait_closed<'p>(&self, py: Python<'p>) -> PyResult<&'p PyAny> {
         let mut receiver = self.shutdown_done.resubscribe();
         pyo3_asyncio::tokio::future_into_py(py, async move {
```

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/local_redirector.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/local_redirector.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/udp.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/udp.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/server/wireguard.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/server/wireguard.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/stream.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/task.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/task.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/udp_client.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/udp_client.rs`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,17 @@
                                 break;
                             }
                         },
                     }
                 }
             }
         }
+
+        assert!(!packet_needs_sending);
+
         log::debug!("UDP client task shutting down.");
         Ok(())
     }
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `mitmproxy_rs-0.5.1/mitmproxy-rs/src/util.rs` & `mitmproxy_rs-0.5.2/mitmproxy-rs/src/util.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/Cargo.lock` & `mitmproxy_rs-0.5.2/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -25,50 +25,50 @@
 dependencies = [
  "crypto-common",
  "generic-array",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.1"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea5d730647d4fadd988536d06fecce94b7b4f2a7efdae548f1cf4b63205518ab"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.3"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b84bf0a05bbb2a83e5eb6fa36bb6e87baa08193c35ff52bbf6b38d8af2890e46"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anyhow"
-version = "1.0.75"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4668cab20f66d8d020e1fbc0ebe47217433c1b6c8f2040faf858554e394ace6"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
 name = "apple-security-framework"
 version = "2.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07831f002eaa83d94f7e2c1300f3268a8f949c35a41dd99faceb6575c191d871"
 dependencies = [
  "apple-security-framework-sys",
- "bitflags 2.4.0",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "apple-security-framework-sys"
@@ -78,17 +78,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "arc-swap"
-version = "1.6.0"
+version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
@@ -107,42 +107,42 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.74"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a66537f1bb974b254c98ed142ff995236e81b9d0fe4db0575f46612cb15eb0f9"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "atomic-polyfill"
-version = "0.1.11"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3ff7eb3f316534d83a8a2c3d1674ace8a5a71198eba31e2e2b597833f699b28"
+checksum = "8cf2bce30dfe09ef0bfaef228b9d414faaf7e563035494d7fe092dba54b300f4"
 dependencies = [
  "critical-section",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "axum"
 version = "0.6.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b829e4e32b91e643de6eafe82b1d90675f5874230191a4ffbc1b336dec4d6bf"
 dependencies = [
@@ -183,17 +183,17 @@
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -204,17 +204,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.4"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ba43ea6f343b788c8764558649e08df62f86c6ef251fdaeb1ffd010a9ae50a2"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bit_field"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc827186963e592360843fb5ba4b973e145841266c1357f7180c43526f2e5b61"
 
@@ -222,17 +222,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4682ae6287fcf752ecaabbfcc7b6f9b72aa33933dc23a554d853aea8eea8635"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
@@ -270,50 +270,47 @@
  "tracing",
  "untrusted 0.9.0",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.0"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
 name = "byteorder"
-version = "1.4.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -339,37 +336,37 @@
  "cipher",
  "poly1305",
  "zeroize",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
 dependencies = [
  "ciborium-io",
- "half 1.8.2",
+ "half",
 ]
 
 [[package]]
 name = "cipher"
 version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
@@ -377,36 +374,36 @@
  "crypto-common",
  "inout",
  "zeroize",
 ]
 
 [[package]]
 name = "clap"
-version = "4.4.4"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1d7b8d5ec32af0fadc644bf1fd509a688c2103b185644bb1e29d164e0703136"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.4.4"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5179bb514e4d7c2051749d8fcefa2ed6d06a9f4e6d69faf3805f5d80b8cf8d56"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.5.1"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd7cc57abe963c6d3b9d8be5b06ba7c8957a930305ca90304f24ef040aa6f961"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
@@ -445,42 +442,42 @@
  "tracing",
  "tracing-core",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.5.1"
@@ -521,54 +518,45 @@
 name = "critical-section"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7059fff8937831a9ae6f0fe4d658ffabf58f2ca96aa9dec1c889f936f705f216"
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.8"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
- "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if",
  "crossbeam-utils",
- "memoffset",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
-dependencies = [
- "cfg-if",
-]
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -597,57 +585,57 @@
  "rustc_version",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "curve25519-dalek-derive"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83fdaf97f4804dcebfa5862639bc9ce4121e82140bec2a987ac5140294865b5b"
+checksum = "f46882e17999c6cc590af592290432be3bce0428cb0d5f8b6715e4dc7b383eb3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "data-encoding"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
 
 [[package]]
 name = "defmt"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2d011b2fee29fb7d659b83c43fce9a2cb4df453e16d441a51448e448f3f98"
+checksum = "3939552907426de152b3c2c6f51ed53f98f448babd26f28694c95f5906194595"
 dependencies = [
  "bitflags 1.3.2",
  "defmt-macros",
 ]
 
 [[package]]
 name = "defmt-macros"
-version = "0.3.6"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54f0216f6c5acb5ae1a47050a6645024e6edafc2ee32d421955eccfef12ef92e"
+checksum = "18bdc7a7b92ac413e19e95240e75d3a73a8d8e78aa24a594c22cbb4d44b4bbda"
 dependencies = [
  "defmt-parser",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "defmt-parser"
-version = "0.3.3"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "269924c02afd7f94bc4cecbfa5c379f6ffcf9766b3408fe63d22c728654eccd0"
+checksum = "ff4a5fefe330e8d7f31b16a318f9ce81000d8e35e69b93eae154d16d2278f70f"
 dependencies = [
  "thiserror",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
@@ -657,109 +645,104 @@
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "env_logger"
-version = "0.10.1"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95b3f3e67048839cb0d0781f445682a35113da7121f7c949db0e2be96a4fbece"
+checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
  "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
-name = "errno"
-version = "0.3.3"
+name = "equivalent"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "136526188508e25c6fef639d7927dfb3e0e3084488bf202267829cf7fc23dbdd"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys",
-]
+checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
+name = "errno"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "etherparse"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "827292ea592108849932ad8e30218f8b1f21c0dfd0696698a18b5d0aed62d990"
 dependencies = [
  "arrayvec",
 ]
 
 [[package]]
 name = "exr"
-version = "1.71.0"
+version = "1.72.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "832a761f35ab3e6664babfbdc6cef35a4860e816ec3916dcfd0882954e98a8a8"
+checksum = "887d93f60543e9a9362ef8a21beedd0a833c5d9610e18c67abe15a5963dcb1a4"
 dependencies = [
  "bit_field",
  "flume",
- "half 2.2.1",
+ "half",
  "lebe",
  "miniz_oxide",
  "rayon-core",
  "smallvec",
  "zune-inflate",
 ]
 
 [[package]]
 name = "fdeflate"
-version = "0.3.0"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
+checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
 dependencies = [
  "simd-adler32",
 ]
 
 [[package]]
 name = "fiat-crypto"
 version = "0.1.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e825f6987101665dea6ec934c09ec6d721de7bc1bf92248e1d5810c8cd636b77"
 
 [[package]]
 name = "filetime"
-version = "0.2.22"
+version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4029edd3e734da6fe05b6cd7bd2960760a616bd2ddd0d59a0124746d6272af0"
+checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6c98ee8095e9d1dcbf2fcc6d95acccb90d1c81db1e44725c6a984b1dbdfb010"
+checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
@@ -774,88 +757,88 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "futures"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.28"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf34a163b5c4c52d0478a4d757da8fb65cabef42ba90515efee0f6f9fa45aaa"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53b153fd91e4b0147f4aced87be237c98248656bb01050b96bf3ee89220a8ddb"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36d3378ee38c2a36ad710c5d30c2911d752cb941c00c72dbabfb786a7970817"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efd193069b0ddadc69c46389b740bbccdd97203899b48d09c5f7969591d6bae2"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -873,70 +856,65 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gif"
-version = "0.12.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80792593675e051cf94a4b111980da2ba60d4a83e43e0048c5693baab3977045"
+checksum = "3fb2d69b19215e18bb912fa30f7ce15846e301408695e44e0ef719f1da9e19f2"
 dependencies = [
  "color_quant",
  "weezl",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "h2"
-version = "0.3.21"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91fc23aa11be92976ef4729127f1a74adf36d8436f7816b185d18df956790833"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap",
+ "indexmap 2.2.6",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "1.8.2"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
-
-[[package]]
-name = "half"
-version = "2.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
+ "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hash32"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -948,44 +926,56 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hashbrown"
+version = "0.14.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+
+[[package]]
 name = "hdrhistogram"
-version = "7.5.2"
+version = "7.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f19b9f54f7c7f55e31401bb647626ce0cf0f67b0004982ce815b3ee72a02aa8"
+checksum = "765c9198f173dd59ce26ff9f95ef0aafd0a0fe01fb9d72841bc5066a4c06511d"
 dependencies = [
- "base64 0.13.1",
+ "base64 0.21.7",
  "byteorder",
  "flate2",
  "nom",
  "num-traits",
 ]
 
 [[package]]
 name = "heapless"
-version = "0.7.16"
+version = "0.7.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db04bc24a18b9ea980628ecf00e6c0264f3c1426dac36c00cb49b6fbad8b0743"
+checksum = "cdc6457c0eb62c71aac4bc17216026d8410337c4126773b9c5daba343f17964f"
 dependencies = [
  "atomic-polyfill",
  "hash32",
  "rustc_version",
  "spin 0.9.8",
  "stable_deref_trait",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -996,28 +986,28 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.9"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -1036,30 +1026,30 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.27"
+version = "0.14.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
+checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.4.9",
+ "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -1072,46 +1062,55 @@
  "pin-project-lite",
  "tokio",
  "tokio-io-timeout",
 ]
 
 [[package]]
 name = "image"
-version = "0.24.7"
+version = "0.24.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f3dfdbdd72063086ff443e297b61695500514b1e41095b6fb9a5ab48a70a711"
+checksum = "5690139d2f55868e080017335e4b94cb7414274c74f1669c84fb5feba2c9f69d"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
  "exr",
  "gif",
  "jpeg-decoder",
- "num-rational",
  "num-traits",
  "png",
  "qoi",
  "tiff",
 ]
 
 [[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
- "hashbrown",
+ "hashbrown 0.12.3",
+]
+
+[[package]]
+name = "indexmap"
+version = "2.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
+dependencies = [
+ "equivalent",
+ "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inout"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
@@ -1154,61 +1153,61 @@
 name = "ip_network_table-deps-treebitmap"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e537132deb99c0eb4b752f0346b6a836200eaaa3516dd7e5514b63930a09e5d"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
  "hermit-abi",
- "rustix",
- "windows-sys",
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.11.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jpeg-decoder"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
+checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
 dependencies = [
  "rayon",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -1219,49 +1218,49 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.7"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a9bad9f94746442c783ca431b22403b519cd7fbeed0533fdd6328b2f2212128"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lru_time_cache"
 version = "0.11.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9106e1d747ffd48e6be5bb2d97fa706ed25b144fbee4d5c02eae110cd8d6badd"
 
 [[package]]
 name = "macos-certificate-truster"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "apple-security-framework",
 ]
 
 [[package]]
 name = "managed"
 version = "0.8.0"
@@ -1281,23 +1280,23 @@
 name = "matchit"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e7465ac9959cc2b1404e8e2367b43684a6d13790fe23056cc8c6c5a6b7bcb94"
 
 [[package]]
 name = "memchr"
-version = "2.6.3"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f232d6ef707e1956a43342693d2a31e72989554d58299d7a88738cc95b0d35c"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
@@ -1308,47 +1307,47 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.9"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3dce281c5e46beae905d4de1870d8b1509a9142b62eedf18b443b011ca8343d0"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mitm-wg-test-client"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "anyhow",
  "boringtun",
  "data-encoding",
  "hex",
  "smoltcp",
 ]
 
 [[package]]
 name = "mitmproxy"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "anyhow",
  "apple-security-framework",
  "async-trait",
  "boringtun",
  "console-subscriber",
  "criterion",
@@ -1369,15 +1368,15 @@
  "tokio-util",
  "windows 0.52.0",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy_rs"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "anyhow",
  "boringtun",
  "console-subscriber",
  "data-encoding",
  "env_logger",
  "log",
@@ -1405,15 +1404,15 @@
 
 [[package]]
 name = "nix"
 version = "0.27.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2eb04e9c688eff1c89d72b407f168cf79bb9e867a9d3323ed6c01519eb9cc053"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags 2.5.0",
  "cfg-if",
  "libc",
 ]
 
 [[package]]
 name = "nom"
 version = "7.1.3"
@@ -1421,39 +1420,18 @@
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
-name = "num-rational"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1462,105 +1440,105 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opaque-debug"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
+checksum = "c08d65885ee38876c4f86fa503fb49d7b507c2b62552df7c70b2fce627e06381"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.3.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project"
-version = "1.1.3"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fda4ed1c6c173e3fc7a83629421152e01d7b1f9b7f65fb301e490e8cfc656422"
+checksum = "b6bf43b791c5b9e34c3d182969b4abb522f9343702850a2e57f460d00d09b4b3"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.3"
+version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4359fd9c9171ec6e8c62926d6faaf553a8dc3f64e1507e76da7911b4f6a04405"
+checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "platforms"
-version = "3.1.2"
+version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4503fa043bf02cee09a9582e9554b4c6403b2ef55e4612e96561d294419429f8"
+checksum = "db23d408679286588f4d4644f965003d056e3dd5abcaaa938116871d7ce2fee7"
 
 [[package]]
 name = "plotters"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
@@ -1584,17 +1562,17 @@
 checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "png"
-version = "0.17.10"
+version = "0.17.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd75bf2d8dd3702b9707cdbc56a5b9ef42cec752eb8b3bafc01234558442aa64"
+checksum = "06e4b0d3d1312775e782c86c91a111aa1f910cbb65e1337f9975b5f9a554b5e1"
 dependencies = [
  "bitflags 1.3.2",
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
@@ -1607,24 +1585,30 @@
 dependencies = [
  "cpufeatures",
  "opaque-debug",
  "universal-hash",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "pretty-hex"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6b968ed37d62e35b4febaba13bfa231b0b7929d68b8a94e65445a17e2d35f"
+checksum = "bbc83ee4a840062f368f9096d80077a9841ec117e17e7f700df81958f1451254"
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
@@ -1644,99 +1628,100 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.67"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d433d9f1a3e8c1263d9456598b16fec66f4acc9a74dacffd35c7bb09b3a1328"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "146c289cda302b98a28d40c8b3b90498d6e526dd24ac2ecea73e4e491685b94a"
+checksum = "d0f5d036824e4761737860779c906171497f6d55681139d8312388f8fe398922"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efb6c9a1dd1def8e2124d17e83a20af56f1570d6c2d2bd9e266ccb768df3840e"
+checksum = "19de2de2a00075bf566bee3bd4db014b11587e84184d3f7a791bc17f1a8e9e48"
 dependencies = [
  "anyhow",
- "itertools 0.11.0",
+ "itertools 0.12.1",
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "prost-types"
-version = "0.12.1"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e081b29f63d83a4bc75cfc9f3fe424f9156cf92d8a4f0c9407cce9a1b67327cf"
+checksum = "3235c33eb02c1f1e212abdbe34c78b264b038fb58ca612664343271e36e55ffe"
 dependencies = [
  "prost",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "anyhow",
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-asyncio"
-version = "0.19.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2cc34c1f907ca090d7add03dc523acdd91f3a4dab12286604951e2f5152edad"
+checksum = "6ea6b68e93db3622f3bb3bf363246cf948ed5375afe7abff98ccbdd50b184995"
 dependencies = [
  "futures",
  "once_cell",
  "pin-project-lite",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -1747,49 +1732,51 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "qoi"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1818,84 +1805,84 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c27db03db7734835b3f53954b534c91069375ce6ccaa2e065441e07d9b6cdb1"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.12.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ce3fb6ad83f861aac485e76e1985cd109d9a3713802152be56c3b1f0e0658ed"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.5"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "697061221ea1b4a94a624f67d0ae2bfe4e22b8a17b6a192afb11046542cc8c47"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.3.8",
- "regex-syntax 0.7.5",
+ "regex-automata 0.4.6",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
  "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.8"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2f401f4955220693b56f8ec66ee9c78abffd8d1c4f23dc41a23839eb88f0795"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.5",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.5"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ring"
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
@@ -1921,36 +1908,36 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.14"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "747c788e9ce8e92b12cd485c49ddf90723550b654b32508f979b71a7b1ecda4f"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.0",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -1961,54 +1948,54 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.19"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad977052201c6de01a8ef2aa3378c4bd23217a056337d1d6da40468d267a4fb0"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.107"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b420ce6e3d8bd882e9b243c6eed35dbc9a6110c9769e74b584e0d68d1f20c65"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sharded-slab"
-version = "0.1.4"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "signal-hook-registry"
 version = "1.4.1"
@@ -2031,17 +2018,17 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "942b4a808e05215192e39f4ab80813e599068285906cc91aa64f923db842bd5a"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smoltcp"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d2e3a36ac8fea7b94e666dfa3871063d6e0a5c9d5d4fec9a1a6b7b6760f0229"
 dependencies = [
@@ -2053,30 +2040,20 @@
  "libc",
  "log",
  "managed",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.4.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
-dependencies = [
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
@@ -2105,23 +2082,22 @@
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
- "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.37"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7303ef2c05cd654186cb250d29049a24840ca25d2747c25c0381c8d9e2f582e8"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2139,62 +2115,62 @@
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.11"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "termcolor"
-version = "1.3.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6093bad37da69aab9d123a8091e4be0aa4a03e4d601ec641c327398315f62b64"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.48"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d6d7a740b8a666a7e828dd00da9c0dc290dff53154ea77ac109281de90589b7"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.48"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49922ecae66cc8a249b77e68d1d0623c1b2c514f0060c27cdc68bd62a1219d35"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "tiff"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d172b0f4d3fba17ba89811858b9d3d97f928aece846475bbda076ca46736211"
+checksum = "ba1310fcea54c6a9a4fd1aad794ecc02c31682f6bfbecdf460bf19533eed1e3e"
 dependencies = [
  "flate2",
  "jpeg-decoder",
  "weezl",
 ]
 
 [[package]]
@@ -2205,29 +2181,29 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.34.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0c014766411e834f7af5b8f4cf46257aab4036ca95e9d2c144a10f59ad6f5b9"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2 0.5.5",
+ "socket2",
  "tokio-macros",
  "tracing",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-io-timeout"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30b74022ada614a1b4834de765f9bb43877f910cc8ce4be40e89042c9223a8bf"
@@ -2240,22 +2216,22 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.14"
+version = "0.1.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
+checksum = "267ac89e0bec6e691e5813911606935d77c476ff49024f98abcea3e7b15e37af"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
@@ -2286,15 +2262,15 @@
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d560933a0de61cf715926b9cac824d4c883c2c43142f787595e48280c40a1d0e"
 dependencies = [
  "async-stream",
  "async-trait",
  "axum",
- "base64 0.21.4",
+ "base64 0.21.7",
  "bytes",
  "h2",
  "http",
  "http-body",
  "hyper",
  "hyper-timeout",
  "percent-encoding",
@@ -2312,15 +2288,15 @@
 name = "tower"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b8fa9be0de6cf49e536ce1851f987bd21a43b771b09473c3549a6c853db37c1c"
 dependencies = [
  "futures-core",
  "futures-util",
- "indexmap",
+ "indexmap 1.9.3",
  "pin-project",
  "pin-project-lite",
  "rand",
  "slab",
  "tokio",
  "tokio-util",
  "tower-layer",
@@ -2338,65 +2314,64 @@
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.26"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-subscriber"
-version = "0.3.17"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30a651bc37f915e81f087d86e62a18eec5f79550c7faff886f7090b4ea757c77"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
 dependencies = [
  "matchers",
  "once_cell",
  "regex",
  "sharded-slab",
  "thread_local",
  "tracing",
  "tracing-core",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
@@ -2404,17 +2379,17 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "universal-hash"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1de2c688dc15305988b563c3854064043356019f97a4b46276fe734c4f07ea"
 dependencies = [
@@ -2444,17 +2419,17 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
@@ -2469,81 +2444,81 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "weezl"
-version = "0.1.7"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
+checksum = "53a85b86a771b1c87058196170769dd264f66c0782acf1ae6cc51bfd64b39082"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -2607,29 +2582,29 @@
 [[package]]
 name = "windows"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-redirector"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
  "anyhow",
  "env_logger",
  "hex",
  "internet-packet",
  "log",
  "lru_time_cache",
@@ -2646,14 +2621,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
  "windows_aarch64_gnullvm 0.48.5",
  "windows_aarch64_msvc 0.48.5",
@@ -2662,110 +2646,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
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
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winres"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b68db261ef59e9e52806f688020631e987592bd83619edccda9c47d42cde4f6c"
 dependencies = [
@@ -2782,39 +2773,41 @@
  "rand_core",
  "serde",
  "zeroize",
 ]
 
 [[package]]
 name = "xattr"
-version = "1.0.1"
+version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4686009f71ff3e5c4dbcf1a282d0a44db3f021ba69350cd42086b3e5f1c6985"
+checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
  "libc",
+ "linux-raw-sys",
+ "rustix",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.6.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.37",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zune-inflate"
 version = "0.2.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73ab332fe2f6680068f3582b16a24f90ad7096d5d39b974d1c0aff0125116f02"
```

### Comparing `mitmproxy_rs-0.5.1/Cargo.toml` & `mitmproxy_rs-0.5.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 members = ["mitmproxy-rs"]
 
 [workspace.package]
 authors = [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version = "0.5.1"
+version = "0.5.2"
 publish = false
 repository = "https://github.com/mitmproxy/mitmproxy-rs"
 edition = "2021"
-rust-version = "1.70"
+rust-version = "1.74"  # MSRV
 
 [package]
 name = "mitmproxy"
 license = "MIT"
 authors.workspace = true
 version.workspace = true
 repository.workspace = true
 edition.workspace = true
 rust-version.workspace = true
 publish.workspace = true
 
 [dependencies]
-anyhow = { version = "1.0.75", features = ["backtrace"] }
+anyhow = { version = "1.0.79", features = ["backtrace"] }
 log = "0.4.18"
 once_cell = "1"
-pretty-hex = "0.4.0"
+pretty-hex = "0.4.1"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
 smoltcp = "0.10"
-tokio = { version = "1.34.0", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util", "process"] }
+tokio = { version = "1.35.1", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util", "process"] }
 boringtun = { version = "0.6", default-features = false }
 x25519-dalek = "=2.0.0-rc.3"
-async-trait = "0.1.74"
+async-trait = "0.1.77"
 console-subscriber = { version = "0.2.0", optional = true }
-image = "0.24.6"
+image = "0.24.8"
 prost = "0.12.3"
 tokio-util = { version = "0.7.10", features = ["codec"] }
-futures-util = { version = "0.3.29", features = ["sink"] }
+futures-util = { version = "0.3.30", features = ["sink"] }
 lru_time_cache = "0.11.11"
 internet-packet = { version = "0.2.0", features = ["smoltcp"] }
 
 # [patch.crates-io]
 # tokio = { path = "../tokio/tokio" }
 # smoltcp = { git = 'https://github.com/mhils/smoltcp', rev = 'f65351adfa92db5193f368368cb668bac721fe43' }
```

### Comparing `mitmproxy_rs-0.5.1/pyproject.toml` & `mitmproxy_rs-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
 ]
 
 dependencies = [
-    "mitmproxy_windows==0.5.1; os_name == 'nt'",
-    "mitmproxy_macos==0.5.1; sys_platform == 'darwin'",
+    "mitmproxy_windows==0.5.2; os_name == 'nt'",
+    "mitmproxy_macos==0.5.2; sys_platform == 'darwin'",
 ]
 
 [tool.black]
 line-length = 140
 include = '\.pyi?$'
 
 [project.entry-points.pyinstaller40]
```

### Comparing `mitmproxy_rs-0.5.1/mitmproxy_rs/__init__.pyi` & `mitmproxy_rs-0.5.2/mitmproxy_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.5.1/PKG-INFO` & `mitmproxy_rs-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mitmproxy_rs
-Version: 0.5.1
+Version: 0.5.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Dist: mitmproxy_windows ==0.5.1 ; os_name == 'nt'
-Requires-Dist: mitmproxy_macos ==0.5.1 ; sys_platform == 'darwin'
+Requires-Dist: mitmproxy_windows ==0.5.2 ; os_name == 'nt'
+Requires-Dist: mitmproxy_macos ==0.5.2 ; sys_platform == 'darwin'
 Author: Fabio Valentini <decathorpe@gmail.com>, Maximilian Hils <cargo@maximilianhils.com>
 Author-email: Fabio Valentini <decathorpe@gmail.com>, Maximilian Hils <cargo@maximilianhils.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/mitmproxy/mitmproxy-rs
```

