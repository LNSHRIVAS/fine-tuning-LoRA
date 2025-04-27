# Exploring LoRA Fine-Tuning with TinyLlama-1.1B

## Introduction
In this mini-exploration, I experimented with **Low-Rank Adaptation (LoRA)** to fine-tune **TinyLlama-1.1B** on a subset of the **Alpaca dataset**.  
The goal was to understand how LoRA enables efficient fine-tuning of large language models using minimal compute and storage.

---

## What I did
- **Loaded TinyLlama-1.1B** in 4-bit precision (quantized) using `bitsandbytes`
- **Injected LoRA adapters** using Huggingface `peft`
- **Trained** on 1000 samples from Alpaca dataset
- **Saved** the LoRA-adapted model to Google Drive
- **Compared** responses before and after fine-tuning

---

## Key Learnings
- Even lightweight fine-tuning improves instruction-following behavior.
- LoRA allows fine-tuning massive models on low-resource hardware (e.g., Colab GPUs).
- Observed minor but meaningful changes in output quality after a short training cycle.
- Fine-tuning needs careful prompt formatting and dataset quality to maximize impact.

---

## Why LoRA Matters
- Industry shift towards **parameter-efficient fine-tuning** (PEFT) methods like LoRA.
- Crucial for startups, researchers, and smaller teams to customize LLMs without massive infrastructure.

---

## Resources Used
- Model: [TinyLlama/TinyLlama-1.1B-Chat-v1.0](https://huggingface.co/TinyLlama/TinyLlama-1.1B-Chat-v1.0)
- Dataset: [tatsu-lab/alpaca](https://huggingface.co/datasets/tatsu-lab/alpaca)

---

## Future Work
- Explore full fine-tuning with larger subsets.
- Test LoRA adaptation on real-world domain-specific datasets.
- Experiment with QLoRA and other PEFT techniques.

---

## Let's Connect
I'm passionate about scalable ML solutions, model optimization, and applied AI engineering.  
Always open to learning, discussions, and collaborations!

👉 [LinkedIn Profile](https://www.linkedin.com/in/lakshminarayan-shrivas/)

---
