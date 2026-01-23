# PhD Thesis/Dissertation Template

A comprehensive PhD thesis/dissertation template with front matter, chapters, appendices, and bibliography. This template is customizable for different university requirements and provides a professional structure for doctoral work.

## Usage

1. **Review University Requirements**: Before using this template, check your university's specific formatting requirements (margins, spacing, font size, etc.)

2. **Customize the Preamble**: Edit `main.tex` to adjust:
   - Page margins (geometry package)
   - Line spacing (setspace package)
   - Citation style (biblatex options)
   - Header/footer format (fancyhdr)

3. **Replace Placeholders**: Search for `{{PLACEHOLDER}}` patterns and replace with your content

4. **Add Chapters**: Copy `chapter1.tex` or `chapter2.tex` as templates for additional chapters and include them in `main.tex`

5. **Compile**: Use pdflatex and biber (for biblatex):
   ```bash
   pdflatex main
   biber main
   pdflatex main
   pdflatex main
   ```

## File Structure

```
phd-thesis/
├── main.tex              # Main document (compile this)
├── references.bib        # Bibliography database
├── README.md             # This file
├── front/
│   └── abstract.tex      # Abstract page
├── chapters/
│   ├── chapter1.tex      # Introduction chapter
│   └── chapter2.tex      # Literature review chapter
└── back/
    └── appendix.tex      # Appendix material
```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Thesis title | Deep Learning Methods for Medical Image Analysis |
| `{{AUTHOR}}` | Your full name | John Alexander Smith |
| `{{DEGREE}}` | Degree being awarded | Doctor of Philosophy |
| `{{FIELD}}` | Field of study | Computer Science |
| `{{UNIVERSITY}}` | University name | Stanford University |
| `{{DEPARTMENT}}` | Department name | Department of Computer Science |
| `{{ADVISOR}}` | Advisor's name | Professor Jane Doe |
| `{{YEAR}}` | Graduation year | 2024 |
| `{{MONTH}}` | Graduation month | May |
| `{{ABSTRACT}}` | Thesis abstract | This dissertation investigates... |
| `{{KEYWORDS}}` | Keywords for abstract | machine learning, medical imaging |
| `{{DEDICATION}}` | Dedication text | To my family... |
| `{{ACKNOWLEDGMENTS}}` | Acknowledgments text | I would like to thank... |

## Structure

### Front Matter
- Title page
- Copyright page
- Abstract
- Dedication (optional)
- Acknowledgments
- Table of Contents
- List of Figures
- List of Tables

### Main Chapters
1. **Introduction** - Background, problem statement, research questions, contributions, dissertation structure
2. **Literature Review** - Theoretical foundations, related work, research gaps
3. **Methodology** (add as needed)
4. **Experiments/Results** (add as needed)
5. **Discussion** (add as needed)
6. **Conclusion** (add as needed)

### Back Matter
- References (bibliography)
- Appendices

## Requirements

### Required Packages (included in template)
- `geometry` - Page layout
- `setspace` - Line spacing
- `fancyhdr` - Headers and footers
- `amsmath`, `amssymb`, `amsthm` - Mathematics
- `graphicx` - Figures
- `booktabs`, `longtable` - Tables
- `algorithm`, `algorithmic` - Algorithms
- `hyperref` - Hyperlinks
- `biblatex` - Bibliography management

### Compilation Requirements
- pdfLaTeX
- Biber (for biblatex)

## Customization

### Page Layout
Edit the geometry package options in `main.tex`:
```latex
\usepackage[top=1in, bottom=1in, left=1.5in, right=1in]{geometry}
```

### Line Spacing
The template uses double spacing by default. Modify with:
```latex
\singlespacing   % Single spacing
\onehalfspacing  % 1.5 spacing
\doublespacing   % Double spacing
```

### Citation Style
Change the biblatex style option:
```latex
\usepackage[backend=biber,style=apa]{biblatex}  % APA style
\usepackage[backend=biber,style=ieee]{biblatex}  % IEEE style
\usepackage[backend=biber,style=chicago-authordate]{biblatex}  % Chicago
```

### Adding Chapters
1. Create a new file in `chapters/` (e.g., `chapter3.tex`)
2. Add `\include{chapters/chapter3}` in `main.tex`
3. Use `\chapter{Title}` and `\label{ch:label}` at the start

## Tips

- Use `\label{ch:name}` for chapter labels and `\ref{ch:name}` for cross-references
- Use theorem environments for formal statements: `theorem`, `lemma`, `definition`, `example`
- Keep figures in a separate `figures/` directory
- Use `\cite{key}` for citations with biblatex
- Run biber instead of bibtex when using biblatex

## Common Issues

1. **Bibliography not showing**: Ensure you run biber (not bibtex) between pdflatex runs
2. **Cross-references showing "??"**: Run pdflatex twice to resolve references
3. **TOC not updated**: Run pdflatex twice after adding/removing chapters

## License

This template is provided for academic use. Customize freely for your institution's requirements.
