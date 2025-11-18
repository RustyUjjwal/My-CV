# Ujjwal Keshri - Curriculum Vitae (CV)

This repository serves as the **single source of truth** for my professional Curriculum Vitae. The CV is written in LaTeX and is automatically compiled into a PDF directly from its source file (`cv.tex`) using GitHub Actions.

**NOTE:** This repository is a personalized fork and adaptation of the excellent [autoCV template by Jitin Nair](https://github.com/jitinnair1/autoCV).

The latest version of the CV is always available and can be accessed directly:

**Latest CV Link:** (This link will point to your GitHub Pages URL, e.g., `https://rustyujjwal.github.io/my-cv/`)

## About the CV

The CV is written in LaTeX (`cv.tex`) and follows a clean, structured format.

## Repository Structure

| File | Description |
| :--- | :--- |
| `cv.tex` | The main LaTeX source file containing all CV content. |
| `citations.bib` | A bibliography file for any academic publications or references. |
| `index.html` | A redirect page to ensure the latest PDF is served via GitHub Pages or a backup link. |
| `Makefile` | Commands for compiling the PDF locally. |
| `.github/workflows/build.yml` | The GitHub Action workflow that automatically compiles and deploys the PDF on every push. |

## Development and Building

The CV is automatically built and deployed to the `build` branch on every push to the main branch via GitHub Actions.

### Workflow

The automated workflow uses the `dante-ev/latex-action` to compile the `.tex` file and `peaceiris/actions-gh-pages` to deploy the resulting PDF and the `index.html` file to the `build` branch, which is configured for GitHub Pages.
