---
title: "DFC 3.33: silent 16-bit output demotion produces inconsistent HEFs (runtime demux errors / stale dequantization params)"
url: "https://community.hailo.ai/t/dfc-3-33-silent-16-bit-output-demotion-produces-inconsistent-hefs-runtime-demux-errors-stale-dequantization-params/19705#post_1"
date: "2026-08-27"
author: "@Toshiyuki_Yasui"
feed_url: "https://community.hailo.ai/posts.rss"
---
## Environment - Hailo AI SW Suite 2025-10 (DFC 3.33.0), HailoRT 4.23.0, Hailo-8 (Raspberry Pi 5 + AI HAT) - SSD-style model, 12 output layers (6 scales × cls/loc), all end nodes are plain convs ## Summary When requesting 16-bit outputs, the optimizer applies the request correctly, but the **compiler silently demotes some outputs back to 8-bit** , and the resulting HEFs are internally inconsistent in two different ways depending on how the request was written. There is no warning at any point; the compile reports success. ## Fact 1: optimize stage is fine With `quantization_param(output_layerN
