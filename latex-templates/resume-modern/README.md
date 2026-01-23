# Modern Resume

Clean, professional one-page resume template with modern styling. Suitable for industry positions across various fields. Features a clean layout with sections for experience, education, skills, projects, and certifications.

## Usage

1. Replace all `{{PLACEHOLDER}}` values with your information
2. Compile with XeLaTeX or LuaLaTeX (recommended for fontawesome5): `xelatex main.tex`
3. Alternatively, use pdfLaTeX if you have fontawesome5 properly installed
4. Adjust sections as needed for your background

## Placeholders

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{NAME}}` | Your full name | John Smith |
| `{{PROFESSIONAL_TITLE}}` | Your professional title | Senior Software Engineer |
| `{{EMAIL}}` | Your email address | john.smith@email.com |
| `{{PHONE}}` | Your phone number | (555) 123-4567 |
| `{{LINKEDIN}}` | LinkedIn profile (username) | linkedin.com/in/johnsmith |
| `{{LOCATION}}` | City, State/Country | Boston, MA |
| `{{PROFESSIONAL_SUMMARY}}` | Brief professional summary | Results-driven software engineer with 5+ years... |
| `{{JOB_TITLE_1}}` | Most recent job title | Senior Software Engineer |
| `{{COMPANY_1}}` | Most recent employer | Tech Corp Inc. |
| `{{EMPLOYMENT_TYPE_1}}` | Employment type | Full-time |
| `{{DATE_RANGE_1}}` | Employment dates | Jan 2022 - Present |
| `{{ACHIEVEMENT_1_1}}` | First achievement at job 1 | Led development of microservices architecture |
| `{{ACHIEVEMENT_1_2}}` | Second achievement at job 1 | Reduced API response time by 40% |
| `{{ACHIEVEMENT_1_3}}` | Third achievement at job 1 | Mentored 3 junior developers |
| `{{JOB_TITLE_2}}` | Second job title | Software Engineer |
| `{{COMPANY_2}}` | Second employer | ABC Solutions |
| `{{EMPLOYMENT_TYPE_2}}` | Employment type | Full-time |
| `{{DATE_RANGE_2}}` | Employment dates | Jun 2019 - Dec 2021 |
| `{{ACHIEVEMENT_2_1}}` | First achievement at job 2 | Developed RESTful APIs serving 1M+ requests/day |
| `{{ACHIEVEMENT_2_2}}` | Second achievement at job 2 | Implemented CI/CD pipeline |
| `{{ACHIEVEMENT_2_3}}` | Third achievement at job 2 | Collaborated with cross-functional teams |
| `{{JOB_TITLE_3}}` | Third job title | Junior Developer |
| `{{COMPANY_3}}` | Third employer | Startup XYZ |
| `{{EMPLOYMENT_TYPE_3}}` | Employment type | Internship |
| `{{DATE_RANGE_3}}` | Employment dates | May 2018 - Aug 2018 |
| `{{ACHIEVEMENT_3_1}}` | First achievement at job 3 | Built frontend components using React |
| `{{ACHIEVEMENT_3_2}}` | Second achievement at job 3 | Wrote unit tests with 90% coverage |
| `{{DEGREE_1}}` | Primary degree | Master of Science in Computer Science |
| `{{GRADUATION_DATE_1}}` | Graduation date | May 2019 |
| `{{UNIVERSITY_1}}` | University name | Massachusetts Institute of Technology |
| `{{GPA_1}}` | GPA (optional) | 3.9/4.0 |
| `{{EDUCATION_DETAIL_1}}` | Additional education detail | Thesis: Machine Learning for NLP |
| `{{DEGREE_2}}` | Secondary degree | Bachelor of Science in Computer Science |
| `{{GRADUATION_DATE_2}}` | Graduation date | May 2017 |
| `{{UNIVERSITY_2}}` | University name | University of California, Berkeley |
| `{{TECHNICAL_SKILLS}}` | Technical skills list | Python, Java, JavaScript, SQL, AWS, Docker |
| `{{TOOLS}}` | Tools and software | Git, Jenkins, Kubernetes, Terraform |
| `{{LANGUAGES}}` | Programming or spoken languages | English (Native), Spanish (Intermediate) |
| `{{SOFT_SKILLS}}` | Soft skills | Leadership, Communication, Problem-solving |
| `{{PROJECT_1_NAME}}` | First project name | Open Source Contribution |
| `{{PROJECT_1_DATE}}` | Project date | 2023 |
| `{{PROJECT_1_DESCRIPTION}}` | Project description | Contributed to TensorFlow documentation |
| `{{PROJECT_2_NAME}}` | Second project name | Personal Portfolio Website |
| `{{PROJECT_2_DATE}}` | Project date | 2022 |
| `{{PROJECT_2_DESCRIPTION}}` | Project description | Built responsive website using React and Next.js |
| `{{CERTIFICATION_1}}` | First certification | AWS Solutions Architect Associate |
| `{{CERTIFICATION_1_DATE}}` | Certification date | 2023 |
| `{{CERTIFICATION_2}}` | Second certification | Google Cloud Professional Data Engineer |
| `{{CERTIFICATION_2_DATE}}` | Certification date | 2022 |

## Structure

- **Header**: Name, title, contact information with icons
- **Professional Summary**: Brief overview of qualifications
- **Professional Experience**: Work history with achievements
- **Education**: Degrees and relevant coursework
- **Skills**: Technical skills, tools, languages, soft skills
- **Projects**: Notable personal or open source projects
- **Certifications**: Professional certifications

## Requirements

- LaTeX distribution (TeX Live, MiKTeX, or MacTeX)
- Packages: `fontawesome5`, `geometry`, `titlesec`, `enumitem`, `hyperref`, `xcolor`, `tabularx`, `multicol`
- XeLaTeX or LuaLaTeX recommended for best font support

## Compilation

```bash
xelatex main.tex
```

Or with pdfLaTeX:
```bash
pdflatex main.tex
```

## Customization Tips

1. Remove sections that don't apply to your background
2. Reorder sections based on what's most relevant
3. Adjust colors by modifying the `\definecolor` commands
4. Keep to one page for most positions
5. Use action verbs and quantify achievements where possible
