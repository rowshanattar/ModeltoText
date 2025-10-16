# Enhancing Model-to-Text Transformations with LLMs

This repository accompanies the scientific report:

> **Enhancing Model-to-Text Transformations with LLMs:  
> A Comparative Study of Existing Tools and Opportunities for AI-driven Improvements**  
> *Rowshanak Hosseinzadeh Attar & Bradley Aiken – University of Rostock, 2025*

## 📘 Contents
- `main.ipynb` — Implementation pipeline for LLM- and traditional M2T transformations  
- `data/` — BPMN and Mermaid models, golden descriptions, and generated outputs  
- `LLM-Generated M2T Results Analysis - CLEANED.csv` — Evaluation data  
- `Report_4EM-5.pdf` — Full report  

## 🧠 Method Summary
This project investigates how **Large Language Models (LLMs)** can improve the transformation of **enterprise process models** into **readable natural-language descriptions**.  
We compared a **traditional hybrid Model-to-Text (M2T)** method — based on rule-based tree traversal and static templates — with **LLM-based** approaches using **GPT-4o-mini** and **LLaMA 3.1 (8B)**.

A dataset of **25 BPMN models** of varying complexity was transformed into **Mermaid.js** notation and processed through three prompt strategies:
1. **Open-ended generation** — free description from the model structure.  
2. **Simplified generation** — avoiding technical terms (e.g., “gateway”, “event”).  
3. **Hybrid refinement** — improving traditional M2T output using an LLM.
   

Evaluation combined **quantitative** and **qualitative** metrics:
- **Text Similarity (contextual & non-contextual)**  
- **Flesch Reading Ease (FRE)** readability  
- **Manual ratings** for instruction following, correctness, and writing quality  
- **Conflict analysis and self-correction** to detect hallucinations  
- **Regression analysis** linking textual correctness to model complexity  

Results show that **LLM-generated texts** are more fluent and natural, while **traditional methods** remain more deterministic and structurally faithful.  
Combining both approaches yields the most reliable results, highlighting the potential of **hybrid LLM-assisted M2T pipelines**.

## 🧩 Tools
Python 3.12, pandas, NumPy, Matplotlib, Seaborn  
Ruby (for traditional M2T transformation via CPEE)

## 📄 License
MIT License © 2025 Rowshanak Hosseinzadeh Attar
