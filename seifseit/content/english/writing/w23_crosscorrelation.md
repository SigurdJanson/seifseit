---
title: "The R Cross Correlation Function"
date: 2020-03-18
author: Jan Seifert
image : "images/blog/crosscorrelation.webp"
bg_image: "images/writing-bg.webp"
categories: ["Statistics"]
tags: ["R"]
languages: ["English"]
description: "What the man page will not tell you…"
draft: false
type: "writing"
information:
  - label : "Target Group"
    info : "Data & social scientists"

mediumlink: /the-r-cross-correlation-function-f5f426006425?source=friends_link&sk=60e3a85df26d2eebd0c47ab84c3407c0
abstract: ""
---

R is awesome! Let‘s just take these two vectors, put it in that function and voila … R is the plague. I wanted to use the ccf-function in a project. I had so much trouble understanding it's output. There are quite a few things about the cross-correlation function in R that the manual does not tell us. Reading it carefully did not help. I had to experiment with the function and write it down. It took me a day to find out what you can read here. And only because I had to figure it out the hard way, does not mean you have to.

The function `ccf(x, y)` expects two vectors to estimate the correlation between `x[t+k]` and `y[t]`. That means, it will not just correlate the vectors. It will correlate them after shifting their position relative to one another by `k` elements and then correlate the vectors. Furthermore, usually we do not just specify one value of `k`... 

