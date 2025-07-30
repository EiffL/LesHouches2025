# Simulation-Based Inference for Cosmology

**Lecture at the Les Houches School of Physics Summer School on Dark Universe, 2025**

<p align="left">
  <a href="https://creativecommons.org/licenses/by/4.0/" target="_blank">
    <img src="https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg" alt="License: CC BY 4.0">
  </a>
  <a href="https://flanusse.net/talks/LesHouches2025/" target="_blank">
    <img src="https://img.shields.io/badge/View-Slides-blue.svg" alt="View Slides">
  </a>
  <!-- <a href="https://github.com/EiffL/LesHouches2025/releases/latest/download/main.pdf" target="_blank">
    <img src="https://img.shields.io/badge/Download-PDF-red.svg" alt="Download PDF">
  </a> -->
</p>

This repository contains lecture materials for a one-hour introduction to Simulation-Based Inference (SBI) in cosmology, presented at the [Les Houches Summer School on Dark Universe](https://indico.iap.fr/event/25/) at the Les Houches School of Physics, France.

## 📚 Lecture Overview

This lecture provides an introduction to modern simulation-based inference techniques for cosmological data analysis, focusing on how we can leverage neural networks to perform Bayesian inference when traditional likelihood-based approaches are intractable.

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


## 🧠 AI Statement

These lecture materials were produced with Claude Sonnet 4 via [Claude Code CLI](https://www.anthropic.com/claude-code) under close guidance, supervision, and review from the Author, [@EiffL](https://github.com/EiffL/).

