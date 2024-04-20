# Comparing `tmp/reflex-chat-0.0.1a6.tar.gz` & `tmp/reflex_chat-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-chat-0.0.1a6.tar", last modified: Sat Apr 13 04:15:02 2024, max compression
+gzip compressed data, was "reflex_chat-0.0.1a7.tar", last modified: Sat Apr 20 21:02:41 2024, max compression
```

## Comparing `reflex-chat-0.0.1a6.tar` & `reflex_chat-0.0.1a7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.771173 reflex-chat-0.0.1a6/
--rw-r--r--   0 nikhil     (501) staff       (20)     2646 2024-04-13 04:15:02.770977 reflex-chat-0.0.1a6/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)     2164 2024-04-13 00:01:45.000000 reflex-chat-0.0.1a6/README.md
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.768806 reflex-chat-0.0.1a6/custom_components/
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.769696 reflex-chat-0.0.1a6/custom_components/reflex_chat/
--rw-r--r--   0 nikhil     (501) staff       (20)       19 2024-04-05 22:25:08.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat/__init__.py
--rw-r--r--   0 nikhil     (501) staff       (20)      929 2024-04-12 23:47:25.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat/api.py
--rw-r--r--   0 nikhil     (501) staff       (20)     5538 2024-04-13 00:14:04.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat/chat.py
-drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-13 04:15:02.770702 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/
--rw-r--r--   0 nikhil     (501) staff       (20)     2646 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/PKG-INFO
--rw-r--r--   0 nikhil     (501) staff       (20)      405 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/SOURCES.txt
--rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/dependency_links.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/requires.txt
--rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-13 04:15:02.000000 reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/top_level.txt
--rw-r--r--   0 nikhil     (501) staff       (20)      646 2024-04-13 04:14:55.000000 reflex-chat-0.0.1a6/pyproject.toml
--rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-13 04:15:02.771209 reflex-chat-0.0.1a6/setup.cfg
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:02:41.659729 reflex_chat-0.0.1a7/
+-rw-r--r--   0 nikhil     (501) staff       (20)     3797 2024-04-20 21:02:41.659515 reflex_chat-0.0.1a7/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)     3315 2024-04-19 00:01:12.000000 reflex_chat-0.0.1a7/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:02:41.656682 reflex_chat-0.0.1a7/custom_components/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:02:41.658107 reflex_chat-0.0.1a7/custom_components/reflex_chat/
+-rw-r--r--   0 nikhil     (501) staff       (20)       20 2024-04-18 23:20:53.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat/__init__.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     1171 2024-04-18 23:58:57.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat/api.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     5077 2024-04-20 20:59:25.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat/chat.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     1809 2024-04-18 23:20:53.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat/components.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2024-04-20 21:02:41.659196 reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)     3797 2024-04-20 21:02:41.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      449 2024-04-20 21:02:41.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2024-04-20 21:02:41.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       33 2024-04-20 21:02:41.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       12 2024-04-20 21:02:41.000000 reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      646 2024-04-20 20:59:53.000000 reflex_chat-0.0.1a7/pyproject.toml
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2024-04-20 21:02:41.659766 reflex_chat-0.0.1a7/setup.cfg
```

### Comparing `reflex-chat-0.0.1a6/PKG-INFO` & `reflex_chat-0.0.1a7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-chat
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: Reflex custom component chat
 Author-email: nikhil@reflex.dev
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/picklelo/reflex-chat
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
@@ -22,14 +22,16 @@
 
 ```bash
 pip install reflex-chat
 ```
 
 ## Usage
 
+See the `chat_demo` folder for an example app.
+
 ```python
 import reflex as rx
 from reflex_chat import chat, api
 
 @rx.page()
 def index() -> rx.Component:
     return rx.container(
@@ -75,18 +77,56 @@
             chat(process=api.openai(model="gpt-3.5-turbo")),
             height="100vh",
         ),
         size="2",
     )
 ```
 
-## API
+## Accessing the Chat State
 
-The chat component contains all the user interface and state needed for a chat interface. You can create multiple chat components on the same page.
+Once you create a chat component, you can access its state through the `chat.State` object.
 
+Get the messages from the chat state.
 
+```python
+chat1 = chat()
 
-- `processing` (bool): Whether the chat is processing a request.
-- `messages` (List[Dict[str, str]]): A list of messages in the chat in the format `{"role": str, "content": str}`.
-- `last_user_message` (str): The last message sent by the user.
-- `append_to_response` (Callable[[str], None]): 
+@rx.page()
+def index() -> rx.Component:
+    return rx.container(
+        # Get the messages through chat1.State.messages.
+        rx.text("Total Messages: ", chat1.State.messages.length()),
+        rx.hstack(
+            chat1,
+            height="100vh",
+        ),
+        # Get the processing state through chat1.State.processing.
+        background_color=rx.cond(chat1.State.processing, "gray", "white"),
+        size="4",
+    )
+```
 
