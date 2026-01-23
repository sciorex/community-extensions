# Beamer Metropolis Presentation Template

A modern, minimal presentation template using the popular Metropolis theme for Beamer. Features clean typography, professional appearance, and a distraction-free design ideal for academic and professional presentations.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with XeLaTeX (recommended) or pdflatex:
   ```bash
   xelatex main.tex
   biber main
   xelatex main.tex
   ```
   Or with pdflatex (comment out fontspec):
   ```bash
   pdflatex main.tex
   biber main
   pdflatex main.tex
   ```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Presentation title | Advances in Neural Network Architecture Design |
| `{{SUBTITLE}}` | Subtitle (optional) | A Comprehensive Analysis |
| `{{AUTHOR}}` | Presenter name | Dr. Sarah Johnson |
| `{{INSTITUTE}}` | Institution | Stanford University |
| `{{DATE}}` | Presentation date | January 15, 2024 |
| `{{EMAIL}}` | Contact email | sarah.johnson@stanford.edu |
| `{{GITHUB_REPO}}` | GitHub repository | username/project-name |

## Structure

1. **Title Slide** - Automatically generated from metadata
2. **Outline** - Table of contents
3. **Introduction** - Background and research questions
4. **Methods** - Approach overview, mathematical framework, algorithm
5. **Results** - Experimental setup, main results, ablation study
6. **Conclusion** - Summary and future directions
7. **Questions** - Standout frame for Q&A
8. **Appendix** - References and supplementary slides

## Customization

### Aspect Ratio

Change the aspect ratio in the documentclass:
```latex
\documentclass[aspectratio=169]{beamer}  % 16:9 (default)
\documentclass[aspectratio=43]{beamer}   % 4:3
\documentclass[aspectratio=1610]{beamer} % 16:10
```

### Color Theme

Customize colors by adding after `\usetheme{metropolis}`:
```latex
\setbeamercolor{frametitle}{bg=blue!80!black}
\setbeamercolor{progress bar}{fg=orange}
\setbeamercolor{alerted text}{fg=red}
```

### Font Options

For pdflatex (instead of XeLaTeX):
```latex
% Comment out:
% \usepackage{fontspec}

% Uncomment:
\usepackage[T1]{fontenc}
\usepackage{lmodern}
```

### Progress Bar

Control the progress bar:
```latex
\metroset{progressbar=frametitle}  % In frame title (default)
\metroset{progressbar=head}        % In header
\metroset{progressbar=foot}        % In footer
\metroset{progressbar=none}        % No progress bar
```

## Slide Types

### Standard Slide
```latex
\begin{frame}{Title}
    Content
\end{frame}
```

### Standout Slide (Full-screen emphasis)
```latex
\begin{frame}[standout]
    Questions?
\end{frame}
```

### Two-Column Layout
```latex
\begin{frame}{Title}
    \begin{columns}[T]
        \begin{column}{0.5\textwidth}
            Left content
        \end{column}
        \begin{column}{0.5\textwidth}
            Right content
        \end{column}
    \end{columns}
\end{frame}
```

### Slide with Pauses (Progressive reveal)
```latex
\begin{frame}{Title}
    \begin{itemize}
        \item First point
        \pause
        \item Second point (appears on click)
        \pause
        \item Third point
    \end{itemize}
\end{frame}
```

## Adding Content

### Figures
```latex
\begin{figure}
    \includegraphics[width=0.8\textwidth]{figure.pdf}
    \caption{Caption text}
\end{figure}
```

### Tables
```latex
\begin{table}
    \begin{tabular}{@{}lcc@{}}
        \toprule
        Header 1 & Header 2 & Header 3 \\
        \midrule
        Data 1 & Data 2 & Data 3 \\
        \bottomrule
    \end{tabular}
    \caption{Caption text}
\end{table}
```

### Blocks
```latex
\begin{block}{Block Title}
    Standard block content
\end{block}

\begin{alertblock}{Alert}
    Important information
\end{alertblock}

\begin{exampleblock}{Example}
    Example content
\end{exampleblock}
```

### Equations
```latex
\begin{equation*}
    E = mc^2
\end{equation*}
```

## Requirements

- LaTeX distribution (TeX Live, MiKTeX)
- Metropolis theme (included in TeX Live 2016+)
- Required packages: appendixnumberbeamer, booktabs, graphicx, amsmath, amssymb, ccicons
- For XeLaTeX: fontspec package
- For bibliography: biblatex with biber backend

## Tips

- Keep slides minimal - one idea per slide
- Use the `\pause` command sparingly for progressive reveals
- Include speaker notes with `\note{...}` (enable with `\setbeameroption{show notes}`)
- Use `\alert{text}` to highlight important terms
- The standout frame works great for section breaks and Q&A
- Test your presentation with different projector settings
- Export to PDF for compatibility: the output is a standard PDF file
