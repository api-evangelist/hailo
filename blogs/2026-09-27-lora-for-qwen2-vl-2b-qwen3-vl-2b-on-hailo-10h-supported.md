---
title: "LoRA for Qwen2-VL-2B / Qwen3-VL-2B on Hailo-10H — supported? (+ logits access in GenAI VLM API)"
url: "https://community.hailo.ai/t/lora-for-qwen2-vl-2b-qwen3-vl-2b-on-hailo-10h-supported-logits-access-in-genai-vlm-api/19801#post_1"
date: "2026-09-27"
author: "@Sangwon_Byun"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi all, I’m a university researcher building an on-device assistive system for blind pedestrians (Raspberry Pi 5 + Hailo-10H): the user speaks a destination, and a VLM reads indoor wayfinding signs and returns only the direction for that destination as one label out of 14 fixed classes. From this thread ( Is there a documented flow for compiling a custom/fine-tuned LLM to the Hailo-10H LLM pipeline? ) I understand that compiling your own LLM is not possible yet, but LoRA on supported models is.
