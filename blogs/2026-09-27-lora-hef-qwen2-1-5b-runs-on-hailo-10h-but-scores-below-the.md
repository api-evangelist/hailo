---
title: "LoRA HEF (Qwen2-1.5B) runs on Hailo-10H but scores below the base model (100% on GPU, 39% on device)"
url: "https://community.hailo.ai/t/lora-hef-qwen2-1-5b-runs-on-hailo-10h-but-scores-below-the-base-model-100-on-gpu-39-on-device/19798#post_1"
date: "2026-09-27"
author: "@Boris_Pavelka"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi, I’ve been trying to get a small LoRA adapter running on a Raspberry Pi 5 with the AI HAT+ 2, following DFC_7_LoRA_Tutorial pretty much to the letter. The good part is the whole thing works end to end: the HEF compiles, loads, and generates text. The bad part is that on the device the adapter makes the model worse than no adapter at all, and I’ve run out of things to check on my side.
