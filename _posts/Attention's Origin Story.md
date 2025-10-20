---
layout: single
title: "Attention’s Origin Story"
excerpt: 'Trying to understand the origin of "Attention Head"'
permalink: /blog/<slug>/
categories: [paper-notes]
tags: [llm, review, ml, attention]   # edit freely
toc: true
toc_sticky: true
read_time: true
share: true
---

> **Attention, at its core, is just a probability — computed from how similar a Query is to a Key — and the result is simply the weighted sum of the corresponding Values.**


### A Simple Intuition for Key–Value Memory Networks

```python
Key: blog is awesome!
Value: Jaz's
Key: weather is cold.
Value: Winter
Query: Whose blog is awesome!
```


We compute the **similarity** between the **Query** and every **Key**.

That similarity acts as a **weight** on the **corresponding Value**.


```python
Sim (blog is awesome!, Whose blog is awesome!) = 0.99
Sim (weather is cold., Whose blog is awesome!) = 0.01
```

So the output is simply a **weighted sum of all values**:
```bash
Results = 0.99 * (Jaz's) + 0.01 * (Winter) ≈ Jaz's
```

**That’s the core idea.**  
Attention = "which memory is most relevant?"  
Value = "what answer does that memory contain?"

## One Sentence to Summarize the Original Attention

The context vector is computed as a weighted sum of the encoder’s annotations, where each weight reflects how relevant the annotation — centered on a specific input word — is to the decoder’s current state. This context vector is then fed into the decoder, instead of the single fixed sentence embedding used in earlier encoder–decoder models.


