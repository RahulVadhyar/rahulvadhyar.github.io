---
title: 'All Too Well: Optimizing a PyTorch model for training on single GPU systems'
date: 2023-05-17
categories: [Machine Learning]
tags: [pytorch, optimization, deep learning, machine learning, compile, cuda, transformers, atttention]     # TAG names should always be lowercase
description: In this post I shall discuss the various methods to optimize a PyTorch model.
comments: true
math: true
---

# Introduction

# Why do we want to optimize?

# How to check how optmized your model is
* Profiling
* Nvidia-smi

# Optimization Methods
* Doing more on CPU
* Tensor size and batch size
* Better OS
* Run less other processes on GPU
* Use tensor cores
* Torch.compile
* Flash Attention
* Mixed Precision
* Fused Optimizer and instant application
* Paged Optimizer
* Advanced: Custom CUDA Kernels

# Conclusion