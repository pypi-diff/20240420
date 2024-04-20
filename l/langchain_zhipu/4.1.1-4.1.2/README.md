# Comparing `tmp/langchain_zhipu-4.1.1.tar.gz` & `tmp/langchain_zhipu-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_zhipu-4.1.1.tar", max compression
+gzip compressed data, was "langchain_zhipu-4.1.2.tar", max compression
```

## Comparing `langchain_zhipu-4.1.1.tar` & `langchain_zhipu-4.1.2.tar`

### file list

```diff
@@ -1,53 +1,15 @@
--rw-r--r--   0        0        0     3069 2024-03-27 14:16:13.949508 langchain_zhipu-4.1.1/README.md
--rw-r--r--   0        0        0     1443 2024-04-13 03:09:45.316481 langchain_zhipu-4.1.1/langchain_zhipu/__init__.py
--rw-r--r--   0        0        0       23 2024-04-13 03:09:56.467160 langchain_zhipu-4.1.1/langchain_zhipu/__version__.py
--rw-r--r--   0        0        0     2579 2024-03-28 15:59:03.809176 langchain_zhipu-4.1.1/langchain_zhipu/_client.py
--rw-r--r--   0        0        0      147 2024-04-12 15:34:05.266385 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:05.266769 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/chat/__init__.py
--rw-r--r--   0        0        0     3118 2024-04-12 15:34:05.267060 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/chat/async_completions.py
--rw-r--r--   0        0        0      451 2024-04-12 15:34:05.267290 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/chat/chat.py
--rw-r--r--   0        0        0     2790 2024-04-12 15:34:05.267521 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/chat/completions.py
--rw-r--r--   0        0        0     1633 2024-04-12 15:34:05.267759 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/embeddings.py
--rw-r--r--   0        0        0     2323 2024-04-12 15:34:05.267978 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/files.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:05.268207 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/fine_tuning/__init__.py
--rw-r--r--   0        0        0      311 2024-04-12 15:34:05.268459 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0     3470 2024-04-12 15:34:05.269395 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1818 2024-04-12 15:34:05.269837 langchain_zhipu-4.1.1/langchain_zhipu/api_resource/images.py
--rw-r--r--   0        0        0    15864 2024-04-07 11:17:39.809084 langchain_zhipu-4.1.1/langchain_zhipu/chat.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:05.270126 langchain_zhipu-4.1.1/langchain_zhipu/core/__init__.py
--rw-r--r--   0        0        0      406 2024-04-12 15:34:05.270458 langchain_zhipu-4.1.1/langchain_zhipu/core/_base_api.py
--rw-r--r--   0        0        0     3392 2024-04-12 15:34:05.272267 langchain_zhipu-4.1.1/langchain_zhipu/core/_base_type.py
--rw-r--r--   0        0        0     2038 2024-04-12 15:34:05.272714 langchain_zhipu-4.1.1/langchain_zhipu/core/_errors.py
--rw-r--r--   0        0        0     1384 2024-04-12 15:34:05.275395 langchain_zhipu-4.1.1/langchain_zhipu/core/_files.py
--rw-r--r--   0        0        0    12233 2024-04-12 15:34:05.278500 langchain_zhipu-4.1.1/langchain_zhipu/core/_http_client.py
--rw-r--r--   0        0        0      713 2024-04-12 15:34:05.278835 langchain_zhipu-4.1.1/langchain_zhipu/core/_jwt_token.py
--rw-r--r--   0        0        0     1694 2024-04-12 15:34:05.280017 langchain_zhipu-4.1.1/langchain_zhipu/core/_request_opt.py
--rw-r--r--   0        0        0     3394 2024-04-12 15:34:05.281411 langchain_zhipu-4.1.1/langchain_zhipu/core/_response.py
--rw-r--r--   0        0        0     4085 2024-04-12 15:34:05.282603 langchain_zhipu-4.1.1/langchain_zhipu/core/_sse_client.py
--rw-r--r--   0        0        0      443 2024-04-12 15:34:05.283079 langchain_zhipu-4.1.1/langchain_zhipu/core/_utils.py
--rw-r--r--   0        0        0     1499 2024-04-12 15:33:28.452985 langchain_zhipu-4.1.1/langchain_zhipu/embeddings.py
--rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.1/langchain_zhipu/http/__init__.py
--rw-r--r--   0        0        0     4720 2024-04-13 03:38:13.595777 langchain_zhipu-4.1.1/langchain_zhipu/http/api.py
--rw-r--r--   0        0        0    13988 2024-04-13 03:38:47.857352 langchain_zhipu-4.1.1/langchain_zhipu/http/base.py
--rw-r--r--   0        0        0     7873 2024-04-13 03:29:56.275613 langchain_zhipu-4.1.1/langchain_zhipu/http/chat.py
--rw-r--r--   0        0        0     1714 2024-04-13 03:17:37.336032 langchain_zhipu-4.1.1/langchain_zhipu/http/embeddings.py
--rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.1/langchain_zhipu/http/enum.py
--rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.1/langchain_zhipu/http/env.py
--rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.1/langchain_zhipu/http/manager.py
--rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.1/langchain_zhipu/http/types.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:05.283423 langchain_zhipu-4.1.1/langchain_zhipu/types/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 15:34:05.283788 langchain_zhipu-4.1.1/langchain_zhipu/types/chat/__init__.py
--rw-r--r--   0        0        0      568 2024-04-12 15:34:05.285073 langchain_zhipu-4.1.1/langchain_zhipu/types/chat/async_chat_completion.py
--rw-r--r--   0        0        0      879 2024-04-12 15:34:05.286840 langchain_zhipu-4.1.1/langchain_zhipu/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1226 2024-04-12 15:34:05.288657 langchain_zhipu-4.1.1/langchain_zhipu/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      171 2024-04-12 15:34:05.288987 langchain_zhipu-4.1.1/langchain_zhipu/types/chat/chat_completions_create_param.py
--rw-r--r--   0        0        0      446 2024-04-12 15:34:05.290012 langchain_zhipu-4.1.1/langchain_zhipu/types/embeddings.py
--rw-r--r--   0        0        0      550 2024-04-12 15:34:05.291312 langchain_zhipu-4.1.1/langchain_zhipu/types/file_object.py
--rw-r--r--   0        0        0      244 2024-04-12 15:34:05.291828 langchain_zhipu-4.1.1/langchain_zhipu/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1051 2024-04-12 15:34:05.292643 langchain_zhipu-4.1.1/langchain_zhipu/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0     1121 2024-04-12 15:34:05.293310 langchain_zhipu-4.1.1/langchain_zhipu/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0      339 2024-04-12 15:34:05.293603 langchain_zhipu-4.1.1/langchain_zhipu/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      394 2024-04-12 15:34:05.294518 langchain_zhipu-4.1.1/langchain_zhipu/types/image.py
--rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.1/langchain_zhipu/utils.py
--rw-r--r--   0        0        0      750 2024-04-13 03:10:06.016161 langchain_zhipu-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     3914 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4221 2024-04-19 01:27:50.154822 langchain_zhipu-4.1.2/README.md
+-rw-r--r--   0        0        0      971 2024-04-20 11:17:13.232062 langchain_zhipu-4.1.2/langchain_zhipu/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-20 11:12:51.678450 langchain_zhipu-4.1.2/langchain_zhipu/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:37:31.905694 langchain_zhipu-4.1.2/langchain_zhipu/http/__init__.py
+-rw-r--r--   0        0        0     4844 2024-04-20 11:05:25.768200 langchain_zhipu-4.1.2/langchain_zhipu/http/api.py
+-rw-r--r--   0        0        0    13779 2024-04-13 06:21:01.194348 langchain_zhipu-4.1.2/langchain_zhipu/http/base.py
+-rw-r--r--   0        0        0     7825 2024-04-13 06:21:17.673386 langchain_zhipu-4.1.2/langchain_zhipu/http/chat.py
+-rw-r--r--   0        0        0     1714 2024-04-13 03:17:37.336032 langchain_zhipu-4.1.2/langchain_zhipu/http/embeddings.py
+-rw-r--r--   0        0        0      500 2024-04-02 14:02:48.067993 langchain_zhipu-4.1.2/langchain_zhipu/http/enum.py
+-rw-r--r--   0        0        0      382 2024-04-09 02:22:51.583321 langchain_zhipu-4.1.2/langchain_zhipu/http/env.py
+-rw-r--r--   0        0        0     8994 2024-04-09 02:58:49.863351 langchain_zhipu-4.1.2/langchain_zhipu/http/manager.py
+-rw-r--r--   0        0        0     4099 2024-04-06 13:39:34.256771 langchain_zhipu-4.1.2/langchain_zhipu/http/types.py
+-rw-r--r--   0        0        0     1721 2024-03-26 15:19:10.785090 langchain_zhipu-4.1.2/langchain_zhipu/utils.py
+-rw-r--r--   0        0        0      750 2024-04-20 11:12:58.052250 langchain_zhipu-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5066 1970-01-01 00:00:00.000000 langchain_zhipu-4.1.2/PKG-INFO
```

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/chat.py` & `langchain_zhipu-4.1.2/langchain_zhipu/http/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,41 @@
+from langchain_core.language_models.base import LanguageModelInput
+from langchain_core.runnables import RunnableConfig
+from langchain_core.runnables.config import ensure_config, run_in_executor
+from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult, LLMResult
+from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
+from langchain_core.load import dumpd, dumps
+
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
+    CallbackManager,
     CallbackManagerForLLMRun,
 )
 
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
     generate_from_stream,
 )
 
-from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
-from langchain_core.pydantic_v1 import BaseModel, Field, root_validator
+from langchain_community.adapters.openai import (
+    convert_message_to_dict,
+    convert_dict_to_message,    
+)
 
 # common types
 from typing import (
     Type, Any, Mapping, Dict, Iterator, List, Optional, cast,
     AsyncIterator, Union, Literal, AbstractSet, Collection
 )
 
-# async
-import asyncio
+from abc import ABC, abstractmethod
 
+import asyncio
 import tiktoken
+import inspect
 
 # all message types
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     BaseMessageChunk,
@@ -36,107 +47,24 @@
     FunctionMessageChunk,
     SystemMessage,
     SystemMessageChunk,
     ChatMessage,
     ChatMessageChunk,
 )
 
-from ._client import ZhipuAI
-
-def _convert_dict_to_message(_dict: Mapping[str, Any]) -> BaseMessage:
-    """Convert a dictionary to a LangChain message.
-
-    Args:
-        _dict: The dictionary.
-
-    Returns:
-        The LangChain message.
-    """
-    role = _dict.get("role")
-    id_ = _dict.get("id")
-    if role == "user":
-        return HumanMessage(content=_dict.get("content", ""), id=id_)
-    elif role == "assistant":
-        # Fix for azure
-        # Also OpenAI returns None for tool invocations
-        content = _dict.get("content", "") or ""
-        additional_kwargs: Dict = {}
-        if function_call := _dict.get("function_call"):
-            additional_kwargs["function_call"] = dict(function_call)
-        if tool_calls := _dict.get("tool_calls"):
-            additional_kwargs["tool_calls"] = tool_calls
-        return AIMessage(content=content, additional_kwargs=additional_kwargs, id=id_)
-    elif role == "system":
-        return SystemMessage(content=_dict.get("content", ""), id=id_)
-    elif role == "function":
-        return FunctionMessage(
-            content=_dict.get("content", ""), name=_dict.get("name"), id=id_
-        )
-    elif role == "tool":
-        additional_kwargs = {}
-        if "name" in _dict:
-            additional_kwargs["name"] = _dict["name"]
-        return ToolMessage(
-            content=_dict.get("content", ""),
-            tool_call_id=_dict.get("tool_call_id"),
-            additional_kwargs=additional_kwargs,
-            id=id_,
-        )
-    else:
-        return ChatMessage(content=_dict.get("content", ""), role=role, id=id_)
-
+from .api import RestAPI
 
-def _convert_message_to_dict(message: BaseMessage) -> dict:
-    """Convert a LangChain message to a dictionary.
+def get_all_attributes(obj):
+    attrs = {}
+    for cls in inspect.getmro(obj.__class__):
+        attrs.update(vars(cls))
+    attrs.update(vars(obj))  # 实例属性覆盖类属性
+    return attrs
 
-    Args:
-        message: The LangChain message.
-
-    Returns:
-        The dictionary.
-    """
-    message_dict: Dict[str, Any]
-    if isinstance(message, ChatMessage):
-        message_dict = {"role": message.role, "content": message.content}
-    elif isinstance(message, HumanMessage):
-        message_dict = {"role": "user", "content": message.content}
-    elif isinstance(message, AIMessage):
-        message_dict = {"role": "assistant", "content": message.content}
-        if "function_call" in message.additional_kwargs:
-            message_dict["function_call"] = message.additional_kwargs["function_call"]
-            # If function call only, content is None not empty string
-            if message_dict["content"] == "":
-                message_dict["content"] = None
-        if "tool_calls" in message.additional_kwargs:
-            message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
-            # If tool calls only, content is None not empty string
-            if message_dict["content"] == "":
-                message_dict["content"] = None
-    elif isinstance(message, SystemMessage):
-        message_dict = {"role": "system", "content": message.content}
-    elif isinstance(message, FunctionMessage):
-        message_dict = {
-            "role": "function",
-            "content": message.content,
-            "name": message.name,
-        }
-    elif isinstance(message, ToolMessage):
-        message_dict = {
-            "role": "tool",
-            "content": message.content,
-            "tool_call_id": message.tool_call_id,
-        }
-    else:
-        raise TypeError(f"Got unknown type {message}")
-    if "name" in message.additional_kwargs:
-        message_dict["name"] = message.additional_kwargs["name"]
-    return message_dict
-
-
-def _convert_delta_to_message_chunk(
+def convert_delta_to_message_chunk(
     _dict: Mapping[str, Any], default_class: Type[BaseMessageChunk]
 ) -> BaseMessageChunk:
     id_ = _dict.get("id")
     role = cast(str, _dict.get("role"))
     content = cast(str, _dict.get("content") or "")
     additional_kwargs: Dict = {}
     if _dict.get("function_call"):
@@ -162,18 +90,23 @@
             content=content, tool_call_id=_dict["tool_call_id"], id=id_
         )
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role, id=id_)
     else:
         return default_class(content=content, id=id_)  # type: ignore
 
+def _gen_info_and_msg_metadata(
+    generation: Union[ChatGeneration, ChatGenerationChunk],
+) -> dict:
+    return {
+        **(generation.generation_info or {}),
+        **getattr(generation.message, 'response_metadata', {}),
+    }
 
-class ChatZhipuAI(BaseChatModel):
-    """支持最新的智谱API"""
-
+class BaseChatZhipuAI(BaseChatModel, ABC):
     @property
     def lc_secrets(self) -> Dict[str, str]:
         return {"zhipuai_api_key": "ZHIPUAI_API_KEY"}
 
     @property
     def _llm_type(self) -> str:
         """Return the type of chat model."""
@@ -197,160 +130,105 @@
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "chat_models", "ZhipuAI"]
     
     client: Any = None
     """访问智谱AI的客户端"""
-    
-    api_key: str = None
 
     model: str = Field(default="glm-4")
     """所要调用的模型编码"""
 
-    request_id: Optional[str] = None
-    """
-    由用户端传参，需保证唯一性；用于区分每次请求的唯一标识，用户端不传时平台会默认生成。
-    """
-    
-    do_sample: Optional[bool] = None
-    """
-    do_sample 为 true 时启用采样策略;
-    do_sample 为 false 时采样策略 temperature、top_p 将不生效
-    """
-
-    temperature: Optional[float] = None
-    """
-    采样温度，控制输出的随机性，必须为正数；
-    取值范围是：
-      - (0.0,1.0]，不能等于 0，默认值为 0.95,值越大，会使输出更随机，更具创造性；
-      - 值越小，输出会更加稳定或确定；
-
-    建议您根据应用场景调整 top_p 或 temperature 参数，但不要同时调整两个参数。
-    """
-
-    top_p: Optional[float] = None
-    """
-    用温度取样的另一种方法，称为核取样：
-    取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1，默认值为 0.7。
-    模型考虑具有 top_p 概率质量tokens的结果。
-
-    例如：0.1 意味着模型解码器只考虑从前 10% 的概率的候选集中取tokens
-    建议您根据应用场景调整 top_p 或 temperature 参数，但不要同时调整两个参数。
-    """
-
-    max_tokens: Optional[int] = None
-    """模型输出最大tokens"""
-
-    stop: Optional[List[str]] = None
-    """
-    模型在遇到stop所制定的字符时将停止生成，目前仅支持单个停止词，格式为["stop_word1"]    
-    """
-
-    tools: List[Any] = None
-    """
-    可供模型调用的工具列表,tools字段会计算 tokens ，同样受到tokens长度的限制。
-    """
-
-    tool_choice: Optional[str] = "auto"
-    """
-    用于控制模型是如何选择要调用的函数，仅当工具类型为function时补充。默认为auto，当前仅支持auto。
-    """
-    
-    streaming: Optional[bool] = False
-    """
-    流式输出。
-    """
+    base_url: str = None
+    """访问智谱AI的服务器地址"""
 
+    api_key: str = None
+    """访问智谱AI的ZHIPU_API_KEY"""
+    
     allowed_special: Union[Literal["all"], AbstractSet[str]] = set()
     """Set of special tokens that are allowed。"""
 
     disallowed_special: Union[Literal["all"], Collection[str]] = "all"
     """Set of special tokens that are not allowed。"""
+
+    @root_validator()
+    def base_validate_environment(cls, values: Dict) -> Dict:
+        values["client"] =  RestAPI(base_url=values["base_url"], api_key=values["api_key"])
+        return values
     
     @classmethod
     def filter_model_kwargs(cls):
-        """
-        ZhipuAI在调用时只接受这些参数。
-        """
-        return [
-            "model",
-            "request_id",
-            "do_sample",
-            "temperature",
-            "top_p",
-            "max_tokens",
-            "stop",
-            "tools",
-            "tool_choice",
-        ]
-        
+        """过滤可以在调用时使用的参数"""
+        return {}
+
+    @abstractmethod
+    def _ask_remote(self, prompt: Any, stop: Optional[List[str]] = None, **kwargs):
+        """同步调用"""
+
+    @abstractmethod
+    def _ask_remote_sse(self, prompt: Any, stop: Optional[List[str]] = None, **kwargs):
+        """同步的SSE调用"""
+
+    async def _ask_aremote_sse(self, prompt: Any, stop: Optional[List[str]] = None, **kwargs):
+        """异步的SSE调用"""
+        def _func():
+            return list(self._ask_remote_sse(prompt, stop, **kwargs))
+
+        loop = asyncio.get_running_loop()
+        results = await loop.run_in_executor(None, _func)
+        for obj in results:
+            yield obj
+
     # 获得模型调用参数
     def get_model_kwargs(self):
         params = {}
-        for attr, value in self.__dict__.items():
+        attrs = get_all_attributes(self)
+        for attr, value in attrs.items():
             if attr in self.__class__.filter_model_kwargs() and value is not None:
                 params[attr] = value
         return params
 
-    @root_validator()
-    def validate_environment(cls, values: Dict) -> Dict:
-        if values["api_key"] is not None:
-            values["client"] =  ZhipuAI(api_key=values["api_key"])
-        else:
-            values["client"] =  ZhipuAI()
-        return values
-
     # 实现 invoke 调用方法
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         stream: Optional[bool] = None,
         **kwargs: Any,
     ) -> ChatResult:
         """实现 ZhiputAI 的同步调用"""
-        prompt = [_convert_message_to_dict(message) for message in messages]
 
-        # 构造参数序列
-        params = self.get_model_kwargs()
-        params.update(kwargs)
-        params.update({"stream": False})
-        if stop is not None:
-            params.update({"stop": stop})
-    
         # 支持根据 stream 或 streaming 生成流
         should_stream = stream if stream is not None else self.streaming
         if should_stream:
             stream_iter = self._stream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             return generate_from_stream(stream_iter)
-    
-        # 调用模型
-        response = self.client.chat.completions.create(
-            messages=prompt,
-            **params
-        )
+
+        prompt = [convert_message_to_dict(message) for message in messages]
+        response = self._ask_remote(prompt, stop, **kwargs)
 
         generations = []
+        id = response.get("id")
         if not isinstance(response, dict):
             response = response.dict()
         for res in response["choices"]:
-            message = _convert_dict_to_message(res["message"])
+            message_dict = res["message"]
+            message = convert_dict_to_message(message_dict)
             generation_info = dict(finish_reason=res.get("finish_reason"))
             gen = ChatGeneration(
                 message=message,
                 generation_info=generation_info,
             )
             generations.append(gen)
         token_usage = response.get("usage", {})
         llm_output = {
-            "id": response.get("id"),
+            "id": id,
             "created": response.get("created"),
             "token_usage": token_usage,
             "model_name": self.model,
         }
         return ChatResult(generations=generations, llm_output=llm_output)
 
     # 实现 stream 调用方法
@@ -358,102 +236,151 @@
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         """实现 ZhiputAI 的事件流调用"""
-        prompt = [_convert_message_to_dict(message) for message in messages]
-
-        # 使用流输出
-        # 构造参数序列
-        params = self.get_model_kwargs()
-        params.update(kwargs)
-        params.update({"stream": True})
-        if stop is not None:
-            params.update({"stop": stop})
-    
-        responses = self.client.chat.completions.create(
-            messages=prompt,
-            **params
-        )
+        prompt = [convert_message_to_dict(message) for message in messages]
 
         default_chunk_class = AIMessageChunk
-        for response in responses:                
+        for response in self._ask_remote_sse(prompt, stop, **kwargs): 
             if not isinstance(response, dict):
                 response = response.dict()
-            if len(response["choices"]) == 0:
+            if "choices" not in response or len(response["choices"]) == 0:
                 continue
             choice = response["choices"][0]
-            chunk = _convert_delta_to_message_chunk(
-                choice["delta"], default_chunk_class
+            delta = choice["delta"]
+            delta.update({"id": response["id"]})
+            message_chunk = convert_delta_to_message_chunk(
+                delta, default_chunk_class
             )
+            
             generation_info = {}
             if finish_reason := choice.get("finish_reason"):
                 generation_info["finish_reason"] = finish_reason
-            default_chunk_class = chunk.__class__
+                generation_info["model"] = response["model"]
+                generation_info["created"] = response["created"]
+                generation_info["index"] = choice["index"]
+            if usage := response.get("usage"):
+                generation_info["usage"] = usage
+            default_chunk_class = message_chunk.__class__
             chunk = ChatGenerationChunk(
-                message=chunk, generation_info=generation_info or None
+                message=message_chunk,
+                generation_info=generation_info,
             )
-            if run_manager:
+            if run_manager is not None:
                 run_manager.on_llm_new_token(chunk.text, chunk=chunk)
             yield chunk
-
+            
     async def _astream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
         """实现 ZhiputAI 的事件流调用"""
-        prompt = [_convert_message_to_dict(message) for message in messages]
-
-        # 使用流输出
-        # 构造参数序列
-        params = self.get_model_kwargs()
-        params.update(kwargs)
-        params.update({"stream": True})
-        if stop is not None:
-            params.update({"stop": stop})
-
-        # 创建一个新的函数来调用 self.client.chat.completions.create
-        def create_completions():
-            return self.client.chat.completions.create(
-                messages=prompt,
-                **params
-            )
-
-        # 由于ZhipuAI没有基于流的异步返回，因此使用asyncio构建
-        loop = asyncio.get_running_loop()
-        responses = await loop.run_in_executor(None, create_completions)
+        prompt = [convert_message_to_dict(message) for message in messages]
 
         default_chunk_class = AIMessageChunk
-        for response in responses:
+        async for response in self._ask_aremote_sse(prompt, stop, **kwargs):
             if not isinstance(response, dict):
                 response = response.dict()
-            if len(response["choices"]) == 0:
+            if "choices" not in response or len(response["choices"]) == 0:
                 continue
             choice = response["choices"][0]
-            chunk = _convert_delta_to_message_chunk(
-                choice["delta"], default_chunk_class
+            delta = choice["delta"]
+            delta.update({"id": response["id"]})
+            message_chunk = convert_delta_to_message_chunk(
+                delta, default_chunk_class
             )
+            
             generation_info = {}
             if finish_reason := choice.get("finish_reason"):
                 generation_info["finish_reason"] = finish_reason
-            default_chunk_class = chunk.__class__
+                generation_info["model"] = response["model"]
+                generation_info["created"] = response["created"]
+                generation_info["index"] = choice["index"]
+            if usage := response.get("usage"):
+                generation_info["usage"] = usage
+            default_chunk_class = message_chunk.__class__
             chunk = ChatGenerationChunk(
-                message=chunk, generation_info=generation_info or None
+                message=message_chunk,
+                generation_info=generation_info,
             )
             if run_manager:
                 await run_manager.on_llm_new_token(chunk.text, chunk=chunk)
             yield chunk
 
     def get_token_ids(self, text: str) -> List[int]:
         """Get the token IDs using the tiktoken package."""
 
         encoding_model = tiktoken.get_encoding("cl100k_base")
         return encoding_model.encode(
             text,
             allowed_special=self.allowed_special,
             disallowed_special=self.disallowed_special,
-        )
+        )
+
+    # def stream(
+    #     self,
+    #     input: LanguageModelInput,
+    #     config: Optional[RunnableConfig] = None,
+    #     *,
+    #     stop: Optional[List[str]] = None,
+    #     **kwargs: Any,
+    # ) -> Iterator[BaseMessageChunk]:
+    #     """
+    #     重定义stream，以便支持流式输出时的token统计。
+    #     """
+    #     config = ensure_config(config)
+    #     messages = self._convert_input(input).to_messages()
+    #     params = self._get_invocation_params(stop=stop, **kwargs)
+    #     options = {"stop": stop, **kwargs}
+    #     callback_manager = CallbackManager.configure(
+    #         config.get("callbacks"),
+    #         self.callbacks,
+    #         self.verbose,
+    #         config.get("tags"),
+    #         self.tags,
+    #         config.get("metadata"),
+    #         self.metadata,
+    #     )
+    #     (run_manager,) = callback_manager.on_chat_model_start(
+    #         dumpd(self),
+    #         [messages],
+    #         invocation_params=params,
+    #         options=options,
+    #         name=config.get("run_name"),
+    #         # run_id=config.pop("run_id", None),
+    #         batch_size=1,
+    #     )
+    #     generation: Optional[ChatGenerationChunk] = None
+    #     llm_output = {}
+    #     try:
+    #         for chunk in self._stream(
+    #             messages, stop=stop, run_manager=run_manager, **kwargs
+    #         ):
+    #             # chunk.message.response_metadata = _gen_info_and_msg_metadata(chunk)
+    #             yield chunk.message
+                
+    #             if generation is None:
+    #                 generation = chunk
+    #             else:
+    #                 generation += chunk
+    #             if hasattr(chunk, 'generation_info') and chunk.generation_info:
+    #                 llm_output.update(chunk.generation_info)
+    #         assert generation is not None
+    #     except BaseException as e:
+    #         run_manager.on_llm_error(
+    #             e,
+    #             response=LLMResult(
+    #                 generations=[[generation]] if generation else []
+    #             ),
+    #         )
+    #         raise e
+    #     else:
+    #         run_manager.on_llm_end(LLMResult(
+    #             generations=[[generation]],
+    #             llm_output=llm_output
+    #         ))
```

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/embeddings.py` & `langchain_zhipu-4.1.2/langchain_zhipu/http/embeddings.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,42 +13,49 @@
     get_pydantic_field_names,
 )
 
 # async
 import asyncio
 from typing import AsyncIterator
 
