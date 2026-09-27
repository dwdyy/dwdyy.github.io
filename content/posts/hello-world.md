---
title: "Hello, World：博客从这里开始"
date: 2026-09-27T00:00:00+08:00
description: "为什么建立这个博客，以及如何在文章中书写代码与数学公式。"
tags: ["随笔", "Hugo", "LaTeX"]
categories: ["博客"]
draft: false
---

欢迎来到我的技术博客。

作为计算机专业学生，我希望这里不只是知识点的集合，而是一份可以回看、检验和持续修正的学习记录。之后我会分享算法推导、系统实验、工程实践和论文阅读笔记。

## 代码

```python
def binary_search(a, target):
    lo, hi = 0, len(a)
    while lo < hi:
        mid = (lo + hi) // 2
        if a[mid] < target:
            lo = mid + 1
        else:
            hi = mid
    return lo
```

## 数学公式

文章支持 LaTeX。比如，二分查找的时间复杂度是 \(O(\log n)\)。

常见的等差数列求和公式可以写成：

\[
\sum_{k=1}^{n} k = \frac{n(n+1)}{2}
\]

欧拉恒等式则是：

$$
e^{i\pi} + 1 = 0
$$

这些公式会在 Hugo 构建时由 KaTeX 渲染，同时保留 MathML 以改善可访问性。

