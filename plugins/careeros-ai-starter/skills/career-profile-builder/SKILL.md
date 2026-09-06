---
name: career-profile-builder
description: Build or improve a master professional profile from a CV, LinkedIn text, portfolio, notes, or interview answers. Use before tailoring applications or when the user needs clearer positioning. Do not use to invent credentials or experience.
---

# Career Profile Builder

Create an evidence-based master profile that can support resumes, LinkedIn, applications, and interviews.

## Inputs

Use any material the user provides: CV, LinkedIn profile, portfolio, job history, project notes, or answers to questions. If evidence is incomplete, mark it as unknown and ask only the few questions that would materially improve the result.

Do not require personal identifiers that are unnecessary for career analysis. Warn the user before reproducing sensitive information such as an ID number, home address, salary history, or references' contact details.

## Rules

- Never invent employers, dates, titles, degrees, certifications, technologies, metrics, or outcomes.
- Separate confirmed facts from interpretations and opportunities to quantify.
- Reframe real experience strategically without changing its truth.
- Preserve the user's language unless they request another one.
- Prefer specific evidence over adjectives such as “excellent” or “visionary.”

## Output

Return:

1. Positioning statement.
2. Two to four target role families, with reasons.
3. Evidence ledger: role/project, problem, actions, tools, result, proof status.
4. Core skills grouped into domain, execution, technical, and leadership.
5. Achievement bank with confirmed metrics and `[metric needed]` markers.
6. Career risks or unclear claims that need verification.
7. A concise master professional profile.
8. The five highest-value follow-up questions, only if needed.

When the user wants a reusable file, adapt the structure in `../../templates/perfil-profesional.md`.
