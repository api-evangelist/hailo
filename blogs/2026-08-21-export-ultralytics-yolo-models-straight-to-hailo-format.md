---
title: "Export Ultralytics YOLO models straight to Hailo (format=\"hailo\") is now available"
url: "https://community.hailo.ai/t/export-ultralytics-yolo-models-straight-to-hailo-format-hailo-is-now-available/19678#post_5"
date: "2026-08-21"
author: "@Eldad_Rubinstein"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi @Jesus_Royeth , Thanks for your Hailo-related contribution to the Ultralytics repository. Please see here the accuracy reached by the Hailo Model Zoo: Hailo-8: hailo_model_zoo/docs/public_models/HAILO8/HAILO8_object_detection.rst at master · hailo-ai/hailo_model_zoo · GitHub Hailo-10H: hailo_model_zoo/docs/public_models/HAILO10H/HAILO10H_object_detection.rst at master · hailo-ai/hailo_model_zoo · GitHub On the gap: I think the key point is that the recipe is more than the 16-bit change. The version proposed in #25687 (later reverted in #25728 as too model-specific) changes several .alls con
