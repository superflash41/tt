# Report Template

A report template you can use for delivers E1, E2 and E3.

## Structure

*   `base/`: Core LaTeX configuration files.
    *   [`base/commands.tex`](/base/commands.tex): Define common commands like author, title, course, etc.
    *   [`base/packages.tex`](/report/base/packages.tex)
    *   [`base/styles.tex`](/base/styles.tex)
    *   [`base/document.tex`](/base/document.tex)
*   `tex/`: Contents of the report.
    *   [`tex/main.tex`](/tex/main.tex): The main content file that includes other `.tex` files.
    *   Other `.tex` files in this directory represent different sections of the report (e.g., [`tex/general.tex`](/tex/general.tex), [`tex/methodology.tex`](/tex/methodology.tex)). **These need edition.**
*   `bib/`: Contains bibliography files.
    *   [`bib/bibliography.bib`](/report/bib/bibliography.bib): Add BibTeX references here.
*   `images/`: Add images here.
*   `pdf/`
*   `Makefile`

## Usage

### 1. Customize Information
Edit [`base/commands.tex`](/report/base/commands.tex) to set your report's metadata (title, author, course, etc.).

### 2. Add Contents
Edit the `.tex` files within the `tex/` directory to write the content of your report. For example, edit [`tex/general.tex`](/report/tex/general.tex) for the generalities section, [`tex/sota.tex`](/report/tex/sota.tex) for the state-of-the-art, etc.

Add bibliographic entries to [`bib/bibliography.bib`](/report/bib/bibliography.bib).

Place any images you use in the `images/` folder.

### 3. Compile
To generate the PDF report, run `make all`. The output PDF will be `pdf/document.pdf`.