-from ._client import ZhipuAI
+from .api import RestAPI
 
 class ZhipuAIEmbeddings(BaseModel, Embeddings):
     """支持最新的智谱API向量模型"""
 
     client: Any = None
     """访问智谱AI的客户端"""
     
+    base_url: str = None
+    """访问智谱AI的服务器地址"""
+
     api_key: str = None
+    """访问智谱AI的ZHIPU_API_KEY"""
     
     model: str = Field(default="embedding-2")
     """所要调用的模型编码"""
 
     @root_validator()
-    def validate_environment(cls, values: Dict) -> Dict:        
-        if values["api_key"] is not None:
-            values["client"] =  ZhipuAI(api_key=values["api_key"])
-        else:
-            values["client"] =  ZhipuAI()
+    def validate_environment(cls, values: Dict) -> Dict:
+        values["client"] =  RestAPI(base_url=values["base_url"], api_key=values["api_key"])
         return values
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Embed search docs."""
         return [self._get_embedding(text) for text in texts]
 
     def embed_query(self, text: str) -> List[float]:
         """Embed query text."""
         return self._get_embedding(text)
         
     def _get_embedding(self, text: str) -> List[float]:
-        response = self.client.embeddings.create(
+        response = self.client.action_post(
+            request="api/paas/v4/embeddings", 
             model=self.model,
-            input=text
+            input=text,
         )
-        return response.data[0].embedding
+        if 'data' in response:
+            results = response['data']
+            if len(results) == 1:
+                return results[0]['embedding']
+
+        raise BaseException(response)
```

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/http/api.py` & `langchain_zhipu-4.1.2/langchain_zhipu/http/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import cachetools.func
 import requests
 from requests.exceptions import SSLError
 import json
 import time
 import jwt
 import os
 from typing import Any, Dict
@@ -28,130 +29,129 @@
     访问智谱官方的 ZHIPU_API_KEY
     """
 
     exp_seconds: int = 600
     """
     构造令牌的默认过期时间是600秒
     """
