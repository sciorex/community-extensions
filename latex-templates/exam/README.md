# Exam Paper

Comprehensive examination paper template with cover page, instructions, multiple question types, and answer spaces. Suitable for midterms, finals, quizzes, and standardized tests.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your content
2. Compile with pdfLaTeX: `pdflatex main.tex`
3. Run twice for correct page numbering
4. Customize question types and sections as needed

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{INSTITUTION}}` | University/institution name | Stanford University |
| `{{DEPARTMENT}}` | Department name | Department of Computer Science |
| `{{EXAM_TYPE}}` | Type of exam | Final Examination |
| `{{COURSE_CODE}}` | Course identifier | CS 229 |
| `{{COURSE_NAME}}` | Course name | Machine Learning |
| `{{SEMESTER}}` | Semester/term | Fall 2024 |
| `{{DATE}}` | Exam date | December 15, 2024 |
| `{{DURATION}}` | Exam duration | 3 hours |
| `{{TOTAL_POINTS}}` | Total points | 100 |
| `{{INSTRUCTOR}}` | Instructor name | Prof. Andrew Ng |
| `{{Q1_POINTS}}` | Points for question 1 | 10 |
| `{{Q2_POINTS}}` | Points for question 2 | 10 |
| `{{Q3_POINTS}}` | Points for question 3 | 20 |
| `{{Q4_POINTS}}` | Points for question 4 | 25 |
| `{{Q5_POINTS}}` | Points for question 5 | 25 |
| `{{INSTRUCTION_1}}` | Instruction 1 | Write clearly in blue or black ink |
| `{{INSTRUCTION_2}}` | Instruction 2 | Answer all questions |
| `{{INSTRUCTION_3}}` | Instruction 3 | This is a closed-book exam |
| `{{INSTRUCTION_4}}` | Instruction 4 | Calculators are not permitted |
| `{{MATERIALS_ALLOWED}}` | Allowed materials | One 8.5x11 handwritten cheat sheet |
| `{{MC_QUESTION_1}}` | Multiple choice question 1 | Which algorithm has O(n log n) complexity? |
| `{{MC_1_OPTION_A}}` | Option A | Bubble Sort |
| `{{MC_1_OPTION_B}}` | Option B | Merge Sort |
| `{{MC_1_OPTION_C}}` | Option C | Selection Sort |
| `{{MC_1_OPTION_D}}` | Option D | Insertion Sort |
| `{{MC_QUESTION_2}}` | Multiple choice question 2 | What is the gradient of f(x) = x^2? |
| `{{MC_2_OPTION_A}}` | Option A | x |
| `{{MC_2_OPTION_B}}` | Option B | 2x |
| `{{MC_2_OPTION_C}}` | Option C | x^2 |
| `{{MC_2_OPTION_D}}` | Option D | 2 |
| `{{TF_QUESTION_1}}` | True/False question 1 | SVMs always find a global optimum |
| `{{TF_QUESTION_2}}` | True/False question 2 | Neural networks are convex models |
| `{{SHORT_ANSWER_1}}` | Short answer question | Explain the bias-variance tradeoff |
| `{{SHORT_1A}}` | Subquestion a | Define bias in ML |
| `{{Q3A_POINTS}}` | Points for 3a | 10 |
| `{{SHORT_1B}}` | Subquestion b | Define variance in ML |
| `{{Q3B_POINTS}}` | Points for 3b | 10 |
| `{{PROBLEM_1}}` | Problem solving question | Derive the gradient descent update |
| `{{GIVEN_1}}` | Given condition 1 | Loss function L(w) = ||Xw - y||^2 |
| `{{GIVEN_2}}` | Given condition 2 | Learning rate alpha |
| `{{FIND_1}}` | What to find | The update rule for w |
| `{{PROBLEM_2}}` | Problem 2 statement | Consider the following neural network |
| `{{PROBLEM_2A}}` | Subproblem a | Compute the forward pass |
| `{{Q5A_POINTS}}` | Points for 5a | 10 |
| `{{PROBLEM_2B}}` | Subproblem b | Compute the backward pass |
| `{{Q5B_POINTS}}` | Points for 5b | 10 |
| `{{PROBLEM_2C}}` | Subproblem c | Update the weights |
| `{{Q5C_POINTS}}` | Points for 5c | 5 |
| `{{Q6_POINTS}}` | Points for essay | 10 |
| `{{ESSAY_QUESTION}}` | Essay question | Compare and contrast decision trees and neural networks |
| `{{FORMULA_CATEGORY_1}}` | Formula category 1 | Derivatives |
| `{{FORMULA_1}}` | Formula 1 | \frac{d}{dx}(x^n) = nx^{n-1} |
| `{{FORMULA_2}}` | Formula 2 | \frac{d}{dx}(e^x) = e^x |
| `{{FORMULA_CATEGORY_2}}` | Formula category 2 | Linear Algebra |
| `{{FORMULA_3}}` | Formula 3 | (AB)^{-1} = B^{-1}A^{-1} |
| `{{FORMULA_4}}` | Formula 4 | \det(AB) = \det(A)\det(B) |

## Structure

- **Cover Page**: Institution, course info, student info box, grading table
- **Instructions**: Detailed exam instructions
- **Part A**: Multiple Choice questions
- **Part B**: True/False questions
- **Part C**: Short Answer questions
- **Part D**: Problem Solving questions
- **Part E**: Essay/Long Answer questions
- **Additional Space**: Extra pages for overflow
- **Formula Sheet**: Detachable reference sheet

## Question Types

The template includes environments for:
- `question` - Numbered questions with point values
- `subquestions` - Lettered subparts (a), (b), (c)
- `\choices{A}{B}{C}{D}` - Multiple choice options
- `\truefalse` - True/False circles
- `\answerbox{height}` - Bordered answer boxes
- `\answerspace{height}` - Blank answer space
- `\blank[width]` - Fill-in-the-blank lines
- `\subpoints{n}` - Point values for subquestions

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Packages: `amsmath`, `amssymb`, `enumitem`, `tcolorbox`, `fancyhdr`, `lastpage`, `multicol`, `array`

## Compilation

```bash
pdflatex main.tex
pdflatex main.tex  # Run twice for page references
```

## Customization

- **Add/remove sections**: Comment out entire `\section*{}` blocks
- **Adjust grading table**: Modify the table in the cover page
- **Change page layout**: Adjust `\geometry` settings
- **Modify colors**: Use `\definecolor` commands
- **Add more questions**: Copy question environments
- **Create solution key**: Add solutions in separate boxes

## Tips for Instructors

1. Print the formula sheet on colored paper for easy identification
2. Consider adding page numbers to the grading table
3. Include clear point breakdowns for partial credit
4. Leave adequate space for student answers
5. Test print before the exam to verify formatting
