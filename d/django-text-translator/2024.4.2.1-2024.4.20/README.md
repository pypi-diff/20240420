# Comparing `tmp/django_text_translator-2024.4.2.1.tar.gz` & `tmp/django_text_translator-2024.4.20.tar.gz`

## Comparing `django_text_translator-2024.4.2.1.tar` & `django_text_translator-2024.4.20.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/.github/FUNDING.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/__init__.py
--rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/admin.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/apps.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/views.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0001_initial.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0004_alter_openaitranslator_model.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0008_geminitranslator.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0010_claudetranslator.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0012_geminitranslator_interval.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0013_deeplwebtranslator.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0014_testtranslator_interval.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0015_googletranslatewebtranslator_max_characters.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0018_alter_claudetranslator_model.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0019_alter_openaitranslator_model.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0020_moonshotaitranslator.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0021_alter_claudetranslator_model.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/0022_alter_geminitranslator_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/migrations/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/__init__.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/azureai.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/base.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/caiyun.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/claude.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/deepl.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/deeplweb.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/deeplx.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/dev.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/gemini.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/google_translate_web.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/microsoft_translate.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/moonshotai.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/models/openai.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/django_text_translator/static/img/icon-loading.svg
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/LICENSE
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/pyproject.toml
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 django_text_translator-2024.4.2.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/__init__.py
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/admin.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/apps.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/views.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0004_alter_openaitranslator_model.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0008_geminitranslator.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0010_claudetranslator.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0012_geminitranslator_interval.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0013_deeplwebtranslator.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0014_testtranslator_interval.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0015_googletranslatewebtranslator_max_characters.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0018_alter_claudetranslator_model.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0019_alter_openaitranslator_model.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0020_moonshotaitranslator.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0021_alter_claudetranslator_model.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0022_alter_geminitranslator_model.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0023_azureaitranslator_summary_prompt_and_more.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/0024_alter_claudetranslator_model_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/migrations/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/__init__.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/azureai.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/base.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/caiyun.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/claude.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/deepl.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/deeplweb.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/deeplx.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/dev.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/gemini.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/google_translate_web.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/microsoft_translate.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/moonshotai.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/models/openai.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/django_text_translator/static/img/icon-loading.svg
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/LICENSE
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/README.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/pyproject.toml
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 django_text_translator-2024.4.20/PKG-INFO
```

### Comparing `django_text_translator-2024.4.2.1/.github/workflows/python-publish.yml` & `django_text_translator-2024.4.20/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/admin.py` & `django_text_translator-2024.4.20/django_text_translator/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,23 +39,23 @@
             return f"{api_key[:3]}...{api_key[-3:]}"
         return ""
     masked_api_key.short_description = "API Key"
 
 @admin.register(OpenAITranslator)
 class OpenAITranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "api_key", "base_url", "model", "prompt", "temperature", "top_p", "frequency_penalty",
-              "presence_penalty", "max_tokens"]
-    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "base_url"]
+              "presence_penalty", "max_tokens",  "summary_prompt"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "base_url",  "summary_prompt"]
 
 
 @admin.register(AzureAITranslator)
 class AzureAITranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "api_key", "endpoint", "version", "deloyment_name", "prompt", "temperature", "top_p",
-              "frequency_penalty", "presence_penalty", "max_tokens"]
-    list_display = ["name", "is_valid", "masked_api_key", "deloyment_name", "version", "prompt", "max_tokens", "endpoint"]
+              "frequency_penalty", "presence_penalty", "max_tokens",  "summary_prompt"]
+    list_display = ["name", "is_valid", "masked_api_key", "deloyment_name", "version", "prompt", "max_tokens", "endpoint",  "summary_prompt"]
 
 
 @admin.register(DeepLTranslator)
 class DeepLTranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "api_key", "server_url", "proxy", "max_characters"]
     list_display = ["name", "is_valid", "masked_api_key", "server_url", "proxy", "max_characters"]
 
@@ -81,44 +81,44 @@
 class CaiYunTranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "token", "url", "max_characters"]
     list_display = ["name", "is_valid", "masked_api_key", "url", "max_characters"]
 
 
 @admin.register(GeminiTranslator)
 class GeminiTranslatorAdmin(BaseTranslatorAdmin):
