---
title: "Hailo-8 vs Hailo-8L: YOLOv11s inference latency only improves from ~19 ms to ~13 ms"
url: "https://community.hailo.ai/t/hailo-8-vs-hailo-8l-yolov11s-inference-latency-only-improves-from-19-ms-to-13-ms/19745#post_2"
date: "2026-09-09"
author: "@Klaus_Koschinsky"
feed_url: "https://community.hailo.ai/posts.rss"
---
The performance difference between running a model on the Hailo-8 and Hailo-8L can vary widely depending on the limiting factors. For example, a model that fits well within a single context on the Hailo-8 but requires multiple contexts on the Hailo-8L could potentially run 10× faster on the Hailo-8. On the other hand, a small model may run at roughly the same speed on both devices if the Dataflow Compiler cannot take advantage of the Hailo-8’s additional hardware resources.
