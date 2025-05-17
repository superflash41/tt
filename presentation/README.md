# Thesis Presentation Template

A beamer for showing information about your thesis.

## Directory Structure

*   **`base/`**: core configuration files.
    *   [`base/commands.tex`](presentation/base/commands.tex): Define presentation title, author, date, and custom commands.
    *   [`base/packages.tex`](presentation/base/packages.tex): Lists LaTeX packages used.
    *   [`base/presentation.tex`](presentation/base/presentation.tex): Main LaTeX file to compile. **DO NOT MODIFY.**
    *   [`base/styles.tex`](presentation/base/styles.tex): Beamer theme and style settings.
*   **`bib/`**: holds bibliography files.
    *   [`bib/bibliography.bib`](presentation/bib/bibliography.bib): Add your BibTeX entries here.
*   **`images/`**: Store images for your presentation.
*   **`pdf/`**: Output directory for the compiled PDF.
    *   `presentation.pdf`: Final presentation.
*   **`tex/`**: Contains the content of the presentation.
    *   [`tex/main.tex`](presentation/tex/main.tex): Defines the overall structure by including section files.
    *   `tex/section-*.tex`: Files for individual sections.
    *   `tex/subsection-*.tex`: Files for subsections within sections.
    *   [`tex/contents.tex`](presentation/tex/contents.tex): Generates the table of contents.
*   **`Makefile`**: Serves for compilation. Run `make all` to build the presentation.

## How to Use

1.  **Set Metadata**:
    *   Open [`presentation/base/commands.tex`](presentation/base/commands.tex).
    *   Modify `\title`, `\subtitle`, `\author`, `\institute`, and `\date`.

2.  **Add Content**:
    *   Edit existing files in the [`presentation/tex/`](presentation/tex/) directory (e.g., [`presentation/tex/section-intro.tex`](presentation/tex/section-intro.tex), [`presentation/tex/subsection-topic.tex`](presentation/tex/subsection-topic.tex)) to add your content.
    *   To add new sections, create a `section-yourname.tex` file in [`presentation/tex/`](presentation/tex/) and include it in [`presentation/tex/main.tex`](presentation/tex/main.tex).
    *   To add new subsections, create a `subsection-yourname.tex` file in [`presentation/tex/`](presentation/tex/) and include it within a relevant section file.

3.  **Manage Bibliography**:
    *   Add your references in BibTeX format to [`presentation/bib/bibliography.bib`](presentation/bib/bibliography.bib).
    *   Use `\cite{your_bib_key}` in your `.tex` files to cite them.

4.  **Include Images**:
    *   Place image files (e.g., `.png`, `.jpg`) in the [`presentation/images/`](presentation/images/) folder.
    *   Include them in your `.tex` files.

5.  **Compile**:
    *   Navigate to the `presentation/` directory in your terminal and run `make all`.
    *   An output PDF will be generated in [`presentation/pdf/presentation.pdf`](presentation/pdf/presentation.pdf).

6.  **Clean**:
    *   To remove generated files (e.g., `.aux`, `.log`, `.pdf`), run `make clean`.