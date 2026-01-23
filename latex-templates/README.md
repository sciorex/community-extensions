# LaTeX Templates

Professional LaTeX document templates for academic papers, presentations, theses, CVs, and more. **35 templates** across 7 categories with multi-page preview images. Available through the Sciorex Community modal with placeholder value substitution.

## Available Templates (35)

### Academic Papers (15)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [IEEE Conference](ieee/) | Standard IEEE conference paper for engineering and CS | Intermediate |
| [ACM Conference](acm/) | Official ACM sigconf format | Intermediate |
| [ACM CHI](acm-chi/) | ACM CHI for Human-Computer Interaction | Intermediate |
| [arXiv Preprint](arxiv/) | Clean arXiv-compatible preprint | Beginner |
| [Springer LNCS](springer-lncs/) | Springer Lecture Notes in Computer Science | Intermediate |
| [NeurIPS](neurips/) | NeurIPS machine learning conference | Intermediate |
| [CVPR/ICCV/ECCV](cvpr/) | IEEE Computer Vision conferences | Intermediate |
| [ICLR](iclr/) | ICLR deep learning conference | Intermediate |
| [AAAI](aaai/) | AAAI artificial intelligence conference | Intermediate |
| [JMLR](jmlr/) | Journal of Machine Learning Research | Intermediate |
| [Elsevier Article](elsevier-article/) | Elsevier journal format | Intermediate |
| [Nature](nature/) | Nature journal style | Advanced |
| [APA 7th Edition](apa7/) | APA format for psychology/social sciences | Intermediate |
| [RevTeX/APS](revtex/) | APS physics journals (PRL, PRA-E) | Intermediate |
| [ACS Article](acs-article/) | American Chemical Society format | Intermediate |

