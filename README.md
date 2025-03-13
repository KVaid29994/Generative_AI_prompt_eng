# Prompt Engineering with LLaMA 2

## Introduction
This notebook demonstrates **Prompt Engineering techniques** with the **LLaMA 2 open-source LLM**. We will explore key ideas behind prompt engineering and analyze how different prompt elements influence the model's responses.

## Installation
To run this notebook, install the necessary dependencies using:
```bash
pip install huggingface_hub
```

## Prompt Parameters
Below are the prompt parameters used in this notebook along with their explanations:

### **1. max_tokens**
- Specifies the **maximum** number of tokens that the model should generate.
- **Value used**: `256`

### **2. temperature**
- Controls the **randomness** of the generated response.
- **Higher values** (e.g., `1.0`) → More random output.
- **Lower values** (e.g., `0.0`) → More deterministic output.
- **Value used**: `0` (deterministic response)

### **3. top_p**
- Controls the **diversity** of the response.
- A higher value (close to `1.0`) results in **more diverse** responses.
- A lower value results in **less diverse** responses.
- **Value used**: `0.95`

### **4. repeat_penalty**
- Controls the **penalty** for repeating tokens.
- Higher values reduce repetition probability.
- **Value used**: `1.2`

### **5. top_k**
- Limits the **number of tokens** considered during response generation.
- A lower value narrows the model’s token choices.
- **Value used**: `50`

### **6. stop**
- Specifies **tokens** that should stop the model from generating further.
- **Value used**: `['INST']`

### **7. echo**
- Determines whether the model should **echo the prompt** back to the user.
- **Value used**: `False`

## Summary
Through this notebook, we aim to highlight how different prompt elements influence **output quality, creativity, and coherence** when working with **LLaMA 2**. Experimenting with these parameters will help optimize model responses for various NLP applications.

---
Feel free to modify the parameters and experiment with different configurations!

