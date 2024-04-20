# Comparing `tmp/pixel_forge-0.1.0.tar.gz` & `tmp/pixel_forge-0.1.1.tar.gz`

## Comparing `pixel_forge-0.1.0.tar` & `pixel_forge-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,31 @@
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 pixel_forge-0.1.0/Cargo.toml
--rw-r--r--   0        0        0     1443 2024-04-18 21:58:17.000000 pixel_forge-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2024-04-07 15:16:51.000000 pixel_forge-0.1.0/LICENSE
--rw-r--r--   0        0        0      708 2024-04-19 07:51:28.000000 pixel_forge-0.1.0/README.md
--rw-r--r--   0        0        0   141756 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/docs/img/pixel_forge_banner.png
--rw-r--r--   0        0        0     3139 2024-04-19 08:06:54.000000 pixel_forge-0.1.0/pixel_forge.pyi
--rw-r--r--   0        0        0    12228 2024-04-18 22:32:07.000000 pixel_forge-0.1.0/src/capture.rs
--rw-r--r--   0        0        0     1650 2024-04-17 22:20:10.000000 pixel_forge-0.1.0/src/capture_utils.rs
--rw-r--r--   0        0        0     3484 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/src/direct_x.rs
--rw-r--r--   0        0        0     3278 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/src/frame.rs
--rw-r--r--   0        0        0      729 2024-04-18 22:21:47.000000 pixel_forge-0.1.0/src/lib.rs
--rw-r--r--   0        0        0    10055 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/src/monitor.rs
--rw-r--r--   0        0        0     7193 2024-04-18 21:58:17.000000 pixel_forge-0.1.0/src/window.rs
--rw-r--r--   0        0        0       79 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1331 2024-04-15 23:04:09.000000 pixel_forge-0.1.0/tests/test_capture.py
--rw-r--r--   0        0        0      676 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/tests/test_monitor.py
--rw-r--r--   0        0        0      360 2024-04-15 23:02:32.000000 pixel_forge-0.1.0/tests/test_window.py
--rw-r--r--   0        0        0    13242 2024-04-19 08:07:44.000000 pixel_forge-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1511 2024-04-19 08:07:27.000000 pixel_forge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 pixel_forge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 pixel_forge-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0     1443 2024-04-19 16:58:16.000000 pixel_forge-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2024-04-15 23:02:32.000000 pixel_forge-0.1.1/.gitignore
+-rw-r--r--   0        0        0      325 2024-04-20 19:22:44.000000 pixel_forge-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1091 2024-04-07 15:16:51.000000 pixel_forge-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2070 2024-04-20 19:40:31.000000 pixel_forge-0.1.1/README.md
+-rw-r--r--   0        0        0     2198 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      339 2024-04-20 15:17:12.000000 pixel_forge-0.1.1/docs/content/acknowledgements.rst
+-rw-r--r--   0        0        0      109 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/docs/content/capture.rst
+-rw-r--r--   0        0        0     1358 2024-04-20 15:17:12.000000 pixel_forge-0.1.1/docs/content/getting_started.rst
+-rw-r--r--   0        0        0      934 2024-04-20 15:17:12.000000 pixel_forge-0.1.1/docs/content/install.rst
+-rw-r--r--   0        0        0      214 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/docs/content/monitor.rst
+-rw-r--r--   0        0        0      211 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/docs/content/window.rst
+-rw-r--r--   0        0        0   141756 2024-04-15 23:02:32.000000 pixel_forge-0.1.1/docs/img/pixel_forge_banner.png
+-rw-r--r--   0        0        0      817 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0       62 2024-04-20 19:35:40.000000 pixel_forge-0.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0     4037 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/pixel_forge.pyi
+-rw-r--r--   0        0        0    13337 2024-04-20 19:22:08.000000 pixel_forge-0.1.1/src/capture.rs
+-rw-r--r--   0        0        0     1650 2024-04-17 22:20:10.000000 pixel_forge-0.1.1/src/capture_utils.rs
+-rw-r--r--   0        0        0     3484 2024-04-15 23:02:32.000000 pixel_forge-0.1.1/src/direct_x.rs
+-rw-r--r--   0        0        0     3278 2024-04-15 23:02:32.000000 pixel_forge-0.1.1/src/frame.rs
+-rw-r--r--   0        0        0      729 2024-04-19 08:26:55.000000 pixel_forge-0.1.1/src/lib.rs
+-rw-r--r--   0        0        0    10599 2024-04-20 15:17:12.000000 pixel_forge-0.1.1/src/monitor.rs
+-rw-r--r--   0        0        0     7121 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/src/window.rs
+-rw-r--r--   0        0        0       79 2024-04-15 23:02:32.000000 pixel_forge-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1331 2024-04-15 23:04:09.000000 pixel_forge-0.1.1/tests/test_capture.py
+-rw-r--r--   0        0        0      880 2024-04-20 19:24:12.000000 pixel_forge-0.1.1/tests/test_monitor.py
+-rw-r--r--   0        0        0      359 2024-04-20 19:34:52.000000 pixel_forge-0.1.1/tests/test_window.py
+-rw-r--r--   0        0        0    13725 2024-04-19 17:07:02.000000 pixel_forge-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1908 2024-04-20 19:52:37.000000 pixel_forge-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 pixel_forge-0.1.1/PKG-INFO
```

### Comparing `pixel_forge-0.1.0/Cargo.toml` & `pixel_forge-0.1.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pixel_forge"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pixel_forge"
 crate-type = ["cdylib"]
