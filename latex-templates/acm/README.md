# ACM Conference Template

This template provides a starting point for ACM conference papers following the official ACM article format (sigconf style).

## Prerequisites

- A LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- The acmart document class (available from ACM or most TeX distributions)

## Getting Started

1. Open `main.tex` in your LaTeX editor
2. Replace the placeholders:
   - `{{TITLE}}` - Your paper title
   - `{{AUTHOR}}` - Your name
   - `{{EMAIL}}` - Your email address
3. Update the conference information and metadata
4. Modify the institution and affiliation information
5. Update the CCS concepts and keywords
6. Write your content in each section
7. Add your references to `references.bib`
8. Compile with: `pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex`

## Template Structure

- `main.tex` - Main document file
- `references.bib` - Bibliography database
- `acmart.cls` - ACM article document class (placeholder - download from ACM or use from your TeX distribution)
- `preview.png` - Template preview image

## Key Features

- ACM sigconf format for conference papers
- Proper citation support with BibTeX
- CCS concepts classification
- Author/affiliation blocks
- Standard ACM paper structure

## Official Documentation

For the official acmart documentation and latest class files, visit:
https://www.acm.org/publications/proceedings-template

## License

This template follows ACM's template usage guidelines. The acmart class is copyright ACM.
