# LaTeX Templates

Professional LaTeX document templates for academic papers, presentations, and general-purpose documents. These templates are available through the Sciorex Community modal and can be scaffolded directly into your workspace with placeholder value substitution.

## Available Templates

### Academic Papers

- **IEEE Conference Paper** - Standard IEEE conference paper template for engineering and computer science conferences
- **ACM Conference Paper** - Official ACM conference paper template (sigconf format) for ACM conferences and publications
- **arXiv Preprint** - Clean template for arXiv preprints compatible with arXiv submission requirements
- **Basic Article** - Simple article template for essays, reports, documentation, and general-purpose documents

### Presentations

- **Beamer Presentation** - Professional presentation template for academic and technical talks

## Template Structure

Each template directory must contain:

```
template-name/
├── main.tex              # Main LaTeX document (required)
├── references.bib        # BibTeX bibliography file (optional)
├── preview.png           # Preview image (800x1000 recommended)
├── README.md             # Template-specific documentation
└── *.cls/*.sty           # Document class or style files (if needed)
```

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
