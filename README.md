# Lecture Notes for MA52112: Statistics for Data Science

This repository contains the source code for the lecture notes of the course **MA52112: Statistics for Data Science** at the University of Bath. The notes are authored by **Karim Anaya-Izquierdo** (based on original notes by Vangelis Evangelou).

## Course Overview

**Statistics for Data Science** provides a foundation in the theory of probability and statistics, with a focus on practical application in data science.

### Synopsis
In this unit, students develop an understanding of the basic theory of probability and statistics and learn to recognise when this theory can be applied in practice.

### Learning Outcomes
By the end of the unit, students will be able to:
*   Perform elementary mathematical operations in probability and statistics.
*   Translate real-world problems into a probabilistic or statistical framework.
*   Solve statistical problems in abstract form.
*   Critically interpret the outcomes of statistical analysis in a real-world context.
*   Relate underlying theory to requirements in practical data science.

### Content
The course covers:
*   The laws of probability.
*   Discrete and continuous random variables.
*   Expectation, variance, and correlation.
*   Conditional and marginal distributions.
*   Common distributions (Normal, Binomial, Poisson).
*   Statistical estimation (including Maximum Likelihood).
*   Hypothesis testing and confidence intervals.

## Repository Structure

The project is built using [Quarto](https://quarto.org/) and is structured as a Quarto Book.

*   **`index.qmd`**: The landing page containing the course overview and syllabus.
*   **`ch1.qmd` - `ch5.qmd`**: Source files for the lecture chapters.
*   **`Problem sheets/`**: Directory containing exercise sheets and solutions.
*   **`images/`**: Directory for static image assets used in the notes.
*   **`_quarto.yml`**: Quarto project configuration file.
*   **`docs/`**: The generated output directory (HTML and PDF files).
*   **`references.bib` / `packages.bib`**: Bibliography files.

## Building the Notes

To render the lecture notes locally, you will need **Quarto** installed.

### Prerequisites
*   [Quarto CLI](https://quarto.org/docs/get-started/)
*   [R](https://www.r-project.org/) (for executing R code chunks)
*   A LaTeX distribution (e.g., TinyTeX, TeX Live) for PDF generation.

### Rendering
To render the entire book to both HTML and PDF formats:

```bash
quarto render
```

To preview the book locally (with live reload):

```bash
quarto preview
```

## License & Authors
*   **Author:** Karim Anaya-Izquierdo
*   **Original Notes:** Vangelis Evangelou
