---
layout: page
title: MindSync
description: EEG to text translation
img: assets/img/9.jpg
importance: 2
category: fun
---


**MindSync** is a novel framework that translates brain activity recorded via EEG signals into natural language text. The model is designed to handle both word-level EEG features and raw EEG waveforms.

## Model Pipeline
1. **Preprocessing**:
  - Dataset: ZuCo: [LINK](https://www.nature.com/articles/sdata2018291)
  - Band-pass filtering and feature extraction applied to EEG signals.
  - A pretrained feature extractor (DreamDiffusion) was employed to process raw EEG waves, reducing noise and improving signal clarity.
  
2. **EEG Feature Representation**:
   - EEG features are mapped into a **vector-quantized (VQ-VAE)** discrete codex to stabilize input variability.
   - The codex generated from transformer layers serves as an intermediary between EEG signals and the language model.

3. **Text Generation**:
   - Encoded EEG representations are passed to a **pretrained BART transformer** to generate corresponding text.

4. **Training Process**:
   - **Fine-tuning**: The model is fine-tuned using **cross-entropy loss** to optimize text predictions.

<div class="row justify-content-sm-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/mindsync/mindsync_method.png" title="method" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Two-Stage Training Approach:
1. **Stage 1**: Learn discrete EEG representations without updating the language model.
2. **Stage 2**: Fine-tune the full system with lower learning rates to ensure stable optimization.

## Experimental Results
- The model was trained on the **ZuCo** dataset, which contains EEG signals recorded during natural reading.
- **Performance**: Outperformed prior models with a **BLEU-1 score** of **29.6** for raw EEG-to-text conversion, surpassing the previous best score of **21**.
- Examples of output: 
  **Predicted:** was in the United States Army from a Republican from 1955 from is is is ( ( ( ( ( ( ( ( ( (
  **Ground Truth:** He served in the United States Senate as a Republican from Minnesota.

<div class="row justify-content-sm-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/mindsync/results_mindsync.png" title="results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>


## Contributors
- **Yash Sharma**
- **Anurag Maurya**
- **Avni Mittal**

{% raw %}

{% endraw %}