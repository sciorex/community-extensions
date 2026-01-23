# Course Syllabus Template

A comprehensive course syllabus template with schedule table, grading policies, and university policy sections. Suitable for any academic course at the undergraduate or graduate level.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your course information
2. Compile with pdfLaTeX: `pdflatex main.tex`
3. Customize sections as needed for your institution

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| {{COURSE_CODE}} | Course code/number | CS 101 |
| {{COURSE_NAME}} | Full course name | Introduction to Computer Science |
| {{SEMESTER}} | Academic semester | Fall |
| {{YEAR}} | Academic year | 2026 |
| {{INSTRUCTOR}} | Instructor's full name | Dr. Jane Smith |
| {{EMAIL}} | Instructor's email | jsmith@university.edu |
| {{OFFICE}} | Office location | Science Building 301 |
| {{OFFICE_HOURS}} | Office hours | Mon/Wed 2:00-4:00 PM |
| {{CLASS_TIME}} | Class meeting time | MWF 10:00-10:50 AM |
| {{LOCATION}} | Classroom location | Lecture Hall A |
| {{COURSE_DESCRIPTION}} | Description of the course | This course introduces fundamental concepts... |
| {{OBJECTIVE_1}} through {{OBJECTIVE_5}} | Learning objectives | Understand basic programming concepts |
| {{TEXTBOOK_TITLE}} | Required textbook title | Introduction to Algorithms |
| {{TEXTBOOK_AUTHOR}} | Textbook author(s) | Cormen, Leiserson, Rivest, Stein |
| {{TEXTBOOK_EDITION}} | Textbook edition | 4th Edition |
| {{TEXTBOOK_ISBN}} | Textbook ISBN | 978-0262046305 |
| {{GRADE_COMPONENT_1}} through {{GRADE_COMPONENT_5}} | Grading components | Homework Assignments |
| {{GRADE_WEIGHT_1}} through {{GRADE_WEIGHT_5}} | Component weights | 25% |
| {{WEEK_1_DATES}} through {{WEEK_15_DATES}} | Week date ranges | Jan 15-19 |
| {{WEEK_2_TOPIC}} through {{WEEK_13_TOPIC}} | Weekly topics | Variables and Data Types |
| {{WEEK_2_ASSIGNMENT}} through {{WEEK_12_ASSIGNMENT}} | Weekly assignments | HW 1 Due |
| {{UNIVERSITY}} | University name | State University |
| {{COUNSELING_CENTER_CONTACT}} | Counseling center contact | (555) 123-4567 |

## Structure

The syllabus includes the following sections:

1. **Instructor Information** - Contact details and office hours
2. **Course Description** - Overview of the course
3. **Learning Objectives** - What students will learn
4. **Required Materials** - Textbooks and other materials
5. **Grading Policy** - Grade distribution and scale
6. **Course Schedule** - Week-by-week schedule table
7. **Course Policies** - Attendance, late work, academic integrity
8. **University Policies** - Disability accommodations, Title IX
9. **Additional Resources** - Tutoring, writing center, etc.

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Required packages (all standard):
  - geometry
  - fancyhdr
  - lastpage
  - microtype
  - parskip
  - booktabs
  - longtable
  - enumitem
  - hyperref
  - xcolor
  - titlesec

## Compilation

```bash
pdflatex main.tex
```

For the table of contents to work correctly, run pdflatex twice.

## Customization Tips

- Modify the color scheme by changing `headerblue` in the color definitions
- Adjust margins using the geometry package options
- Add or remove weeks in the schedule table as needed
- Customize university policies to match your institution's requirements
- Add a course logo by including the graphicx package and using `\includegraphics`

## Notes

- The schedule uses a longtable for multi-page support
- Page numbers show "Page X of Y" format
- All hyperlinks are clickable in the PDF
- The template is designed for US Letter paper; change to a4paper in geometry for A4
