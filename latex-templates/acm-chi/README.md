# ACM CHI Conference Paper Template

Official ACM CHI (Conference on Human Factors in Computing Systems) paper template. The premier venue for Human-Computer Interaction (HCI) research. Uses the ACM Article template (acmart) with SIGCHI format.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your research content
2. Add your references to `references.bib`
3. Generate CCS concepts at https://dl.acm.org/ccs and update the CCSXML block
4. Compile with pdfLaTeX and BibTeX:
   ```bash
   pdflatex main.tex
   bibtex main
   pdflatex main.tex
   pdflatex main.tex
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{TITLE}} | Paper title | Understanding User Behavior in AI-Assisted Design |
| {{SUBTITLE}} | Paper subtitle (optional) | A Mixed-Methods Study |
| {{AUTHOR_1}} | First author name | Jane Smith |
| {{AUTHOR_1_EMAIL}} | First author email | jsmith@university.edu |
| {{AUTHOR_1_ORCID}} | First author ORCID | 0000-0001-2345-6789 |
| {{AUTHOR_1_INSTITUTION}} | First author institution | MIT |
| {{AUTHOR_1_DEPARTMENT}} | First author department | CSAIL |
| {{AUTHOR_1_CITY}} | First author city | Cambridge |
| {{AUTHOR_1_COUNTRY}} | First author country | USA |
| {{AUTHOR_2}} | Second author name | John Doe |
| {{AUTHOR_2_EMAIL}} | Second author email | jdoe@company.com |
| {{AUTHOR_2_INSTITUTION}} | Second author institution | Google |
| {{AUTHOR_2_DEPARTMENT}} | Second author department | Research |
| {{AUTHOR_2_CITY}} | Second author city | Mountain View |
| {{AUTHOR_2_COUNTRY}} | Second author country | USA |
| {{KEYWORDS}} | Paper keywords | human-AI interaction, user study, design tools |
| {{ABSTRACT}} | Paper abstract (150-250 words) | We present a study investigating... |
| {{INTRODUCTION}} | Introduction section | Human-AI collaboration is becoming... |
| {{CONTRIBUTION_1}} - {{CONTRIBUTION_3}} | Paper contributions | A novel design framework for... |
| {{RELATED_WORK_TOPIC_1}} - {{RELATED_WORK_TOPIC_3}} | Related work topics | Human-AI Interaction |
| {{RELATED_WORK_1}} - {{RELATED_WORK_3}} | Related work content | Prior work has explored... |
| {{METHODOLOGY_SECTION_TITLE}} | Section title | System Design / Design Process |
| {{DESIGN_GOAL_1_NAME}} - {{DESIGN_GOAL_3_NAME}} | Design goal names | Transparency |
| {{DESIGN_GOAL_1_DESCRIPTION}} - {{DESIGN_GOAL_3_DESCRIPTION}} | Design goal descriptions | System should explain its decisions |
| {{SYSTEM_OVERVIEW}} | System overview | Our system consists of three components... |
| {{COMPONENT_1_NAME}} - {{COMPONENT_2_NAME}} | Component names | AI Suggestion Engine |
| {{COMPONENT_1_DESCRIPTION}} - {{COMPONENT_2_DESCRIPTION}} | Component descriptions | The suggestion engine analyzes... |
| {{IMPLEMENTATION_DETAILS}} | Implementation details | We implemented the system using React... |
| {{PARTICIPANTS_DESCRIPTION}} | Participant recruitment | We recruited 24 participants... |
| {{P1_AGE}} - {{P3_AGE}} | Participant ages | 25-34 |
| {{P1_GENDER}} - {{P3_GENDER}} | Participant genders | Female |
| {{P1_EXPERIENCE}} - {{P3_EXPERIENCE}} | Participant experience | 3 years |
| {{STUDY_DESIGN}} | Study design description | We conducted a within-subjects study... |
| {{PROCEDURE}} | Study procedure | Each session lasted approximately 60 minutes... |
| {{MEASURE_1_NAME}} - {{MEASURE_3_NAME}} | Measure names | Task Completion Time |
| {{MEASURE_1_DESCRIPTION}} - {{MEASURE_3_DESCRIPTION}} | Measure descriptions | Time to complete each design task |
| {{ANALYSIS_APPROACH}} | Analysis approach | We used thematic analysis for qualitative data... |
| {{QUANTITATIVE_RESULTS}} | Quantitative results | Participants in the AI condition were significantly faster... |
| {{RESULTS_TABLE_CAPTION}} | Results table caption | Task Performance Across Conditions |
| {{METRIC_1}} - {{METRIC_3}} | Metric column headers | Time (s) |
| {{CONDITION_1}} - {{CONDITION_2}} | Condition names | With AI |
| {{C1_M1}} - {{C2_M3}} | Table cell values | 45.2 |
| {{THEME_1}} - {{THEME_3}} | Qualitative themes | Appreciation for AI Suggestions |
| {{THEME_1_FINDINGS}} - {{THEME_3_FINDINGS}} | Theme findings | Participants consistently reported... |
| {{PARTICIPANT_QUOTE_1}} | Participant quote | The AI really helped me think differently... |
| {{QUOTE_1_PARTICIPANT}} | Quote participant ID | 7 |
| {{DISCUSSION_TOPIC_1}} - {{DISCUSSION_TOPIC_2}} | Discussion topics | Balancing AI Autonomy and User Control |
| {{DISCUSSION_1}} - {{DISCUSSION_2}} | Discussion content | Our findings suggest that... |
| {{DESIGN_IMPLICATION_1}} - {{DESIGN_IMPLICATION_3}} | Design implications | AI systems should provide explanations... |
| {{LIMITATIONS}} | Limitations | Our study has several limitations... |
| {{FUTURE_WORK_1}} - {{FUTURE_WORK_2}} | Future work items | Longitudinal deployment study |
| {{CONCLUSION}} | Conclusion | We presented a study of... |
| {{ACKNOWLEDGMENTS}} | Acknowledgments | We thank our participants and reviewers... |

## Structure

The template follows standard CHI paper structure:

1. **Abstract** - 150-250 word summary
2. **Introduction** - Motivation, problem, contributions
3. **Related Work** - Literature review with subsections
4. **System Design / Methodology** - Design goals, system overview, implementation
5. **User Study** - Participants, study design, procedure, measures, analysis
6. **Results** - Quantitative and qualitative findings with themes
7. **Discussion** - Interpretation, design implications, limitations
8. **Conclusion** - Summary of contributions
9. **Acknowledgments** - Funding and thanks
10. **References** - Bibliography

## Document Options

The template includes several options in the document class:

```latex
\documentclass[sigchi,review,anonymous]{acmart}
```

- `sigchi` - CHI conference format
- `review` - Enables line numbers for review
- `anonymous` - Anonymizes author information

For camera-ready submission, change to:
```latex
\documentclass[sigchi]{acmart}
```

And update copyright information as instructed by ACM.

## CCS Concepts

The ACM Computing Classification System (CCS) concepts are required. Generate them at:
https://dl.acm.org/ccs

Replace the CCSXML block with your generated concepts.

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- ACM acmart class (included in most TeX distributions)
- Required packages:
  - acmart (document class)
  - booktabs (tables)
  - graphicx (figures)
  - balance (column balancing)

## Compilation

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Customization Tips

### Adding Figures
```latex
\begin{figure}[h]
  \centering
  \includegraphics[width=\columnwidth]{figures/interface.png}
  \caption{The system interface showing...}
  \Description{Alt text for accessibility - required by ACM}
  \label{fig:interface}
\end{figure}
```

### Adding More Authors
Copy the author block and modify:
```latex
\author{Author Name}
\email{email@institution.edu}
\affiliation{%
  \institution{Institution}
  \city{City}
  \country{Country}
}
```

### Sidebar/Marginal Notes
```latex
\marginpar{Important note here}
```

### Teaser Figure
Add before `\maketitle`:
```latex
\begin{teaserfigure}
  \includegraphics[width=\textwidth]{teaser.png}
  \caption{Teaser caption}
  \Description{Teaser description}
\end{teaserfigure}
```

## Notes

- CHI papers typically have a page limit (check current year's guidelines)
- The Description field in figures is required for accessibility
- Include participant quotes to support qualitative findings
- Use design goals (DG) and design implications (DI) format common in CHI
- Tables should use booktabs style (no vertical lines)
- The template is set up for anonymous review; update for camera-ready

## CHI-Specific Conventions

- **Design Goals (DG)**: State upfront what your system aims to achieve
- **Research Questions (RQ)**: Frame your investigation clearly
- **Design Implications (DI)**: Derive actionable implications from findings
- **Participant Quotes**: Use format "quote" (P#)
- **Mixed Methods**: Combine quantitative and qualitative approaches
