# Comparing `tmp/dbt_llm_tools-0.1.1a0.tar.gz` & `tmp/dbt_llm_tools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_llm_tools-0.1.1a0.tar", max compression
+gzip compressed data, was "dbt_llm_tools-0.2.0.tar", max compression
```

## Comparing `dbt_llm_tools-0.1.1a0.tar` & `dbt_llm_tools-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1659 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/LICENSE.md
--rw-r--r--   0        0        0     7313 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/README.md
--rw-r--r--   0        0        0      496 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/__init__.py
--rw-r--r--   0        0        0     7321 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/chatbot.py
--rw-r--r--   0        0        0     3090 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/dbt_model.py
--rw-r--r--   0        0        0    10330 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/dbt_project.py
--rw-r--r--   0        0        0     7195 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/documentation_generator.py
--rw-r--r--   0        0        0     2499 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/instructions.py
--rw-r--r--   0        0        0     1457 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/types.py
--rw-r--r--   0        0        0     6789 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/dbt_llm_tools/vector_store.py
--rw-r--r--   0        0        0     1548 2024-04-02 12:53:43.360433 dbt_llm_tools-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     8439 1970-01-01 00:00:00.000000 dbt_llm_tools-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1665 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     3925 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/README.md
+-rw-r--r--   0        0        0      496 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/__init__.py
+-rw-r--r--   0        0        0     7647 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/chatbot.py
+-rw-r--r--   0        0        0     3389 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/dbt_model.py
+-rw-r--r--   0        0        0    10696 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/dbt_project.py
+-rw-r--r--   0        0        0     7195 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/documentation_generator.py
+-rw-r--r--   0        0        0     2312 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/instructions.py
+-rw-r--r--   0        0        0     1457 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/types.py
+-rw-r--r--   0        0        0     6869 2024-04-20 08:22:59.401624 dbt_llm_tools-0.2.0/dbt_llm_tools/vector_store.py
+-rw-r--r--   0        0        0     1729 2024-04-20 08:22:59.405624 dbt_llm_tools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5131 1970-01-01 00:00:00.000000 dbt_llm_tools-0.2.0/PKG-INFO
```

### Comparing `dbt_llm_tools-0.1.1a0/LICENSE.md` & `dbt_llm_tools-0.2.0/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 The MIT License (MIT)
 
 Copyright (c) 2024 [Pragun Bhutani](https://pragunbhutani.com) & [Delta 4 Technologies](https://delta4.tech).
 
 Portions of this software are licensed as follows:
 
 - All content that resides under the "ee/" directory of this repository, if that directory exists, is licensed under the license defined in "ee/LICENSE".
-- All third party components incorporated into the Ragstar Software are licensed under the original license provided by the owner of the applicable component.
+- All third party components incorporated into the dbt-llm-tools Software are licensed under the original license provided by the owner of the applicable component.
 - Content outside of the above mentioned directories or restrictions above is available under the "MIT Expat" license as defined below.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/chatbot.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/chatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from openai import OpenAI
 
+from dbt_llm_tools.dbt_model import DbtModel
 from dbt_llm_tools.dbt_project import DbtProject
 from dbt_llm_tools.instructions import ANSWER_QUESTION_INSTRUCTIONS
 from dbt_llm_tools.types import ParsedSearchResult, PromptMessage
 from dbt_llm_tools.vector_store import VectorStore
 
 
 class Chatbot:
@@ -24,33 +25,39 @@
         ask_question: Ask the chatbot a question and get a response.
     """
 
     def __init__(
         self,
         dbt_project_root: str,
         openai_api_key: str,
+        database_path: str = ".local_storage/db.json",
+        vector_db_path: str = ".local_storage/chroma.db",
         embedding_model: str = "text-embedding-3-large",
-        chatbot_model: str = "gpt-4-turbo-preview",
-        vector_db_path: str = "./database/chroma.db",
-        database_path: str = "./database/directory.json",
+        chatbot_model: str = "gpt-4-turbo",
     ) -> None:
         """
         Initializes a chatbot object along with a default set of instructions.
 
         Args:
             dbt_project_root (str): The absolute path to the root of the dbt project.
             openai_api_key (str): Your OpenAI API key.
 
-            embedding_model (str, optional): The name of the OpenAI embedding model to be used.
-            Defaults to "text-embedding-3-large".
+            database_path (str, optional):
+                The path to the persistent database files. Defaults to ".local_storage/db.json".
 
-            chatbot_model (str, optional): The name of the OpenAI chatbot model to be used.
-            Defaults to "gpt-4-turbo-preview".
+            vector_db_path (str, optional):
+                The path to the persistent vector database. Defaults to ".local_storage/chroma.db".
 
-            db_persist_path (str, optional): The path to the persistent database file. Defaults to "./chroma.db".
+            embedding_model (str, optional):
+                The name of the OpenAI embedding model to be used.
+                Defaults to "text-embedding-3-large".
+
+            chatbot_model (str, optional):
+                The name of the OpenAI chatbot model to be used.
+                Defaults to "gpt-4-turbo-preview".
 
         Returns:
             None
         """
         self.__chatbot_model: str = chatbot_model
         self.__openai_api_key: str = openai_api_key
 
@@ -158,15 +165,17 @@
             exclude_folders (list[str], optional): A list of paths to all folders that should be excluded
             in model search. Paths are relative to dbt project root.
 
         Returns:
             None
         """
         models = self.project.get_models(models, included_folders, excluded_folders)
-        self.store.upsert_models(models)
+        self.store.upsert_models(
+            list(map(lambda x: DbtModel(x.get("documentation")), models))
+        )
 
     def reset_model_db(self) -> None:
         """
         This will reset and remove all the models from the vector store.
         You'll need to load the models again using the load_models method if you want to use the chatbot.
 
         Returns:
```

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/dbt_model.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/dbt_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,61 +6,70 @@
 class DbtModel:
     """
     A class representing a dbt model.
 
     Attributes:
         name (str): The name of the model.
         description (str, optional): The description of the model.
-        columns (list[DbtModelColumn], optional): A list of columns contained in the model.
-        May or may not be exhaustive.
+        columns (list[DbtModelColumn], optional):
+            A list of columns contained in the model. May or may not be exhaustive.
     """
 
-    def __init__(self, model_dict: DbtModelDict) -> None:
+    def __init__(self, documentation: DbtModelDict) -> None:
         """
         Initializes a dbt model object.
 
         Args:
             model_dict (dict): A dictionary containing the model name, description and columns.
         """
-        self.name = model_dict.get("name")
+        self.name = documentation.get("name")
 
         if self.name is None:
             raise Exception("Cannot create a model without a valid name.")
 
-        config = model_dict.get("config", {})
+        config = documentation.get("config", {})
         self.tags = config.get("tags", [])
 
-        self.description = model_dict.get("description", "")
+        self.description = documentation.get("description", "")
 
-        raw_columns = filter(lambda x: "name" in x, model_dict.get("columns", []))
-        self.columns = map(
-            lambda x: {"name": x.get("name"), "description": x.get("description")},
-            raw_columns,
+        raw_columns = filter(lambda x: "name" in x, documentation.get("columns", []))
+        self.columns = list(
+            map(
+                lambda x: {"name": x.get("name"), "description": x.get("description")},
+                raw_columns,
+            )
         )
 
     def __print_model_doc(self) -> str:
         """
         Template function that takes a model name, description and a list of columns as arguments
         and returns a text description of the model. This description can be used as a part of a prompt
         for an LLM.
 
         Args:
             model (DbtModelDict): A dictionary representation of the dbt model.
 
         Returns:
             str: A text description of the model, including the list of columns with their descriptions.
         """
-        model = self.as_dict()
-
-        model_text = f"The table { model['name'] } is described as follows: { model['description'] }"
-        model_text += "\nThis table contains the following columns:\n"
-
-        for col in model["columns"]:
-            model_text += "\n"
-            model_text += f"- { col['name'] }: { col['description'] }"
+        if self.description == "":
+            model_text = f"The table { self.name } does not have a description."
+        else:
+            model_text = (
+                f"The table { self.name } is described as follows: { self.description }"
+            )
+
+        if len(list(self.columns)) > 0:
+            model_text += "\nThis table contains the following columns:\n"
+
+            for col in self.columns:
+                model_text += "\n"
+                model_text += (
+                    f"- { col['name'] }: { col.get('description', 'No description')}"
+                )
 
         return model_text
 
     def as_dict(self) -> DbtModelDict:
         """
         Returns the dbt model as a dictionary.
```

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/dbt_project.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/dbt_project.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 import json
 import os
 import re
 from typing import Union
 
 import yaml
 
-from dbt_llm_tools.dbt_model import DbtModel
+from tinydb import TinyDB, Query
+
 from dbt_llm_tools.types import DbtModelDirectoryEntry, DbtProjectDirectory
 
 SOURCE_SEARCH_EXPRESSION = r"source\(['\"]*(.*?)['\"]*?\)"
 REF_SEARCH_EXPRESSION = r"ref\(['\"]*(.*?)['\"]*\)"
 
 
 class DbtProject:
     """
     A class representing a DBT project.
     """
 
     def __init__(
         self,
         dbt_project_root: str,
-        database_path: str = "./directory.json",
+        database_path: str = ".local_storage/db.json",
     ) -> None:
         """
         Initializes a dbt project parser object.
 
         Args:
             dbt_project_root (str): Root of the dbt prject
             database_path (str, optional): Path to the directory file that stores the parsed dbt project.
@@ -33,27 +34,24 @@
         Methods:
             parse: Parse the dbt project and store details in a manifest file.
             get_single_model: Get a single model by name.
             get_models: Get a list of models based on the provided filters.
             update_model_directory: Update a model in the directory.
         """
         self.__project_root = dbt_project_root
-        self.__directory_path = database_path
-
         project_file = os.path.join(dbt_project_root, "dbt_project.yml")
 
         if not os.path.isfile(project_file):
             raise Exception("No dbt project found in the specified folder")
 
+        self.__database_path = database_path
+        os.makedirs(os.path.dirname(database_path), exist_ok=True)
+
         with open(project_file, encoding="utf-8") as f:
             project_config = yaml.safe_load(f)
-
-            if "model-paths" not in project_config:
-                raise Exception("No model-paths defined in the dbt project file")
-
             self.__model_paths = project_config.get("model-paths", ["models"])
 
         self.__sql_files = self.__get_all_files("sql")
         self.__yaml_files = self.__get_all_files("yml")
 
     def __get_all_files(self, file_extension: str):
         """
@@ -100,20 +98,26 @@
             file_contents = f.read()
 
         search_results = re.findall(REF_SEARCH_EXPRESSION, file_contents)
         unique_results = list(set(search_results))
 
         if recursive:
             for result in unique_results:
+                if result in dependencies or result in file_path:
+                    continue
+
                 sub_file_path = next(
-                    (x for x in self.__sql_files if x.endswith(f"{result}.sql")), None
-                )
-                dependencies = self.__find_upstream_references(
-                    file_path=sub_file_path, recursive=True, dependencies=dependencies
+                    (x for x in self.__sql_files if x.endswith(f"/{result}.sql")), None
                 )
+                if sub_file_path is not None:
+                    dependencies = self.__find_upstream_references(
+                        file_path=sub_file_path,
+                        recursive=True,
+                        dependencies=dependencies,
+                    )
 
         return dependencies + unique_results
 
     def __parse_sql_file(self, sql_file: str):
         """
         Parse a SQL file and return a dictionary with the file metadata.
 
@@ -127,17 +131,19 @@
             sql_contents = f.read()
 
         sources = []
         source_search = re.findall(SOURCE_SEARCH_EXPRESSION, sql_contents)
 
         for raw_source in source_search:
             source = raw_source.replace("'", "").replace('"', "").split(",")
-            sources.append({"name": source[0], "table": source[1]})
+            if len(source) == 2:
+                sources.append({"name": source[0], "table": source[1]})
 
         return {
+            "type": "model",
             "absolute_path": sql_file,
             "relative_path": sql_file.replace(self.__project_root, ""),
             "name": os.path.basename(sql_file).replace(".sql", ""),
             "refs": self.__find_upstream_references(sql_file, False),
             "deps": self.__find_upstream_references(sql_file, True),
             "sources": sources,
             "sql_contents": sql_contents,
@@ -157,60 +163,64 @@
         models = {}
         sources = {}
 
         for yaml_path in yaml_files:
             with open(yaml_path, encoding="utf-8") as f:
                 yaml_contents = yaml.safe_load(f)
 
+            if yaml_contents is None:
+                continue
+
             for model in yaml_contents.get("models", []):
                 model["yaml_path"] = yaml_path
-
-                parsed_columns = {}
-                for col in model.get("columns", []):
-                    col_name = col.pop("name")
-                    parsed_columns[col_name] = col
-
-                model["columns"] = parsed_columns
-
                 models[model["name"]] = model
 
             for source in yaml_contents.get("sources", []):
+                source["type"] = "source"
                 source["yaml_path"] = yaml_path
                 sources[source["name"]] = source
 
         return models, sources
 
     def __get_directory(self):
         """
         Get the parsed directory from the directory file.
 
         Returns:
             dict: The parsed directory.
         """
-        with open(self.__directory_path, encoding="utf-8") as f:
+        with open(self.__database_path, encoding="utf-8") as f:
             return json.load(f)
 
     def __save_directory(self, directory):
         """
         Save the parsed directory to a file.
 
         Args:
             directory (dict): The directory to save.
         """
-        with open(self.__directory_path, "w", encoding="utf-8") as f:
-            json.dump(directory, f, ensure_ascii=False, indent=4)
+        db = TinyDB(self.__database_path, sort_keys=True, indent=4)
+        Model = Query()  # pylint: disable=invalid-name
+        Source = Query()  # pylint: disable=invalid-name
+
+        for name, model in directory["models"].items():
+            if "name" in model:
+                db.upsert(model, Model.name == name)
+
+        for name, source in directory["sources"].items():
+            if "name" in source:
+                db.upsert(source, Source.name == source["name"])
 
     def parse(self) -> DbtProjectDirectory:
         """
         Parse the dbt project and store details in a manifest file.
 
         Returns:
             dict: The parsed directory.
         """
-        # source_sql_models = list(map(self.__parse_sql_file, self.__sql_files))
         source_sql_models = {}
 
         for sql_file in self.__sql_files:
             parsed_model = self.__parse_sql_file(sql_file)
             source_sql_models[parsed_model["name"]] = parsed_model
 
         documented_models, documented_sources = self.__parse_yaml_files(
@@ -247,17 +257,19 @@
 
         Returns:
             dict: The model object.
         """
         if model_name is None:
             raise Exception("No model name provided")
 
-        directory = self.__get_directory()
+        # directory = self.__get_directory()
+        db = TinyDB(self.__database_path)
+        Model = Query()  # pylint: disable=invalid-name
 
-        return directory["models"].get(model_name)
+        return db.get(Model.name == model_name)
 
     def get_models(
         self,
         models: list[str] = None,
         included_folders: list[str] = None,
         excluded_folders: list[str] = None,
     ):
@@ -270,43 +282,40 @@
             excluded_folders (list, optional): A list of folders to exclude from the search for sql or yaml files.
 
         Returns:
             list: A list of DbtModel objects.
         """
         searched_models = []
 
-        directory = self.__get_directory()
+        db = TinyDB(self.__database_path)
+        Model = Query()  # pylint: disable=invalid-name
+        File = Query()  # pylint: disable=invalid-name
 
         if models is None and included_folders is None:
-            searched_models = list(directory["models"].values())
+            searched_models = db.search(File.type == "model")
 
         for model in models or []:
-            searched_models.append(directory["models"].get(model))
+            if model := db.get(Model.name == model):
+                searched_models.append(model)
 
         for included_folder in included_folders or []:
-            for model in directory["models"].values():
+            for model in db.search(File.type == "model"):
                 if included_folder in model.get(
                     "absolute_path", ""
                 ) or included_folder in model.get("yaml_path", ""):
                     searched_models.append(model)
 
         for excluded_folder in excluded_folders or []:
             for model in searched_models.copy():
                 if excluded_folder in model.get(
                     "absolute_path", ""
                 ) or excluded_folder in model.get("yaml_path", ""):
                     searched_models.remove(model)
 
-        models_to_return = []
-
-        for model in searched_models:
-            if model["documentation"] is not None:
-                models_to_return.append(DbtModel(model["documentation"]))
-
-        return models_to_return
+        return searched_models
 
     def update_model_directory(self, model: dict):
         """
         Update a model in the directory.
 
         Args:
             model (dict): The model to update.
```

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/documentation_generator.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/instructions.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/instructions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-INTERPRET_MODEL_INSTRUCTIONS = r"""
-    You are a data analyst trying to understand the meaning and schema of a dbt model.
-    You will be provided with the name of the model and the Jinja SQL code that defines the model.
+INTERPRET_MODEL_INSTRUCTIONS = r"""You are a data analyst trying to understand the meaning and schema of a dbt model.
+You will be provided with the name of the model and the Jinja SQL code that defines the model.
 
-    The Jinja files may contain references to other models, using the \{\{ ref('model_name') \}\} syntax,
-    or references to source tables using the \{\{ source('schema_name', 'table_name') \}\} syntax.
+The Jinja files may contain references to other models, using the \{\{ ref('model_name') \}\} syntax,
+or references to source tables using the \{\{ source('schema_name', 'table_name') \}\} syntax.
 
-    The interpretation for all upstream models will be provided to you in the form of a
-    JSON object that contains the following keys: model, description, columns.
+The interpretation for all upstream models will be provided to you in the form of a
+JSON object that contains the following keys: model, description, columns.
 
-    A source table is a table that is not defined in the dbt project, but is instead a table that is present in the
-    data warehouse.
+A source table is a table that is not defined in the dbt project, but is instead a table that is present in the
+data warehouse.
 
-    Your response should be in the form of a JSON object that contains the following keys: model, description, columns.
+Your response should be in the form of a JSON object that contains the following keys: model, description, columns.
 
-    The columns key should contain a list of JSON objects, each of which should contain
-    the following keys: name, description.
+The columns key should contain a list of JSON objects, each of which should contain
+the following keys: name, description.
 
-    Your response should only contain an unformatted JSON string described above and nothing else.
+Your response should only contain an unformatted JSON string described above and nothing else.
 """
 
-ANSWER_QUESTION_INSTRUCTIONS = r"""
-    You are a data analyst working with a data warehouse. You should provide the user with the information
-    they need to answer their question.
-
-    You should only provide information that you are confident is correct. When you are not sure about the answer,
-    you should let the user know.
-
-    If you are able to construct a SQL query that would answer the user's question, you should do so. However
-    please refrain from doing so if the user's question is ambiguous or unclear. When writing a SQL query,
-    you should only use column values if these values have been explicitly provided to you in the information
-    you have been given.
-
-    Do not write a SQL query if you are unsure about the correctness of the query or about the values contained
-    in the columns. Only write a SQL query if you are confident that the query is exhaustive and that it will
-    return the correct results. If it is not possible to write a SQL that fulfils these conditions,
-    you should instead respond with the names of the tables or columns that you think are relevant to the user's
-    question.
+ANSWER_QUESTION_INSTRUCTIONS = r"""You are a data analyst working with a data warehouse.
+You should provide the user with the information they need to answer their question.
 
-    You should also refrain from providing any information that is not directly related to the user's question or that
-    which cannot be inferred from the information you have been given.
+You should only provide information that you are confident is correct. When you are not sure about the answer,
+you should let the user know.
 
-    The following information about tables and columns is available to you:
+If you are able to construct a SQL query that would answer the user's question, you should do so. However
+please refrain from doing so if the user's question is ambiguous or unclear. When writing a SQL query,
+you should only use column values if these values have been explicitly provided to you in the information
+you have been given.
+
+Do not write a SQL query if you are unsure about the correctness of the query or about the values contained
+in the columns. Only write a SQL query if you are confident that the query is exhaustive and that it will
+return the correct results. If it is not possible to write a SQL that fulfils these conditions,
+you should instead respond with the names of the tables or columns that you think are relevant to the user's
+question.
+
+You should also refrain from providing any information that is not directly related to the user's question or that
+which cannot be inferred from the information you have been given.
 """
```

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/types.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/types.py`

 * *Files identical despite different names*

### Comparing `dbt_llm_tools-0.1.1a0/dbt_llm_tools/vector_store.py` & `dbt_llm_tools-0.2.0/dbt_llm_tools/vector_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import json
 
 import chromadb
 from chromadb.utils import embedding_functions
 
 from dbt_llm_tools.dbt_model import DbtModel
 from dbt_llm_tools.types import ParsedSearchResult
@@ -17,32 +18,34 @@
         reset_collection: Clear the collection of all documents.
     """
 
     def __init__(
         self,
         openai_api_key: str,
         embedding_model_name: str = "text-embedding-3-large",
-        db_persist_path: str = "./chroma.db",
+        vector_db_path: str = ".local_storage/chroma.db",
         test_mode: bool = False,
     ) -> None:
         """
         Initializes a vector store for dbt models.
 
         Args:
             openai_api_key (str): Your OpenAI API key.
             embedding_model_name (str, optional): The name of the OpenAI embedding model to be used.
             db_persist_path (str, optional): The path to the persistent database file. Defaults to "./chroma.db".
             test_mode (bool, optional): Whether the vector store is being used in test mode. Defaults to False.
         """
-        if not isinstance(db_persist_path, str) or db_persist_path == "":
+        if not isinstance(vector_db_path, str) or vector_db_path == "":
             raise Exception("Please provide a valid path for the persistent database.")
 
+        os.makedirs(vector_db_path, exist_ok=True)
+        self.__client = chromadb.PersistentClient(vector_db_path)
+        self.__collection_name = "model_documentation"
+
         self.__openai_api_key = openai_api_key
-        self.__client = chromadb.PersistentClient(db_persist_path)
-        self.__collection_name = "dbt_models"
 
         self.__embedding_fn = self.__get_embedding_fn(
             embedding_model_name, test_mode=test_mode
         )
 
         self.__collection = self.__create_collection()
```

### Comparing `dbt_llm_tools-0.1.1a0/pyproject.toml` & `dbt_llm_tools-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-llm-tools"
-version = "0.1.1a0"
+version = "0.2.0"
 description = "LLM based tools for dbt projects. Answer data questions, generate documentation and more."
 authors = [
     "Pragun Bhutani <1109752+pragunbhutani@users.noreply.github.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pragunbhutani/dbt-llm-tools"
@@ -26,38 +26,47 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^1.16.0"
 chromadb = "^0.4.24"
 PyYAML = "^6.0.1"
 typing-extensions = "^4.10.0"
+streamlit = "^1.33.0"
+tinydb = "^4.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.1.0"
 flake8 = "^7.0.0"
 black = "^24.3.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 flake8-pyproject = "^1.2.3"
 
 
 [tool.poetry.group.local.dependencies]
 notebook = "^7.1.2"
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx-rtd-theme = "^2.0.0"
+
 [tool.flake8]
 max-line-length = 120
 per-file-ignores = """
     __init__.py: F401
 """
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length=120
 disable = """
     missing-module-docstring,
     too-many-arguments,
     too-few-public-methods,
-    broad-exception-raised
+    broad-exception-raised,
+    missing-function-docstring,
+    redefined-builtin,
+    duplicate-code
 """
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

