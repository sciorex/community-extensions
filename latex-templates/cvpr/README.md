# CVPR/ICCV/ECCV Conference Paper Template

Template for IEEE Computer Vision conferences including CVPR (Conference on Computer Vision and Pattern Recognition), ICCV (International Conference on Computer Vision), ECCV (European Conference on Computer Vision), and WACV (Winter Conference on Applications of Computer Vision). These are the premier venues for computer vision research.

## Usage

1. **Download Required Files**: Before compiling, download the official CVPR style file:
   - Visit: https://cvpr.thecvf.com/Conferences/2024/AuthorGuidelines
   - Download the official LaTeX template package
   - Extract `cvpr.sty` to this directory
   - Note: Style files may vary slightly between conferences/years

2. **Set Paper ID**: For camera-ready submission, update the paper ID:
   ```latex
   \def\cvprPaperID{1234}  % Your assigned paper ID
   ```

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
| `{{TITLE}}` | Paper title | Vision Transformers for Dense Prediction |
| `{{PAPER_ID}}` | Paper ID (for camera-ready) | 1234 |
| `{{AUTHOR_1}}` | First author name | Alice Johnson |
| `{{AUTHOR_1_AFFILIATION}}` | First author institution | Google Research |
| `{{AUTHOR_1_EMAIL}}` | First author email | alice@google.com |
| `{{AUTHOR_2}}` | Second author name | Bob Chen |
| `{{AUTHOR_2_AFFILIATION}}` | Second author institution | Stanford University |
| `{{AUTHOR_2_EMAIL}}` | Second author email | bob@stanford.edu |
| `{{AUTHOR_3}}` | Third author name | Carol Williams |
| `{{AUTHOR_3_AFFILIATION}}` | Third author institution | Meta AI |
| `{{AUTHOR_3_EMAIL}}` | Third author email | carol@meta.com |
| `{{ABSTRACT}}` | Paper abstract | We present a novel... |
| `{{ACKNOWLEDGMENTS}}` | Acknowledgments text | We thank... |

## Structure

The template includes the following sections:

1. **Introduction** - Motivation, challenges, and contributions
2. **Related Work** - CNNs, Vision Transformers, Self-supervised learning, Detection/Segmentation
3. **Method** - Overview, feature extraction, proposed module, loss function
4. **Experiments**
   - Datasets (ImageNet, COCO, ADE20K)
   - Implementation details
   - Main results with tables
   - Ablation studies
   - Qualitative results
5. **Discussion** - Efficiency, limitations, failure cases
6. **Conclusion** - Summary and future work

## Requirements

### Required Packages (included)
- `times` - Times font
- `epsfig`, `graphicx` - Figures
- `amsmath`, `amssymb` - Mathematics
- `booktabs` - Professional tables
- `multirow` - Multi-row table cells
- `subcaption` - Subfigures
- `algorithm`, `algorithmic` - Algorithms
- `hyperref` - Hyperlinks

### Required External Files
- `cvpr.sty` - CVPR style file (download from conference website)

## Formatting Guidelines

- **Page Limit**: 8 pages (main content), unlimited references
- **Paper Size**: Letter (8.5 x 11 inches)
- **Columns**: Two-column format
- **Font Size**: 10pt
- **Abstract**: Keep concise, typically 150-200 words
- **Anonymization**: Remove author info for submission; add for camera-ready

## Tips

- Use `\eg` and `\ie` for proper formatting of e.g. and i.e.
- Include figure placeholders with proper sizing during writing
- Check supplementary material guidelines for additional content
- Use `\cite{}` for numbered citations
- Tables should fit within column width or span both columns

## Conference-Specific Notes

### CVPR
- Main venue for computer vision
- Usually held in June
- Accepts both oral and poster presentations

### ICCV
- Held every two years (odd years)
- Similar format to CVPR

### ECCV
- European venue, held every two years (even years)
- Uses Springer LNCS for proceedings

### WACV
- Winter conference, typically January
- Focus on applications

## License

This template structure is provided for academic use. Check the official conference guidelines for current submission requirements.
