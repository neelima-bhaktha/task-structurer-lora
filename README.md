# LoRA-Tuned Summarization Assistant

## Overview
This project fine-tunes a small open-source language model using **LoRA (Low-Rank Adaptation)** to generate summaries in my personal writing style.

Instead of producing generic summaries, the model learns:
- what details I prioritise
- how concise I am
- the tone and structure I naturally use when summarising content

The goal is to demonstrate **practical model adaptation for a narrow, real-world task**.

---

## Problem Statement
Most summarization models optimise for generic “coverage,” often resulting in long or unfocused summaries.  
In practice, summarization is subjective — different users focus on different aspects of the same content.

This project adapts a model to:
- produce short, exam- or review-ready summaries
- emphasise core ideas over examples
- match my natural writing style rather than a generic one

---

## Approach
- Collected ~20 articles from online sources  
- Wrote my own 2–3 sentence summaries for each article  
- Created article → summary training pairs  
- Fine-tuned the model using **LoRA**, keeping the base model frozen  

This setup allows the model to adapt behaviour and style without relearning language knowledge.

---

## Project Structure
data/ # articles and reference summaries
src/ # training and inference scripts
models/ # LoRA fine-tuned checkpoints
notebooks/ # experiments and debugging


---

## Results
After fine-tuning:
- summaries became more concise and consistent
- irrelevant details were reduced
- outputs required fewer manual edits compared to the base model

Evaluation was done qualitatively by comparing base vs fine-tuned outputs on unseen articles.

---

## Key Takeaways
- LoRA is effective for **style and preference alignment**
- Small, high-quality datasets can meaningfully change model behaviour
- Narrow task focus leads to more reliable and deployable systems

