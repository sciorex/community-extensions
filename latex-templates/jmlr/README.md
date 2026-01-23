# Journal of Machine Learning Research (JMLR) Template

Official template for articles submitted to the Journal of Machine Learning Research (JMLR). JMLR is a premier open-access journal for machine learning research, known for its rigorous peer review and high-quality publications.

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
2. Write your content in each section
3. Add your references to `references.bib`
4. Compile using the commands above

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Full paper title | Statistical Learning Theory for Deep Neural Networks |
| `{{SHORT_TITLE}}` | Abbreviated title for header | Statistical Learning for DNNs |
| `{{SHORT_AUTHORS}}` | Author names for header | Smith and Jones |
| `{{AUTHOR_1}}` | First author name | Alice Smith |
| `{{AUTHOR_1_EMAIL}}` | First author email | alice@university.edu |
| `{{AUTHOR_1_AFFILIATION}}` | First author department/institution | Department of Computer Science, Stanford University |
| `{{AUTHOR_1_ADDRESS}}` | First author address | Stanford, CA 94305, USA |
| `{{AUTHOR_2}}` | Second author name | Bob Jones |
| `{{AUTHOR_2_EMAIL}}` | Second author email | bob@institute.org |
| `{{AUTHOR_2_AFFILIATION}}` | Second author institution | Machine Learning Institute |
| `{{AUTHOR_2_ADDRESS}}` | Second author address | Cambridge, MA 02139, USA |
| `{{EDITOR_NAME}}` | Action editor name | John Editor |
| `{{ABSTRACT}}` | Paper abstract | This paper presents a comprehensive theoretical... |
| `{{KEYWORDS}}` | Keywords (comma-separated) | machine learning, statistical learning, generalization bounds |
| `{{PROBLEM_DOMAIN}}` | Your research area | supervised learning with limited labels |
| `{{ACKNOWLEDGMENTS}}` | Funding and thanks | This work was supported by... |

## Structure

The template follows the standard JMLR structure:

1. **Abstract** - Summary of contributions and findings
2. **Introduction** - Motivation, problem statement, contributions
3. **Background and Related Work** - Context and prior work
4. **Proposed Method** - Your approach and algorithm
5. **Theoretical Analysis** - Formal guarantees and proofs
6. **Experiments** - Empirical evaluation
7. **Discussion** - Insights, limitations, future work
8. **Conclusion** - Summary
9. **Acknowledgments** - Funding sources
10. **Appendix** - Proofs and supplementary material
11. **References** - Bibliography

## Requirements

### Required Packages

- `jmlr2e.sty` - JMLR style file (download from JMLR website)
- `amsmath`, `amssymb`, `amsthm` - Mathematical typesetting
- `algorithm`, `algorithmic` - Algorithm formatting
- `graphicx` - Figure inclusion
- `booktabs` - Professional tables
- `hyperref` - Hyperlinks

### Style File

Download `jmlr2e.sty` from the official JMLR author information page:
https://www.jmlr.org/format/format.html

## Formatting Guidelines

### Length

- JMLR has no strict page limit
- Papers should be as long as necessary but as short as possible
- Typical papers range from 20-50 pages

### Mathematics

Use standard LaTeX environments:
```latex
\begin{theorem}
Your theorem statement.
\end{theorem}

\begin{proof}
Your proof.
\end{proof}
```

### Figures and Tables

- Place at top of page when possible
- Use vector graphics (PDF, EPS) for diagrams
- Include informative captions

### Citations

Use natbib-style citations:
- `\citep{key}` for parenthetical: (Author, Year)
- `\citet{key}` for textual: Author (Year)

## Tips for JMLR Submissions

1. **Theoretical rigor**: JMLR values theoretical contributions with formal proofs
2. **Reproducibility**: Include implementation details and consider releasing code
3. **Clear writing**: Explain intuition before formal statements
4. **Thorough experiments**: Include baselines, ablations, and error bars
5. **Literature review**: Comprehensive coverage of related work

## Additional Authors

To add more authors:

```latex
\author{\name {{AUTHOR_1}} \email {{AUTHOR_1_EMAIL}}\\
       \addr {{AUTHOR_1_AFFILIATION}}
       \AND
       \name {{AUTHOR_2}} \email {{AUTHOR_2_EMAIL}}\\
       \addr {{AUTHOR_2_AFFILIATION}}
       \AND
       \name {{AUTHOR_3}} \email {{AUTHOR_3_EMAIL}}\\
       \addr {{AUTHOR_3_AFFILIATION}}}
```

## Resources

- [JMLR Homepage](https://www.jmlr.org/)
- [JMLR Author Information](https://www.jmlr.org/author-info.html)
- [JMLR Format Guidelines](https://www.jmlr.org/format/format.html)
- [JMLR Style File](https://www.jmlr.org/format/jmlr2e.sty)
