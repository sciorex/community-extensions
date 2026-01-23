# Conference Poster Template (A0)

A professional A0-sized conference poster template using the tikzposter class. Features a clean multi-column layout suitable for academic conferences and symposiums. Dimensions: 841mm x 1189mm (portrait).

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdflatex:
   ```bash
   pdflatex main.tex
   ```
   Note: If using biblatex, run:
   ```bash
   pdflatex main.tex
   biber main
   pdflatex main.tex
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Poster title | Deep Learning for Medical Image Segmentation |
| `{{AUTHOR_1}}` | First author name | John A. Smith |
| `{{AUTHOR_2}}` | Second author name | Emily R. Johnson |
| `{{AUTHOR_3}}` | Third author name | Michael K. Chen |
| `{{AFFILIATION_1}}` | First affiliation | Stanford University, Department of Computer Science |
| `{{AFFILIATION_2}}` | Second affiliation | MIT, Department of EECS |
| `{{EMAIL}}` | Contact email | john.smith@stanford.edu |
| `{{CONFERENCE}}` | Conference name | NeurIPS 2024 |
| `{{INTRODUCTION}}` | Introduction paragraph | Medical image segmentation is a critical task... |
| `{{ACKNOWLEDGMENTS}}` | Acknowledgments text | This work was supported by NIH grant R01-123456... |

## Structure

The poster uses a three-column layout:

### Left Column
- Introduction
- Background
- Objectives

### Middle Column
- Methods
- Key Findings (highlighted box)

### Right Column
- Results (with table and figure)
- Conclusions
- References
- Acknowledgments

## Customization

### Changing Colors

Modify the color palette in the preamble:

```latex
\definecolorpalette{CustomPalette}{
    \definecolor{colorOne}{HTML}{2C3E50}    % Dark blue-gray (headers)
    \definecolor{colorTwo}{HTML}{3498DB}    % Bright blue (accents)
    \definecolor{colorThree}{HTML}{ECF0F1}  % Light gray (backgrounds)
}
```

### Changing Layout

**Landscape orientation:**
```latex
\documentclass[a0paper,landscape,25pt]{tikzposter}
```

**Different column widths:**
```latex
\begin{columns}
\column{0.4}  % Left column (40%)
\column{0.6}  % Right column (60%)
\end{columns}
```

### Adding Logos

Uncomment and modify the titlegraphic line:
```latex
\titlegraphic{\includegraphics[width=10cm]{university-logo.png}}
```

### Using Different Themes

tikzposter includes built-in themes:
```latex
\usetheme{Default}
\usetheme{Rays}
\usetheme{Basic}
\usetheme{Simple}
\usetheme{Envelope}
\usetheme{Wave}
\usetheme{Board}
\usetheme{Autumn}
\usetheme{Desert}
```

## Block Types

The template supports various block styles:

```latex
% Standard block
\block{Title}{Content}

% Colored box (highlighted)
\coloredbox[bgcolor=colorThree, framecolor=colorTwo]{Content}

% Inner block (nested)
\innerblock{Title}{Content}
```

## Adding Figures

```latex
\begin{tikzfigure}[Caption text]
    \includegraphics[width=0.9\linewidth]{figure.png}
\end{tikzfigure}
```

Or use standard LaTeX figures:
```latex
\begin{center}
    \includegraphics[width=0.8\linewidth]{figure.png}
    \captionof{figure}{Caption text}
\end{center}
```

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Required packages: tikzposter, graphicx, amsmath, amssymb, booktabs, enumitem, biblatex (optional)

## Tips

- Keep text concise - posters should be readable from 1-2 meters away
- Use bullet points rather than long paragraphs
- Include one key visual/figure per column
- Use the highlighted box for your main finding
- Font size is controlled by the documentclass option (25pt is standard)
- Test print at reduced size (A4) to check readability
- Include a QR code linking to your paper or supplementary materials