-    
+
+    def __hash__(self):
+        return hash((self.base_url, self.api_key, self.exp_seconds))
+
     @root_validator()
     def base_validate_environment(cls, values: Dict) -> Dict:
         values["base_url"] = init_base_url(values["base_url"])
         values["api_key"] = init_api_key(values["api_key"])
         values["session"] = requests.Session()
         return values
 
     def action_get(self, request: str, **kwargs):
         """GET"""
         
         url = f'{self.base_url}/{request}'
         headers = self._generate_headers()
-        response = self.session.get(url, headers=headers, params=kwargs)
-        
+
+        response = self._retry_request(self.session.get, url, headers=headers, params=kwargs)
+
         obj = json.loads(response.text)
         if obj["code"] == 200:
             return obj
         else:
-            raise Exception(obj)
+            raise BaseException(obj)        
 
     def action_post(self, request: str, files=None, **kwargs):
         """POST"""
         
         url = f'{self.base_url}/{request}'
         headers = self._generate_headers(files)
-        
         # 如果提供了 files 参数就需要将 kwargs 视作表单来处理
         data = kwargs if files else json.dumps(kwargs)
-        response = self.session.post(url, headers=headers, data=data, files=files)
 
-        if response.status_code == 200:
-            if response.text:
-                return response.json()
+        response = self._retry_request(self.session.post, url, headers=headers, data=data, files=files)
+
+        if response.text:
+            resp = response.json()
+            if "code" in resp and resp["code"] != 200:
+                raise BaseException(resp)
             else:
