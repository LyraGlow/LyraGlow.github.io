---
layout: post
read_time: true
show_date: true
title:  轨迹预测（重置版）
date:   2026-03-02 20:33:20 +0800
description: 这是一篇在重装系统丢失了原文件的基础上重置的，主要删除了数学推导（再写一次太累了），强调代码实现。
img: posts/20260311/1.png
tags: [Technology]
author: 黄建豪
github:  LyraGlow/STP-Reproduction
mathjax: yes
---
## 重置版的原因

我在2026年的3月4日预存了一篇轨迹预测的文章，可惜在3月10日的时候将Ubuntu22.04重装到24.04时忘记备份了，上一版记载了我推导论文[Inland Ship Trajectory Restoration by Recurrent Neural Network(基于循环神经网络的内河船舶轨迹恢复)](https://www.cambridge.org/core/journals/journal-of-navigation/article/abs/inland-ship-trajectory-restoration-by-recurrent-neural-network/3F48B53752FC16D12EADC883DAA58CB9)中前置RNN与LSTM的数学公式推到，补充了一些矩阵相关的知识，包括奇异值分解和特征值分解。因此有了这一版的诞生。这一版不再重新推到相关数学基础，聚焦于相关的代码实现。

## 代码实现

### 数据集来源