+## Specifying your own process function
+
+You can specify your own `process` function that will be called every time the user submits a question on the chat box. The `process` function should be an async function that takes in the current chat state and yields after appending parts of the streamed response.
+
+The OpenAI `process` function is defined as below:
+
+```python
+async def process(chat: Chat):
+    # Start a new session to answer the question.
+    session = client.chat.completions.create(
+        model=model,
+        # Use chat.get_messages() to get the messages when processing.
+        messages=chat.get_messages(),
+        stream=True,
+    )
+
+    # Stream the results, yielding after every word.
+    for item in session:
+        delta = item.choices[0].delta.content
+        # Append to the last bot message (which defaults as an empty string).
+        chat.append_to_response(delta)
+        yield
+
+return process
+```
```

### Comparing `reflex-chat-0.0.1a6/README.md` & `reflex_chat-0.0.1a7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 ```bash
 pip install reflex-chat
 ```
 
 ## Usage
 
+See the `chat_demo` folder for an example app.
+
 ```python
 import reflex as rx
 from reflex_chat import chat, api
 
 @rx.page()
 def index() -> rx.Component:
     return rx.container(
@@ -59,18 +61,56 @@
             chat(process=api.openai(model="gpt-3.5-turbo")),
             height="100vh",
         ),
         size="2",
     )
 ```
 
-## API
+## Accessing the Chat State
 
-The chat component contains all the user interface and state needed for a chat interface. You can create multiple chat components on the same page.
+Once you create a chat component, you can access its state through the `chat.State` object.
 
+Get the messages from the chat state.
 
+```python
+chat1 = chat()
 
-- `processing` (bool): Whether the chat is processing a request.
-- `messages` (List[Dict[str, str]]): A list of messages in the chat in the format `{"role": str, "content": str}`.
-- `last_user_message` (str): The last message sent by the user.
-- `append_to_response` (Callable[[str], None]): 
+@rx.page()
+def index() -> rx.Component:
+    return rx.container(
+        # Get the messages through chat1.State.messages.
+        rx.text("Total Messages: ", chat1.State.messages.length()),
+        rx.hstack(
+            chat1,
+            height="100vh",
+        ),
+        # Get the processing state through chat1.State.processing.
+        background_color=rx.cond(chat1.State.processing, "gray", "white"),
+        size="4",
+    )
+```
 
+## Specifying your own process function
+
+You can specify your own `process` function that will be called every time the user submits a question on the chat box. The `process` function should be an async function that takes in the current chat state and yields after appending parts of the streamed response.
+
+The OpenAI `process` function is defined as below:
+
+```python
+async def process(chat: Chat):
+    # Start a new session to answer the question.
+    session = client.chat.completions.create(
+        model=model,
+        # Use chat.get_messages() to get the messages when processing.
+        messages=chat.get_messages(),
+        stream=True,
+    )
+
+    # Stream the results, yielding after every word.
+    for item in session:
+        delta = item.choices[0].delta.content
+        # Append to the last bot message (which defaults as an empty string).
+        chat.append_to_response(delta)
+        yield
+
+return process
+```
```

### Comparing `reflex-chat-0.0.1a6/custom_components/reflex_chat/api.py` & `reflex_chat-0.0.1a7/custom_components/reflex_chat/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 """Define common AI API functions."""
 
 import os
 
 try:
     from openai import OpenAI
+
     client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
 except ImportError:
     print("OpenAI is not installed. Please install it with `pip install openai`.")
 
 
+async def default_process(chat):
+    """Process the chat messages.
+
+    Args:
+        chat: The chat object.
+    """
+    chat.append_to_response(
+        "Pass the `process` argument to connect the chat to a model."
+    )
+    yield
+
+
 def openai(
     client=OpenAI(api_key=os.getenv("OPENAI_API_KEY")),
     model=os.getenv("OPENAI_MODEL", "gpt-3.5-turbo"),
 ):
     """Get the response from the API.
 
     Args:
         form_data: A dict with the current question.
     """
+
     async def process(chat):
         # Start a new session to answer the question.
         session = client.chat.completions.create(
             model=model,
-            messages=chat.messages,
+            messages=chat.get_messages(),
             stream=True,
         )
 
         # Stream the results, yielding after every word.
         for item in session:
             delta = item.choices[0].delta.content
             chat.append_to_response(delta)
