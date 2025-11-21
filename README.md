# LoRA Note Structurer

This is an experiment where I fine-tune a small model using LoRA to turn my messy class notes into clean, structured explanations. The model is heavily personalised because it’s trained directly on my own notes.

## Why I’m Building This
During my DS class, I couldn’t keep up with the pace and ended up writing only keywords and broken sentences. I realised I needed something that could turn those tiny jotted points into proper notes without me rewriting everything manually. So I’m building it.

## How It Works
I collect pairs of messy notes and clean explanations. Then I fine-tune an open-source model using LoRA so it learns my structure and tone.

## Project Structure
data/ – raw notes and processed dataset  
src/ – training and inference scripts  
models/ – fine-tuned checkpoints  
notebooks/ – experiments/debugging  

## How to Run It
After training, run `inference.py` with your messy notes to generate structured output.

## Current Status
Dataset creation in progress.  
Training script scaffold coming next.
