# APA 7th Edition Template

APA 7th Edition format for psychology, education, and social sciences research papers.

## Overview

The APA (American Psychological Association) format is the standard for:
- Psychology journals
- Education research
- Social sciences
- Nursing and health sciences
- Business and economics

This template uses the `apa7` document class for full APA 7 compliance.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdfLaTeX and Biber for bibliography

```bash
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

### Document Format Options

The `apa7` class supports different formats:
- `man` - Manuscript format (for journal submission)
- `jou` - Journal format (two-column, like published articles)
- `doc` - Document format (for class papers, theses)
- `stu` - Student paper format (simplified title page)

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{TITLE}} | Full paper title | The Effects of Mindfulness Training on Academic Performance |
| {{SHORT_TITLE}} | Running head (50 characters max) | MINDFULNESS AND ACADEMIC PERFORMANCE |
| {{AUTHOR_1}} | Author name | Sarah M. Johnson |
| {{AFFILIATION_1}} | Author institution | Department of Psychology, Stanford University |
| {{ORCID}} | Author ORCID ID | 0000-0002-1234-5678 |
| {{AUTHOR_NOTE}} | Author note content | This research was supported by Grant X... |
| {{DEPARTMENT}} | Department name | Department of Psychology |
| {{UNIVERSITY}} | University name | Stanford University |
| {{ADDRESS}} | Mailing address | 450 Serra Mall, Stanford, CA 94305 |
| {{EMAIL}} | Contact email | sjohnson@stanford.edu |
| {{ABSTRACT}} | Abstract (150-250 words) | This study examined the relationship... |
| {{KEYWORDS}} | Keywords (3-5 terms) | mindfulness, academic performance, college students |
| {{INTRODUCTION}} | Introduction text | Mindfulness-based interventions have gained... |
| {{LITERATURE_REVIEW}} | Literature review text | Previous research has demonstrated... |
| {{SUBSECTION_1_TITLE}} | First subsection heading | Theoretical Framework |
| {{SUBSECTION_1_CONTENT}} | First subsection content | Self-determination theory posits... |
| {{SUBSECTION_2_TITLE}} | Second subsection heading | Empirical Evidence |
| {{SUBSECTION_2_CONTENT}} | Second subsection content | Several studies have found... |
| {{PARTICIPANTS}} | Participant description | Participants were 120 undergraduate students... |
| {{MATERIALS}} | Materials/instruments | The Mindful Attention Awareness Scale (MAAS)... |
| {{PROCEDURE}} | Procedure description | After providing informed consent, participants... |
| {{DATA_ANALYSIS}} | Data analysis plan | Data were analyzed using SPSS Version 28... |
| {{RESULTS}} | Results section intro | Descriptive statistics and correlations... |
| {{RESULTS_SUBSECTION_1}} | First results heading | Preliminary Analyses |
| {{RESULTS_SUBSECTION_1_CONTENT}} | First results content | Missing data were handled using... |
| {{RESULTS_SUBSECTION_2}} | Second results heading | Main Analyses |
| {{RESULTS_SUBSECTION_2_CONTENT}} | Second results content | A hierarchical regression revealed... |
| {{DISCUSSION}} | Discussion text | The present study found that... |
| {{THEORETICAL_IMPLICATIONS}} | Theoretical implications | These findings extend our understanding... |
| {{PRACTICAL_IMPLICATIONS}} | Practical implications | Educators may consider implementing... |
| {{LIMITATIONS}} | Limitations and future directions | Several limitations should be noted... |
| {{CONCLUSION}} | Conclusion text | In conclusion, this study provides... |
| {{TABLE_1_TITLE}} | Table 1 title | Descriptive Statistics and Correlations |
| {{TABLE_1_CONTENT}} | Table 1 content | Variable 1 & 3.45 & 0.89 & 120 |
| {{TABLE_1_NOTE}} | Table 1 note | *p* < .05. **p* < .01. |
| {{FIGURE_1_CAPTION}} | Figure 1 caption | Mean scores by condition with 95% CI error bars |
| {{APPENDIX_A_TITLE}} | Appendix A title | Survey Instruments |
| {{APPENDIX_A_CONTENT}} | Appendix A content | The following scales were used... |

## Structure

1. Title page (with author note)
2. Abstract with keywords
3. Introduction (no heading label)
4. Literature Review (optional as separate section)
5. Method
   - Participants
   - Materials
   - Procedure
   - Data Analysis
6. Results
7. Discussion
   - Theoretical Implications
   - Practical Implications
   - Limitations and Future Directions
8. Conclusion
9. References
10. Tables (at end for manuscript format)
11. Figures (at end for manuscript format)
12. Appendices

## Requirements

- LaTeX distribution with `apa7` class
- Biber for bibliography processing
- Required packages: babel, csquotes, biblatex (with apa style)

## APA Heading Levels

| Level | Format |
|-------|--------|
| 1 | Centered, Bold |
| 2 | Left-aligned, Bold |
| 3 | Left-aligned, Bold, Italic |
| 4 | Indented, Bold, ending with period. |
| 5 | Indented, Bold, Italic, ending with period. |

## Statistical Reporting

APA format for common statistics:
- t-test: *t*(45) = 2.34, *p* = .024, *d* = 0.65
- ANOVA: *F*(2, 87) = 4.56, *p* = .013, eta-squared = .09
- Correlation: *r*(48) = .42, *p* < .001
- Chi-square: chi-squared(2) = 8.24, *p* = .016
