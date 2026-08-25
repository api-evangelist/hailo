---
title: "DFC 3.34.0 / Hailo-8L — Compiler SIGABRT on fixed selection-matrix matmuls"
url: "https://community.hailo.ai/t/dfc-3-34-0-hailo-8l-compiler-sigabrt-on-fixed-selection-matrix-matmuls/19666#post_2"
date: "2026-08-16"
author: "@Jesus_Royeth"
feed_url: "https://community.hailo.ai/posts.rss"
---
Hi @Vishal_Ganpisetti : I’m on DFC 3.33.0, not 3.34, but I isolated this with a small synthetic model and it looks like both of your symptoms come from the same root cause: the row count of the selection matmul output. I swept the row count of a [1,N,256] selection matmul, everything else fixed: N = 500, 508, 513, 516, 524 -> fails (silent crash or "Agent infeasible") N = 512, 520, 528 -> compiles clean The pattern is N % 8 == 0 . Your first matmul ( [1,512,256] ) already satisfies that, which is why it compiled fine on its own.
