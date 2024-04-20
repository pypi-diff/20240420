# Comparing `tmp/esbmc_ai-0.5.0rc3.tar.gz` & `tmp/esbmc_ai-0.5.0rc4.tar.gz`

## Comparing `esbmc_ai-0.5.0rc3.tar` & `esbmc_ai-0.5.0rc4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/config.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/README.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/pyproject.toml
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc3/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/config.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/latest_state_solution_generator.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/reverse_order_solution_generator.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0rc4/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/config.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,27 +40,29 @@
 temp_file_dir: str = "."
 ai_model: AIModel = AIModels.GPT_3.value
 
 esbmc_output_type: str = "full"
 source_code_format: str = "full"
 
 fix_code_max_attempts: int = 5
+fix_code_message_history: str = ""
 
 requests_max_tries: int = 5
 requests_timeout: float = 60
 verifier_timeout: float = 60
 
 loading_hints: bool = False
 allow_successful: bool = False
 # Show the raw conversation after the command ends
 raw_conversation: bool = False
 
 cfg_path: str
 
 
+# TODO Get rid of this class as soon as ConfigTool with the pyautoconfig
 class AIAgentConversation(NamedTuple):
     """Immutable class describing the conversation definition for an AI agent. The
     class represents the system messages of the AI agent defined and contains a load
     class method for efficiently loading it from config."""
 
     messages: tuple[BaseMessage, ...]
 
@@ -380,14 +382,25 @@
     )
 
     if esbmc_output_type not in ["full", "vp", "ce"]:
         raise Exception(
             f"ESBMC output type in the config is not valid: {esbmc_output_type}"
         )
 
