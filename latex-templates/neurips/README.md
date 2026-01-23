# NeurIPS Conference Paper Template

Official NeurIPS (Neural Information Processing Systems) conference paper template. NeurIPS is the premier venue for machine learning and AI research, featuring cutting-edge work in deep learning, reinforcement learning, and computational neuroscience.

## Usage

1. **Download Required Files**: Before compiling, download the official NeurIPS style file:
   - Visit: https://neurips.cc/Conferences/2024/PaperInformation/StyleFiles
   - Download the official style package
   - Extract `neurips_2024.sty` to this directory
   - Note: Update the year in the \usepackage command for your submission year

2. **Choose Submission Mode**: Edit the \usepackage options in main.tex:
   - `[preprint]` - For arXiv preprints (shows authors, has line numbers)
   - `[final]` - For camera-ready submission (no line numbers)
   - `[nonatbib]` - If you have natbib package conflicts

3. **Replace Placeholders**: Search for `{{PLACEHOLDER}}` patterns and replace with your content

4. **Compile**: Use pdflatex and bibtex:
   ```bash
   pdflatex main
   bibtex main
   pdflatex main
   pdflatex main
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Paper title | Attention-Based Methods for Graph Learning |
| `{{AUTHOR_1}}` | First author name | Alice Johnson |
| `{{AUTHOR_1_AFFILIATION}}` | First author institution | Google DeepMind |
| `{{AUTHOR_1_EMAIL}}` | First author email | alice@deepmind.com |
| `{{AUTHOR_2}}` | Second author name | Bob Chen |
| `{{AUTHOR_2_AFFILIATION}}` | Second author institution | Stanford University |
| `{{AUTHOR_2_EMAIL}}` | Second author email | bob@stanford.edu |
| `{{AUTHOR_3}}` | Third author name | Carol Williams |
| `{{AUTHOR_3_AFFILIATION}}` | Third author institution | MIT |
| `{{AUTHOR_3_EMAIL}}` | Third author email | carol@mit.edu |
| `{{ABSTRACT}}` | Paper abstract (limited length) | We propose a novel... |
| `{{ACKNOWLEDGMENTS}}` | Acknowledgments text | We thank... |

## Structure

The template includes the following sections:

1. **Introduction** - Motivation, challenges, and contributions
2. **Related Work** - Literature review by topic (transformers, self-supervised learning, NAS)
3. **Method** - Problem setup, architecture, and training procedure
4. **Experiments** - Datasets, baselines, main results, ablations, and analysis
5. **Discussion** - Insights, limitations, and broader impact
6. **Conclusion** - Summary and future directions
7. **Appendix** (optional) - Additional results, proofs, implementation details

## Requirements

### Required Packages (included)
- `hyperref` - Hyperlinks
- `url` - URL formatting
- `booktabs` - Professional tables
- `amsfonts`, `amsmath`, `amssymb` - Mathematics
- `nicefrac`, `microtype` - Typography
- `graphicx` - Figures
- `algorithm`, `algorithmic` - Algorithms
- `subcaption` - Subfigures

### Required External Files
- `neurips_2024.sty` - NeurIPS style file (download from NeurIPS)

## Formatting Guidelines

- **Page Limit**: 9 pages (main content), unlimited references and appendix
- **Abstract**: Maximum 200 words
- **Anonymization**: Use `[preprint]` for arXiv; submission version should be anonymous
- **References**: Use natbib with plainnat style
- **Supplementary Material**: Include in appendix after references

## Tips

- Use `\citep{}` for parenthetical citations: (Author, Year)
- Use `\citet{}` for textual citations: Author (Year)
- Define custom commands for frequently used notation
- Include broader impact statement for camera-ready
- Check page limit carefully before submission

## Common Issues

1. **natbib conflicts**: Use `[nonatbib]` option
2. **Line numbers in final**: Make sure to use `[final]` option
3. **Missing style file**: Download from NeurIPS website

## License

This template structure is provided for academic use. Check NeurIPS official guidelines for current submission requirements.
