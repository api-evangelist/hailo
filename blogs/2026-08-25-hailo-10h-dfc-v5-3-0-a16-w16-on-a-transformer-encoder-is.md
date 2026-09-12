---
title: "Hailo-10H / DFC v5.3.0: a16_w16 on a transformer encoder is not a blanket allocator wall — it's a 3-stage cascade (attention crash → a16-conv nan exponent → needs super-defuse). What is the intended 16-bit path?"
url: "https://community.hailo.ai/t/hailo-10h-dfc-v5-3-0-a16-w16-on-a-transformer-encoder-is-not-a-blanket-allocator-wall-its-a-3-stage-cascade-attention-crash-a16-conv-nan-exponent-needs-super-defuse-what-is-the-intended-16-bit-path/19530#post_4"
date: "2026-08-25"
author: "@Leo_Nonnenmacher"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi Fernando — this is genuinely useful, thanks for going through the repo and reporting back in such detail. On your direct question : no, I haven’t gotten a16 through the attention block either. My own a16_w16 usage is limited to input_layer1 (the embedding input, far from attention — matches what you saw) and ew_add* layers on the encoder recipe.
