---
title: "Error when compiling model with deconvolution"
url: "https://community.hailo.ai/t/error-when-compiling-model-with-deconvolution/18177#post_6"
date: "2026-08-27"
author: "@Toshiyuki_Yasui"
feed_url: "https://community.hailo.ai/posts.rss"
---
We hit what appears to be the same issue, and we managed to isolate it to a **minimal, shareable reproduction** . Posting our findings here in case it helps. ## Environment - Hailo AI SW Suite 2025-10 (DFC 3.33.0), HailoRT 4.23.0 - Device: Hailo-8 (Raspberry Pi 5 + AI HAT), driver/firmware matching 4.23.0 - Compilation on x86_64 Ubuntu 20.04 (Docker suite container) ## Symptom (production model) SSD-style detector with a MobileNetV3 backbone and an FPN-like top-down path using three chained `ConvTranspose` layers (kernel 2x2, stride 2, pad 0; e.g.
