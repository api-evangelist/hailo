---
title: "I compiled an LLM for the hailo-10h"
url: "https://community.hailo.ai/t/i-compiled-an-llm-for-the-hailo-10h/19685#post_1"
date: "2026-08-24"
author: "@Leo_Nonnenmacher"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi everyone, I’d like to share hailo-10h-llm-compiler , an open-source (MIT) project that compiles your own Hugging Face LLM into a self-contained HEF for the Hailo-10H, served with hailo-ollama — no model-zoo HEF required. It drives the Dataflow Compiler’s LLM flow ( set_kv_cache_global_params , prefill + token-by-token network groups, KV-cache quantization) as a six-step pipeline: ONNX export → HAR parse → graph surgery → INT4/INT8 quantization → HEF compile → registration into hailo-ollama’s model store. The compiler itself is not redistributed — you obtain it from Hailo’s developer portal;
