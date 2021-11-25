---
title: 'Accuracy of Self-Made R Functions'
date: '2020-01-14'
author: Jan Seifert
image: images/blog/accuracy.webp
bg_image: images/feature-bg.jpg
categories:
  - Software Testing
tags:
  - 'R'
languages:
  - English
description: 'A story about abrasion, leakage, and drift'
draft: false
type: writing
---


I did some testing on statistical functions in R, lately. When I wrote unit tests for my functions I only had a few test cases available. So I had the idea to use inverse functions to improve my tests. In R there are many functions that operate inversively. It means that `f'(x)` unmakes whatever `f(x)` made. That means, in theory: `f'(f(x)) == x`. In practice, this way of testing code always bears the risk that errors in both functions cancel each other out. A test cannot solely rely on such a procedure. But I thought that this would be a great addition to routine unit testing because this way I can test a function rather extensively without having to write much code or ...</p>

<a class="btn btn-main" href="https://medium.com/@jan.seifert/accuracy-of-self-made-r-functions-8b3ff097f915?source=friends_link&sk=ba40877a80b410235c0c5011bcd9a85b">Read the full story on Medium</a>

