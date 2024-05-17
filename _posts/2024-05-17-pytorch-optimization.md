---
title: 'Optimizing a PyTorch model for training on single GPU systems'
date: 2023-05-17
categories: [Machine Learning]
tags: [pytorch, optimization, deep learning, machine learning, compile, cuda, transformers, attention]     # TAG names should always be lowercase
description: In this post I shall discuss the various methods to optimize a PyTorch model.
comments: true
math: true
toc: true
---

# Introduction

In this post, I shall be showing you how to optimize your pytorch model for maximum performance. We shall be exploring various methods to optimize your model such as using tensor cores, torch.compile, flash attention etc. This is a very important topic as it can help you train your model faster and more efficiently. 

For this tutorial, I shall be optimizing a transformer model on the openwebtext2 dataset.
The code for this can be found here.

My system specifications are as follows:

* **CPU**: Intel i9-12900K
* **Memory**: 48GB DDR4 - 3200MT/s
* **GPU**: Nvidia RTX 3080 10GB LHR
* **OS**: Fedora 40 with KDE Plasma
* **PyTorch**: 2.3.0

Read on to find out more.

> Note that this tutorial largely applies to single GPU systems. Multi-GPU systems are not covered in this tutorial.
{: .prompt-info}

# What is optimization?

Optimization is the process of making your model more efficient to run. This can involve a number of different things such as reducing the memory footprint of your model, reducing the training time of your model, or reducing the number of parameters in your model. 

Generally for maxmimum performance, you want to make sure that your GPU is always occupied at maximum capacity. This ensures that your model is running as fast as possible and that you are getting the most out of your hardware. Else, there might be periods where your GPU is idle and not being used to its full potential.

# Why do we want to optimize?

Generally you want to optimize your model for various reasons such as:

* **Faster training**: Optimizing your model could mean the difference between a 2 day training time and a 2hr trainig time. This is not only important for ensuring that you do not waste resources and time but also for ensuring that you can iterate on your model faster.

* **Better performance**: Optimizing your model can also lead to better performance. This is because you can train your model on larger datasets and with more complex architectures.

* **Cost savings**: Optimizing your model can also lead to cost savings. This is because you can train your model faster and more efficiently which means that you can save on resources such as electricity and hardware.

* **Model size**: By properly profiling and optimizing your model, you can reduce the memory neeeded for training your model, which can be important for training on smaller GPUs with less VRAM, or scaling your model to the limits of your hardware.

# How to check how optmized your model is

Before we start optimizing our model, it is important to check and visualize how optimized our model is. This is crucial as it can tell you which optimized techiniques you need and how much you can improve your model. Sometimes a lot of the optimization techniques are not needed if your model is already optimized due to various circumstances.

One of the best methods to check how optimized your model is to use the PyTorch profiler. The PyTorch profiler is a tool that allows you to profile your model and see how much time is spent on each operation. This can help you identify bottlenecks in your model and optimize them.
It also shows GPU usage, 

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