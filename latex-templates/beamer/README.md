# Beamer Presentation Template

This template provides a professional starting point for academic and technical presentations using the Beamer class.

## Prerequisites

- A LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Beamer class (included with most LaTeX distributions)

## Getting Started

1. Open `main.tex` in your LaTeX editor
2. Replace the placeholders:
   - `{{TITLE}}` - Your presentation title
   - `{{AUTHOR}}` - Your name
   - `{{EMAIL}}` - Your email address
3. Update the institution name
4. Modify or add slides as needed
5. Add your references to `references.bib`
6. Compile with: `pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex`

## Template Structure

- `main.tex` - Main presentation file
- `references.bib` - Bibliography database
- `preview.png` - Template preview image

## Key Features

- Madrid theme with professional appearance
- Title slide with author and institution
- Automatic table of contents
- Multiple slide types (itemize, enumerate, blocks, columns)
- Support for figures and tables
- Bibliography support
- Section organization
- Thank you slide with contact information

## Customization

You can easily customize:
- Theme: Change `\usetheme{Madrid}` to other themes (Berlin, Copenhagen, Warsaw, etc.)
- Color: Change `\usecolortheme{default}` to other colors (dolphin, beaver, crane, etc.)
- Slide layout: Add or remove sections and frames
- Blocks: Use `block`, `alertblock`, or `exampleblock` for emphasis

## Slide Types

The template includes examples of:
- Title frames
- Itemized lists
- Enumerated lists
- Block environments
- Multi-column layouts
- Tables with booktabs
- Figure placeholders
- Bibliography frames

## Tips

- Keep slides simple and focused
- Use bullet points instead of long paragraphs
- Include visual elements (figures, diagrams)
- Limit text per slide for better readability
- Use animations sparingly
- Test your presentation before presenting

## License

This template is free to use and modify for any purpose.
