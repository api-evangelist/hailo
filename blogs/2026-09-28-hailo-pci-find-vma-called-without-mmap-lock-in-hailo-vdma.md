---
title: "hailo_pci: find_vma() called without mmap_lock in hailo_vdma_buffer_map()— kernel warning storm and hard crash under sustained inference"
url: "https://community.hailo.ai/t/hailo-pci-find-vma-called-without-mmap-lock-in-hailo-vdma-buffer-map-kernel-warning-storm-and-hard-crash-under-sustained-inference/19635#post_2"
date: "2026-09-28"
author: "@Jesus_Royeth"
feed_url: "https://community.hailo.ai/posts.rss"
---
We ran into the same issue on a production counting system (Hailo-8, hailo_pci 4.23.0). The trigger was the same pattern you describe: allocation churn in the inference process. For us it came from clients connecting to and disconnecting from an MJPEG/HTTP video stream served by that process.
