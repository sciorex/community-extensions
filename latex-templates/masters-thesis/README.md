# Master's Thesis Template

A comprehensive Master's thesis template with multi-file structure. Suitable for MS, MA, MEng, and similar graduate degrees. Features proper front matter, chapters, and back matter organization.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Edit individual chapter files in the `chapters/` directory
3. Compile with pdflatex:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Thesis title | Machine Learning Approaches for Climate Prediction |
| `{{AUTHOR}}` | Your full name | Jane Elizabeth Smith |
| `{{DEGREE}}` | Degree name | Master of Science |
| `{{FIELD}}` | Field of study | Computer Science |
| `{{UNIVERSITY}}` | University name | University of California, Berkeley |
| `{{DEPARTMENT}}` | Department name | Department of Electrical Engineering and Computer Sciences |
| `{{ADVISOR}}` | Advisor's name | Professor Robert A. Johnson, Ph.D. |
| `{{YEAR}}` | Graduation year | 2024 |
| `{{MONTH}}` | Graduation month | May |
| `{{COMMITTEE_MEMBER_1}}` | First committee member | Professor Maria Garcia, Ph.D. |
| `{{COMMITTEE_MEMBER_2}}` | Second committee member | Professor David Chen, Ph.D. |
| `{{ACKNOWLEDGMENTS}}` | Acknowledgments text | I would like to thank my advisor... |
| `{{ABSTRACT}}` | Thesis abstract | This thesis presents novel methods for... |
| `{{KEYWORDS}}` | Keywords for the abstract | machine learning, climate science, neural networks |

## File Structure

```
masters-thesis/
├── main.tex              # Main document file
├── references.bib        # Bibliography database
├── front/
│   └── abstract.tex      # Abstract page
├── chapters/
│   ├── introduction.tex  # Chapter 1: Introduction
│   ├── background.tex    # Chapter 2: Background and Related Work
│   ├── methodology.tex   # Chapter 3: Methodology
│   ├── results.tex       # Chapter 4: Results and Discussion
│   └── conclusion.tex    # Chapter 5: Conclusion
└── README.md
```

## Structure

### Front Matter
- Title page
- Approval page
- Abstract
- Acknowledgments
- Table of Contents
- List of Figures
- List of Tables

### Main Content
- Chapter 1: Introduction
- Chapter 2: Background and Related Work
- Chapter 3: Methodology
- Chapter 4: Results and Discussion
- Chapter 5: Conclusion

### Back Matter
- Bibliography
- Appendices

## Customization

### Adding/Removing Chapters

To add a new chapter:
1. Create a new file in `chapters/` (e.g., `chapters/newchapter.tex`)
2. Add `\include{chapters/newchapter}` in main.tex

To remove a chapter:
1. Comment out or delete the corresponding `\include` line in main.tex

### Changing Formatting

- **Line spacing**: Modify `\doublespacing` to `\onehalfspacing` or `\singlespacing`
- **Margins**: Adjust the `geometry` package options
- **Font size**: Change `12pt` in documentclass to `11pt` or `10pt`

### Adding Appendices

Additional appendices can be added after the `\appendix` command in main.tex:

```latex
\appendix
\chapter{Supplementary Materials}
\chapter{Code Listings}
\chapter{Additional Data}
```

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Required packages: inputenc, fontenc, lmodern, geometry, setspace, graphicx, amsmath, amssymb, amsthm, booktabs, caption, subcaption, hyperref, fancyhdr, tocloft, tocbibind, appendix

## Tips

- Keep each chapter in a separate file for easier management
- Use `\label` and `\ref` for cross-references between chapters
- Add figures to a `figures/` directory for organization
- Use consistent citation style throughout
- Check your university's specific formatting requirements
