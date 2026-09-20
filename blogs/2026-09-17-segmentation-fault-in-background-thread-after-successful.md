---
title: "Segmentation fault in background thread after successful synchronous inference (VStreams API), Hailo-8, HailoRT 4.24.0"
url: "https://community.hailo.ai/t/segmentation-fault-in-background-thread-after-successful-synchronous-inference-vstreams-api-hailo-8-hailort-4-24-0/19764#post_1"
date: "2026-09-17"
author: "@Egor_Sorokin"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi, I’m hitting a 100% reproducible segfault on Hailo-8 with a simple synchronous single-shot inference script (load one HEF, configure, send one frame, receive outputs, exit). The output is computed and written to disk correctly, print() calls after inference execute fine — but the process still crashes with SIGSEGV afterward, in a background thread HailoRT spawns internally (~40-50 threads for a single synchronous call). Environment HailoRT: 4.24.0 ( hailortcli --version and pip show hailort both confirm) Firmware: 4.24.0 (release,app,extended context switch buffer) Device: HAILO-8 AI ACC M.
