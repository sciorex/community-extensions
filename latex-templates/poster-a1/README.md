# A1 Research Poster Template

An A1-sized (594mm x 841mm) research poster template using TikZposter. Suitable for smaller conference presentations, departmental seminars, or symposiums. Features a professional three-column layout with customizable color scheme.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your research content
2. Add figures to a `figures/` directory
3. Compile with pdfLaTeX:
   ```bash
   pdflatex main.tex
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{TITLE}} | Poster title | Machine Learning for Climate Prediction |
| {{AUTHOR_1}} - {{AUTHOR_3}} | Author names | John Smith |
| {{AFFILIATION_1}} - {{AFFILIATION_2}} | Institutional affiliations | MIT Computer Science |
| {{EMAIL}} | Corresponding author email | jsmith@mit.edu |
| {{INTRODUCTION}} | Introduction text | Climate change poses significant challenges... |
| {{RESEARCH_QUESTION_1}} - {{RESEARCH_QUESTION_2}} | Research questions | Can deep learning improve predictions? |
| {{BACKGROUND}} | Background/motivation | Previous approaches have focused on... |
| {{OBJECTIVE_1}} - {{OBJECTIVE_3}} | Research objectives | Develop a novel ML framework |
| {{METHODS_OVERVIEW}} | Methods overview | We employ a multi-stage approach... |
| {{METHOD_1_NAME}} | First method name | Data Collection |
| {{METHOD_1_DESCRIPTION}} | First method description | We gathered data from 50 sources... |
| {{METHOD_2_NAME}} | Second method name | Model Architecture |
| {{METHOD_2_DESCRIPTION}} | Second method description | Our neural network consists of... |
| {{RESULTS_OVERVIEW}} | Results overview | Our experiments demonstrate... |
| {{FIGURE_1_CAPTION}} | Main figure caption | Comparison of prediction accuracy |
| {{FINDING_1}} - {{FINDING_3}} | Key findings | 25% improvement over baseline |
| {{ANALYSIS}} | Analysis discussion | The results indicate that... |
| {{TABLE_1_CAPTION}} | Table caption | Performance metrics comparison |
| {{COL_1_HEADER}} - {{COL_3_HEADER}} | Table column headers | Method |
| {{ROW_1_COL_1}} - {{ROW_3_COL_3}} | Table cell values | Baseline |
| {{CONCLUSIONS}} | Conclusions text | This research demonstrates... |
| {{TAKEAWAY_1}} - {{TAKEAWAY_3}} | Key takeaways | ML significantly improves accuracy |
| {{FUTURE_WORK_1}} - {{FUTURE_WORK_2}} | Future work items | Extend to other climate variables |
| {{REFERENCE_1}} - {{REFERENCE_4}} | Inline references | Smith et al. (2024), J. Methods 42:145 |
| {{ACKNOWLEDGMENTS}} | Acknowledgments | This work was supported by NSF grant... |
| {{CONFERENCE}} | Conference name | ICML 2026 |
| {{CONFERENCE_DATE}} | Conference date | July 15-20, 2026 |
| {{CONFERENCE_LOCATION}} | Conference location | Vienna, Austria |

## Structure

The poster uses a three-column layout:

**Left Column:**
- Introduction
- Background
- Objectives

**Middle Column:**
- Methods (with inner blocks for sub-methods)
- Results (with figure placeholder)

**Right Column:**
- Analysis (with table)
- Conclusions (with key takeaways)
- Future Work
- References
- Acknowledgments

## Color Customization

The template includes customizable colors:

```latex
\definecolor{primarycolor}{RGB}{0,51,102}      % Dark blue (headers)
\definecolor{secondarycolor}{RGB}{0,120,174}   % Accent blue (block titles)
\definecolor{highlightcolor}{RGB}{255,165,0}   % Orange (inner blocks)
```

Modify these RGB values to match your institution or conference theme.

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Required packages:
  - tikzposter (core poster class)
  - fontenc, lmodern (fonts)
  - amsmath, amssymb (math)
  - graphicx (figures)
  - natbib (optional, for BibTeX)
  - qrcode (optional, for QR codes)

## Compilation

```bash
pdflatex main.tex
```

For best results, ensure you have the TikZposter package installed. It is included in most modern TeX distributions.

## Customization Tips

### Adding Logos
Uncomment and modify the `\titlegraphic` command:
```latex
\titlegraphic{
    \includegraphics[height=8cm]{logo.png}
}
```

### Adding Figures
Place figures in a `figures/` directory and uncomment the `\includegraphics` lines in the appropriate blocks:
```latex
\begin{center}
    \includegraphics[width=0.9\linewidth]{figures/results.png}
\end{center}
```

### Adding QR Codes
Uncomment the qrcode package and use:
```latex
\qrcode[height=3cm]{https://yourpaper.link}
```

### Changing Layout
- Adjust column widths in the `\column{0.33}` commands (must sum to 1.0)
- For two-column layout, use `\column{0.5}` twice
- For landscape orientation, change to `\documentclass[a1paper,landscape]{tikzposter}`

### Block Styles
Available block styles:
- Default, Basic, Envelope, Corner, Slide, TornOut, Minimal

Change with: `\useblockstyle{StyleName}`

## Dimensions

- **A1 Portrait**: 594mm x 841mm (23.4" x 33.1")
- **Recommended viewing distance**: 1-2 meters
- **Font sizes**: Automatically scaled by TikZposter

## Notes

- The template is optimized for portrait A1; for A0 posters, see the poster-a0 template
- References are formatted inline (numbered list) for space efficiency
- Inner blocks (colored boxes) are used for emphasis
- The color scheme uses blue tones suitable for most academic contexts
- Consider print margins when finalizing your poster
