# Comparing `tmp/langtrace_python_sdk-2.0.1.tar.gz` & `tmp/langtrace_python_sdk-2.0.2.tar.gz`

## Comparing `langtrace_python_sdk-2.0.1.tar` & `langtrace_python_sdk-2.0.2.tar`

### file list

```diff
@@ -1,122 +1,130 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    25572 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    36773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/conftest.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/LICENSE
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    25572 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    36773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/LICENSE
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.2/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.1/src/run_example.py` & `langtrace_python_sdk-2.0.2/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.2/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.2/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.0.2/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.2/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.0.2/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.0.2/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.0.2/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.2/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.2/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.0.2/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.0.2/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.2/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.2/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.2/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.0.2/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.0.2/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.0.2/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/langtrace.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 from langtrace.trace_attributes import Event, LLMSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.cohere import APIS
 from langtrace_python_sdk.constants.instrumentation.common import (
-    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY, SERVICE_PROVIDERS)
+    LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
+    SERVICE_PROVIDERS,
+)
 
 
 def rerank(original_method, version, tracer):
     """Wrap the `rerank` method."""
 
     def traced_method(wrapped, instance, args, kwargs):
         service_provider = SERVICE_PROVIDERS["COHERE"]
@@ -99,17 +101,15 @@
                             ),
                             "search_units": (
                                 usage.search_units
                                 if usage.search_units is not None
                                 else 0
                             ),
                         }
-                        span.set_attribute(
-                            "llm.token.counts", json.dumps(usage_dict)
-                        )
+                        span.set_attribute("llm.token.counts", json.dumps(usage_dict))
 
             span.set_status(StatusCode.OK)
             span.end()
             return result
 
         except Exception as error:
             span.record_exception(error)
@@ -183,17 +183,15 @@
                             ),
                             "search_units": (
                                 usage.search_units
                                 if usage.search_units is not None
                                 else 0
                             ),
                         }
-                        span.set_attribute(
-                            "llm.token.counts", json.dumps(usage_dict)
-                        )
+                        span.set_attribute("llm.token.counts", json.dumps(usage_dict))
 
             span.set_status(StatusCode.OK)
             span.end()
             return result
 
         except Exception as error:
             span.record_exception(error)
@@ -222,17 +220,15 @@
         if chat_history:
             history = [
                 {
                     "role": (
                         item.get("role") if item.get("role") is not None else "USER"
                     ),
                     "content": (
-                        item.get("message")
-                        if item.get("message") is not None
-                        else ""
+                        item.get("message") if item.get("message") is not None else ""
                     ),
                 }
                 for item in chat_history
             ]
         if len(history) > 0:
             prompts = history + prompts
         if len(system_prompts) > 0:
@@ -308,41 +304,42 @@
                 span.set_attribute("llm.response_id", result.response_id)
             if (hasattr(result, "is_search_required")) and (
                 result.is_search_required is not None
             ):
                 span.set_attribute("llm.is_search_required", result.is_search_required)
 
             if kwargs.get("stream") is False or kwargs.get("stream") is None:
-                if hasattr(result, "text") and result.text is not None and result.text != "":
+                if (
+                    hasattr(result, "text")
+                    and result.text is not None
+                    and result.text != ""
+                ):
                     if (
                         hasattr(result, "chat_history")
                         and result.chat_history is not None
                     ):
                         responses = [
                             {
                                 "role": (
                                     item.role
-                                    if hasattr(item, "role")
-                                    and item.role is not None
+                                    if hasattr(item, "role") and item.role is not None
                                     else "USER"
                                 ),
                                 "content": (
                                     item.message
                                     if hasattr(item, "message")
                                     and item.message is not None
                                     else ""
                                 ),
                             }
                             for item in result.chat_history
                         ]
                         span.set_attribute("llm.responses", json.dumps(responses))
                     else:
-                        responses = [
-                            {"role": "CHATBOT", "content": result.text}
-                        ]
+                        responses = [{"role": "CHATBOT", "content": result.text}]
                         span.set_attribute("llm.responses", json.dumps(responses))
                 elif hasattr(result, "tool_calls") and result.tool_calls is not None:
                     tool_calls = []
                     for tool_call in result.tool_calls:
                         tool_calls.append(tool_call.json())
                     span.set_attribute("llm.tool_calls", json.dumps(tool_calls))
                     span.set_attribute("llm.responses", json.dumps([]))
@@ -418,17 +415,15 @@
         if chat_history:
             history = [
                 {
                     "role": (
                         item.get("role") if item.get("role") is not None else "USER"
                     ),
                     "content": (
-                        item.get("message")
-                        if item.get("message") is not None
-                        else ""
+                        item.get("message") if item.get("message") is not None else ""
                     ),
                 }
                 for item in chat_history
             ]
         if len(history) > 0:
             prompts = history + prompts
         if len(system_prompts) > 0:
@@ -481,15 +476,15 @@
         if kwargs.get("tools") is not None:
             # stringify the list of objects
             attributes.llm_tools = json.dumps(kwargs.get("tools"))
         if kwargs.get("tool_results") is not None:
             # stringify the list of objects
             attributes.llm_tool_results = json.dumps(kwargs.get("tool_results"))
 
-        span = tracer.start_span(APIS["CHAT_CREATE"]["METHOD"], kind=SpanKind.CLIENT)
+        span = tracer.start_span(APIS["CHAT_STREAM"]["METHOD"], kind=SpanKind.CLIENT)
         for field, value in attributes.model_dump(by_alias=True).items():
             if value is not None:
                 span.set_attribute(field, value)
         try:
             # Attempt to call the original method
             result = wrapped(*args, **kwargs)
             span.add_event(Event.STREAM_START.value)
@@ -499,27 +494,36 @@
                         content = event.text
                     else:
                         content = ""
                     span.add_event(
                         Event.STREAM_OUTPUT.value, {"response": "".join(content)}
                     )
 
-                    if hasattr(event, "finish_reason") and event.finish_reason == "COMPLETE":
+                    if (
+                        hasattr(event, "finish_reason")
+                        and event.finish_reason == "COMPLETE"
+                    ):
                         response = event.response
 
                         if (hasattr(response, "generation_id")) and (
                             response.generation_id is not None
                         ):
-                            span.set_attribute("llm.generation_id", response.generation_id)
-                        if (hasattr(response, "response_id")) and (response.response_id is not None):
+                            span.set_attribute(
+                                "llm.generation_id", response.generation_id
+                            )
+                        if (hasattr(response, "response_id")) and (
+                            response.response_id is not None
+                        ):
                             span.set_attribute("llm.response_id", response.response_id)
                         if (hasattr(response, "is_search_required")) and (
                             response.is_search_required is not None
                         ):
-                            span.set_attribute("llm.is_search_required", response.is_search_required)
+                            span.set_attribute(
+                                "llm.is_search_required", response.is_search_required
+                            )
 
                         # Set the response attributes
                         if hasattr(response, "text") and response.text is not None:
                             if (
                                 hasattr(response, "chat_history")
                                 and response.chat_history is not None
                             ):
@@ -536,20 +540,24 @@
                                             if hasattr(item, "message")
                                             and item.message is not None
                                             else ""
                                         ),
                                     }
                                     for item in response.chat_history
                                 ]
-                                span.set_attribute("llm.responses", json.dumps(responses))
+                                span.set_attribute(
+                                    "llm.responses", json.dumps(responses)
+                                )
                             else:
                                 responses = [
                                     {"role": "CHATBOT", "content": response.text}
                                 ]
-                                span.set_attribute("llm.responses", json.dumps(responses))
+                                span.set_attribute(
+                                    "llm.responses", json.dumps(responses)
+                                )
 
                         # Get the usage
                         if hasattr(response, "meta") and response.meta is not None:
                             if (
                                 hasattr(response.meta, "billed_units")
                                 and response.meta.billed_units is not None
                             ):
```

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.0.2/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.0.2/src/tests/anthropic/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,10 +29,7 @@
 def vcr_config():
     return {"filter_headers": ["authorization", "x-api-key"]}
 
 
 @pytest.fixture(scope="session", autouse=True)
 def instrument():
     AnthropicInstrumentation().instrument()
