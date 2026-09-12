---
title: "Is host-CPU NMS generally faster than on-core NMS for lightweight detectors on Hailo-8L? (end-to-end pipeline FPS, not just NPU throughput)"
url: "https://community.hailo.ai/t/is-host-cpu-nms-generally-faster-than-on-core-nms-for-lightweight-detectors-on-hailo-8l-end-to-end-pipeline-fps-not-just-npu-throughput/19687#post_3"
date: "2026-08-25"
author: "@jungmin_jeon"
feed_url: "https://community.hailo.ai/posts.rss"
---
Thanks for the detailed breakdown — this clears up a lot. You’re right that I was treating yolov5xs_wo_spp vs yolov5xs_wo_spp_nms_core as a clean “same model, NMS moved on/off core” comparison, when it’s actually two different checkpoints with very different NMS configs (0.20/0.60/80 vs 0.01/0.45/800) plus a different context count (2 vs 3). So the 2.3–3.6x gap I measured isn’t isolating NMS placement at all — it’s conflating that with a ~10x bigger NMS workload and whatever the extra context switch costs.