-                return {}
+                return resp
         else:
-            raise Exception({
-                "status_code": response.status_code,
-                "headers": response.headers,
-                "text": response.text,
-            })
+            return {}
     
     def action_sse_post(self, request: str, **kwargs):
         """POST for SSE"""
         
         url = f'{self.base_url}/{request}'
         headers = self._generate_headers()
         data = json.dumps(kwargs)
 
-        # 尝试发送请求，如果发生 SSLError 异常，重试请求        
-        for _ in range(3):
-            try:
-                return self.session.post(url, headers=headers, data=data, stream=True)
-            except SSLError:
-                continue
-        else:
-            raise Exception("Max retries exceeded with SSLError")
-
-        if response.status_code != 200:
-            raise Exception({
-                "status_code": response.status_code,
-                "headers": response.headers,
-                "text": response.text,
-            })
+        response =  self._retry_request(self.session.post, url, headers=headers, data=data, stream=True)
+        return response
 
     def action_put(self, request: str, **kwargs):
         """PUT"""
         
         url = f'{self.base_url}/{request}'
         headers = self._generate_headers()
-        response = self.session.put(url, headers=headers, data=json.dumps(kwargs))
+        data = json.dumps(kwargs)
         
-        if response.status_code == 200:
-            return response.json()
-        else:
-            raise Exception({
-                "status_code": response.status_code,
-                "headers": response.headers,
-                "text": response.text,
-            })
+        response = self._retry_request(self.session.put, url, headers=headers, data=data)
+        return response.json()
 
     def action_delete(self, request: str):
         """DELETE"""
         
         url = f'{self.base_url}/{request}'
         headers = self._generate_headers()
         response = self.session.delete(url, headers=headers)
         
