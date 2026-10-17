---
name: weekly-revision-checklist
description: "Helps university students turn their course materials and available study time into a weekly revision checklist. Use when a student says \"help me revise\", \"quiz me\", or asks to plan weekly revision. It is not for completing graded homework, exams, or other assessed work."
license: MIT
---

# Weekly Revision Checklist

## When to use this skill

Use this skill when a university student wants a manageable plan for reviewing course material over the coming week, or wants to practise recall with a short quiz based on material they provide.

Do not activate it to answer graded questions or produce work for submission.

## Gather first

Ask for any details that are missing and relevant to the request:

- The course or subject and the topics or materials to review.
- The days and approximate study time available this week.
- Any assessment or class dates the student wants the plan to account for.
- Whether they prefer a checklist, a quiz, or both.
- For a quiz, notes, learning objectives, or other source material to base questions on.

Do not require private or identifying information. If the student has not supplied enough information, ask a concise follow-up or clearly label the plan as a general template. Never invent course content, deadlines, or available study time.

## Process

1. Confirm the week or date range and the student's stated goals. If dates are unclear, use “this week” without inventing dates.
2. Collect and organize the topics from the student's materials. Flag gaps or ambiguous items instead of filling them with guesses.
3. Fit review tasks to the time and days the student actually gives. If time is unknown, avoid specific duration estimates.
4. Break each topic into a concrete study action, such as reviewing a provided set of notes, recalling key ideas from memory, or answering a practice question based on supplied material.
5. Put any student-provided deadlines in the appropriate order. Do not infer urgency from unsupported assumptions.
6. If asked to quiz the student, ask one question at a time from the provided material, wait for their answer, then give brief feedback grounded in that material. If the source does not support an answer, say so.
7. Present the checklist and invite the student to adjust it if their availability or priorities change.

## Output format

Use a concise weekly checklist. Include only information supported by the user's input.

- **Week:** user-provided date range, or “this week”
- **Goal:** one short statement based on the user's request
- **Checklist:** tasks grouped by day when availability is known; otherwise an unassigned list
- **Assessment dates:** include only dates the student provided
- **Open questions:** note missing details that materially affect the plan

Use Markdown checkboxes (`- [ ]`) for tasks. For quiz requests, start an interactive one-question-at-a-time quiz instead of presenting an answer key.

## Boundaries

- Do not complete, solve, or write answers for graded homework, exams, or assessed submissions.
- Do not help the student evade course rules or misrepresent generated work as their own.
- Do not invent facts about a course, a student's schedule, assessment requirements, or source material.
- Do not present a checklist as a guarantee of a grade or outcome.
- Keep the plan proportional to the details provided; ask rather than overcomplicate it.
