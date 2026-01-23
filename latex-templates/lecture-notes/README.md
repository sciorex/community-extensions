# Lecture Notes

Academic lecture notes template with professional formatting for theorems, definitions, examples, and exercises. Ideal for instructors preparing course materials or students organizing their notes.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdfLaTeX: `pdflatex main.tex`
3. Run twice for table of contents and cross-references
4. For citations, run: `pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex`

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{COURSE_CODE}}` | Course identifier | CS 229 |
| `{{COURSE_NAME}}` | Course name | Machine Learning |
| `{{LECTURE_NUM}}` | Lecture number | 5 |
| `{{LECTURE_TITLE}}` | Lecture topic | Support Vector Machines |
| `{{INSTRUCTOR}}` | Instructor name | Prof. Andrew Ng |
| `{{INSTITUTION}}` | University/institution | Stanford University |
| `{{DATE}}` | Lecture date | January 15, 2024 |
| `{{OBJECTIVE_1}}` | Learning objective 1 | Understand the margin concept |
| `{{OBJECTIVE_2}}` | Learning objective 2 | Derive the SVM optimization problem |
| `{{OBJECTIVE_3}}` | Learning objective 3 | Apply kernel methods |
| `{{INTRO_TEXT}}` | Introduction paragraph | In this lecture, we explore... |
| `{{TOPIC}}` | Main topic | support vector machines |
| `{{PREVIOUS_TOPIC}}` | Previous lecture topic | linear classifiers |
| `{{KEY_CONCEPT}}` | Key concept | maximum margin classification |
| `{{DEFINITION_1_NAME}}` | First definition name | Support Vector |
| `{{DEFINITION_1_TEXT}}` | Definition text | A support vector is a data point... |
| `{{EXAMPLE_1_TEXT}}` | Example explanation | Consider a binary classification... |
| `{{EXAMPLE_VALUE}}` | Example value | 3 |
| `{{EXAMPLE_EQUATION}}` | Example equation | f(x) = w^T x + b |
| `{{DEFINITION_2_NAME}}` | Second definition name | Margin |
| `{{DEFINITION_2_TEXT}}` | Definition text | The margin is the distance... |
| `{{RELATIONSHIP_TEXT}}` | Relationship between concepts | the constraint that... |
| `{{THEOREM_NAME}}` | Main theorem name | Maximum Margin Theorem |
| `{{THEOREM_STATEMENT}}` | Theorem statement | For a linearly separable dataset... |
| `{{PROOF_TEXT}}` | Proof introduction | We prove this by contradiction... |
| `{{PROOF_METHOD}}` | Proof method | Lagrangian optimization |
| `{{PROOF_STEP_1}}` | First proof step | Define the Lagrangian L = ... |
| `{{PROOF_STEP_2}}` | Second proof step | Take derivatives and set to zero... |
| `{{PROOF_CONCLUSION}}` | Proof conclusion | the optimal hyperplane is unique |
| `{{COROLLARY_TEXT}}` | Corollary statement | The optimal margin depends only on... |
| `{{APPLICATION_EXAMPLE}}` | Application example | In text classification, we can... |
| `{{SPECIAL_CASES_TEXT}}` | Special cases discussion | When the data is not separable... |
| `{{LEMMA_NAME}}` | Lemma name | Kernel Trick |
| `{{LEMMA_STATEMENT}}` | Lemma statement | Any algorithm using dot products... |
| `{{CONNECTIONS_TEXT}}` | Connections to other topics | This relates to logistic regression... |
| `{{WARNING_TEXT}}` | Important warning | Kernel choice significantly affects... |
| `{{WORKED_EXAMPLE_NAME}}` | Worked example title | Linear SVM Classification |
| `{{WORKED_PROBLEM}}` | Problem statement | Given the following data points... |
| `{{WORKED_SOLUTION}}` | Solution | We solve the QP problem to find... |
| `{{SUMMARY_POINT_1}}` | Summary point 1 | SVMs maximize the margin |
| `{{SUMMARY_POINT_2}}` | Summary point 2 | Support vectors determine the boundary |
| `{{SUMMARY_POINT_3}}` | Summary point 3 | Kernels enable non-linear classification |
| `{{TAKEAWAY_1}}` | Key takeaway 1 | Maximum margin leads to better generalization |
| `{{TAKEAWAY_2}}` | Key takeaway 2 | The kernel trick avoids explicit feature mapping |
| `{{EXERCISE_1}}` | Exercise 1 | Prove that the margin equals... |
| `{{EXERCISE_2}}` | Exercise 2 | Implement an SVM classifier... |
| `{{EXERCISE_3}}` | Challenge exercise | Derive the dual formulation... |
| `{{READING_1}}` | Recommended reading 1 | Bishop, Chapter 7 |
| `{{READING_2}}` | Recommended reading 2 | Hastie et al., Chapter 12 |
| `{{NEXT_LECTURE_TOPIC}}` | Preview of next lecture | Kernel Methods and Gaussian Processes |

## Structure

- **Learning Objectives**: Clear goals for the lecture
- **Introduction**: Context and motivation
- **Definitions**: Key terms with formal definitions
- **Examples**: Illustrative examples with solutions
- **Theorems and Proofs**: Main theoretical results
- **Remarks and Warnings**: Important notes and caveats
- **Worked Examples**: Step-by-step problem solutions
- **Summary**: Key points and takeaways
- **Exercises**: Practice problems for students
- **Further Reading**: Additional resources

## Environments

The template provides several colored theorem environments:
- `theorem` - For main theorems (blue)
- `definition` - For definitions (brown)
- `lemma` - For lemmas (light blue)
- `corollary` - For corollaries (light blue)
- `proposition` - For propositions (blue)
- `example` - For examples (green)
- `remark` - For remarks (gray)
- `warning` - For important notes (orange)
- `exercise` - For exercises (numbered)
- `solution` - For solutions (can be hidden)

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Packages: `amsmath`, `amssymb`, `amsthm`, `tcolorbox`, `fancyhdr`, `hyperref`, `xcolor`
- The `tcolorbox` library with `theorems`, `skins`, and `breakable` options

## Compilation

```bash
pdflatex main.tex
pdflatex main.tex  # Run twice for TOC
```

With bibliography:
```bash
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Customization

- Modify colors using `\definecolor` commands
- Add new theorem environments using `\newtcbtheorem`
- Adjust header/footer content in the `fancyhdr` setup
- Enable/disable table of contents as needed
