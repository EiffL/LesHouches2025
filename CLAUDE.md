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

## Writing Style Guidelines

When editing or creating content for this lecture, maintain the following style:

### Tone and Approach
- **Authoritative yet pedagogical** - scholarly and precise with deliberate explanatory moments
- Appropriate for graduate-level lecture notes that are both rigorous and teachable
- Academic formality with clarity - rigorous but accessible language

### Formatting and Structure
- **Strategic emphasis** - selective use of bold for key conceptual distinctions
- **Balanced structure** - logical flow with clear paragraph organization
- **Forward-looking organization** - sections that summarize and set expectations

### Language Conventions
- **Precise technical terminology** - exact language over colloquial explanations
- **Explanatory clarifications** - helpful parenthetical remarks without repetition
- **Comprehensive but concise** - thorough coverage while maintaining brevity

### Pedagogical Structure
- **Logic of discovery over logic of exposition** - Follow the intellectual journey that led to method development, not just final technical descriptions
- **Motivational pedagogy** - Always establish necessity/problems before presenting solutions. Never introduce techniques without clear motivation
- **Causal narrative structure** - Each concept should arise naturally from limitations of previous concepts. Make transitions explicit and motivated
- **Problem-solution chains** - Structure content around explicit problem → solution → new problem → better solution sequences
- **Reader journey mapping** - Consider what natural questions the target cosmologist audience would have and address them in logical order
- **Intellectual evolution** - Show WHY methods were developed historically (e.g., "2-point functions became dominant BECAUSE their likelihoods were analytically tractable"), not just HOW they work
- **Information architecture** - Present concepts in order of increasing complexity, establishing foundations before building upon them
- **Avoid "technique catalog" writing** - Don't list methods sequentially without showing their conceptual relationships and evolutionary necessity

### Strategic Bold Emphasis Guidelines
- Bold text should create a coherent narrative when read in isolation - a reader should understand the key conceptual flow by scanning bold phrases alone
- Use bold for key concepts, fundamental limitations, and crucial insights - NOT for paragraph headers or organizational markers
- Strategic bold emphasis should highlight conceptual distinctions and turning points in the argument
- Bold phrases should capture the essential logic: problem identification → methodological solutions → information costs → theoretical advances → practical limitations

## Development Workflow

1. Edit LaTeX files in the `notes/` directory
2. Test compilation locally with pdflatex
3. Push changes to trigger automatic GitHub Actions compilation
4. Check the build status via the PDF Status badge
5. Access the compiled PDF via the Download PDF badge or GitHub releases