# Thesis Presentation Template

A beamer for showing information about your thesis.

## How to Use

#### 1. Set Metadata
*   Open [`base/commands.tex`](base/commands.tex) and modify `\title`, `\subtitle`, `\author`, `\institute`, and `\date`.

#### 2. Add Contents
*   Edit existing files in the [`tex/`](tex/) directory (e.g., [`tex/section-intro.tex`](tex/section-intro.tex), [`tex/subsection-topic.tex`](tex/subsection-topic.tex)) to add your content.
*   To add new sections, create a `section-yourname.tex` file in [`tex/`](tex/) and include it in [`tex/main.tex`](tex/main.tex).
*   To add new subsections, create a `subsection-yourname.tex` file in [`presentation/tex/`](presentation/tex/) and include it within a relevant section file.
*   Add references in BibTeX format to [`bib/bibliography.bib`](bib/bibliography.bib).
*   Place image files (e.g., `.png`, `.jpg`) in the [`images/`](images/) folder.

#### 3. Compile
*   Navigate to the `presentation/` directory and run `make all`.
*   An output PDF will be generated in [`pdf/presentation.pdf`](pdf/presentation.pdf).