-    fields = ["name", "api_key", "model", "prompt", "temperature", "top_p", "top_k", "max_tokens", "interval"]
-    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "interval"]
+    fields = ["name", "api_key", "model", "prompt", "temperature", "top_p", "top_k", "max_tokens",  "summary_prompt", "interval"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens",  "summary_prompt", "interval"]
 
 
 @admin.register(GoogleTranslateWebTranslator)
 class GoogleTranslateWebTranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "base_url", "interval", "proxy", "max_characters"]
     list_display = ["name", "is_valid", "base_url", "proxy", "interval", "max_characters"]
 
 @admin.register(ClaudeTranslator)
 class ClaudeTranslatorAdmin(BaseTranslatorAdmin):
-    fields = ["name", "api_key", "base_url", "model", "prompt", "temperature", "top_p", "top_k", "max_tokens", "proxy"]
-    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "base_url"]
+    fields = ["name", "api_key", "base_url", "model", "prompt", "temperature", "top_p", "top_k", "max_tokens",  "summary_prompt", "proxy"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "base_url",  "summary_prompt"]
 
 @admin.register(MoonshotAITranslator)
 class MoonshotAITranslatorAdmin(BaseTranslatorAdmin):
     fields = ["name", "api_key", "base_url", "model", "prompt", "temperature", "top_p", "frequency_penalty",
-              "presence_penalty", "max_tokens"]
-    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "base_url"]
+              "presence_penalty", "max_tokens",  "summary_prompt"]
+    list_display = ["name", "is_valid", "masked_api_key", "model", "prompt", "max_tokens", "base_url",  "summary_prompt"]
 
 if settings.DEBUG:
     @admin.register(Translated_Content)
     class Translated_ContentAdmin(admin.ModelAdmin):
-        #fields = ["original_content", "translated_content", "translated_language", "tokens", "characters"]
+        fields = ["original_content", "translated_content", "translated_language", "tokens", "characters"]
         list_display = ["original_content", "translated_language", "translated_content", "tokens", "characters"]
     
-        def has_change_permission(self, request, obj=None):
-            return False
+        # def has_change_permission(self, request, obj=None):
+        #     return False
 
-        def has_add_permission(self, request):
-            return False
+        # def has_add_permission(self, request):
+        #     return False
 
 
     @admin.register(TestTranslator)
     class TestTranslatorAdmin(BaseTranslatorAdmin):
         fields = ["name", "translated_text", "max_characters", "interval"]
         list_display = ["name", "is_valid", "translated_text", "max_characters", "interval"]
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0001_initial.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0002_openaitranslator_base_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0003_azureaitranslator_openaitranslator_frequency_penalty_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0004_alter_openaitranslator_model.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0004_alter_openaitranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0005_caiyuntranslator_deeplxtranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0006_testtranslator_alter_openaitranslator_prompt.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0007_caiyuntranslator_max_characters_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0008_geminitranslator.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0008_geminitranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0009_deepltranslator_proxy_deepltranslator_server_url.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0010_claudetranslator.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0010_claudetranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0011_googletranslatewebtranslator_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0013_deeplwebtranslator.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0013_deeplwebtranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0016_alter_deeplwebtranslator_max_characters_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0017_remove_translated_content_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0018_alter_claudetranslator_model.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0018_alter_claudetranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0019_alter_openaitranslator_model.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0019_alter_openaitranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0020_moonshotaitranslator.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0020_moonshotaitranslator.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/migrations/0021_alter_claudetranslator_model.py` & `django_text_translator-2024.4.20/django_text_translator/migrations/0021_alter_claudetranslator_model.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/__init__.py` & `django_text_translator-2024.4.20/django_text_translator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/azureai.py` & `django_text_translator-2024.4.20/django_text_translator/models/azureai.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     deloyment_name = models.CharField(max_length=100)
     prompt = models.TextField(default="Translate the following to {target_language},only returns translations.\n{text}")
     temperature = models.FloatField(default=0.5)
     top_p = models.FloatField(default=0.95)
     frequency_penalty = models.FloatField(default=0)
     presence_penalty = models.FloatField(default=0)
     max_tokens = models.IntegerField(default=1000)
+    
+    summary_prompt = models.TextField(default="Summarize the following text in {target_language}:\n{text}")
 
     class Meta:
         verbose_name = "Azure OpenAI"
         verbose_name_plural = "Azure OpenAI"
 
     def _init(self):
         return AzureOpenAI(
@@ -40,21 +42,22 @@
                     messages=[{"role": "user", "content": 'Hi'}],
                     max_tokens=10,
                 )
                 return True
             except Exception as e:
                 return False
 
