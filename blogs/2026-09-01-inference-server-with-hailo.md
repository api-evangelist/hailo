---
title: "Inference Server with Hailo"
url: "https://community.hailo.ai/t/inference-server-with-hailo/19711#post_2"
date: "2026-09-01"
author: "@Eldad_Rubinstein"
feed_url: "https://community.hailo.ai/posts.rss"
---
It’s hard to tell without the full details on the application, video resolution, analytics FPS, analytics pipeline, and so on. Under a lightweight application assumption that the only AI model is a small detector like yolov8n running at 10 FPS per stream, each Hailo-8 runs at >1000FPS, so it can even handle 100 streams. Choosing a bigger detector such as yolov5m will result in 242/10=24 streams per Hailo device.
