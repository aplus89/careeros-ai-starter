---
name: job-fit-analyzer
description: Compare a real candidate profile or CV with a specific job description, estimate fit, identify ATS keywords and gaps, and recommend Apply, Maybe, or Skip. Use for application decisions and truthful tailoring, not as a guarantee of ATS or hiring outcomes.
---

# Job Fit Analyzer

Compare the candidate's documented evidence with the job description and produce an honest, actionable decision.

## Required inputs

- Candidate profile, CV, or equivalent evidence.
- Full job description or enough text to identify responsibilities and requirements.

If one is missing, request it. Do not infer qualifications from a job title alone.

## Scoring model

Calculate an **estimated fit score**, not an ATS score:

- Must-have requirements: 40%
- Experience evidence: 25%
- ATS keyword overlap: 15%
- Seniority and domain fit: 10%
- Location, language, and work model: 5%
- Risk flags: 5%

Explain the evidence behind every component. A missing signal is not automatically a missing skill; label the distinction.

## Decision bands

- **Apply:** 80–100 and no disqualifying constraint.
- **Maybe:** 65–79, or a resolvable uncertainty materially affects fit.
- **Skip:** below 65 or a confirmed disqualifier makes the application inefficient.

Adjust the recommendation when compensation, location, legal eligibility, schedule, or an explicit degree/certification requirement is a real blocker.

## Truth rules

- Never invent experience, metrics, certifications, degrees, tools, or eligibility.
- Do not rewrite a gap as experience.
- Suggest keywords only when the candidate has evidence for them.
- Distinguish `confirmed gap`, `missing evidence`, and `transferable evidence`.
- Do not promise an interview or claim access to an employer's ATS algorithm.

## Output

Return:

1. Decision and estimated fit score.
2. Score breakdown with concise evidence.
3. Strong matches.
4. Confirmed gaps and missing signals.
5. ATS keywords: supported, unsupported, and absent from the CV.
6. Recommended positioning angle.
7. Truthful CV changes, ordered by impact.
8. Short recruiter or hiring-manager message when useful.
9. Interview risks and likely questions.
10. One next action.

Use `../../templates/analisis-vacante.md` when the user asks for an editable analysis.
