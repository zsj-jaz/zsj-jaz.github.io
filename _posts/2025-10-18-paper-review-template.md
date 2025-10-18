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


## Where Does Attention Come From?

We all know Attention Is All You Need changed everything — it became the foundation of modern LLMs. But I kept wondering: **where did the idea of “attention” even come from in the first place?**

It clearly didn’t just appear out of nowhere.

Before Transformers, researchers were already experimenting with ideas like neural memory networks and key–value retrieval. Somewhere in those early works, the concept of “attention” began to form — long before it had that name.

This blog is my attempt to trace that origin and understand how attention truly began.

---

## the TL;DR Version
Neural Turing Machines (2014) — neural networks with external memory
        ↓
Memory Networks (2014–2015) — store facts as memory slots
        ↓
End-to-End Memory Networks (2015) — multi-hop reasoning over memory
        ↓
Key–Value Memory Networks (2016) — separate keys for matching, values for retrieval
        ↓
Self-Attention (2017, Attention Is All You Need) — tokens attend to each other instead of external memory


## Key results
- Main figure/table that matters and why
- Any surprising outcomes or ablations

## What’s strong
- ✅ Clarity / insight / practicality

## What I’m skeptical about
- ❓ Limitations / assumptions / dataset caveats

## Connections
- Related work I know
- How it compares to X / Y

## Replication / engineering notes
- Dataset / code links (if any)
- Repro steps I’d try next

## Next questions for me
- A small experiment I could run this week
- How it might fit my projects

## Reference
- Authors, *Title*, Venue Year. Link: <url>