```

### Comparing `pixel_forge-0.1.0/.github/workflows/CI.yml` & `pixel_forge-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/.gitignore` & `pixel_forge-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/LICENSE` & `pixel_forge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/docs/img/pixel_forge_banner.png` & `pixel_forge-0.1.1/docs/img/pixel_forge_banner.png`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/src/capture.rs` & `pixel_forge-0.1.1/src/capture.rs`

 * *Files 12% similar despite different names*

```diff
@@ -54,18 +54,20 @@
 
 impl From<CaptureError> for PyErr {
     fn from(error: CaptureError) -> PyErr {
         PyRuntimeError::new_err(error.to_string())
     }
 }
 
-// The Capture struct is the central struct of pixel_forge. The main idea is to get either a monitor
-// or a window as target, create a Capture struct, and then start a capture thread that will update
-// the texture of the Capture struct whenever a new frame is available. We only materialize the
-// frame when the user requests it to avoid unnecessary copies.
+/// Capture class to capture frames from a monitor or a window.
+///
+/// The idea is to get either a :class:`.Monitor` or a :class:`.Window` as target, create a Capture
+/// object, and then start a capture thread that will update the internal frame of the Capture
+/// object whenever a new frame is available. Frames are only materialized, converted to NumPy
+/// arrays and passed over to Python when the user requests it to avoid unnecessary copies.
 #[pyclass]
 pub struct Capture {
     thread: Option<JoinHandle<Result<(), CaptureError>>>,
     thread_id: Arc<Mutex<Option<u32>>>,
     frame: Arc<Mutex<Option<Frame>>>,
 }
 
@@ -76,14 +78,30 @@
         Self {
             thread: None,
             thread_id: Arc::new(Mutex::new(None)),
             frame: Arc::new(Mutex::new(None)),
         }
     }
 
+    /// start(capture_target: CaptureTarget, await_first_frame: bool = True)
+    ///
+    /// Start the capture.
+    ///
+    /// This registeres an event handler that automatically updates the latest frame whenever a new
+    /// frame is available. The frame can be accessed using :meth:`frame`. Since the event handler
+    /// runs in a separate thread, the first frame might not be available immediately. To ensure a
+    /// frame is available before continuing, set ``await_first_frame`` to True. This will block the
+    /// main thread until the first frame is available.
+    ///
+    /// .. note::
+    ///    You have to call :meth:`start` before any frames become available.
+    ///
+    /// Args:
+    ///     capture_target: The :class:`.Monitor` or :class:`.Window` to capture.
+    ///     await_first_frame: Waits for the first frame to arrive if True.
     pub fn start(
         &mut self,
         capture_target: CaptureTarget,
         await_first_frame: Option<bool>,
     ) -> Result<(), CaptureError> {
         // In case of a window capture, check if the window is valid
         match capture_target {
@@ -226,35 +244,38 @@
             while self.frame.lock().is_none() & self.thread.is_some() {
                 sleep(Duration::from_millis(10));
             }
         }
         Ok(())
     }
 
-    // Python property to check if the capture thread is running
+    /// :``bool``: True if the capture thread is running, False otherwise.
     #[getter]
     pub fn active(&self) -> bool {
         self.thread.is_some()
     }
 
-    // Stop the capture thread and wait for it to join
+    /// Stop the capture thread, wait for it to join and invalidate the last frame.
     pub fn stop(&mut self) {
         // If the thread_id is set, send a WM_QUIT message to the message pumping thread. The
         // message pumping thread will receive the WM_QUIT message, stop its loop and close the
         // dispatcher queue
         if let Some(thread_id) = self.thread_id.lock().take() {
             let _ = unsafe { PostThreadMessageW(thread_id, WM_QUIT, WPARAM(0), LPARAM(0)) };
         }
         if let Some(thread) = self.thread.take() {
             let _ = thread.join().expect("Failed to join capture thread");
         }
         self.frame.lock().take(); // Clear the frame when the capture is stopped
     }
 
-    // Convert the frame into a numpy array and return it to the user
+    /// frame() -> np.ndarray
+    /// Convert the latest frame to an array and return it.
+    ///
+    /// :returns: The frame as a 3D NumPy array with dimensions [h w 4].
     #[pyo3(name = "frame")]
     pub fn py_frame(&self, py: Python) -> PyResult<Py<PyArray3<u8>>> {
         if self.thread.is_none() {
             return Err(PyRuntimeError::new_err("Capture thread is not running."));
         }
         let frame_guard = self.frame.lock();
         let frame = frame_guard.as_ref().ok_or(CaptureError::NoFrameAvailable)?;
```

