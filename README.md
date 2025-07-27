# Simulation-Based Inference for Cosmology

**Lecture at the Dark Universe Summer School, Les Houches 2025**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![PDF Status](https://github.com/EiffL/LesHouches2025/actions/workflows/compile-latex.yml/badge.svg)](https://github.com/EiffL/LesHouches2025/actions/workflows/compile-latex.yml)
[![View PDF](https://img.shields.io/badge/View-PDF-blue.svg)](https://github.com/EiffL/LesHouches2025/blob/main/notes/main.pdf)
[![Download PDF](https://img.shields.io/badge/Download-PDF-red.svg)](https://github.com/EiffL/LesHouches2025/releases/latest/download/main.pdf)

This repository contains lecture materials for a one-hour introduction to Simulation-Based Inference (SBI) in cosmology, presented at the [Dark Universe Summer School](https://indico.iap.fr/event/25/) at École de Physique des Houches, France.

## 📚 Lecture Overview

This lecture provides a comprehensive introduction to modern simulation-based inference techniques for cosmological data analysis, focusing on how we can leverage neural networks to perform Bayesian inference when traditional likelihood-based approaches are intractable.

## 🎯 Learning Objectives

By the end of this lecture, you will understand:
- The fundamental differences between SBI and traditional inference approaches
- How to estimate distributions implicitly using neural networks
- Modern techniques for neural density estimation
- Practical strategies for implementing SBI in cosmological analyses
- Key considerations for robust SBI applications

## 📋 Lecture Outline

### 1. **What Makes SBI Different?**
- **Analytic Likelihoods**: Traditional approaches and their limitations
- **Full-field / Hierarchical Inference**: When complexity meets reality
- **Simulation-Based Inference**: Learning implicit distributions from simulations

### 2. **Neural Density Estimation: The Foundation**
- **What is a Neural Network?** Core concepts and training principles
- **Mixture Density Networks (MDNs)**: Understanding density estimation through the simplest approach
- **Normalizing Flows**: Building flexible, invertible transformations
- **Advanced Methods**: Score matching, stochastic interpolants, and beyond

### 3. **From Density Estimation to Bayesian Inference**
- **Sequential Neural Posterior Estimation (SNPE)**: Learning posteriors directly
- **Sequential Neural Likelihood Estimation (SNLE)**: When likelihoods are preferred
- **Likelihood Ratios**: Efficient inference through ratio estimation
- **The SBI Package**: Practical implementation with [sbi](https://github.com/mackelab/sbi)

### 4. **Dimensionality Reduction for SBI**
- **Beyond 2-Point Functions**: Capturing non-Gaussian field information
- **Compression Strategies**: From raw data to informative summaries
- **Preserving Information**: Balancing compression with inference quality

### 5. **Robust SBI in Practice**
- **Frozen Summarizers**: Why and how to keep feature extraction fixed
- **Sample Efficiency**: Strategies to reduce simulation requirements
- **Ensemble Learning**: Improving robustness through multiple models
- **Limitations and Pitfalls**: What to watch out for in real applications


## 📄 License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

[![CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

This means you are free to:
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

## 🧠 AI Statement

These lecture materials were produced with Claude Sonnet 4 via [Claude Code CLI](https://www.anthropic.com/claude-code) under close guidance, supervision, and review from the Author, [@EiffL](https://github.com/EiffL/).