-
-    yield
-    # exporter.shutdown()
```

### Comparing `langtrace_python_sdk-2.0.1/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.2/src/tests/openai/test_chat_completion.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,152 @@
 import pytest
-import json
 import importlib
-from langtrace_python_sdk.constants.instrumentation.anthropic import APIS
+import json
+from langtrace_python_sdk.constants.instrumentation.openai import APIS
+from tests.utils import assert_response_format, assert_token_count
 
 
 @pytest.mark.vcr()
-def test_anthropic(anthropic_client, exporter):
-    llm_model_value = "claude-3-opus-20240229"
-    messages_value = [{"role": "user", "content": "How are you today?"}]
+def test_chat_completion(exporter, openai_client):
+    llm_model_value = "gpt-4"
+    messages_value = [{"role": "user", "content": "Say this is a test three times"}]
 
     kwargs = {
         "model": llm_model_value,
         "messages": messages_value,
-        # "system": "Respond only in Yoda-speak.",
         "stream": False,
-        "max_tokens": 1024,
     }
-    response = anthropic_client.messages.create(**kwargs)
+
+    openai_client.chat.completions.create(**kwargs)
     spans = exporter.get_finished_spans()
     completion_span = spans[-1]
+    assert completion_span.name == "openai.chat.completions.create"
 
