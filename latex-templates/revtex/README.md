# RevTeX 4.2 Physics Template

RevTeX 4.2 template for APS (American Physical Society) and AIP (American Institute of Physics) journals.

## Overview

RevTeX is the standard format for:
- Physical Review Letters (PRL)
- Physical Review A-E
- Physical Review X (PRX)
- Reviews of Modern Physics
- Journal of Chemical Physics
- Applied Physics Letters
- And many other physics journals

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdfLaTeX

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

### Journal Options

Change the document class options for different journals:
- `aps,prl` - Physical Review Letters
- `aps,pra` - Physical Review A (Atomic, Molecular, Optical)
- `aps,prb` - Physical Review B (Condensed Matter)
- `aps,prc` - Physical Review C (Nuclear Physics)
- `aps,prd` - Physical Review D (Particles, Fields, Gravitation)
- `aps,pre` - Physical Review E (Statistical, Nonlinear, Soft Matter)
- `aps,prx` - Physical Review X
- `aip,jcp` - Journal of Chemical Physics
- `aip,apl` - Applied Physics Letters

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{TITLE}} | Paper title | Observation of Quantum Entanglement in Solid-State Qubits |
| {{AUTHOR_1}} | First author name | J. M. Smith |
| {{AUTHOR_1_EMAIL}} | First author email | smith@physics.university.edu |
| {{AFFILIATION_1}} | First institution | Department of Physics, University of Example, City, State 12345, USA |
| {{AUTHOR_2}} | Second author name | A. B. Jones |
| {{AFFILIATION_2}} | Second institution | National Laboratory, City, Country |
| {{AUTHOR_3}} | Third author name | C. D. Wilson |
| {{ABSTRACT}} | Abstract text | We report experimental observation of... |
| {{PACS_NUMBERS}} | PACS classification codes | 03.67.-a, 42.50.Dv, 73.21.La |
| {{KEYWORDS}} | Keywords | quantum entanglement, qubits, coherence |
| {{INTRODUCTION}} | Introduction text | Quantum information processing requires... |
| {{THEORY}} | Theoretical framework | The system is described by the Hamiltonian... |
| {{THEORY_SUBSECTION_1}} | Theory subsection heading | Model Hamiltonian |
| {{THEORY_SUBSECTION_1_CONTENT}} | Theory subsection content | We consider a system of coupled spins... |
| {{THEORY_SUBSECTION_2}} | Theory subsection heading | Decoherence Mechanisms |
| {{THEORY_SUBSECTION_2_CONTENT}} | Theory subsection content | The dominant sources of decoherence... |
| {{METHODS}} | Methods overview | Experiments were performed using... |
| {{EXPERIMENTAL_SETUP}} | Experimental setup description | The sample was mounted in a dilution refrigerator... |
| {{MEASUREMENT_PROCEDURE}} | Measurement procedure | Qubit states were initialized by... |
| {{RESULTS}} | Results section intro | Figure 1 shows the measured... |
| {{RESULTS_SUBSECTION_1}} | Results subsection heading | Coherence Times |
| {{RESULTS_SUBSECTION_1_CONTENT}} | Results subsection content | We measured T1 = 50 microseconds and T2 = 20 microseconds... |
| {{RESULTS_SUBSECTION_2}} | Results subsection heading | Entanglement Verification |
| {{RESULTS_SUBSECTION_2_CONTENT}} | Results subsection content | Bell state fidelity was determined... |
| {{DISCUSSION}} | Discussion text | These results demonstrate that... |
| {{CONCLUSION}} | Conclusion text | In summary, we have demonstrated... |
| {{ACKNOWLEDGMENTS}} | Acknowledgments | This work was supported by NSF Grant No. PHY-XXXXXXX... |
| {{APPENDIX_A_TITLE}} | Appendix A title | Derivation of Effective Hamiltonian |
| {{APPENDIX_A_CONTENT}} | Appendix A content | Starting from the full system Hamiltonian... |
| {{FIGURE_1_CAPTION}} | Figure 1 caption | (Color online) Schematic of the experimental setup... |
| {{FIGURE_2_CAPTION}} | Figure 2 caption | Measured Rabi oscillations as a function of drive amplitude... |
| {{TABLE_1_CAPTION}} | Table 1 caption | Summary of measured qubit parameters |
| {{TABLE_1_CONTENT}} | Table 1 data | $T_1$ & $50 \pm 2$ & $\mu$s |

## Structure

1. Title and authors
2. Abstract
3. PACS numbers and keywords
4. Introduction
5. Theoretical Framework / Model
6. Methods (Experimental or Numerical)
7. Results
8. Discussion
9. Conclusion
10. Acknowledgments
11. Appendices
12. References
13. Figures and Tables

## Requirements

- LaTeX distribution with RevTeX 4.2 (included in TeX Live and MiKTeX)
- Standard packages: amsmath, graphicx, hyperref
- Optional: siunitx for SI units, physics for notation

## PACS Numbers

Find PACS codes at: https://journals.aps.org/PACS

Common categories:
- 01.xx.xx - Physics education, communication
- 03.xx.xx - Quantum mechanics, field theory
- 42.xx.xx - Optics
- 73.xx.xx - Electronic structure of surfaces
- 74.xx.xx - Superconductivity
- 85.xx.xx - Electronic devices

## Tips

- Use `\bm{}` for bold math symbols
- Use `\SI{}{unit}` from siunitx for proper SI units
- PRL has strict length limits (typically 4 pages)
- Two-column format is standard for most APS journals
- Use `superscriptaddress` option for multiple affiliations
