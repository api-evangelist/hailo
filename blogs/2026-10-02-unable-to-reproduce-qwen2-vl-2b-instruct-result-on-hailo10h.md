---
title: "Unable to reproduce Qwen2-VL-2B-Instruct result on Hailo10H"
url: "https://community.hailo.ai/t/unable-to-reproduce-qwen2-vl-2b-instruct-result-on-hailo10h/19821#post_1"
date: "2026-10-02"
author: "@Jeffery_Hsu"
feed_url: "https://community.hailo.ai/posts.rss"
---
Dear Hailo Community, I am trying to reproduce this example from Hugging Face using Qwen2-VL-2B-Instruct for zero-shot object detection. I modified the simple_vlm_chat example from Hailo-apps and fed the API the same prompts and images as the HuggingFace example . prompt = [ { "role": "user", "content": [ {"type": "image"}, {"type": "text", "text": 'You are a helpfull assistant to detect objects in images.
