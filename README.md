# An Offline, Voice-Enabled Mobile System for Leaf Disease Detection in Low-Resource Agricultural Settings of Bangladesh

**Author:** Nafisa Tabassum (ID: 2221466042)  
**Supervisor:** Prof. Dr. Sumaiya Tabassum Nimi  
**Course:** CSE498R – Directed Research  
**Institution:** North South University, Department of Electrical and Computer Engineering  
**Date:** May 5, 2026

## Abstract

This project presents the design, implementation, and evaluation of an offline, voice-enabled mobile system for leaf disease detection tailored to low-resource agricultural settings in Bangladesh. The system combines on-device computer vision (MobileNetV2, 3.8 MB after INT8 quantization, 95.8% accuracy) with Bangla voice guidance (eSpeakNG + pre‑recorded templates) and locally stored decision support.

Experimental results on a consolidated dataset of 31,000 field‑captured images (9 crops, 35 disease classes) show:
- 185 ms inference time on a low‑end Samsung Galaxy J2 Core
- 0.23 J energy consumption per inference
- 385 ms end‑to‑end latency (capture → voice output)
- 100% task completion and 4.7/5 satisfaction in usability tests with 10 farmers

The system operates completely offline and is designed to run on affordable Android devices (1‑2 GB RAM).

## Repository Contents

- `main.tex` – Full LaTeX source of the directed research report
- `references.bib` – Bibliography in BibTeX format
- `figures/` – All images (leaf samples, logo, etc.)
- `README.md` – This file
- `.gitignore` – Excludes temporary LaTeX files

## How to Compile

1. Install a LaTeX distribution (TeX Live, MiKTeX) or use Overleaf.
2. Clone this repository.
3. Run:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
