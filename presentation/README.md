# Thesis Presentation Template

A beamer for showing information about your thesis.

## How to Use

#### 1. Set Metadata
*   Open [`presentation/base/commands.tex`](presentation/base/commands.tex) and modify `\title`, `\subtitle`, `\author`, `\institute`, and `\date`.

#### 2. Add Contents
*   Edit existing files in the [`presentation/tex/`](presentation/tex/) directory (e.g., [`presentation/tex/section-intro.tex`](presentation/tex/section-intro.tex), [`presentation/tex/subsection-topic.tex`](presentation/tex/subsection-topic.tex)) to add your content.
*   To add new sections, create a `section-yourname.tex` file in [`presentation/tex/`](presentation/tex/) and include it in [`presentation/tex/main.tex`](presentation/tex/main.tex).
*   To add new subsections, create a `subsection-yourname.tex` file in [`presentation/tex/`](presentation/tex/) and include it within a relevant section file.
*   Add references in BibTeX format to [`presentation/bib/bibliography.bib`](presentation/bib/bibliography.bib).
*   Place image files (e.g., `.png`, `.jpg`) in the [`presentation/images/`](presentation/images/) folder.

#### 3. Compile
*   Navigate to the `presentation/` directory and run `make all`.
*   An output PDF will be generated in [`presentation/pdf/presentation.pdf`](presentation/pdf/presentation.pdf).