### Comparing `pixel_forge-0.1.0/src/capture_utils.rs` & `pixel_forge-0.1.1/src/capture_utils.rs`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/src/direct_x.rs` & `pixel_forge-0.1.1/src/direct_x.rs`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/src/frame.rs` & `pixel_forge-0.1.1/src/frame.rs`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/src/lib.rs` & `pixel_forge-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/src/monitor.rs` & `pixel_forge-0.1.1/src/monitor.rs`

 * *Files 4% similar despite different names*

```diff
@@ -41,40 +41,45 @@
 
 impl From<MonitorError> for PyErr {
     fn from(error: MonitorError) -> PyErr {
         PyRuntimeError::new_err(error.to_string())
     }
 }
 
-/// Monitor device for the Windows operating system.
+/// Monitor(id: int | None = None) -> Monitor
+/// Monitor class for the Windows operating system.
 ///
-/// # Example
-/// ```no_run
-/// use pixel_forge::monitor::Monitor;
+/// Monitor can be used as capture target for the :class:`.Capture` class. It also provides some
+/// convenience methods to get information about the monitor.
 ///
-/// fn main() -> Result<(), Box<dyn std::error::Error>> {
-///     let monitor = primary_monitor()?;
-///     println!("Primary Monitor: {}", monitor.device_name()?);
-///
-///     Ok(())
-/// }
+/// Args:
+///    id: The index of the monitor. If None, the primary monitor is used.
 #[derive(Eq, PartialEq, Clone, Copy, Debug)]
 #[pyclass]
 pub struct Monitor {
     monitor_handle: HMONITOR,
 }
 
 #[pymethods]
 impl Monitor {
+    /// new(id: int | None = None) -> Monitor
+    ///
+    /// Create a :class:`.Monitor` instance.
+    ///
+    /// Args:
+    ///    id: The monitor ID. If None, the primary monitor is used.
     #[new]
-    pub fn new() -> Self {
-        primary_monitor().unwrap()
+    pub fn new(id: Option<usize>) -> Self {
+        match id {
+            Some(id) => Monitor::from_index(id).unwrap(),
+            None => primary_monitor().unwrap(),
+        }
     }
 
-    /// Return the pixel width of the monitor.
+    /// :``int``: The pixel width of the monitor.
     #[getter]
     pub fn width(&self) -> Result<u32, MonitorError> {
         let mut device_mode = DEVMODEW {
             dmSize: u16::try_from(mem::size_of::<DEVMODEW>()).unwrap(),
             ..DEVMODEW::default()
         };
         let name = HSTRING::from(self.device_name()?);
@@ -88,15 +93,15 @@
         } {
             return Err(MonitorError::MonitorSettingsError);
         }
 
         Ok(device_mode.dmPelsWidth)
     }
 
-    /// Returns the pixel height of the monitor.
+    /// :``int``: The pixel height of the monitor.
     #[getter]
     pub fn height(&self) -> Result<u32, MonitorError> {
         let mut device_mode = DEVMODEW {
             dmSize: u16::try_from(mem::size_of::<DEVMODEW>()).unwrap(),
             ..DEVMODEW::default()
         };
         let name = HSTRING::from(self.device_name()?);
@@ -110,22 +115,22 @@
         } {
             return Err(MonitorError::MonitorSettingsError);
         }
 
         Ok(device_mode.dmPelsHeight)
     }
 
