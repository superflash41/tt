# Report Template

A report template you can use for delivers E1, E2 and E3.

## Usage

### 1. Customize Information
Edit [`base/commands.tex`](/report/base/commands.tex) to set your report's metadata (title, author, course, etc.).

### 2. Add Contents
Edit the `.tex` files within the `tex/` directory to write the content of your report. For example, edit [`tex/general.tex`](/report/tex/general.tex) for the generalities section, [`tex/sota.tex`](/report/tex/sota.tex) for the state-of-the-art, etc.

Add bibliographic entries to [`bib/bibliography.bib`](/report/bib/bibliography.bib).

Place any images you use in the `images/` folder.

### 3. Compile
To generate the PDF report, run `make all`. The output PDF will be `pdf/document.pdf`.