+    global fix_code_message_history
+    fix_code_message_history, _ = _load_config_value(
+        config_file=config_file["chat_modes"]["generate_solution"],
+        name="message_history",
+    )
+
+    if fix_code_message_history not in ["normal", "latest_only", "reverse"]:
+        raise ValueError(
+            f"error: fix code mode message history not valid: {fix_code_message_history}"
+        )
+
     global requests_max_tries
     requests_max_tries = int(
         _load_config_real_number(
             config_file=config_file["llm_requests"],
             name="max_tries",
             default=requests_max_tries,
         )
```

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/logging.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/logging.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/solution_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,58 +78,51 @@
         case _:
             raise ValueError(f"Not a valid ESBMC output type: {esbmc_output_type}")
 
 
 class SolutionGenerator(BaseChatInterface):
     def __init__(
         self,
-        ai_model_agent: DynamicAIModelAgent,
+        ai_model_agent: DynamicAIModelAgent | ChatPromptSettings,
         llm: BaseLanguageModel,
-        source_code: str,
-        esbmc_output: str,
         ai_model: AIModel,
         scenario: str = "",
         source_code_format: str = "full",
         esbmc_output_type: str = "full",
     ) -> None:
-        # Convert to chat prompt
-        chat_prompt: ChatPromptSettings = DynamicAIModelAgent.to_chat_prompt_settings(
-            ai_model_agent=ai_model_agent, scenario=scenario
-        )
+        """Initializes the solution generator. This ModelChat provides Dynamic
+        Prompting. Will get the correct scenario from the DynamicAIModelAgent
+        supplied and create a ChatPrompt."""
+
+        chat_prompt: ChatPromptSettings = ai_model_agent
+        if isinstance(ai_model_agent, DynamicAIModelAgent):
+            # Convert to chat prompt
+            chat_prompt = DynamicAIModelAgent.to_chat_prompt_settings(
+                ai_model_agent=ai_model_agent, scenario=scenario
+            )
 
         super().__init__(
             ai_model_agent=chat_prompt,
             ai_model=ai_model,
             llm=llm,
         )
 
-        self.initial_prompt = ai_model_agent.initial_prompt
-
         self.esbmc_output_type: str = esbmc_output_type
         self.source_code_format: str = source_code_format
-        self.source_code_raw: str = source_code
-        # Used for resetting state.
-        self._original_source_code: str = source_code
 
-        # Format ESBMC output
-        try:
-            self.esbmc_output = get_esbmc_output_formatted(
-                esbmc_output_type=self.esbmc_output_type,
-                esbmc_output=esbmc_output,
-            )
-        except SourceCodeParseError:
-            # When clang output is displayed, show it entirely as it doesn't get very
-            # big.
-            self.esbmc_output = esbmc_output
+        self.source_code_raw: Optional[str] = None
+        self.source_code_formatted: Optional[str] = None
+        self.esbmc_output: Optional[str] = None
 
     @override
     def compress_message_stack(self) -> None:
         # Resets the conversation - cannot summarize code
+        # If generate_solution is called after this point, it will start new
+        # with the currently set state.
         self.messages: list[BaseMessage] = []
-        self.source_code_raw = self._original_source_code
 
     @classmethod
     def get_code_from_solution(cls, solution: str) -> str:
         """Strip the source code of any leftover text as sometimes the AI model
         will generate text and formatting despite being told not to."""
         try:
             code_start: int = solution.index("```") + 3
@@ -149,35 +142,51 @@
             assert code_start <= code_end + 1
 
             solution = solution[code_start:code_end]
         except (ValueError, AssertionError):
             pass
         return solution
 
-    def update_state(
-        self, source_code: Optional[str] = None, esbmc_output: Optional[str] = None
-    ) -> None:
-        if source_code:
-            self.source_code_raw = source_code
-        if esbmc_output:
-            self.esbmc_output = esbmc_output
+    def update_state(self, source_code: str, esbmc_output: str) -> None:
+        """Updates the latest state of the code and ESBMC output. This should be
+        called before generate_solution."""
+        self.source_code_raw = source_code
 
-    def generate_solution(self) -> tuple[str, FinishReason]:
-        self.push_to_message_stack(HumanMessage(content=self.initial_prompt))
+        # Format ESBMC output
+        try:
+            self.esbmc_output = get_esbmc_output_formatted(
+                esbmc_output_type=self.esbmc_output_type,
+                esbmc_output=esbmc_output,
+            )
+        except SourceCodeParseError:
+            # When clang output is displayed, show it entirely as it doesn't get very
+            # big.
+            self.esbmc_output = esbmc_output
 
         # Format source code
-        source_code_formatted: str = get_source_code_formatted(
+        self.source_code_formatted = get_source_code_formatted(
             source_code_format=self.source_code_format,
-            source_code=self.source_code_raw,
+            source_code=source_code,
             esbmc_output=self.esbmc_output,
         )
 
+    def generate_solution(self) -> tuple[str, FinishReason]:
+        assert (
+            self.source_code_raw is not None
+            and self.source_code_formatted is not None
+            and self.esbmc_output is not None
+        ), "Call update_state before calling generate_solution."
+
+        self.push_to_message_stack(
+            HumanMessage(content=self.ai_model_agent.initial_prompt)
+        )
+
         # Apply template substitution to message stack
         self.apply_template_value(
-            source_code=source_code_formatted,
+            source_code=self.source_code_formatted,
             esbmc_output=self.esbmc_output,
         )
 
         # Generate the solution
         response: ChatResponse = self.send_message()
         solution: str = str(response.message.content)
```

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/commands/fix_code_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # Author: Yiannis Charalambous
 
 import sys
 from typing import Any, Tuple
 from typing_extensions import override
-from langchain.schema import AIMessage, HumanMessage
 
 from esbmc_ai.chat_response import FinishReason
+from esbmc_ai.latest_state_solution_generator import LatestStateSolutionGenerator
+from esbmc_ai.reverse_order_solution_generator import ReverseOrderSolutionGenerator
 
 from .chat_command import ChatCommand
 from .. import config
 from ..msg_bus import Signal
 from ..loading_widget import create_loading_widget
 from ..esbmc_util import (
     esbmc_get_error_type,
     esbmc_load_source_code,
 )
 from ..solution_generator import (
     ESBMCTimedOutException,
     SolutionGenerator,
-    SourceCodeParseError,
-    get_esbmc_output_formatted,
 )
 from ..logging import print_horizontal_line, printv, printvv
 
 # TODO Remove built in messages and move them to config.
 
 
 class FixCodeCommand(ChatCommand):
@@ -57,33 +56,68 @@
         printv(f"Scenario: {scenario}")
         printv(
             f"Using dynamic prompt..."
             if scenario in config.chat_prompt_generator_mode.scenarios
             else "Using generic prompt..."
         )
 
+        match config.fix_code_message_history:
+            case "normal":
+                solution_generator = SolutionGenerator(
+                    ai_model_agent=config.chat_prompt_generator_mode,
+                    ai_model=config.ai_model,
+                    llm=config.ai_model.create_llm(
+                        api_keys=config.api_keys,
+                        temperature=config.chat_prompt_generator_mode.temperature,
+                        requests_max_tries=config.requests_max_tries,
+                        requests_timeout=config.requests_timeout,
+                    ),
+                    scenario=scenario,
+                    source_code_format=config.source_code_format,
+                    esbmc_output_type=config.esbmc_output_type,
+                )
+            case "latest_only":
+                solution_generator = LatestStateSolutionGenerator(
+                    ai_model_agent=config.chat_prompt_generator_mode,
+                    ai_model=config.ai_model,
+                    llm=config.ai_model.create_llm(
+                        api_keys=config.api_keys,
+                        temperature=config.chat_prompt_generator_mode.temperature,
+                        requests_max_tries=config.requests_max_tries,
+                        requests_timeout=config.requests_timeout,
+                    ),
+                    scenario=scenario,
+                    source_code_format=config.source_code_format,
+                    esbmc_output_type=config.esbmc_output_type,
+                )
+            case "reverse":
+                solution_generator = ReverseOrderSolutionGenerator(
+                    ai_model_agent=config.chat_prompt_generator_mode,
+                    ai_model=config.ai_model,
+                    llm=config.ai_model.create_llm(
+                        api_keys=config.api_keys,
+                        temperature=config.chat_prompt_generator_mode.temperature,
+                        requests_max_tries=config.requests_max_tries,
+                        requests_timeout=config.requests_timeout,
+                    ),
+                    scenario=scenario,
+                    source_code_format=config.source_code_format,
+                    esbmc_output_type=config.esbmc_output_type,
+                )
+            case _:
+                raise NotImplementedError(
+                    f"error: {config.fix_code_message_history} has not been implemented in the Fix Code Command"
+                )
+
         try:
-            solution_generator = SolutionGenerator(
-                ai_model_agent=config.chat_prompt_generator_mode,
+            solution_generator.update_state(
                 source_code=source_code,
                 esbmc_output=esbmc_output,
-                ai_model=config.ai_model,
-                llm=config.ai_model.create_llm(
-                    api_keys=config.api_keys,
-                    temperature=config.chat_prompt_generator_mode.temperature,
-                    requests_max_tries=config.requests_max_tries,
-                    requests_timeout=config.requests_timeout,
-                ),
-                scenario=scenario,
-                source_code_format=config.source_code_format,
-                esbmc_output_type=config.esbmc_output_type,
             )
         except ESBMCTimedOutException:
-            if config.raw_conversation:
-                print_raw_conversation()
             print("error: ESBMC has timed out...")
             sys.exit(1)
 
         print()
 
         max_retries: int = config.fix_code_max_attempts
         for idx in range(max_retries):
@@ -91,17 +125,15 @@
             # gets full, then need to compress and retry.
             while True:
                 # Generate AI solution
                 self.anim.start("Generating Solution... Please Wait")
                 llm_solution, finish_reason = solution_generator.generate_solution()
                 self.anim.stop()
                 if finish_reason == FinishReason.length:
-                    self.anim.start("Compressing message stack... Please Wait")
                     solution_generator.compress_message_stack()
-                    self.anim.stop()
                 else:
                     source_code = llm_solution
                     break
 
             # Print verbose lvl 2
             printvv("\nGeneration:")
             print_horizontal_line(2)
@@ -133,33 +165,21 @@
                 if config.raw_conversation:
                     print_raw_conversation()
 
                 printv("ESBMC-AI Notice: Successfully verified code")
 
                 return False, source_code
 
-            # TODO Move this process into Solution Generator since have (beginning) is done
-            # inside, and the other half is done here.
-            # Get formatted ESBMC output
             try:
-                esbmc_output = get_esbmc_output_formatted(
-                    esbmc_output_type=config.esbmc_output_type,
-                    esbmc_output=esbmc_output,
-                )
-            except SourceCodeParseError:
-                pass
+                # Update state
+                solution_generator.update_state(source_code, esbmc_output)
             except ESBMCTimedOutException:
-                if config.raw_conversation:
-                    print_raw_conversation()
                 print("error: ESBMC has timed out...")
                 sys.exit(1)
 
             # Failure case
             print(f"ESBMC-AI Notice: Failure {idx+1}/{max_retries}: Retrying...")
 
-            # Update state
-            solution_generator.update_state(source_code, esbmc_output)
-
         if config.raw_conversation:
             print_raw_conversation()
 
         return True, "ESBMC-AI Notice: Failed all attempts..."
```

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0rc4/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/.gitignore` & `esbmc_ai-0.5.0rc4/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/LICENSE` & `esbmc_ai-0.5.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/README.md` & `esbmc_ai-0.5.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/pyproject.toml` & `esbmc_ai-0.5.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0rc3/PKG-INFO` & `esbmc_ai-0.5.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0rc3
+Version: 0.5.0rc4
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