-        if response.status_code == 200:
-            return response.json()
-        else:
-            raise Exception({
-                "status_code": response.status_code,
-                "headers": response.headers,
-                "text": response.text,
-            })
+        response = self._retry_request(self.session.delete, url, headers=headers)
+        return response.json()
         
     def _generate_headers(self, files = None) -> dict:
         headers = {
             'Authorization': f'Bearer {self._generate_token()}',
             'Content-Type': 'application/json' if not files else None,
         }
         return headers
 
+    # 优先使用60秒内调用过的缓存
+    @cachetools.func.ttl_cache(maxsize=10, ttl=60)
     def _generate_token(self) -> str:
         try:
             id, secret = self.api_key.split(".")
         except Exception as e:
-            raise Exception("invalid apikey", e)
+            raise BaseException("Invalid ZHIPUAI_API_KEY", e)
 
         payload = {
             "api_key": id,
             "exp": int(round(time.time() * 1000)) + self.exp_seconds * 1000,
             "timestamp": int(round(time.time() * 1000)),
         }
 
         return jwt.encode(
             payload,
             secret,
             algorithm="HS256",
             headers={"alg": "HS256", "sign_type": "SIGN"},
-        )
+        )
+        
+    def _retry_request(self, func, *args, **kwargs):
+        last_exception = None
+        for _ in range(3):
+            try:
+                response = func(*args, **kwargs)
+            except Exception as e:
+                last_exception = e
+                print("Retry for HTTP Error ...")
+                continue
+            else:
+                # 如果响应状态码不是 200，也引发一个异常
+                if response.status_code != 200:
+                    raise Exception({
+                        "status_code": response.status_code,
+                        "headers": response.headers,
+                        "text": response.text,
+                    })
+                return response
+        else:
+            raise last_exception
```

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/http/chat.py` & `langchain_zhipu-4.1.2/langchain_zhipu/http/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
     def raise_invalid_params(cls, values: Dict) -> Dict:
         if values["application_id"] is None:
             raise Exception("MUST supply application_id")
         return values
 
     def _ask_remote(self, prompt: Any, stop: Optional[List[str]] = None, **kwargs):
         params = self.get_model_kwargs()
-        # print(params)
         params.update({"prompt": prompt, **kwargs})
         if stop is not None:
             params.update({"stop": stop})
 
         reply = self.client.action_post(request=f"api/llm-application/open/model-api/{self.application_id}/invoke", **params)
         
         return ({
@@ -176,15 +175,14 @@
         })
 
     def _ask_remote_sse(self, prompt: Any, stop: Optional[List[str]] = None, **kwargs):
         """
         这是V3版本的SSE接口解析。
         """
         params = self.get_model_kwargs()
-        # print(params)
         params.update({"prompt": prompt, **kwargs})
         if stop is not None:
             params.update({"stop": stop})
 
         replies = self.client.action_sse_post(request=f"api/llm-application/open/model-api/{self.application_id}/sse-invoke", **params)
 
         # 使用 iter_lines 方法处理 SSE 响应
```

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/http/manager.py` & `langchain_zhipu-4.1.2/langchain_zhipu/http/manager.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/http/types.py` & `langchain_zhipu-4.1.2/langchain_zhipu/http/types.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.1/langchain_zhipu/utils.py` & `langchain_zhipu-4.1.2/langchain_zhipu/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_zhipu-4.1.1/pyproject.toml` & `langchain_zhipu-4.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain_zhipu"
-version = "4.1.1"
+version = "4.1.2"
 description = "将智谱AI集成到LangChain"
 license = "MIT"
 authors = ["arcstep <43801@qq.com>"]
 homepage = "https://github.com/arcstep/langchain_zhipuai"
 repository = "https://github.com/arcstep/langchain_zhipuai.git"
 readme = "README.md"
