# Problem Set / Homework

Homework and problem set template with clear formatting for problems, hints, and solutions. Suitable for instructors creating assignments or students preparing neat homework submissions.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdfLaTeX: `pdflatex main.tex`
3. For answer key version, uncomment the `\begin{solution}` environments
4. Add or remove problems as needed

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{COURSE_CODE}}` | Course identifier | MATH 201 |
| `{{COURSE_NAME}}` | Course name | Linear Algebra |
| `{{PSET_NUMBER}}` | Problem set number | 3 |
| `{{PSET_TITLE}}` | Problem set topic | Eigenvalues and Eigenvectors |
| `{{INSTRUCTOR}}` | Instructor name | Prof. Jane Smith |
| `{{DUE_DATE}}` | Due date | February 15, 2024, 11:59 PM |
| `{{TOTAL_POINTS}}` | Total points | 100 |
| `{{INSTRUCTION_1}}` | Instruction 1 | Write your name on every page |
| `{{INSTRUCTION_2}}` | Instruction 2 | Justify all answers |
| `{{INSTRUCTION_3}}` | Instruction 3 | Staple pages together |
| `{{POINTS_1}}` | Points for problem 1 | 20 |
| `{{PROBLEM_1_TEXT}}` | Problem 1 statement | Consider the matrix A = ... |
| `{{PROBLEM_1A}}` | Subproblem 1a | Find the eigenvalues of A |
| `{{PROBLEM_1B}}` | Subproblem 1b | Find the corresponding eigenvectors |
| `{{PROBLEM_1C}}` | Subproblem 1c | Diagonalize A if possible |
| `{{SOLUTION_1}}` | Solution to problem 1 | The characteristic polynomial is... |
| `{{POINTS_2}}` | Points for problem 2 | 15 |
| `{{PROBLEM_2_TEXT}}` | Problem 2 statement | Prove the following theorem... |
| `{{GIVEN_1}}` | Given condition 1 | A is a symmetric matrix |
| `{{GIVEN_2}}` | Given condition 2 | A has real entries |
| `{{PROBLEM_2_FIND}}` | What to find | All eigenvalues are real |
| `{{HINT_2}}` | Hint for problem 2 | Consider the complex conjugate... |
| `{{POINTS_3}}` | Points for problem 3 | 20 |
| `{{PROBLEM_3_TEXT}}` | Problem 3 statement | Let T: R^n -> R^m be a linear map |
| `{{PROBLEM_3A}}` | Subproblem 3a | Show that ker(T) is a subspace |
| `{{PROBLEM_3B}}` | Subproblem 3b | Prove the rank-nullity theorem |
| `{{POINTS_4}}` | Points for problem 4 | 15 |
| `{{PROBLEM_4_TEXT}}` | Problem 4 statement | Compute the following values |
| `{{COL_1_HEADER}}` | Table column 1 header | Matrix |
| `{{COL_2_HEADER}}` | Table column 2 header | Determinant |
| `{{COL_3_HEADER}}` | Table column 3 header | Trace |
| `{{ROW_1_COL_1}}` | Row 1, Column 1 | A |
| `{{ROW_2_COL_1}}` | Row 2, Column 1 | B |
| `{{ROW_3_COL_1}}` | Row 3, Column 1 | AB |
| `{{POINTS_5}}` | Points for problem 5 | 20 |
| `{{PROBLEM_5_TEXT}}` | Problem 5 statement | Prove the following statement |
| `{{THEOREM_TO_PROVE}}` | Statement to prove | det(AB) = det(A)det(B) |
| `{{HINT_5}}` | Hint for problem 5 | Use the definition of determinant |
| `{{POINTS_6}}` | Points for bonus | 10 |
| `{{PROBLEM_6_TEXT}}` | Bonus problem | Generalize the result to n matrices |
| `{{FORMULA_1}}` | Reference formula 1 | \det(A) = \sum_{\sigma} \text{sgn}(\sigma) \prod a_{i\sigma(i)} |
| `{{FORMULA_2}}` | Reference formula 2 | \text{tr}(A) = \sum_{i} a_{ii} |
| `{{FORMULA_3}}` | Reference formula 3 | Av = \lambda v |

## Structure

- **Header**: Course info, due date, total points
- **Student Info Box**: Name, ID, collaborators
- **Instructions**: Submission guidelines
- **Problems**: Numbered problems with point values
- **Subproblems**: Lettered parts (a), (b), (c)
- **Hints**: Optional hints in colored boxes
- **Reference Formulas**: Useful formulas section
- **Submission Checklist**: Final checklist

## Environments

The template provides several useful environments:
- `problem` - Main problem environment with points
- `subproblems` - Enumerated subparts (a), (b), (c)
- `solution` - Solution environment (for answer keys)
- `hint` - Hint boxes in amber color
- `\points{n}` - Command to display point values
- `\answerspace{height}` - Blank space for answers
- `\answerbox{height}` - Bordered box for answers

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Packages: `amsmath`, `amssymb`, `amsthm`, `enumitem`, `tcolorbox`, `fancyhdr`, `lastpage`, `framed`

## Compilation

```bash
pdflatex main.tex
pdflatex main.tex  # Run twice for page references
```

## Creating Answer Keys

To create an answer key version:
1. Uncomment all `\begin{solution}...\end{solution}` blocks
2. Optionally add "[ANSWER KEY]" to the title
3. Compile as usual

## Customization

- Add more problems by copying the problem environment
- Adjust point values as needed
- Modify colors using `\definecolor` commands
- Add/remove the formula sheet section
- Customize instructions for your course