-    assert completion_span.name == "anthropic.messages.create"
     attributes = completion_span.attributes
-
     assert attributes.get("langtrace.sdk.name") == "langtrace-python-sdk"
-    assert attributes.get("langtrace.service.name") == "Anthropic"
+    assert attributes.get("langtrace.service.name") == "OpenAI"
     assert attributes.get("langtrace.service.type") == "llm"
     assert attributes.get("langtrace.service.version") == importlib.metadata.version(
-        "anthropic"
+        "openai"
     )
     assert attributes.get("langtrace.version") == "1.0.0"
-    assert attributes.get("url.full") == "https://api.anthropic.com"
-    assert attributes.get("llm.api") == APIS["MESSAGES_CREATE"]["ENDPOINT"]
-    assert attributes.get("llm.model") == llm_model_value
+    assert attributes.get("url.full") == "https://api.openai.com/v1/"
+    assert attributes.get("llm.api") == APIS["CHAT_COMPLETION"]["ENDPOINT"]
+    assert attributes.get("llm.model") == "gpt-4-0613"
     assert attributes.get("llm.prompts") == json.dumps(messages_value)
     assert attributes.get("llm.stream") is False
 
-    tokens = json.loads(attributes.get("llm.token.counts"))
-    output_tokens = tokens.get("output_tokens")
-    prompt_tokens = tokens.get("input_tokens")
-    total_tokens = tokens.get("total_tokens")
+    assert_token_count(attributes)
+    assert_response_format(attributes)
 
-    assert output_tokens and prompt_tokens and total_tokens
-    assert output_tokens + prompt_tokens == total_tokens
+    langtrace_responses = json.loads(attributes.get("llm.responses"))
+    assert isinstance(langtrace_responses, list)
+    for langtrace_response in langtrace_responses:
+        assert isinstance(langtrace_response, dict)
+        assert "role" in langtrace_response
+        assert "content" in langtrace_response
 
     langtrace_responses = json.loads(attributes.get("llm.responses"))
     assert isinstance(langtrace_responses, list)
     for langtrace_response in langtrace_responses:
         assert isinstance(langtrace_response, dict)
         assert "role" in langtrace_response
         assert "content" in langtrace_response
 
 
 @pytest.mark.vcr()
-def test_anthropic_streaming(anthropic_client, exporter):
-    llm_model_value = "claude-3-opus-20240229"
-    messages_value = [{"role": "user", "content": "How are you today?"}]
+def test_chat_completion_streaming(exporter, openai_client):
+    llm_model_value = "gpt-4"
+    messages_value = [{"role": "user", "content": "Say this is a test three times"}]
 
     kwargs = {
         "model": llm_model_value,
         "messages": messages_value,
-        # "system": "Respond only in Yoda-speak.",
         "stream": True,
-        "max_tokens": 1024,
     }
-    response = anthropic_client.messages.create(**kwargs)
-    chunk_count = 0
 
-    for chunk in response:
-        if chunk:
-            chunk_count += 1
+    response = openai_client.chat.completions.create(**kwargs)
+    chunk_count = 0
+    for _ in response:
+        chunk_count += 1
 
     spans = exporter.get_finished_spans()
     streaming_span = spans[-1]
 
-    assert streaming_span.name == "anthropic.messages.create"
+    assert streaming_span.name == "openai.chat.completions.create"
     attributes = streaming_span.attributes
 
     assert attributes.get("langtrace.sdk.name") == "langtrace-python-sdk"
-    assert attributes.get("langtrace.service.name") == "Anthropic"
+    assert attributes.get("langtrace.service.name") == "OpenAI"
     assert attributes.get("langtrace.service.type") == "llm"
     assert attributes.get("langtrace.service.version") == importlib.metadata.version(
-        "anthropic"
+        "openai"
     )
     assert attributes.get("langtrace.version") == "1.0.0"
