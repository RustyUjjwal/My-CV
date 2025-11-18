# Ujjwal Keshri - Curriculum Vitae (CV)

This repository serves as the **single source of truth** for my professional Curriculum Vitae. The CV is written in LaTeX and is automatically compiled into a PDF directly from its source file (`cv.tex`) using GitHub Actions.

**NOTE:** This repository is a personalized fork and adaptation of the excellent [autoCV template by Jitin Nair](https://github.com/jitinnair1/autoCV).

The latest version of the CV is always available and can be accessed directly:

**Latest CV Link:** (This link will point to your GitHub Pages URL, e.g., `https://rustyujjwal.github.io/my-cv/`)

## About the CV

The CV is written in LaTeX (`cv.tex`) and follows a clean, structured format, including the following sections:

* **Summary:** Aspiring Electrical Engineer with hands-on experience in embedded system prototyping and automated control systems.
* **Work Experience:** Industrial Trainee at Indian Oil Corporation Limited (June 2024 - July 2024).
* **Projects:** Detailed descriptions of the **Automated Solar Tracking System** and **IoT Weather Monitoring Station**.
* **Education:** BTech-Electrical Engineering at Odisha University Of Technology and Research.
* **Technical Skills:** C/C++, Python, JavaScript, Altium Designer, MATLAB/Simulink, Arduino, ESP32, STM32, and more.

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

### Compiling Locally

If you wish to compile the PDF on your local machine, you need to have a LaTeX distribution (like TeX Live or MiKTeX) installed.

1.  Navigate to the repository directory.
2.  Run the following command to generate `cv.pdf`:
    ```bash
    make
    ```
3.  To clean up intermediate files:
    ```bash
    make clean
    ```
4.  To clean up intermediate files and the generated PDF:
    ```bash
    make distclean
    ```

### Workflow

The automated workflow uses the `dante-ev/latex-action` to compile the `.tex` file and `peaceiris/actions-gh-pages` to deploy the resulting PDF and the `index.html` file to the `build` branch, which is configured for GitHub Pages.
