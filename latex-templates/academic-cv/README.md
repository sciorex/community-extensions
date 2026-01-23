# Academic Curriculum Vitae Template

A comprehensive academic CV template for faculty positions, grant applications, tenure review, and academic appointments. This template includes all standard sections expected in an academic CV and is designed for researchers at any career stage.

## Usage

1. **Replace Placeholders**: Search for `{{PLACEHOLDER}}` patterns in the header section and replace with your information

2. **Customize Sections**:
   - Remove sections that don't apply to your career stage
   - Add entries to each section following the provided format
   - Reorder sections based on your priorities or position requirements

3. **Compile**: Use pdflatex:
   ```bash
   pdflatex main
   pdflatex main  # Run twice for proper formatting
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{NAME}}` | Your full name | Dr. Jane Elizabeth Smith |
| `{{TITLE}}` | Current title/position | Associate Professor |
| `{{DEPARTMENT}}` | Department name | Department of Computer Science |
| `{{UNIVERSITY}}` | University name | Stanford University |
| `{{ADDRESS}}` | Office address | Gates Building, Room 123, Stanford, CA 94305 |
| `{{EMAIL}}` | Email address | jsmith@stanford.edu |
| `{{PHONE}}` | Phone number | (650) 123-4567 |
| `{{WEBSITE}}` | Personal website URL | https://janesmith.stanford.edu |
| `{{ORCID}}` | ORCID identifier | 0000-0001-2345-6789 |

## Structure

The template includes the following sections:

1. **Header** - Name, title, contact information
2. **Education** - Degrees with details
3. **Academic Positions** - Employment history
4. **Research Interests** - Brief list of areas
5. **Publications**
   - Journal Articles
   - Conference Papers
   - Book Chapters
   - Preprints and Technical Reports
6. **Grants and Funding** - Awards with amounts
7. **Teaching Experience** - Courses and curriculum development
8. **Students Supervised** - PhD, Master's, Undergraduate
9. **Professional Service** - Editorial, conference, departmental
10. **Awards and Honors**
11. **Invited Talks**
12. **Professional Memberships**
13. **Technical Skills**
14. **References**

## Requirements

### Required Packages (included in template)
- `geometry` - Page margins
- `parskip` - Paragraph spacing
- `enumitem` - List formatting
- `xcolor` - Colors
- `hyperref` - Hyperlinks
- `tabularx`, `ltablex` - Tables
- `titlesec` - Section formatting

### Compilation
- pdfLaTeX (standard)

## Customization

### Adjusting Margins
Edit the geometry package options:
```latex
\usepackage[top=0.75in, bottom=0.75in, left=0.75in, right=0.75in]{geometry}
```

### Changing Colors
Modify the custom colors:
```latex
\definecolor{headercolor}{RGB}{0, 51, 102}  % Header color
\definecolor{rulecolor}{RGB}{150, 150, 150}  % Rule color
```

### Adding Icons
Uncomment and use FontAwesome5:
```latex
\usepackage{fontawesome5}
% Then use: \faEnvelope{} for email icon, \faPhone{} for phone, etc.
```

### Section Order
Reorder sections in the document based on:
- Your career stage (students emphasize education; faculty emphasize research)
- Position requirements (teaching positions emphasize teaching)
- Your strengths (lead with your strongest sections)

## Tips

- **Publications**: Use reverse chronological order (newest first)
- **Bold your name** in author lists for easy scanning
- **Be consistent** with formatting throughout
- **Keep it concise**: One-line descriptions where possible
- **Update regularly**: Academic CVs grow over time
- **Tailor for applications**: Emphasize relevant sections

### Career Stage Guidance

**Graduate Students/Postdocs:**
- Emphasize Education, Publications, Awards
- Include all conference presentations
- List all research experience

**Assistant Professors:**
- Emphasize Publications, Grants, Teaching
- Focus on independent work
- Include student supervision

**Senior Faculty:**
- Emphasize major publications and impact
- Highlight leadership roles
- Include invited talks selectively

## Common Sections to Add

Depending on your field and application, you may want to add:

- **Patents**
- **Software/Code Releases**
- **Media Coverage**
- **Industry Experience**
- **Consulting**
- **Outreach Activities**
- **Languages**
- **Certifications**

## License

This template is provided for academic use. Customize freely for your needs.
