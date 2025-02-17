---
layout: page
title: HinglishLM
description: Experimenting with Language Models on Hinglish data
img: assets/img/12.jpg
importance: 1
category: fun
related_publications: false
---
Hinglish—an informal code-mixed blend of Hindi and English—is prevalent across social media, messaging apps, and online forums. The primary motivation for this project was to have a hinglish chatbot which could be use for whatsapp chats but I found it worth investigating hinglish which is a bit different form of code mixing. 
**Hinglish-LM** is a fun project focused on evaluating language model architectures for Hinglish through **custom dataset curation and architectural ablations**

---


### Why?
- Frequent language switching is observed in Hinglish. 
- Variations like "kya", "kyaaa", "kia"
- No grammar: very informal structure of sentences

### Hinglish Dataset Curation  
- Compiled a Hinglish dataset from Reddit and other sources, incorporating real-world conversational data with diverse linguistic variations.  
- Datasets combined: 

### Custom Model Training  
- Pretrained and instruction-finetuned a **decoder-only transformer** from scratch, specifically optimized for Hinglish.  

### Architectural Ablations  
- Conducted in-depth evaluations of embedding techniques:  
  - Sinusoidal vs. Learnable Positional Embeddings 
  - Rotary Positional Embeddings (RoPE) vs. ALiBi Embeddings  

### Finetuning on whatsApp style chats:
- Used conversational data to fine tune the language model
- Some of the conversations produced: 

### Tokenizer Comparisons  
- Assessed performance differences between:  
  - tiktoken tokenizer (optimized for GPT-like architectures)
  - BPE tokenizer trained on Hinglish corpus (capturing subword units more effectively)


- The model still hallucinates a lot. Prehaps the dataset needs to be refined more. Can work on combined embedding approach for reducing gaps between varied tokens 

---

{% raw %}


{% endraw %}