-    def translate(self, text:str, target_language:str) -> dict:
+    def translate(self, text:str, target_language:str, prompt:str=None) -> dict:
         logging.info(">>> AzureAI Translate [%s]:", target_language)
         client = self._init()
         tokens = 0
         translated_text = ''
+        prompt = prompt or self.prompt
         try:
-            prompt = self.prompt.format(target_language=target_language, text=text)
+            prompt = prompt.format(target_language=target_language, text=text)
             res = client.with_options(max_retries=3).chat.completions.create(
                 model=self.deloyment_name,
                 messages=[{"role": "user", "content": prompt}],
                 temperature=self.temperature,
                 top_p=self.top_p,
                 frequency_penalty=self.frequency_penalty,
                 presence_penalty=self.presence_penalty,
@@ -66,7 +69,11 @@
                 translated_text = ''
                 logging.info("AzureAITranslator->%s: %s", res.choices[0].finish_reason, text)
             tokens = res.usage.total_tokens
         except Exception as e:
             logging.error("AzureAITranslator->%s: %s", e, text)
 
         return {'text': translated_text, "tokens": tokens}
+
+    def summarize(self, text:str, target_language:str) -> dict:
+        logging.info(">>> AzureAI Summarize [%s]:", target_language)
+        return self.translate(text, target_language, self.summary_prompt)
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/base.py` & `django_text_translator-2024.4.20/django_text_translator/models/base.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/caiyun.py` & `django_text_translator-2024.4.20/django_text_translator/models/caiyun.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/claude.py` & `django_text_translator-2024.4.20/django_text_translator/models/claude.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 import logging
 from django.db import models
 from encrypted_model_fields.fields import EncryptedCharField
 from django.utils.translation import gettext_lazy as _
 
 class ClaudeTranslator(TranslatorEngine):
     # https://docs.anthropic.com/claude/reference/getting-started-with-the-api
-    claude_models = ['claude-3-haiku-20240307', 'claude-3-sonnet-20240229', 'claude-3-opus-20240229']
-    model = models.CharField(max_length=50, default="claude-instant-1.2", choices=[(x, x) for x in claude_models])
+
+    model = models.CharField(max_length=50, default="claude-3-haiku-20240307", help_text="e.g. claude-3-haiku-20240307, claude-3-sonnet-20240229, claude-3-opus-20240229")
     api_key = EncryptedCharField(_("API Key"), max_length=255)
     max_tokens = models.IntegerField(default=1000)
     base_url = models.URLField(_("API URL"), default="https://api.anthropic.com")
     prompt = models.TextField(
         default="Translate only the text from the following into {target_language},only returns translations.\n{text}")
     proxy = models.URLField(_("Proxy(optional)"), null=True, blank=True, default=None)
     temperature = models.FloatField(default=0.7)
     top_p = models.FloatField(null=True, blank=True, default=0.7)
     top_k = models.IntegerField(default=1)
 
+    summary_prompt = models.TextField(default="Summarize the following text in {target_language}:\n{text}")
+
     class Meta:
         verbose_name = "Anthropic Claude"
         verbose_name_plural = "Anthropic Claude"
 
     def _init(self):
         return anthropic.Anthropic(
             api_key=self.api_key,
@@ -34,21 +36,22 @@
         if self.api_key:
             try:
                 res = self.translate("hi", "Chinese Simplified")
                 return res.get("text") != ""
             except Exception as e:
                 return False
 
-    def translate(self, text:str, target_language:str) -> dict:
+    def translate(self, text:str, target_language:str, prompt:str=None) -> dict:
         logging.info(">>> Claude Translate [%s]:", target_language)
         client = self._init()
         tokens = client.count_tokens(text)
         translated_text = ''
+        prompt = prompt or self.prompt
         try:
-            prompt = self.prompt.format(target_language=target_language, text=text)
+            prompt = prompt.format(target_language=target_language, text=text)
             res = client.messages.create(
                 model=self.model,
                 max_tokens=self.max_tokens,
                 messages=[{"role": "user", "content": prompt}],
                 temperature=self.temperature,
                 top_p=self.top_p,
                 top_k=self.top_k,
@@ -57,7 +60,11 @@
             if result[0].type == "text":
                 translated_text = result[0].text
                 tokens += res.usage.output_tokens
         except Exception as e:
             logging.error("ClaudeTranslator->%s: %s", e, text)
         finally:
             return {'text': translated_text, "tokens": tokens}
+        
+    def summarize(self, text:str, target_language:str) -> dict:
+        logging.info(">>> Claude Summarize [%s]:", target_language)
+        return self.translate(text, target_language, self.summary_prompt)
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/deepl.py` & `django_text_translator-2024.4.20/django_text_translator/models/deepl.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/deeplweb.py` & `django_text_translator-2024.4.20/django_text_translator/models/deeplweb.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/deeplx.py` & `django_text_translator-2024.4.20/django_text_translator/models/deeplx.py`

 * *Files 12% similar despite different names*

```diff
@@ -53,16 +53,19 @@
                 logging.error("DeepLXTranslator->Not support target language:%s", target_language)
 
             data = {
                 "text": text,
                 "source_lang": "auto",
                 "target_lang": target_code,
             }
+            headers = {
+              'Content-Type': 'application/json'
+            }
             post_data = json.dumps(data)
-            resp = httpx.post(url=self.deeplx_api, data=post_data, timeout=10)
+            resp = httpx.post(url=self.deeplx_api, headers=headers, data=post_data, timeout=10)
             if resp.status_code == 429:
                 raise ("DeepLXTranslator-> IP has been blocked by DeepL temporarily")
             translated_text = resp.json()["data"]
         except Exception as e:
             logging.error("DeepLXTranslator->%s: %s", e, text)
         finally:
             sleep(self.interval)
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/dev.py` & `django_text_translator-2024.4.20/django_text_translator/models/dev.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/gemini.py` & `django_text_translator-2024.4.20/django_text_translator/models/gemini.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from time import sleep
 from django.db import models
 from encrypted_model_fields.fields import EncryptedCharField
 from django.utils.translation import gettext_lazy as _
 
 class GeminiTranslator(TranslatorEngine):
     # https://ai.google.dev/tutorials/python_quickstart
-    gemini_models = ['gemini-pro','gemini-1.5-pro']
 
     # base_url = models.URLField(_("API URL"), default="https://generativelanguage.googleapis.com/v1beta/")
     api_key = EncryptedCharField(_("API Key"), max_length=255)
-    model = models.CharField(max_length=100, default="gemini-pro", choices=[(x, x) for x in gemini_models])
+    model = models.CharField(max_length=100, default="gemini-pro", help_text="e.g. gemini-pro, gemini-1.5-pro")
     prompt = models.TextField(
         default="Translate only the text from the following into {target_language},only returns translations.\n{text}")
     temperature = models.FloatField(default=0.5)
     top_p = models.FloatField(default=1)
     top_k = models.IntegerField(default=1)
     max_tokens = models.IntegerField(default=1000)
     interval = models.IntegerField(_("Request Interval(s)"), default=3)
 
+    summary_prompt = models.TextField(default="Summarize the following text in {target_language}:\n{text}")
+
+
     class Meta:
         verbose_name = "Google Gemini"
         verbose_name_plural = "Google Gemini"
 
     def _init(self):
         genai.configure(api_key=self.api_key)
         return genai.GenerativeModel(self.model)
@@ -34,21 +36,22 @@
             try:
                 model = self._init()
                 res = model.generate_content("hi")
                 return res.candidates[0].finish_reason.name == "STOP"
             except Exception as e:
                 return False
 
-    def translate(self, text:str, target_language:str) -> dict:
+    def translate(self, text:str, target_language:str, prompt:str=None) -> dict:
         logging.info(">>> Gemini Translate [%s]:", target_language)
         model = self._init()
         tokens = 0
         translated_text = ''
+        prompt = prompt or self.prompt
         try:
-            prompt = self.prompt.format(target_language=target_language, text=text)
+            prompt = prompt.format(target_language=target_language, text=text)
             generation_config = genai.types.GenerationConfig(
                 candidate_count=1,
                 temperature=self.temperature,
                 top_p=self.top_p,
                 top_k=self.top_k,
                 max_output_tokens=self.max_tokens
             )
@@ -62,8 +65,12 @@
             tokens = model.count_tokens(prompt).total_tokens
         except Exception as e:
             logging.error("GeminiTranslator->%s: %s", e, text)
         finally:
             sleep(self.interval)
 
         return {'text': translated_text, "tokens": tokens}
+    
+    def summarize(self, text:str, target_language:str) -> dict:
+        logging.info(">>> Gemini Summarize [%s]:", target_language)
+        return self.translate(text, target_language, self.summary_prompt)
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/google_translate_web.py` & `django_text_translator-2024.4.20/django_text_translator/models/google_translate_web.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/microsoft_translate.py` & `django_text_translator-2024.4.20/django_text_translator/models/microsoft_translate.py`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/moonshotai.py` & `django_text_translator-2024.4.20/django_text_translator/models/moonshotai.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,30 +3,27 @@
 import logging
 from django.db import models
 from encrypted_model_fields.fields import EncryptedCharField
 from django.utils.translation import gettext_lazy as _
 
 class MoonshotAITranslator(TranslatorEngine):
     # https://platform.moonshot.cn/docs/api-reference
-    moonshotai_models = [
-        "moonshot-v1-8k",
-        "moonshot-v1-32k",
-        "moonshot-v1-128k",
-    ]
     api_key = EncryptedCharField(_("API Key"), max_length=255)
     base_url = models.URLField(_("API URL"), default="https://api.moonshot.cn/v1")
-    model = models.CharField(max_length=100, default="moonshot-v1-8k", choices=[(x, x) for x in moonshotai_models])
+    model = models.CharField(max_length=100, default="moonshot-v1-8k",help_text="e.g. moonshot-v1-8k, moonshot-v1-32k, moonshot-v1-128k")
     prompt = models.TextField(
         default="Translate only the text from the following into {target_language},only returns translations.\n{text}")
     temperature = models.FloatField(default=0.5)
     top_p = models.FloatField(default=0.95)
     frequency_penalty = models.FloatField(default=0)
     presence_penalty = models.FloatField(default=0)
     max_tokens = models.IntegerField(default=1000)
 
+    summary_prompt = models.TextField(default="Summarize the following text in {target_language}:\n{text}")
+
     class Meta:
         verbose_name = "Moonshot AI"
         verbose_name_plural = "Moonshot AI"
 
     def _init(self):
         return OpenAI(
                     api_key=self.api_key,
@@ -43,21 +40,22 @@
                     messages=[{"role": "user", "content": 'Hi'}],
                     max_tokens=10,
                 )
                 return True
             except Exception as e:
                 return False
 
-    def translate(self, text:str, target_language:str) -> dict:
+    def translate(self, text:str, target_language:str, prompt:str=None) -> dict:
         logging.info(">>> Moonshot AI Translate [%s]:", target_language)
         client = self._init()
         tokens = 0
         translated_text = ''
+        prompt = prompt or self.prompt
         try:
-            prompt = self.prompt.format(target_language=target_language, text=text)
+            prompt = prompt.format(target_language=target_language, text=text)
             res = client.with_options(max_retries=3).chat.completions.create(
                 model=self.model,
                 messages=[{"role": "user", "content": prompt}],
                 temperature=self.temperature,
                 top_p=self.top_p,
                 frequency_penalty=self.frequency_penalty,
                 presence_penalty=self.presence_penalty,
@@ -68,8 +66,13 @@
             else:
                 translated_text = ''
                 logging.info("OpenAITranslator->%s: %s", res.choices[0].finish_reason, text)
             tokens = res.usage.total_tokens
         except Exception as e:
             logging.error("OpenAITranslator->%s: %s", e, text)
 
-        return {'text': translated_text, "tokens": tokens}
+        return {'text': translated_text, "tokens": tokens}
+
+    def summarize(self, text:str, target_language:str) -> dict:
+        logging.info(">>> Moonshot AI Summarize [%s]:", target_language)
+        return self.translate(text, target_language, self.summary_prompt)
+
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/models/openai.py` & `django_text_translator-2024.4.20/django_text_translator/models/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,37 @@
 from django.db import models
 from encrypted_model_fields.fields import EncryptedCharField
 from django.utils.translation import gettext_lazy as _
 
 
 class OpenAITranslator(TranslatorEngine):
     # https://platform.openai.com/docs/api-reference/chat
-    openai_models = [
-        "gpt-3.5-turbo",
-        "gpt-4-turbo-preview",
-    ]
 
     api_key = EncryptedCharField(_("API Key"), max_length=255)
     base_url = models.URLField(_("API URL"), default="https://api.openai.com/v1")
-    model = models.CharField(max_length=100, default="gpt-3.5-turbo", choices=[(x, x) for x in openai_models])
+    model = models.CharField(max_length=100, default="gpt-3.5-turbo", help_text="e.g. gpt-3.5-turbo, gpt-4-turbo")
     prompt = models.TextField(
         default="Translate only the text from the following into {target_language},only returns translations.\n{text}")
     temperature = models.FloatField(default=0.5)
     top_p = models.FloatField(default=0.95)
     frequency_penalty = models.FloatField(default=0)
     presence_penalty = models.FloatField(default=0)
     max_tokens = models.IntegerField(default=1000)
 
+    summary_prompt = models.TextField(default="Summarize the following text in {target_language}:\n{text}")
+
     class Meta:
         verbose_name = "OpenAI"
         verbose_name_plural = "OpenAI"
 
     def _init(self):
         return OpenAI(
                     api_key=self.api_key,
                     base_url = self.base_url,
-                    timeout=180.0,
+                    timeout=120.0,
                 )
 
     def validate(self) -> bool:
         if self.api_key:
             try:
                 client = self._init()
                 res = client.with_options(max_retries=3).chat.completions.create(
@@ -46,21 +44,22 @@
                 )
                 fr = res.choices[0].finish_reason # 有些第三方源在key或url错误的情况下，并不会抛出异常代码，而是返回html广告，因此添加该行。
                 logging.info(">>> OpenAI Translate Validate:%s",fr)
                 return True
             except Exception as e:
                 return False
 
-    def translate(self, text:str, target_language:str) -> dict:
+    def translate(self, text:str, target_language:str, prompt:str=None) -> dict:
         logging.info(">>> OpenAI Translate [%s]:", target_language)
         client = self._init()
         tokens = 0
         translated_text = ''
+        prompt = prompt or self.prompt
         try:
-            prompt = self.prompt.format(target_language=target_language, text=text)
+            prompt = prompt.format(target_language=target_language, text=text)
             res = client.with_options(max_retries=3).chat.completions.create(
                 model=self.model,
                 messages=[{"role": "user", "content": prompt}],
                 temperature=self.temperature,
                 top_p=self.top_p,
                 frequency_penalty=self.frequency_penalty,
                 presence_penalty=self.presence_penalty,
@@ -72,7 +71,11 @@
                 translated_text = ''
                 logging.info("OpenAITranslator->%s: %s", res.choices[0].finish_reason, text)
             tokens = res.usage.total_tokens
         except Exception as e:
             logging.error("OpenAITranslator->%s: %s", e, text)
 
         return {'text': translated_text, "tokens": tokens}
+    
+    def summarize(self, text:str, target_language:str) -> dict:
+        logging.info(">>> OpenAI Summarize [%s]:", target_language)
+        return self.translate(text, target_language, self.summary_prompt)
```

### Comparing `django_text_translator-2024.4.2.1/django_text_translator/static/img/icon-loading.svg` & `django_text_translator-2024.4.20/django_text_translator/static/img/icon-loading.svg`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/LICENSE` & `django_text_translator-2024.4.20/LICENSE`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/README.md` & `django_text_translator-2024.4.20/README.md`

 * *Files identical despite different names*

### Comparing `django_text_translator-2024.4.2.1/pyproject.toml` & `django_text_translator-2024.4.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["./"]
 
 [project]
 name = "django-text-translator"
-version = "2024.4.2.1"
+version = "2024.4.20"
 authors = [
   { name="Versun", email="django-text-translator@versun.me" },
 ]
 description = "A Django application that supports adding multiple third-party engines for text translation."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT License"}
```

### Comparing `django_text_translator-2024.4.2.1/PKG-INFO` & `django_text_translator-2024.4.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-text-translator
-Version: 2024.4.2.1
+Version: 2024.4.20
 Summary: A Django application that supports adding multiple third-party engines for text translation.
 Project-URL: Homepage, https://github.com/rss-translator/django-text-translator
 Project-URL: Repository, https://github.com/rss-translator/django-text-translator.git
 Project-URL: Issues, https://github.com/rss-translator/django-text-translator/issues
 Author-email: Versun <django-text-translator@versun.me>
 License: MIT License
 License-File: LICENSE
```