```

### Comparing `reflex-chat-0.0.1a6/custom_components/reflex_chat/chat.py` & `reflex_chat-0.0.1a7/custom_components/reflex_chat/chat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,82 @@
 """A custom component for a chat interface."""
+from __future__ import annotations
+
+from typing import Callable, Generator, Type
 
 import reflex as rx
+from .api import default_process
+from .components import chat_bubble, action_bar
 
 
 class Chat(rx.ComponentState):
     """A chat component with state."""
 
     # The full chat history, in the OpenAI format.
-    messages2: list[dict[str, str]] = [
-        {
-            "role": "system",
-            "content": "You are a friendly chatbot named Reflex. Respond in markdown.",
-        }
-    ]
+    messages: list[dict[str, str]] = []
 
     # Whether we are processing a message.
     processing: bool = False
 
-    @rx.var
-    def messages(self) -> list[dict[str, str]]:
+    def get_messages(self) -> list[dict[str, str]]:
         """Return the chat history including the last submitted user message.
 
         Returns:
             The chat history as a list of dictionaries.
         """
         # Convert to a list before sending.
-        return self.get_value(self.messages2)
-
-    @classmethod
-    def create(self, process, **props):
-        component = super().create(**props)
-        component.State.process = process
-        return component
+        return self.get_value(self.messages)
 
     @classmethod
     def get_id(cls):
         return f"chatbox-{cls.get_full_name()}"
 
     @classmethod
+    def create(
+        cls,
+        initial_messages: list[dict[str, str]] | None = None,
+        process: Callable[[Chat], Generator] | None = default_process,
+        logo: rx.Component | None = rx.logo(),
+        chat_bubble: Callable[[Type[Chat]], rx.Component] | None = chat_bubble,
+        action_bar: Callable[[Type[Chat]], rx.Component] | None = action_bar,
+        **props,
+    ):
+        """Create a chat component.
+
+        Args:
+            process: The function to process the messages.
+            logo: A component to display in the chat header.
+            chat_bubble: A function to display a chat bubble.
+            action_bar: A function to display the action bar.
+            **props: Additional properties.
+
+        Returns:
+            A chat component.
+        """
+        # Set the initial value of the State var.
+        if initial_messages is not None:
+            # Update the pydantic model to use the initial value as default.
+            cls.__fields__["messages"].default = initial_messages
+        return super().create(
+            process=process,
+            logo=logo,
+            chat_bubble=chat_bubble,
+            action_bar=action_bar,
+            **props,
+        )
+
+    @classmethod
     def get_component(cls, **props) -> rx.Component:
