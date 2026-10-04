---
title: "[HailoRT] [error] CHECK_SUCCESS failed with status=HAILO_DRIVER_OPERATION_FAILED(36)"
url: "https://community.hailo.ai/t/hailort-error-check-success-failed-with-status-hailo-driver-operation-failed-36/19794#post_1"
date: "2026-09-25"
author: "@Hardhik_Chinthan"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hailo‑10H on RK3588 (OrangePi 5 Max): device wedges with HAILO_VDMA_LAUNCH_TRANSFER failed with 5, PCIe link drops 8.0 → 2.5 GT/s, only a PCI remove/rescan recovers it. On an OrangePi 5 Max (RK3588), a Hailo‑10H M.2 module wedges within ~20 seconds of a real application starting inference. The kernel logs Failed to launch transfer, userspace gets HAILO_DRIVER_OPERATION_FAILED(36), and the PCIe link retrains down from 8.0 GT/s to 2.5 GT/s.
