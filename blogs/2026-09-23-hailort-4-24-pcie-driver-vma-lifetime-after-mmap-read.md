---
title: "HailoRT 4.24 PCIe driver: VMA lifetime after mmap_read_unlock() in hailo_vdma_buffer_map()"
url: "https://community.hailo.ai/t/hailort-4-24-pcie-driver-vma-lifetime-after-mmap-read-unlock-in-hailo-vdma-buffer-map/19785#post_1"
date: "2026-09-23"
author: "@Robert_Young"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi, I’m preparing to upgrade a Raspberry Pi 5 with a Hailo-8 from HailoRT/PCIe driver 4.23.0 to the official HailoRT 4.24.0 ARM64 packages from the Hailo Developer Zone. System details: Raspberry Pi 5, ARM64 Raspberry Pi OS / Debian 13 (Trixie) Kernel: 6.18.50+rpt-rpi-2712 Accelerator: Hailo-8 Current HailoRT/PCIe driver/firmware: 4.23.0 Proposed upgrade: HailoRT/PCIe driver/firmware 4.24.0 With 4.23.0, hardware inference works, but it produces kernel WARN traces involving find_vma() from hailo_vdma_buffer_map() . I understand this is a known issue in 4.23 related to calling find_vma() without
