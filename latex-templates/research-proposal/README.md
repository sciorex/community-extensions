# Research Proposal Template

A professional research or grant proposal template. Suitable for PhD research proposals, grant applications (NSF, NIH, etc.), and project proposals. Includes all standard sections required by most funding agencies.

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
| `{{TITLE}}` | Project title | Investigating Neural Mechanisms of Decision Making Under Uncertainty |
| `{{PI_NAME}}` | Principal Investigator name | Dr. Sarah M. Thompson |
| `{{PI_AFFILIATION}}` | PI's institution | Harvard University |
| `{{PI_DEPARTMENT}}` | PI's department | Department of Psychology |
| `{{PI_EMAIL}}` | PI's email address | sarah.thompson@harvard.edu |
| `{{FUNDING_AGENCY}}` | Target funding agency | National Science Foundation |
| `{{DURATION}}` | Project duration | 36 months |
| `{{BUDGET}}` | Requested budget | $450,000 |
| `{{DATE}}` | Submission date | January 15, 2024 |
| `{{ABSTRACT}}` | Executive summary (150-300 words) | This project aims to investigate... |
| `{{KEYWORDS}}` | Research keywords | decision making, neuroscience, computational modeling |
| `{{AIM_1}}` | First specific aim | Characterize neural activity patterns during decision making |
| `{{AIM_2}}` | Second specific aim | Develop computational models of decision processes |
| `{{AIM_3}}` | Third specific aim | Validate models with behavioral experiments |

## Structure

1. **Executive Summary**
   - Brief overview of the proposed research

2. **Introduction and Background**
   - Problem statement
   - Motivation
   - Significance

3. **Research Objectives**
   - Primary objective
   - Specific aims
   - Research questions

4. **Literature Review**
   - Theoretical framework
   - Current state of knowledge
   - Research gap

5. **Methodology**
   - Research design
   - Data collection
   - Data analysis
   - Ethical considerations

6. **Project Timeline**
   - Milestones and deliverables
   - Gantt chart or table

7. **Expected Outcomes**
   - Deliverables
   - Anticipated impact

8. **Budget Justification**
   - Personnel
   - Equipment and supplies
   - Travel
   - Other costs

9. **Broader Impacts**
   - Educational benefits
   - Societal benefits
   - Diversity and inclusion

10. **Qualifications**
    - PI background
    - Collaborators

## Customization

### Adapting for Different Agencies

**NSF Format:**
- Emphasize broader impacts
- Include mentoring plan
- Follow 15-page limit for project description

**NIH Format:**
- Use specific aims page format
- Include significance and innovation sections
- Follow R01/R21 specific requirements

**Private Foundations:**
- Adjust sections based on specific requirements
- May require different budget format

### Page Limits

Adjust content to meet page limits. Common limits:
- NSF: 15 pages (project description)
- NIH R01: 12 pages (research strategy)
- PhD proposals: Varies by institution (typically 10-20 pages)

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Required packages: inputenc, fontenc, lmodern, geometry, setspace, graphicx, amsmath, amssymb, booktabs, enumitem, hyperref, xcolor, fancyhdr, titlesec, natbib

## Tips

- Keep the executive summary concise and compelling
- Clearly state the research gap your proposal addresses
- Be specific about methodology and analysis plans
- Include realistic timelines with milestones
- Justify all budget items
- Highlight broader impacts beyond academic contributions
- Have colleagues review your proposal before submission
