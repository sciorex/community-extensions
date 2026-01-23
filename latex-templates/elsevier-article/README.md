# Elsevier Article Template

Standard Elsevier journal article format. Used by hundreds of Elsevier journals across all scientific disciplines including physics, chemistry, biology, medicine, engineering, and social sciences.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdflatex:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Article title | A Novel Approach to Protein Folding Prediction |
| `{{AUTHOR_1}}` | First author name | John A. Smith |
| `{{AUTHOR_1_AFFILIATION}}` | First author institution | Department of Biochemistry, Stanford University |
| `{{AUTHOR_1_EMAIL}}` | Corresponding author email | john.smith@stanford.edu |
| `{{AUTHOR_1_ADDRESS}}` | First author address | 450 Serra Mall |
| `{{AUTHOR_1_CITY}}` | First author city | Stanford |
| `{{AUTHOR_1_POSTCODE}}` | First author postal code | CA 94305 |
| `{{AUTHOR_1_COUNTRY}}` | First author country | USA |
| `{{AUTHOR_2}}` | Second author name | Emily R. Johnson |
| `{{AUTHOR_2_AFFILIATION}}` | Second author institution | MIT |
| `{{AUTHOR_2_EMAIL}}` | Second author email | emily.johnson@mit.edu |
| `{{AUTHOR_2_ADDRESS}}` | Second author address | 77 Massachusetts Ave |
| `{{AUTHOR_2_CITY}}` | Second author city | Cambridge |
| `{{AUTHOR_2_POSTCODE}}` | Second author postal code | MA 02139 |
| `{{AUTHOR_2_COUNTRY}}` | Second author country | USA |
| `{{ABSTRACT}}` | Article abstract (max 200 words) | This paper presents a novel computational... |
| `{{KEYWORDS}}` | Up to 6 keywords separated by \sep | Protein folding \sep Machine learning \sep Computational biology |
| `{{JOURNAL_NAME}}` | Target journal name | Journal of Molecular Biology |
| `{{ACKNOWLEDGMENTS}}` | Acknowledgments text | This work was supported by NIH grant... |

## Structure

The template includes the following sections:

1. **Front Matter**
   - Title
   - Authors and affiliations
   - Abstract
   - Keywords

2. **Main Content**
   - Introduction
   - Materials and Methods
   - Results
   - Discussion
   - Conclusion

3. **Back Matter**
   - Declaration of Competing Interest
   - Data Availability
   - Acknowledgments
   - References

## Document Class Options

- `preprint` - Single column, 12pt (default for submission)
- `review` - Double line spacing for peer review
- `final,1p` - Final single column layout
- `final,3p` - Final three column layout
- `final,5p` - Final five column layout

To change the layout, modify the `\documentclass` line:

```latex
\documentclass[preprint,review,12pt]{elsarticle}  % For review
\documentclass[final,3p,times]{elsarticle}        % For final 3-column
```

## Requirements

- LaTeX distribution with `elsarticle` class (included in TeX Live and MiKTeX)
- Required packages: lineno, hyperref, graphicx, amsmath, amssymb, booktabs

## Tips

- Enable line numbers for review by uncommenting `\linenumbers`
- Use `\corref{cor1}` to mark the corresponding author
- Multiple authors can share affiliations using the same affiliation number
- Include graphical abstract using the `graphicalabstract` environment
- Add research highlights using the `highlights` environment
