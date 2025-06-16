# 🎓 Glitch Tokens in Large Language Models

**Bachelor's Thesis by Maximilian Stefan Schreber**  
Chair of Software Engineering & AI · TUM · 2025

---

## Overview

This repository contains the written thesis for:

> **"On Studying Glitch Tokens in Large Language Models"**  
> An empirical analysis of token-level vulnerabilities in LLM behavior.

As Large Language Models (LLMs) become deeply integrated into critical domains — from healthcare to legal systems — so do the risks associated with their unpredictable behavior.  
This thesis explores **Glitch Tokens**: rarely used, undertrained, or malformed tokens that can provoke **misleading, harmful, or erratic outputs** in otherwise well-functioning models.

---

## Project Context

This research was conducted as part of my Bachelor's Degree in **Information Systems** at the **Technical University of Munich (TUM)**.  
The project was supervised by [Dr. Mark Huasong Meng](https://www.cs.cit.tum.de/seai/team/mark-huasong-meng/) at the [Chair of Software Engineering & AI (SEAI)](https://www.cs.cit.tum.de/seai/).

---

## Core Contributions

The thesis proposes two key technical approaches:

### 1. Glitch Token Discovery (GTD)  
A modular, prompt-based testing framework for systematically detecting Glitch Tokens across different LLMs using black-box evaluation.

➡️ Code: [github.com/MSchreber/GlitchTokenDiscovery](https://github.com/MSchreber/GlitchTokenDiscovery)

### 2. Glitch Token Avoidance (GTA)  
A defensive mechanism that rephrases contaminated prompts to bypass known Glitch Tokens using auxiliary LLMs.

➡️ Code: [github.com/MSchreber/GlitchTokenAvoidance](https://github.com/MSchreber/GlitchTokenAvoidance)

Both repositories include interface-driven Python implementations, prompt schemas, test predicates, and preconfigured examples for reproducibility.

---

## Thesis Document

You can find the full PDF of the thesis in this repository under:  
**`/Bachelor_Thesis_MSchreber_Studying_Glitch_Tokens.pdf`**

It includes:
- Technical background and tokenizer evolution
- GTD algorithm design (w/ evaluation across 4 LLMs)
- Discussion on metamorphic testing and tokenizer architectures
- Early-stage mitigation techniques for safe LLM deployment

---

## Evaluation Highlights

✔️ Tested on: DeepSeek-V3, Llama3.2, Qwen2.5, Mistral-7b  
✔️ > 7,500 glitch tokens identified  
✔️ Glitch Token rates: up to **3.78%** in real-world tokenizers  
✔️ Avoidance strategy showed **partial success** in rephrasing prompts

---

## Why This Matters

The discovery and neutralization of Glitch Tokens is a **safety-critical task** in modern AI.  
If overlooked, such tokens could lead to:
- **Hallucinations** and **fabricated outputs**
- **Security vulnerabilities** and **data leakage**
- **Bias reinforcement** or **denial-of-service-like behavior**

This work contributes a **generic, reproducible detection framework** to help improve the **robustness and reliability** of LLM deployments.

---

## Contact

Maximilian Schreber  
📧 max.schreber@tum.de  
🔗 [LinkedIn](https://www.linkedin.com/in/maximilian-stefan-schreber-209513299)  
💻 [GitHub Profile](https://github.com/MSchreber) 
---

> *“A single token can change everything. Let’s make sure it doesn’t break everything.”*
