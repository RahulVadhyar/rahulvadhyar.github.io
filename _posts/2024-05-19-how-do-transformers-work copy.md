---
title: 'Give me attention: LLMs and Transformers'
date: 2023-05-19
categories: [Machine Learning]
tags: [attention, transformers, sequential, LLM]     # TAG names should always be lowercase
description: A detailed explaination of attention mechanism and how transformers work.
comments: true
math: true
toc: true
---

# Insert a PIC here

# Introduction
In recent years, the field of artificial intelligence has witnessed a groundbreaking evolution, 
largely driven by an now well known architecture known as transformers. Originally introduced in a 2017
 paper titled "Attention is All You Need," transformers have revolutionized how machines understand 
and generate human language. These powerful models have not only set new benchmarks in natural language 
processing tasks but have also opened up new frontiers for machine learning in areas like question answering, 
text summarization, and even creative writing. As we delve into the intricacies of transformers, we'll 
explore how their unique architecture, is reshaping the landscape of AI and pushing the boundaries of what machines can achieve. 
Read on to learn more about transformers, its history, and what they exactly do.

# What we are trying to do

Before we learn about transformers, it is important to understand what is our task. After all we need a problem to 
come up with a solution. 

Essentially all text data can be considered as sequential data. This is because text data has to be in order. Lets understand this
using an example. Consider the below sentence:

I am holding an apple.

Now, as we can tell, the order of those words are important, suppose we jumble the words to am "apple I holding an", then the sentence
makes no sense. Hence it is vital that order is maintained for proper results. We can see that some of the key characteristics of such data
is as follows

1) The data is sequential in nature, the order has to be maintained.
2) The data can be of variable length. This is due to the fact that 
sentences can be of variable sizes having different number of words and characters.

As we can see, the second point makes traditional feed forward neural networks(FFNN) highly unsuitable for this task.
This is due to the fact that FFNNs can only accept fixed size inputs. We cannot vary the size of the inputs. 
Now this does not mean that we cannot make FFNNs somehow accept sequential data, We can use masking and padding methods to achieve this, but
these networks will be very large, inefficent and not suitable for the task. This is similar to comparing CNNs and FFNNs, where FFNNs can be used for 
image tasks, its just horribly inefficient and large.

So what do we do now? By the title one might think the answer is transformers, and they are partially right,
its just that there is another class of neural networks that can also handle sequential data is... Well I ain't going to spoil it for you, 
you will just have to read on. 

# What we did before
Lets rewind to 2015.


# What is attention

# Attention Explained

# What makes this better

# Transformer Architecture
some markdown

# Conclusion