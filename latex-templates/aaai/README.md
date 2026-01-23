# AAAI Conference Paper Template

Official template for papers submitted to the AAAI Conference on Artificial Intelligence. AAAI is one of the premier venues for artificial intelligence research, covering topics from machine learning and natural language processing to robotics and multi-agent systems.

## Usage

### Compilation

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

### Quick Start

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Add your content to each section
3. Update `references.bib` with your citations
4. Compile using the commands above

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Paper title | Efficient Neural Reasoning for Knowledge Graphs |
| `{{AUTHOR_1}}` | First author name | Jane Smith |
| `{{AUTHOR_1_AFFILIATION}}` | First author institution | Stanford University |
| `{{AUTHOR_1_EMAIL}}` | First author email | jane.smith@stanford.edu |
| `{{AUTHOR_2}}` | Second author name | John Doe |
| `{{AUTHOR_2_AFFILIATION}}` | Second author institution | MIT |
| `{{AUTHOR_2_EMAIL}}` | Second author email | john.doe@mit.edu |
| `{{ABSTRACT}}` | Paper abstract (150-250 words) | This paper presents a novel approach... |
| `{{PROBLEM_DOMAIN}}` | Your research problem area | knowledge graph reasoning |
| `{{ACKNOWLEDGMENTS}}` | Funding and acknowledgments | This work was supported by NSF Grant... |

## Structure

The template includes the following standard AAAI sections:

1. **Abstract** - Concise summary of the paper
2. **Introduction** - Problem motivation and contributions
3. **Related Work** - Survey of relevant prior work
4. **Problem Formulation** - Formal problem definition
5. **Proposed Method** - Your approach and algorithm
6. **Experiments** - Empirical evaluation
7. **Discussion** - Analysis and limitations
8. **Conclusion** - Summary and future work
9. **Acknowledgments** - Funding sources
10. **References** - Bibliography

## Requirements

### Required Packages

- `aaai24.sty` - AAAI style file (download from AAAI website)
- `times`, `helvet`, `courier` - Standard fonts
- `natbib` - Citation management
- `amsmath`, `amssymb` - Mathematical symbols
- `algorithm`, `algorithmic` - Algorithm formatting
- `graphicx` - Figure inclusion
- `booktabs` - Professional tables

### Page Limits

- **Main paper**: 7 pages (excluding references)
- **References**: Unlimited additional pages
- **Supplementary**: Allowed but not guaranteed review

## Formatting Notes

1. **Two-column format**: AAAI uses a two-column layout
2. **Paper size**: US Letter (8.5" x 11")
3. **Font**: Times Roman, 10pt
4. **Margins**: Set by the aaai24.sty file
5. **Anonymous submission**: Remove author information for initial submission

## Tips

- Keep abstract under 250 words
- Use `\citep{}` for parenthetical citations and `\citet{}` for textual citations
- Place figures and tables at the top of columns
- Number all equations, figures, and tables
- Include page numbers during submission

## Additional Authors

To add more authors, extend the author block:

```latex
\author{
    {{AUTHOR_1}}\textsuperscript{\rm 1},
    {{AUTHOR_2}}\textsuperscript{\rm 2},
    {{AUTHOR_3}}\textsuperscript{\rm 3}\\
}

\affiliations{
    \textsuperscript{\rm 1}{{AUTHOR_1_AFFILIATION}}\\
    \textsuperscript{\rm 2}{{AUTHOR_2_AFFILIATION}}\\
    \textsuperscript{\rm 3}{{AUTHOR_3_AFFILIATION}}\\
    {{AUTHOR_1_EMAIL}}, {{AUTHOR_2_EMAIL}}, {{AUTHOR_3_EMAIL}}
}
```

## Resources

- [AAAI Author Kit](https://aaai.org/authorkit/)
- [AAAI Formatting Guidelines](https://aaai.org/conference/aaai/)
- [LaTeX Tips for AAAI](https://aaai.org/authorkit/latex-instructions/)