+        cls.process = props.pop("process", default_process)
+        chat_bubble = props.pop("chat_bubble", lambda message, i: rx.fragment())
+        action_bar = props.pop("action_bar", lambda _: rx.fragment())
+
         return rx.vstack(
             rx.box(
-                rx.logo(),
-                justify="left",
+                props.pop("logo", rx.fragment()),
                 background_color=rx.color("accent", 4),
                 width="100%",
             ),
             rx.spacer(),
             rx.vstack(
                 rx.box(
                     rx.foreach(
@@ -63,16 +93,16 @@
                 background_color=props.pop("background_color", rx.color("mauve", 1)),
                 border=props.pop("border", f"1px solid {rx.color('mauve', 4)}"),
                 height="100%",
                 width="100%",
                 **props,
             ),
             spacing="0",
-            height="100%",
-            width="100%",
+            height=props.pop("height", "100%"),
+            width=props.pop("width", "100%"),
             align="start",
         )
 
     def scroll_to_bottom(self):
         return rx.call_script(
             f"""
     var element = document.getElementById({f"chatbox-{self.get_full_name()}"}');
@@ -94,98 +124,37 @@
         message = form_data[self.__class__.__name__]
 
         # Check if the message is empty
         if message == "":
             return
 
         # Add the message to the list of messages.
-        self.messages2.append({"role": "user", "content": message})
-        self.messages2.append({"role": "assistant", "content": ""})
+        self.messages.append({"role": "user", "content": message})
+        self.messages.append({"role": "assistant", "content": ""})
         self.processing = True
         yield self.scroll_to_bottom()
         yield type(self).process_message
 
     @rx.var
     def last_user_message(self) -> str:
         """Return the last submitted user message.
 
         Returns:
             The last submitted user message.
         """
-        for message in reversed(self.messages2):
+        for message in reversed(self.messages):
             if message["role"] == "user":
                 return message["content"]
         return ""
 
     def append_to_response(self, answer: str):
         """Append to the last answer in the chat history.
 
         Args:
             answer: The answer to add to the chat history.
         """
-        self.messages2[-1]["content"] += answer or ""
-
-
-def chat_bubble(message: str, idx: int = 0) -> rx.Component:
-    """Display a single chat bubble.
-
-    Args:
-        message: The message to display.
-
-    Returns:
-        A component displaying the message/answer pair.
-    """
-    return rx.cond(
-        message["role"] == "system",
-        rx.fragment(),
-        rx.box(
-            rx.markdown(
-                message["content"],
-                background_color=rx.cond(
-                    message["role"] == "user",
-                    rx.color("mauve", 4),
-                    rx.color("accent", 4),
-                ),
-                color=rx.cond(
-                    message["role"] == "user",
-                    rx.color("mauve", 12),
-                    rx.color("accent", 12),
-                ),
-                display="inline-block",
-                padding_x="1em",
-                border_radius="8px",
-                max_width=["30em", "30em", "50em", "50em", "50em", "50em"],
-            ),
-            id=f"message-{idx}",
-            text_align=rx.cond(message["role"] == "user", "right", "left"),
-            margin_top="1em",
-            width="100%",
-        ),
-    )
-
-
-def action_bar(State) -> rx.Component:
-    """The action bar to send a new message."""
-    return rx.form(
-        rx.hstack(
-            rx.input.root(
-                rx.input.input(
-                    placeholder="Type something...",
-                    id=State.__name__,
-                ),
-                width="100%",
-            ),
-            rx.spacer(),
-            rx.button(
-                "Send",
-                type="submit",
-            ),
-            align_items="center",
-            width="100%",
-        ),
-        width="100%",
-        on_submit=State.submit_message,
-        reset_on_submit=True,
-    )
+        self.messages[-1]["content"] += answer or ""
 
 
 chat = Chat.create
+
+chat()
```

### Comparing `reflex-chat-0.0.1a6/custom_components/reflex_chat.egg-info/PKG-INFO` & `reflex_chat-0.0.1a7/custom_components/reflex_chat.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex-chat
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: Reflex custom component chat
 Author-email: nikhil@reflex.dev
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/picklelo/reflex-chat
 Keywords: reflex,reflex-custom-components
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.8
@@ -22,14 +22,16 @@
 
 ```bash
 pip install reflex-chat
 ```
 
 ## Usage
 
+See the `chat_demo` folder for an example app.
+
 ```python
 import reflex as rx
 from reflex_chat import chat, api
 
 @rx.page()
 def index() -> rx.Component:
     return rx.container(
@@ -75,18 +77,56 @@
             chat(process=api.openai(model="gpt-3.5-turbo")),
             height="100vh",
         ),
         size="2",
     )
 ```
 
-## API
+## Accessing the Chat State
 
-The chat component contains all the user interface and state needed for a chat interface. You can create multiple chat components on the same page.
+Once you create a chat component, you can access its state through the `chat.State` object.
 
+Get the messages from the chat state.
 
+```python
+chat1 = chat()
 
-- `processing` (bool): Whether the chat is processing a request.
-- `messages` (List[Dict[str, str]]): A list of messages in the chat in the format `{"role": str, "content": str}`.
-- `last_user_message` (str): The last message sent by the user.
-- `append_to_response` (Callable[[str], None]): 
+@rx.page()
+def index() -> rx.Component:
+    return rx.container(
+        # Get the messages through chat1.State.messages.
+        rx.text("Total Messages: ", chat1.State.messages.length()),
+        rx.hstack(
+            chat1,
+            height="100vh",
+        ),
+        # Get the processing state through chat1.State.processing.
+        background_color=rx.cond(chat1.State.processing, "gray", "white"),
+        size="4",
+    )
+```
 
+## Specifying your own process function
+
+You can specify your own `process` function that will be called every time the user submits a question on the chat box. The `process` function should be an async function that takes in the current chat state and yields after appending parts of the streamed response.
+
+The OpenAI `process` function is defined as below:
+
+```python
+async def process(chat: Chat):
+    # Start a new session to answer the question.
+    session = client.chat.completions.create(
+        model=model,
+        # Use chat.get_messages() to get the messages when processing.
+        messages=chat.get_messages(),
+        stream=True,
+    )
+
+    # Stream the results, yielding after every word.
+    for item in session:
+        delta = item.choices[0].delta.content
+        # Append to the last bot message (which defaults as an empty string).
+        chat.append_to_response(delta)
+        yield
+
+return process
+```
```

### Comparing `reflex-chat-0.0.1a6/pyproject.toml` & `reflex_chat-0.0.1a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-chat"
-version = "0.0.1a6"
+version = "0.0.1a7"
 description = "Reflex custom component chat"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "", email = "nikhil@reflex.dev" }]
 keywords = ["reflex","reflex-custom-components"]
```

