# American Chemical Society (ACS) Article Template

Official template for submitting articles to American Chemical Society (ACS) journals. This template uses the `achemso` package which provides formatting for various ACS publications including JACS, ACS Nano, Chemistry of Materials, and many others.

## Usage

### Compilation

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

### Quick Start

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Select your target journal in the document class options
3. Add your experimental data and results
4. Update `references.bib` with your citations
5. Compile using the commands above

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TITLE}}` | Article title | Novel Catalytic Framework for Sustainable Organic Synthesis |
| `{{AUTHOR_1}}` | First author name | Alice M. Johnson |
| `{{AUTHOR_1_EMAIL}}` | First author email | alice.johnson@university.edu |
| `{{AUTHOR_1_AFFILIATION}}` | First author department | Department of Chemistry |
| `{{AUTHOR_1_ADDRESS}}` | First author address | University of California, Berkeley, CA 94720 |
| `{{AUTHOR_2}}` | Second author name | Robert K. Smith |
| `{{AUTHOR_2_AFFILIATION}}` | Second author institution | National Laboratory |
| `{{AUTHOR_2_ADDRESS}}` | Second author address | Argonne, IL 60439 |
| `{{CORRESPONDING_AUTHOR}}` | Corresponding author name | Prof. David L. Williams |
| `{{CORRESPONDING_EMAIL}}` | Corresponding author email | williams@chem.edu |
| `{{CORRESPONDING_PHONE}}` | Corresponding author phone | +1-555-123-4567 |
| `{{CORRESPONDING_AFFILIATION}}` | Corresponding author institution | Department of Chemistry, MIT |
| `{{CORRESPONDING_ALSO_AFFILIATION}}` | Secondary affiliation | Center for Materials Research |
| `{{ABSTRACT}}` | Article abstract | We report a novel synthetic methodology... |
| `{{RESEARCH_TOPIC}}` | Main research area | heterogeneous catalysis |
| `{{KEY_FACTOR}}` | Important variable | temperature and pressure control |
| `{{CHEMICAL_1}}` | First reagent | palladium acetate |
| `{{CHEMICAL_2}}` | Second reagent | triphenylphosphine |
| `{{SOLVENT}}` | Reaction solvent | dimethylformamide |
| `{{COMPOUND_NAME}}` | Your compound name | MOF-808-Pd |
| `{{CALC_MASS}}` | Calculated mass for HRMS | 425.1856 |
| `{{FOUND_MASS}}` | Found mass for HRMS | 425.1862 |
| `{{APPLICATION}}` | Target application | cross-coupling reactions |
| `{{ACKNOWLEDGMENTS}}` | Funding and acknowledgments | This work was supported by NSF Grant CHE-XXXXXXX |

## Structure

The template follows standard ACS article structure:

1. **Abstract** - Concise summary (150 words max for most journals)
2. **Introduction** - Background and motivation
3. **Experimental Section** - Materials, synthesis, characterization
4. **Results and Discussion** - Data presentation and analysis
5. **Conclusions** - Summary of findings
6. **Acknowledgments** - Funding sources
7. **Supporting Information** - Additional data
8. **References** - Bibliography

## Requirements

### Required Packages

- `achemso` - ACS document class (included in TeX Live)
- `mhchem` - Chemical formulas (\ce{H2O})
- `chemfig` - Chemical structure drawings
- `siunitx` - SI units (\SI{25}{\celsius})
- `graphicx` - Figure inclusion
- `booktabs` - Professional tables

### Journal Options

Change the journal in the document class:

```latex
\documentclass[journal=jacsat,manuscript=article]{achemso}  % JACS
\documentclass[journal=ancham,manuscript=article]{achemso}  % Analytical Chemistry
\documentclass[journal=nalefd,manuscript=letter]{achemso}   % Nano Letters
\documentclass[journal=acsnano,manuscript=article]{achemso} % ACS Nano
\documentclass[journal=chemmater,manuscript=article]{achemso} % Chem. Mater.
```

### Manuscript Types

- `article` - Full research article
- `letter` - Communication/letter
- `review` - Review article
- `perspective` - Perspective article
- `suppinfo` - Supporting information

## Chemistry-Specific Features

### Chemical Formulas

Use `mhchem` for chemical formulas:
```latex
\ce{H2O}           % Water
\ce{Fe2O3}         % Iron oxide
\ce{[Ag(NH3)2]+}   % Silver ammonia complex
\ce{CO2 + H2O -> H2CO3}  % Reaction
```

### Units

Use `siunitx` for consistent units:
```latex
\SI{25}{\celsius}                    % 25 C
\SI{1.5}{\gram}                      % 1.5 g
\SI{100}{\milli\liter}               % 100 mL
\SI{400}{\mega\hertz}                % 400 MHz
\SI{45.2 \pm 2.1}{\kilo\joule\per\mol} % 45.2 +/- 2.1 kJ/mol
```

### NMR Data Format

```latex
\textsuperscript{1}\textbf{H NMR} (\SI{400}{\mega\hertz}, CDCl\textsubscript{3}):
$\delta$ 7.85 (d, $J$ = \SI{8.0}{\hertz}, 2H), ...
```

## Tips for ACS Submissions

1. **Graphics**: Use high-resolution images (300 dpi minimum)
2. **Color**: Consider grayscale compatibility for print
3. **TOC Graphic**: Most journals require a table of contents graphic
4. **Supporting Information**: Include detailed procedures and additional data
5. **ORCID**: Include ORCID iDs for all authors

## Resources

- [ACS Author Guidelines](https://pubs.acs.org/page/4authors/index.html)
- [achemso Documentation](https://ctan.org/pkg/achemso)
- [ACS Paragon Plus](https://acsparagonplus.acs.org/) - Submission system
- [ACS Graphics Guidelines](https://pubs.acs.org/page/4authors/graphics/index.html)
