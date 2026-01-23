# ICLR Conference Paper Template

Template for the International Conference on Learning Representations (ICLR), a top venue for deep learning research.

## Overview

ICLR is a premier conference for:
- Deep learning
- Representation learning
- Neural networks
- Machine learning theory and applications

Papers are submitted through OpenReview with double-blind peer review.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. For anonymous submission, keep `\author{Anonymous}`
3. For camera-ready, uncomment the author block and `\iclrfinalcopy`
4. Compile with pdfLaTeX

```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

### Submission Options

```latex
\usepackage{iclr2025_conference}           % Anonymous submission
\usepackage[final]{iclr2025_conference}    % Camera-ready version
\usepackage[preprint]{iclr2025_conference} % arXiv preprint
```

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{TITLE}} | Paper title | Learning Robust Representations via Contrastive Learning |
| {{AUTHOR_1}} | First author name | Jane Smith |
| {{AFFILIATION_1}} | First author affiliation | Stanford University |
| {{EMAIL_1}} | First author email | jsmith@stanford.edu |
| {{AUTHOR_2}} | Second author name | John Doe |
| {{AFFILIATION_2}} | Second author affiliation | Google DeepMind |
| {{EMAIL_2}} | Second author email | johndoe@deepmind.com |
| {{AUTHOR_3}} | Third author name | Alice Wong |
| {{AFFILIATION_3}} | Third author affiliation | MIT |
| {{EMAIL_3}} | Third author email | awong@mit.edu |
| {{ABSTRACT}} | Abstract text | We propose a novel approach to... |
| {{INTRODUCTION}} | Introduction text | Deep learning has achieved remarkable... |
| {{CONTRIBUTION_1}} | First main contribution | We introduce a new contrastive loss... |
| {{CONTRIBUTION_2}} | Second main contribution | We provide theoretical analysis showing... |
| {{CONTRIBUTION_3}} | Third main contribution | We demonstrate state-of-the-art results on... |
| {{RELATED_WORK}} | Related work overview | Our work builds on several lines of research... |
| {{RELATED_TOPIC_1}} | Related work topic 1 | Contrastive Learning |
| {{RELATED_TOPIC_1_CONTENT}} | Related work content 1 | SimCLR (Chen et al., 2020) introduced... |
| {{RELATED_TOPIC_2}} | Related work topic 2 | Self-Supervised Learning |
| {{RELATED_TOPIC_2_CONTENT}} | Related work content 2 | Recent advances in self-supervised... |
| {{BACKGROUND}} | Background section | We first review the necessary background... |
| {{PROBLEM_FORMULATION}} | Problem formulation | Given a dataset D = {x_1, ..., x_n}... |
| {{NOTATION}} | Notation description | We denote vectors in lowercase bold... |
| {{METHOD_OVERVIEW}} | Method overview | Our approach consists of three main components... |
| {{METHOD_SECTION_1}} | Method section 1 heading | Architecture Design |
| {{METHOD_SECTION_1_CONTENT}} | Method section 1 content | The encoder network f_theta maps... |
| {{METHOD_SECTION_2}} | Method section 2 heading | Training Objective |
| {{METHOD_SECTION_2_CONTENT}} | Method section 2 content | We minimize the following contrastive loss... |
| {{METHOD_SECTION_3}} | Method section 3 heading | Implementation Details |
| {{METHOD_SECTION_3_CONTENT}} | Method section 3 content | We use a ResNet-50 backbone with... |
| {{THEORETICAL_ANALYSIS}} | Theoretical analysis | We provide theoretical guarantees for... |
| {{EXPERIMENTS_OVERVIEW}} | Experiments overview | We evaluate our method on... |
| {{DATASETS}} | Datasets description | We conduct experiments on ImageNet... |
| {{BASELINES}} | Baselines description | We compare against SimCLR, MoCo, BYOL... |
| {{IMPLEMENTATION_DETAILS}} | Implementation details | All models are trained using SGD with... |
| {{MAIN_RESULTS}} | Main results | Table 1 presents our main results... |
| {{ABLATION_STUDIES}} | Ablation studies | We ablate key design choices... |
| {{ANALYSIS}} | Analysis of results | We further analyze the learned representations... |
| {{DISCUSSION}} | Discussion text | Our results demonstrate that... |
| {{LIMITATIONS}} | Limitations | Our approach has several limitations... |
| {{BROADER_IMPACT}} | Broader impact | This work may have implications for... |
| {{CONCLUSION}} | Conclusion text | We presented a novel approach to... |
| {{ACKNOWLEDGMENTS}} | Acknowledgments | We thank the reviewers for... |
| {{APPENDIX_DETAILS}} | Appendix experimental details | Additional hyperparameters... |
| {{APPENDIX_RESULTS}} | Appendix additional results | Full results on all datasets... |
| {{APPENDIX_PROOFS}} | Appendix proofs | Proof of Theorem 1... |

## Structure

1. Title and authors
2. Abstract
3. Introduction (with contributions list)
4. Related Work
5. Background / Preliminaries
6. Method / Approach
7. Theoretical Analysis (optional)
8. Experiments
   - Setup (datasets, baselines, implementation)
   - Main Results
   - Ablation Studies
   - Analysis
9. Discussion (limitations, broader impact)
10. Conclusion
11. Acknowledgments (camera-ready only)
12. References
13. Appendix

## Requirements

- LaTeX distribution with iclr style files
- Standard packages: hyperref, booktabs, amsmath, algorithm

Note: Download the current year's style file from the ICLR website.

## Tips for ICLR Submissions

1. **Anonymous submission**: Do not include author names or acknowledgments
2. **Page limits**: Usually 8 pages for main content, unlimited for references and appendix
3. **Reproducibility**: Include enough details to reproduce results
4. **Code**: Consider providing anonymous code via supplementary materials
5. **Clear contributions**: Explicitly list your contributions in the introduction
6. **Related work**: Be thorough but concise; acknowledge prior work fairly
7. **Ablations**: Include ablation studies to justify design choices
8. **Limitations**: Honestly discuss limitations of your approach
