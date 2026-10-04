---
title: "Deploying an externally QAT-trained ONNX Q/DQ model on Hailo-8"
url: "https://community.hailo.ai/t/deploying-an-externally-qat-trained-onnx-q-dq-model-on-hailo-8/19782#post_1"
date: "2026-09-23"
author: "@Julius_Palsherm"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi everyone, I would like to deploy a quantization-aware-trained model on Hailo-8 using DFC 3.34.0 . I’m trying to understand whether the quantization established during training can be preserved, and what deployment workflow Hailo recommends. Training Setup My TensorFlow/Keras 3 training setup supports QAT using TensorFlow’s fake-quantization operations: Training maintains floating-point weights while simulating 8-bit quantization during the forward pass, with straight-through gradient estimation.