```

### Comparing `langchain_zhipu-4.1.1/PKG-INFO` & `langchain_zhipu-4.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain_zhipu
-Version: 4.1.1
+Version: 4.1.2
 Summary: 将智谱AI集成到LangChain
 Home-page: https://github.com/arcstep/langchain_zhipuai
 License: MIT
 Author: arcstep
 Author-email: 43801@qq.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,41 +20,91 @@
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Project-URL: Repository, https://github.com/arcstep/langchain_zhipuai.git
 Description-Content-Type: text/markdown
 
 # 为什么要开发这个包？
 [![PyPI version](https://img.shields.io/pypi/v/langchain_zhipu.svg)](https://pypi.org/project/langchain_zhipu/)
 
-为了方便在 langchain 中使用，在官方SDK基础上做了如下额外工作：
+为了方便在 langchain 中使用，langchain_zhipu 直接使用官方HTTP接口实现，并避免了如下的现存问题：
 
 - 问题1: 智谱AI的官方SDK使用了 pydantic v2，这与 langchain（尤其是langserve）不兼容
 - 问题2: langchain.community 的国内包更新不及时，无法在 langchain 的 LCEL 语法中使用
 
-# 已支持全部 langchain 接口
+# 能力支持
+
+## 已支持全部 langchain 接口
 
 1. invoke
 2. ainvoke
 3. batch
 4. abatch
 5. stream
 6. astream
 7. astream_events
 8. asteram_log
 
-# 已支持模型能力
+## 已支持模型能力
 
 - 已支持生成模型："glm-3-turbo", "glm-4", "glm-4v"
 - 已支持向量模型："embedding-2"
-- 逻辑推理和对话生成
-- 支持工具回调
+- 已支持官方知识库管理能力：对知识库、文档、应用做增删改查
+- 已支持基于官方知识库的大模型对话
+- 支持工具回调：普通工具，以及在线知识库和网络搜索
 - 支持智能体
 - 支持RAG
 
 # 使用
 
+## 配置
+
+可以将申请到的 `API_KEY` 配置到环境变量 `ZHIPUAI_API_KEY`。
+
+建议使用 `.env` 文件来管理环境变量，这可能安装 `dotenv` 包：
+
+```bash
+pip install dotenv
+```
+
+你的 .env 文件：
+
+```
+ZHIPUAI_API_KEY="你的KEY"
+```
+
+然后在你的代码目录中：
+
+```python
+# 加载 .env 到环境变量
+import os
+from dotenv import load_dotenv, find_dotenv
+load_dotenv(find_dotenv(), override=True)
+```
+
+## 安装 langchain_zhipu
+
+```bash
+pip install langchain langchain_zhipu
+```
+
+其中，langchain 只要 `v0.1.0` ，而 langchain_zhipu 最好安装最新的 4.1.x 版本。
+
+## 代码例子
+
+- [基本用法 usage.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/notes/usage.ipynb)
+- [智能体 agent.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/notes/agent.ipynb)
+- [向量模型 embedding.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/notes/embedding.ipynb)
+- [模型统计 tokens.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/notes/tokens.ipynb)
+- [知识库 knowledge.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/notes/knowledge.ipynb)
+- [知识库应用 knowledge_app.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/notes/knowledge_app.ipynb)
+- [langchain_chinese](https://github.com/arcstep/langchain_chinese)
+
+------------------------------------------
+
+**官方接口指南** 智谱[开放平台](https://open.bigmodel.cn/dev/api)
+
 ## 简单的例子
 
 ```python
 from langchain_zhipu import ChatZhipuAI
 llm = ChatZhipuAI()
 
 # invoke
@@ -119,21 +169,8 @@
           }
         ]),
 ])
 
 (prompt|llm4v).invoke({})
 ```
 
-## 智能体
-
-请查看 [agent.ipynb](https://github.com/arcstep/langchain_zhipuai/blob/main/agent.ipynb)
-
-# 更多用法
-
-请参考 [langchain_chinese](https://github.com/arcstep/langchain_chinese)
-
-------------------------------------------
-
-**官方接口指南** 智谱[开放平台](https://open.bigmodel.cn/dev/api)大模型接口 Python SDK（Big Model API SDK in Python），让开发者更便捷的调用智谱开放API
-
-**官方SDK** [![PyPI version](https://img.shields.io/pypi/v/zhipuai.svg)](https://pypi.org/project/zhipuai/)
```

