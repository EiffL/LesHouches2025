# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a LaTeX-based lecture notes repository for a Simulation-Based Inference (SBI) tutorial presented at the Dark Universe Summer School at Les Houches 2025. The repository contains LaTeX source files for lecture slides/notes and automated GitHub Actions for PDF compilation.

## Build Commands

### Local LaTeX Compilation
To compile the LaTeX document locally:
```bash
cd notes
pdflatex -interaction=nonstopmode -file-line-error main.tex
```

### Automated Compilation
The repository uses GitHub Actions to automatically compile the LaTeX document when changes are pushed to the `notes/` directory. The compiled PDF is:
- Uploaded as an artifact for 90 days
- Published to a GitHub release tagged as "latest"
- Accessible via the Download PDF badge in the README

## Repository Structure

- `notes/main.tex` - Main LaTeX source file for the lecture notes
- `.github/workflows/compile-latex.yml` - GitHub Actions workflow for automatic LaTeX compilation
- `README.md` - Repository documentation with lecture outline and resources

## Key Information

- **Lecturer**: François Lanusse, CNRS/CEA Paris-Saclay
- **License**: Creative Commons Attribution 4.0 International (CC BY 4.0)
- **GitHub Repository**: https://github.com/EiffL/LesHouches2025

## LaTeX Document Structure

The LaTeX document uses a custom Les Houches style with:
- Custom color scheme (leshouches blue: RGB 25,55,95)
- Structured sections following the SBI lecture outline
- Minimal content serving as a skeleton for the full lecture

## Development Workflow

1. Edit LaTeX files in the `notes/` directory
2. Test compilation locally with pdflatex
3. Push changes to trigger automatic GitHub Actions compilation
4. Check the build status via the PDF Status badge
5. Access the compiled PDF via the Download PDF badge or GitHub releases