-    assert attributes.get("url.full") == "https://api.anthropic.com"
-    assert attributes.get("llm.api") == APIS["MESSAGES_CREATE"]["ENDPOINT"]
-    assert attributes.get("llm.model") == llm_model_value
+    assert attributes.get("url.full") == "https://api.openai.com/v1/"
+    assert attributes.get("llm.api") == APIS["CHAT_COMPLETION"]["ENDPOINT"]
+    assert attributes.get("llm.model") == "gpt-4-0613"
     assert attributes.get("llm.prompts") == json.dumps(messages_value)
     assert attributes.get("llm.stream") is True
-    events = streaming_span.events
 
+    events = streaming_span.events
     assert len(events) - 2 == chunk_count  # -2 for start and end events
 
-    tokens = json.loads(attributes.get("llm.token.counts"))
-    output_tokens = tokens.get("output_tokens")
-    prompt_tokens = tokens.get("input_tokens")
-    total_tokens = tokens.get("total_tokens")
+    assert_token_count(attributes)
+    assert_response_format(attributes)
 
-    assert output_tokens and prompt_tokens and total_tokens
-    assert output_tokens + prompt_tokens == total_tokens
+    langtrace_responses = json.loads(attributes.get("llm.responses"))
+    assert isinstance(langtrace_responses, list)
+    for langtrace_response in langtrace_responses:
+        assert isinstance(langtrace_response, dict)
+        assert "role" in langtrace_response
+        assert "content" in langtrace_response
 
     langtrace_responses = json.loads(attributes.get("llm.responses"))
     assert isinstance(langtrace_responses, list)
     for langtrace_response in langtrace_responses:
         assert isinstance(langtrace_response, dict)
         assert "role" in langtrace_response
         assert "content" in langtrace_response
+
+
+@pytest.mark.vcr()
+@pytest.mark.asyncio()
+async def test_async_chat_completion_streaming(exporter, async_openai_client):
+    llm_model_value = "gpt-4"
+    messages_value = [{"role": "user", "content": "Say this is a test three times"}]
+
+    kwargs = {
+        "model": llm_model_value,
+        "messages": messages_value,
+        "stream": True,
+    }
+
+    response = await async_openai_client.chat.completions.create(**kwargs)
+    chunk_count = 0
+    async for _ in response:
+        chunk_count += 1
+
+    spans = exporter.get_finished_spans()
+    streaming_span = spans[-1]
+
+    assert streaming_span.name == "openai.chat.completions.create"
+    attributes = streaming_span.attributes
+
+    assert attributes.get("langtrace.sdk.name") == "langtrace-python-sdk"
+    assert attributes.get("langtrace.service.name") == "OpenAI"
+    assert attributes.get("langtrace.service.type") == "llm"
+    assert attributes.get("langtrace.service.version") == importlib.metadata.version(
+        "openai"
+    )
+    assert attributes.get("langtrace.version") == "1.0.0"
+    assert attributes.get("url.full") == "https://api.openai.com/v1/"
+    assert attributes.get("llm.api") == APIS["CHAT_COMPLETION"]["ENDPOINT"]
+    assert attributes.get("llm.model") == "gpt-4-0613"
+    assert attributes.get("llm.prompts") == json.dumps(messages_value)
+    assert attributes.get("llm.stream") is True
+
+    events = streaming_span.events
+    assert len(events) - 2 == chunk_count  # -2 for start and end events
+
+    assert_token_count(attributes)
+    assert_response_format(attributes)
```

### Comparing `langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.0.2/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.2/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.2/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.2/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.2/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.0.2/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.2/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.0.2/src/tests/openai/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,10 +28,7 @@
 def vcr_config():
     return {"filter_headers": ["authorization", "api-key"]}
 
 
 @pytest.fixture(scope="session", autouse=True)
 def instrument():
     OpenAIInstrumentation().instrument()
-
-    yield
-    # exporter.shutdown()
```

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.2/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.2/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.0.2/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/.gitignore` & `langtrace_python_sdk-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/LICENSE` & `langtrace_python_sdk-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/README.md` & `langtrace_python_sdk-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/pyproject.toml` & `langtrace_python_sdk-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.1/PKG-INFO` & `langtrace_python_sdk-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

