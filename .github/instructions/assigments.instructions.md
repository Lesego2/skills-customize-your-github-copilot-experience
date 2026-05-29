---
description: "Instructions to use whenever creating or editing assignment markdown files to ensure consistency and clarity for students."
applyTo: "assignments/**/*.md"
---

# Assignment Markdown Structure Guidelines

All assignment markdown files in `assignments/` must follow the project template and formatting conventions so students see a consistent experience.

## 1. Template and filename

- Use the template at [`templates/assignment-template.md`](../../templates/assignment-template.md) exactly for section order and icons.
- Each assignment must be a `README.md` located inside its assignment folder (for example `assignments/python-basics/README.md`).
- Do not remove or rename required template sections (Title, Objective, Tasks and each Task's Description/Requirements).

## 2. Required headers and exact icons

Match the template headings and emoji exactly so that generated lists and previews remain consistent:

- `# 📘 Assignment: [Assignment Title]`
- `## 🎯 Objective`
- `## 📝 Tasks`
- For each task: `### 🛠️	[Task Title]`, then `#### Description` and `#### Requirements`

## 3. Section guidance

- **Title**: Use a concise, descriptive name (e.g., Python Basics, Loops and Conditionals).
- **Objective**: 1–2 sentences describing the learning goal or deliverable.
- **Tasks**: Break the assignment into 1..N concrete tasks. For each task:
   - Description: short, actionable instructions for the student.
   - Requirements: a bullet list of concrete, testable outcomes the submission must meet.
   - Include example input/output or sample commands in fenced code blocks where useful.

## 4. Files and starter code

- If the assignment requires starter files, include them in the same assignment folder (e.g., `starter-code.py`, `data.csv`).
- Mention any expected filenames, runtime command (e.g., `python3 starter-code.py`), and required Python version if applicable.

## 5. Formatting and accessibility

- Use fenced code blocks for code and example I/O.
- Use bulleted lists for requirements and steps; keep lines < 80 characters where practical.
- Write clear, student-friendly language and avoid jargon.

## 6. Additional notes for maintainers

- Keep assignments focused: prefer a small number of well-scoped tasks rather than many tiny tasks.
- If extra sections are needed (e.g., "Hints" or "Stretch Goals"), add them after the required sections and label them clearly.
- Updates to the template must be coordinated with course maintainers to avoid breaking existing assignments.

Refer to the canonical template when creating or editing assignments: [`templates/assignment-template.md`](../../templates/assignment-template.md).