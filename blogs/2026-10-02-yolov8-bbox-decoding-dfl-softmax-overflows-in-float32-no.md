---
title: "YOLOv8 bbox decoding: DFL softmax overflows in float32 (no max-subtraction), producing NaN boxes"
url: "https://community.hailo.ai/t/yolov8-bbox-decoding-dfl-softmax-overflows-in-float32-no-max-subtraction-producing-nan-boxes/19815#post_1"
date: "2026-10-02"
author: "@Simon_Hagerlind"
feed_url: "https://community.hailo.ai/posts.rss"
---
Summary The CPU YOLOv8 post-process ( nms_postprocess(..., meta_arch=yolov8, engine=cpu) , also with bbox_decoding_only=True ) decodes each box side with a softmax over the 16 DFL bins. The softmax computes exp(x) in float32 without subtracting the max first. When a dequantized regression logit exceeds about 88.72 (= ln FLT_MAX), exp overflows to +inf , the normalisation becomes inf / inf , and the decoded box coordinates are NaN .
