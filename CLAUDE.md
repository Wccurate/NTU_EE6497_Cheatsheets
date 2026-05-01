# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LaTeX-based ultra-compact cheat sheets for NTU EE6497 Pattern Recognition & Deep Learning (AY2025). Three independent cheat sheet projects covering different exam scopes: Quiz 1 (probability fundamentals, MLE/MAP, EM, HMM), Quiz 2 (neural networks, activation functions, training techniques, CNN basics), and Final (comprehensive summary combining both).

## Build

Each cheat sheet is an independent LaTeX project. Compile with `pdflatex` from within the project folder:

```bash
cd EE6497_Quiz1_Cheatsheet && pdflatex main.tex
cd EE6497_Quiz2_Cheatsheet && pdflatex main.tex
cd EE6497_Final_Cheatsheet && pdflatex main.tex
```

Run `pdflatex` 2-3 times to resolve cross-references. No auxiliary tools (bibtex, biber) are needed despite `biblatex` being loaded in the preamble — there are no actual citations.

## Architecture

Each cheat sheet folder has the same structure:

- `preamble.tex` — shared configuration file (identical across all three folders). Manages packages (math, tables, algorithms, hyperref, biblatex), font settings, and column types.
- `main.tex` — the content file. Sets up the 4-column layout via `multicols*`, imports `preamble.tex`, and contains all cheat sheet content.

The layout is maximally space-efficient: 1pt page margins, `\tiny` or `\scriptsize` font, zero paragraph indentation and display skip, and a blue vertical column separator.

## Key macros

- `\bulletPoint{Topic Name}:` — formats a topic heading (bold, italic, underlined via `soul`). Use this to add new topic sections.
- `\useshortskip` — from `nccmath`, reduces vertical space around equation environments. Use it before every `\begin{equation*}` to keep content dense.

## Content conventions

- Equations use `\begin{equation*}` and `\begin{split}` for multi-line formulas.
- Quiz 2 and Final (other.tex) include inline Python/PyTorch code examples using the `listings` package with `\tiny` monospace font.
- The Final folder contains an additional `other.tex` file (independent document, `\scriptsize` font, black column rules) covering probability, Bayesian inference, GMM/EM, HMM, Markov chains, MCMC, and sampling methods.

## .gitignore

PDF files and all LaTeX build artifacts (`*.aux`, `*.log`, `*.out`, etc.) are gitignored. Only `.tex` source files should be committed.