### Thesis & Dissertation (3)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [PhD Thesis](phd-thesis/) | Complete PhD dissertation with front matter, chapters, appendices | Advanced |
| [Master's Thesis](masters-thesis/) | Master's thesis with chapter structure | Intermediate |
| [Thesis Proposal](thesis-proposal/) | Graduate thesis/dissertation proposal | Intermediate |

### Presentations & Posters (4)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [Beamer](beamer/) | Classic Beamer presentation | Beginner |
| [Beamer Metropolis](beamer-metropolis/) | Modern minimal Metropolis theme | Beginner |
| [Poster A0](poster-a0/) | A0 conference poster (841×1189mm) | Intermediate |
| [Poster A1](poster-a1/) | A1 conference poster (594×841mm) | Intermediate |

### CV & Resume (2)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [Academic CV](academic-cv/) | Comprehensive academic CV for faculty positions | Beginner |
| [Modern Resume](resume-modern/) | Clean one-page industry resume | Beginner |

### Teaching Materials (5)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [Syllabus](syllabus/) | Course syllabus with schedule and policies | Beginner |
| [Lecture Notes](lecture-notes/) | Formatted notes with theorems and examples | Intermediate |
| [Problem Set](problem-set/) | Homework/assignment template | Beginner |
| [Exam](exam/) | Exam paper with point values and answer spaces | Intermediate |
| [Lab Report](lab-report/) | Scientific lab report for courses | Beginner |

### General Documents (4)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [Basic Article](basic-article/) | Simple general-purpose article | Beginner |
| [Technical Report](technical-report/) | Technical documentation for institutions | Beginner |
| [White Paper](white-paper/) | Policy/industry white paper | Intermediate |
| [Literature Review](literature-review/) | Survey/review paper structure | Intermediate |

### Correspondence (2)

| Template | Description | Difficulty |
|----------|-------------|------------|
| [Cover Letter](cover-letter/) | Professional job/academic cover letter | Beginner |
| [Research Proposal](research-proposal/) | Grant/research funding proposal | Intermediate |

## Template Structure

Each template directory contains:

```
template-name/
├── main.tex              # Main LaTeX document (required)
├── references.bib        # BibTeX bibliography file (optional)
├── preview.png           # First page preview (main thumbnail)
├── preview-1.png         # Page 2 preview (if multi-page)
├── preview-2.png         # Page 3 preview, etc.
├── README.md             # Template-specific documentation with placeholders table
└── *.cls/*.sty           # Document class or style files (if needed)
```

Multi-page templates include preview images for all pages (`preview.png`, `preview-1.png`, `preview-2.png`, etc.).

## Placeholder Syntax

Templates support placeholder substitution for easy customization. Use double curly braces for placeholders:

```latex
\title{{{TITLE}}}
\author{{{AUTHOR}}}
\email{{{EMAIL}}}
```

Common placeholders:
- `{{TITLE}}` - Document or paper title
- `{{AUTHOR}}` - Author name
- `{{EMAIL}}` - Contact email
- `{{DATE}}` - Current date (if needed)

The scaffolding workflow will prompt users to provide values for these placeholders before creating the template files.

## Contributing Templates

We welcome contributions of new LaTeX templates! Follow these guidelines:

### 1. Template Requirements

- **Compiles successfully** - Template must compile without errors using standard LaTeX distributions (TeX Live, MiKTeX)
- **Well-documented** - Include a README.md explaining the template's purpose and structure
- **Preview image** - Include a preview.png showing the compiled output (800x1000px recommended)
- **Placeholder support** - Use `{{PLACEHOLDER}}` syntax for customizable values
- **Clean structure** - Well-organized, commented code following LaTeX best practices

### 2. File Organization

```
your-template-name/
├── main.tex              # Main document with placeholder syntax
├── references.bib        # Sample bibliography entries
├── preview.png           # Screenshot of compiled PDF
├── README.md             # Template documentation
└── [optional files]      # .cls, .sty, or other required files
```

### 3. Adding to Index

Update `latex-templates/index.json` with your template metadata:

```json
{
  "id": "your-template-id",
  "name": "Your Template Name",
  "description": "Brief description of the template and its use cases",
  "category": "academic|general|presentation",
  "difficulty": "beginner|intermediate|advanced",
  "tags": ["tag1", "tag2", "tag3"],
  "version": "1.0.0",
  "author": "Your Name or Organization",
  "downloadUrl": "latex-templates/your-template-name",
  "previewUrl": "latex-templates/your-template-name/preview.png",
  "files": ["main.tex", "references.bib", "README.md"],
  "placeholders": {
    "TITLE": "Document title",
    "AUTHOR": "Author name",
    "EMAIL": "Contact email"
  },
  "requiredPackages": ["package1", "package2"],
  "updatedAt": "2026-01-21T00:00:00Z"
}
```

### 4. Testing

Before submitting:

1. Test compilation with pdflatex, xelatex, or lualatex
2. Verify all placeholders work correctly
3. Test the template through Sciorex Community modal (if possible)
4. Ensure preview.png accurately represents the compiled output
5. Check that all required packages are documented

### 5. Submission Process

1. Fork the repository
2. Create your template directory in `latex-templates/`
3. Add your template metadata to `index.json`
4. Test your template locally
5. Submit a merge request with:
   - Clear description of the template
   - Compilation instructions
   - Any special requirements or notes

## Template Categories

- **academic** - Academic papers, conference submissions, journal articles
- **general** - General-purpose documents, reports, essays
- **presentation** - Slides, presentations, beamer templates
- **thesis** - Thesis and dissertation templates
- **cv** - CVs and resumes
- **letter** - Formal letters and correspondence

## Best Practices

1. **Keep it simple** - Templates should be easy to understand and modify
2. **Use standard packages** - Prefer widely-available LaTeX packages
3. **Document dependencies** - List all required packages in the README
4. **Provide examples** - Include sample content that demonstrates features
5. **Test compilation** - Ensure templates compile on standard distributions
6. **Semantic naming** - Use clear, descriptive placeholder names
7. **Follow conventions** - Adhere to LaTeX best practices and style guidelines

## Questions?

- Open an issue for questions about contributing templates
- See [CONTRIBUTING.md](../CONTRIBUTING.md) for general contribution guidelines
- Join our [Discord](https://discord.gg/zSjPjA5j) for community support

## License

All templates are licensed under the MIT License unless otherwise specified in the template's README.