-    /// Return the index of the monitor.
+    /// :``int``: The index of the monitor.
     #[getter]
     pub fn index(&self) -> Result<usize, MonitorError> {
         let device_name = self.device_name()?;
         Ok(device_name.replace("\\\\.\\DISPLAY", "").parse()?)
     }
 
-    /// Return the refresh rate of the monitor in Hertz.
+    /// :``int``: The refresh rate of the monitor in Hz.
     #[getter]
     pub fn refresh_rate(&self) -> Result<u32, MonitorError> {
         let mut device_mode = DEVMODEW {
             dmSize: u16::try_from(mem::size_of::<DEVMODEW>()).unwrap(),
             ..DEVMODEW::default()
         };
         let name = HSTRING::from(self.device_name()?);
@@ -139,15 +144,15 @@
         } {
             return Err(MonitorError::MonitorSettingsError);
         }
 
         Ok(device_mode.dmDisplayFrequency)
     }
 
-    /// Return the device name of the monitor.
+    /// :``str``: The monitor device name.
     #[getter]
     pub fn device_name(&self) -> Result<String, MonitorError> {
         let mut monitor_info = MONITORINFOEXW {
             monitorInfo: MONITORINFO {
                 cbSize: u32::try_from(mem::size_of::<MONITORINFOEXW>()).unwrap(),
                 rcMonitor: RECT::default(),
                 rcWork: RECT::default(),
@@ -174,15 +179,15 @@
                 .copied()
                 .collect::<Vec<u16>>(),
         )?;
 
         Ok(device_name)
     }
 
-    /// Return the device string of the monitor.
+    /// :``str``: The device string of the monitor.
     #[getter]
     pub fn device_string(&self) -> Result<String, MonitorError> {
         let mut monitor_info = MONITORINFOEXW {
             monitorInfo: MONITORINFO {
                 cbSize: u32::try_from(mem::size_of::<MONITORINFOEXW>()).unwrap(),
                 rcMonitor: RECT::default(),
                 rcWork: RECT::default(),
@@ -273,15 +278,20 @@
     /// Returns the raw HMONITOR of the monitor.
     #[must_use]
     pub const fn as_raw_hmonitor(&self) -> HMONITOR {
         self.monitor_handle
     }
 }
 
-/// Return the primary monitor.
+/// primary_monitor() -> Monitor
+///
+/// Get the primary monitor.
+///
+/// Returns:
+///    The monitor.
 #[pyfunction]
 pub fn primary_monitor() -> Result<Monitor, MonitorError> {
     let point = POINT { x: 0, y: 0 };
     let monitor_handle = unsafe { MonitorFromPoint(point, MONITOR_DEFAULTTONULL) };
 
     if monitor_handle.is_invalid() {
         return Err(MonitorError::NotFound);
@@ -300,15 +310,20 @@
     let monitors = &mut *(vec.0 as *mut Vec<Monitor>);
 
     monitors.push(Monitor { monitor_handle });
 
     TRUE
 }
 
-/// Return a list of all monitors.
+/// enumerate_monitors() -> list[Monitor]
+///
+/// Enumerate all monitors connected to the system.
+///
+/// Returns:
+///   The list of all monitors.
 #[pyfunction]
 pub fn enumerate_monitors() -> Result<Vec<Monitor>, MonitorError> {
     let mut monitors: Vec<Monitor> = Vec::new();
 
     unsafe {
         EnumDisplayMonitors(
             None,
```

### Comparing `pixel_forge-0.1.0/src/window.rs` & `pixel_forge-0.1.1/src/window.rs`

 * *Files 3% similar despite different names*

```diff
@@ -33,65 +33,53 @@
 }
 
 impl From<WindowError> for PyErr {
     fn from(error: WindowError) -> PyErr {
         PyRuntimeError::new_err(error.to_string())
     }
 }
-
+/// Window(name: str) -> Window
 /// Window abstraction for the Windows operating system.
 ///
-/// Window instances are one of two possible structs that can be passed as capture targets to the
-/// capture struct.
+/// Windows can be used as capture target for the :class:`.Capture` class.
 ///
-/// # Example
-/// ```no_run
-/// use pixel_forge::window::Window;
-///
-/// fn main() -> Result<(), Box<dyn std::error::Error>> {
-///     let window = foreground_window()?;
-///     println!("Foreground window title: {}", window.title()?);
-///
-///     Ok(())
-/// }
-/// ```
+/// Args:
+///     name: The name of the window.
 #[derive(Eq, PartialEq, Clone, Copy, Debug)]
 #[pyclass]
 pub struct Window {
     window_handle: HWND,
 }
 
 #[pymethods]
 impl Window {
-    /// Create a `Window` instance from a window name.
-    ///
-    /// # Arguments
+    /// from_name(name: str) -> Window
+    /// Create a :class:`.Window` instance from its name.
     ///
-    /// * `title` - The name of the window.
+    /// Args:
+    ///     name: The name of the window.
     ///
-    /// # Errors
+    /// Returns:
+    ///    The window instance.
     ///
-    /// `Error::NotFound`: No window with that name.
+    /// Raises:
+    ///    NotFound: The window with the given name was not found.
     #[new]
-    pub fn from_name(title: &str) -> Result<Window, WindowError> {
-        let hstring_title = HSTRING::from(title);
-        let window_handle = unsafe { FindWindowW(None, &hstring_title) };
+    pub fn new(name: &str) -> Result<Window, WindowError> {
+        let hstring_name = HSTRING::from(name);
+        let window_handle = unsafe { FindWindowW(None, &hstring_name) };
 
         if window_handle.0 == 0 {
-            return Err(WindowError::NotFound(String::from(title)));
+            return Err(WindowError::NotFound(String::from(name)));
         }
 
         Ok(Window { window_handle })
     }
 
-    /// Check if the window is a valid window.
-    ///
-    /// # Returns
-    ///
-    /// `true` if the window is valid, `false` otherwise.
+    /// :``bool``: True if the window is still valid (i.e., open), else False.
     #[getter]
     pub fn valid(&self) -> bool {
         if !unsafe { IsWindowVisible(self.window_handle).as_bool() } {
             return false;
         }
 
         let mut id = 0;
@@ -115,21 +103,17 @@
         } else {
             return false;
         }
 
         true
     }
 
-    /// Get the window title.
-    ///
-    /// # Returns
-    ///
-    /// The title.
+    /// :``str``: The name string of the window.
     #[getter]
-    pub fn title(&self) -> Result<String, WindowError> {
+    pub fn name(&self) -> Result<String, WindowError> {
         let len = unsafe { GetWindowTextLengthW(self.window_handle) };
 
         let mut name = vec![0u16; usize::try_from(len).unwrap() + 1];
         if len >= 1 {
             let copied = unsafe { GetWindowTextW(self.window_handle, &mut name) };
             if copied == 0 {
                 return Ok(String::new());
@@ -191,19 +175,23 @@
     if window.valid() {
         windows.push(window);
     }
 
     TRUE
 }
 
-/// Return a vector of all available windows.
+/// enumerate_windows() -> list[Window]
 ///
-/// # Errors
+/// Enumerate all windows that are currently available.
 ///
-/// `WindowError`: Enumerating the windows has failed.
+/// Returns:
+///     A list of all windows.
+///
+/// Raises:
+///    WindowError: Enumerating the windows has failed.
 #[pyfunction]
 pub fn enumerate_windows() -> Result<Vec<Window>, WindowError> {
     let mut windows: Vec<Window> = Vec::new();
 
     unsafe {
         EnumChildWindows(
             GetDesktopWindow(),
@@ -212,19 +200,23 @@
         )
         .ok()?;
     };
 
     Ok(windows)
 }
 
-/// Get the foreground window.
+/// foreground_window() -> Window
+///
+/// Get the currently active window.
 ///
-/// # Errors
+/// Returns:
+///    The active window.
 ///
-/// `WindowError`: No active window found.
+/// Raises:
+///   NoActiveWindow: No active window was found.
 #[pyfunction]
 pub fn foreground_window() -> Result<Window, WindowError> {
     let window_handle = unsafe { GetForegroundWindow() };
 
     if window_handle.0 == 0 {
         return Err(WindowError::NoActiveWindow);
     }
```

### Comparing `pixel_forge-0.1.0/tests/test_capture.py` & `pixel_forge-0.1.1/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `pixel_forge-0.1.0/tests/test_monitor.py` & `pixel_forge-0.1.1/tests/test_monitor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from pixel_forge import Monitor, enumerate_monitors, primary_monitor
 
 
+def test_monitor_init():
+    m = Monitor()  # primary monitor
+    assert isinstance(m, Monitor)
+    m = Monitor(1)  # Also primary monitor, but with explicit id
+    assert isinstance(m, Monitor)
+
+
 def test_primary_monitor():
     monitor = primary_monitor()
     assert isinstance(monitor, Monitor)
     assert monitor.index == 1
 
 
 def test_enumerate_monitors():
```

### Comparing `pixel_forge-0.1.0/Cargo.lock` & `pixel_forge-0.1.1/Cargo.lock`

 * *Files 21% similar despite different names*

```diff
@@ -1,483 +1,483 @@
-# This file is automatically @generated by Cargo.
-# It is not intended for manual editing.
-version = 3
-
-[[package]]
-name = "autocfg"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
-
-[[package]]
-name = "bitflags"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "cfg-if"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
-
-[[package]]
-name = "heck"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
-
-[[package]]
-name = "indoc"
-version = "2.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
-
-[[package]]
-name = "libc"
-version = "0.2.153"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
-
-[[package]]
-name = "lock_api"
-version = "0.4.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
-dependencies = [
- "autocfg",
- "scopeguard",
-]
-
-[[package]]
-name = "matrixmultiply"
-version = "0.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
-dependencies = [
- "autocfg",
- "rawpointer",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "ndarray"
-version = "0.15.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
-dependencies = [
- "matrixmultiply",
- "num-complex",
- "num-integer",
- "num-traits",
- "rawpointer",
-]
-
-[[package]]
-name = "num-complex"
-version = "0.4.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-integer"
-version = "0.1.46"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-traits"
-version = "0.2.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "numpy"
-version = "0.20.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
-dependencies = [
- "libc",
- "ndarray",
- "num-complex",
- "num-integer",
- "num-traits",
- "pyo3",
- "rustc-hash",
-]
-
-[[package]]
-name = "once_cell"
-version = "1.19.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
-
-[[package]]
-name = "parking_lot"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
-dependencies = [
- "lock_api",
- "parking_lot_core",
-]
-
-[[package]]
-name = "parking_lot_core"
-version = "0.9.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
-dependencies = [
- "cfg-if",
- "libc",
- "redox_syscall",
- "smallvec",
- "windows-targets 0.48.5",
-]
-
-[[package]]
-name = "pixel_forge"
-version = "0.1.0"
-dependencies = [
- "numpy",
- "parking_lot",
- "pyo3",
- "thiserror",
- "windows",
- "windows-result",
-]
-
-[[package]]
-name = "portable-atomic"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
-
-[[package]]
-name = "proc-macro2"
-version = "1.0.79"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
-dependencies = [
- "unicode-ident",
-]
-
-[[package]]
-name = "pyo3"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
-dependencies = [
- "cfg-if",
- "indoc",
- "libc",
- "memoffset",
- "parking_lot",
- "portable-atomic",
- "pyo3-build-config",
- "pyo3-ffi",
- "pyo3-macros",
- "unindent",
-]
-
-[[package]]
-name = "pyo3-build-config"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
-dependencies = [
- "once_cell",
- "target-lexicon",
-]
-
-[[package]]
-name = "pyo3-ffi"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
-dependencies = [
- "libc",
- "pyo3-build-config",
-]
-
-[[package]]
-name = "pyo3-macros"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
-dependencies = [
- "proc-macro2",
- "pyo3-macros-backend",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "pyo3-macros-backend"
-version = "0.20.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
-dependencies = [
- "heck",
- "proc-macro2",
- "pyo3-build-config",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "quote"
-version = "1.0.35"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
-dependencies = [
- "proc-macro2",
-]
-
-[[package]]
-name = "rawpointer"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
-
-[[package]]
-name = "redox_syscall"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
-dependencies = [
- "bitflags",
-]
-
-[[package]]
-name = "rustc-hash"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
-
-[[package]]
-name = "scopeguard"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
-
-[[package]]
-name = "smallvec"
-version = "1.13.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
-
-[[package]]
-name = "syn"
-version = "2.0.55"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "target-lexicon"
-version = "0.12.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
-
-[[package]]
-name = "thiserror"
-version = "1.0.58"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
-dependencies = [
- "thiserror-impl",
-]
-
-[[package]]
-name = "thiserror-impl"
-version = "1.0.58"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
-name = "unicode-ident"
-version = "1.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
-
-[[package]]
-name = "unindent"
-version = "0.2.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
-
-[[package]]
-name = "windows"
-version = "0.54.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9252e5725dbed82865af151df558e754e4a3c2c30818359eb17465f1346a1b49"
-dependencies = [
- "windows-core",
- "windows-targets 0.52.5",
-]
-
-[[package]]
-name = "windows-core"
-version = "0.54.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12661b9c89351d684a50a8a643ce5f608e20243b9fb84687800163429f161d65"
-dependencies = [
- "windows-result",
- "windows-targets 0.52.5",
-]
-
-[[package]]
-name = "windows-result"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "749f0da9cc72d82e600d8d2e44cadd0b9eedb9038f71a1c58556ac1c5791813b"
-dependencies = [
- "windows-targets 0.52.5",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
-dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
-dependencies = [
- "windows_aarch64_gnullvm 0.52.5",
- "windows_aarch64_msvc 0.52.5",
- "windows_i686_gnu 0.52.5",
- "windows_i686_gnullvm",
- "windows_i686_msvc 0.52.5",
- "windows_x86_64_gnu 0.52.5",
- "windows_x86_64_gnullvm 0.52.5",
- "windows_x86_64_msvc 0.52.5",
-]
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
-
-[[package]]
-name = "windows_i686_gnullvm"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
-
-[[package]]
-name = "windows_x86_64_msvc"
-version = "0.52.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+# This file is automatically @generated by Cargo.
+# It is not intended for manual editing.
+version = 3
+
+[[package]]
+name = "autocfg"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+
+[[package]]
+name = "bitflags"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+
+[[package]]
+name = "cfg-if"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
+name = "indoc"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
+
+[[package]]
+name = "libc"
+version = "0.2.153"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+
+[[package]]
+name = "lock_api"
+version = "0.4.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+dependencies = [
+ "autocfg",
+ "scopeguard",
+]
+
+[[package]]
+name = "matrixmultiply"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
+dependencies = [
+ "autocfg",
+ "rawpointer",
+]
+
+[[package]]
+name = "memoffset"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "ndarray"
+version = "0.15.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
+dependencies = [
+ "matrixmultiply",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "rawpointer",
+]
+
+[[package]]
+name = "num-complex"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-integer"
+version = "0.1.46"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "num-traits"
+version = "0.2.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+dependencies = [
+ "autocfg",
+]
+
+[[package]]
+name = "numpy"
+version = "0.20.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bef41cbb417ea83b30525259e30ccef6af39b31c240bda578889494c5392d331"
+dependencies = [
+ "libc",
+ "ndarray",
+ "num-complex",
+ "num-integer",
+ "num-traits",
+ "pyo3",
+ "rustc-hash",
+]
+
+[[package]]
+name = "once_cell"
+version = "1.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
+
+[[package]]
+name = "parking_lot"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+dependencies = [
+ "lock_api",
+ "parking_lot_core",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.9.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "redox_syscall",
+ "smallvec",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "pixel_forge"
+version = "0.1.1"
+dependencies = [
+ "numpy",
+ "parking_lot",
+ "pyo3",
+ "thiserror",
+ "windows",
+ "windows-result",
+]
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
+name = "proc-macro2"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+dependencies = [
+ "unicode-ident",
+]
+
+[[package]]
+name = "pyo3"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+dependencies = [
+ "cfg-if",
+ "indoc",
+ "libc",
+ "memoffset",
+ "parking_lot",
+ "portable-atomic",
+ "pyo3-build-config",
+ "pyo3-ffi",
+ "pyo3-macros",
+ "unindent",
+]
+
+[[package]]
+name = "pyo3-build-config"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
+]
+
+[[package]]
+name = "pyo3-macros"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+dependencies = [
+ "proc-macro2",
+ "pyo3-macros-backend",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "pyo3-macros-backend"
+version = "0.20.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "pyo3-build-config",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "quote"
+version = "1.0.35"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+dependencies = [
+ "proc-macro2",
+]
+
+[[package]]
+name = "rawpointer"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
+
+[[package]]
+name = "redox_syscall"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+dependencies = [
+ "bitflags",
+]
+
+[[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
+name = "scopeguard"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
+
+[[package]]
+name = "smallvec"
+version = "1.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
+
+[[package]]
+name = "syn"
+version = "2.0.55"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "002a1b3dbf967edfafc32655d0f377ab0bb7b994aa1d32c8cc7e9b8bf3ebb8f0"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "target-lexicon"
+version = "0.12.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
+
+[[package]]
+name = "thiserror"
+version = "1.0.58"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.58"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "unicode-ident"
+version = "1.0.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
+
+[[package]]
+name = "unindent"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
+
+[[package]]
+name = "windows"
+version = "0.54.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9252e5725dbed82865af151df558e754e4a3c2c30818359eb17465f1346a1b49"
+dependencies = [
+ "windows-core",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-core"
+version = "0.54.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12661b9c89351d684a50a8a643ce5f608e20243b9fb84687800163429f161d65"
+dependencies = [
+ "windows-result",
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-result"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "749f0da9cc72d82e600d8d2e44cadd0b9eedb9038f71a1c58556ac1c5791813b"
+dependencies = [
+ "windows-targets 0.52.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
+]
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `pixel_forge-0.1.0/pyproject.toml` & `pixel_forge-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pixel_forge"
-version = "0.1.0"
+version = "0.1.1"
 description = "Ultra-fast screen capture in Rust with Python bindings"
 readme = "README.md"
 authors = [{ name = "Martin Schuck", email = "real.amacati@gmail.com" }]
 license = { file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.8.0"
 classifiers = [
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: Microsoft :: Windows",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Rust",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
 ]
 keywords = ["screenshot", "window", "capture"]
 dependencies = ["numpy"]
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.urls]
 Repository = "https://github.com/amacati/pixel_forge"
+Documentation = "https://pixel-forge.readthedocs.io/en/latest"
 
 [tool.pyright]
 extension-pkg-allow-list = "pixel_forge"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [tool.ruff]
 line-length = 100
 indent-width = 4
 target-version = "py312"
+exclude = ["docs"]
 
 [tool.ruff.lint]
 select = ["E4", "E7", "E9", "F", "I", "D", "TCH", "ANN"]
 ignore = ["ANN101", "ANN401"]
 fixable = ["ALL"]
-unfixable = []
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.per-file-ignores]
 "tests/test_*.py" = ["D103", "D100"]
```

