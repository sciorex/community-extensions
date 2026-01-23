# Nature Journal Template

Template following Nature journal style guidelines for high-impact scientific research across disciplines.

## Overview

Nature articles have a distinctive format characterized by:
- Very concise writing (main text typically under 3,000 words)
- Abstract limited to 150 words
- No section headers in the main body text
- Methods section separate from main text
- Extended Data section for supplementary figures/tables

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdfLaTeX or XeLaTeX
3. For submission, ensure line numbers and double spacing are enabled
4. For final version, comment out `\linenumbers` and `\doublespacing`

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{TITLE}} | Paper title (ideally 10 words or fewer) | Quantum coherence in photosynthetic complexes |
| {{AUTHOR_1}} | First author name | Jane A. Smith |
| {{AUTHOR_2}} | Second author name | Robert B. Jones |
| {{AUTHOR_3}} | Third author name | Maria C. Garcia |
| {{AFFILIATION_1}} | First institution | Department of Biology, Harvard University, Cambridge, MA, USA |
| {{AFFILIATION_2}} | Second institution | Max Planck Institute, Munich, Germany |
| {{CORRESPONDING_EMAIL}} | Corresponding author email | j.smith@harvard.edu |
| {{ABSTRACT}} | Abstract text (150 words max) | Here we show that quantum effects... |
| {{MAIN_TEXT}} | Main body of the paper | The phenomenon of... |
| {{METHODS}} | Methods section overview | Experiments were conducted using... |
| {{METHODS_DATA}} | Data collection methods | Samples were collected from... |
| {{METHODS_ANALYSIS}} | Statistical analysis methods | Data were analyzed using... |
| {{METHODS_PROCEDURES}} | Experimental procedures | The protocol consisted of... |
| {{ACKNOWLEDGEMENTS}} | Acknowledgements | We thank X for discussions... |
| {{AUTHOR_CONTRIBUTIONS}} | Author contribution statement | J.S. conceived the study... |
| {{COMPETING_INTERESTS}} | Competing interests declaration | The authors declare no competing interests. |
| {{DATA_AVAILABILITY}} | Data availability statement | Source data are available at... |
| {{CODE_AVAILABILITY}} | Code availability statement | Code is available at GitHub... |
| {{EXTENDED_DATA_FIG_1_CAPTION}} | Extended Data Figure 1 caption | Additional characterization of... |
| {{EXTENDED_DATA_TABLE_1_CAPTION}} | Extended Data Table 1 caption | Summary statistics for... |

## Structure

1. Title (concise, ideally 10 words or fewer)
2. Abstract (150 words maximum)
3. Main text (continuous prose, no section headers)
4. Methods (detailed experimental procedures)
5. References (Nature numbered style)
6. Acknowledgements
7. Author contributions
8. Competing interests
9. Data availability
10. Code availability
11. Extended Data (figures and tables)

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Standard packages: times, natbib, graphicx, hyperref, lineno, setspace
- Bibliography style: naturemag (or apalike as fallback)

## Notes

- Nature articles do NOT use section headers in the main body
- Main text should flow as continuous prose
- Methods can have subsections
- Extended Data items are peer-reviewed but appear only online
- Supplementary Information is NOT peer-reviewed

## Word Limits

- Title: ~10 words (90 characters)
- Abstract: 150 words
- Main text: 2,000-3,000 words (varies by article type)
- Methods: No strict limit but should be concise
