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

## Introduction
In recent years, the field of artificial intelligence has exploded in popularity, 
largely driven by a now well known architecture known as transformers. Originally introduced in a 2017
 paper titled "Attention is All You Need," transformers have revolutionized how machines understand 
and generate human language. These powerful models have not only set new benchmarks in natural language 
processing tasks but have also opened up new frontiers for machine learning in areas like question answering, 
text summarization, and even creative writing. As we delve into the intricacies of transformers, we'll 
explore how their unique architecture, is reshaping the landscape of AI and pushing the boundaries of what machines can achieve. 
Read on to learn more about transformers, its history, and what they exactly do.

## What we are trying to do

Before we learn about transformers, it is important to understand what is our task. After all we need a problem to 
come up with a solution. 

The problem is that we need a way to interpret and generate sequential data.

Wait, what is sequential data?

In simple terms, any data that has an order to it can be considered as sequential data. Some examples of sequential data are stock prices, text, audio, video etc. Any data that has an order to that that is meaningful can be considered as sequential data.

Let's understand this further with an example. Consider the following sentences

```
I am holding an apple.

This is very interesting, how does it work?
```

Now, as we can tell, the order of those words are important, suppose we jumble the words to am "apple I holding an", then the sentence
makes no sense. Hence it is vital that order is maintained for proper results.

However, we can notice one more thing in these examples, it has variable length. The first example has 5 words and the second one has 8 words, thats interesting.

Why you may ask? Traditional feed forward networks make the assumption that the data is fixed in length and predetermined. For a lot of tasks such as classification, regression etc, this is fine and makes feed forwards networks very useful, however, it does not work with variable length data. Now there are some hacks that we can use to get around this if we really wanted to, such as masking and padding. However this makes the network inefficicent, large, and horrible.

So what do we do? 

(You can probably guess that one of the solutions is transformers, but now lets pretend that we don't know about it ;) ) 

## What we did before
Lets rewind back to pre 2017(aka before "attention was all you need" was published). We still had machine learning tasks that were based on text or sequential data. So how did we do it?
Enter RNNs. RNN stands for Recurrent Neural Networks. They are a special class of neural networks designed for sequential data. There are several kinds of RNNs, such as simple RNNs, 
Long Short Term Memory(LSTM), Gated Recurrent Unit(GRU) etc.

Now how they work are out of the scope of this blog as it would take too long to explain. But the main thing, is that these were recurrent networks.

What are recurrent networks?

Essentially, you give the output to the input. The diagram gives a glimpse into how they work. 

# Add a diagram for RNN, recursive and split out.


Well, now the question is how well do they work?  Well, they were fine for translation, classification etc. But they also had some limitations

- The model would forget the context easily. Generally information that was given to the model any more than a few cycles before would be completely lost.
- It was very incredibly unstable and difficult to train.
- It did not scale well.
- It could not generate new information very well.
- It was not very parallelizable

These were just some of the disadvantages, there were many more. But I digress.

Now we can talk about transformers and why they are so special.

## Finally Transformers!

Well, now we can talk about transformers. Transformers are a highly parallel, scalable neural network architecture used for generation, translation, summarization, and all kinds of cool and interesing applications. 
The information for the next few sections is based on the famous paper [Attention is all you need](https://arxiv.org/pdf/1706.03762). 

Lets get into the architecture of this thing. As a start, lets start with the attention layer, the main driver behind this architecture.

## Give me your Attention!

# Insert pic of attention layer


## Transformer Architecture

# insert pic of original transformer

## What makes this better

- highly parallel and scalable
- highly scalable
- optimized
- can generate new information
- can remember context better than RNNs

## Variations to this architecture
## Modern Improvments to Transformer architecture 
### prenormalization
# Insert pic of diagram

### RMS normalization

# Insert pic of diagram

### Rotary embeddings
# Insert pic of diagram


# Conclusion