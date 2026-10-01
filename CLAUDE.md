# Job Search: Cybersecurity Resume & JD Review

This Project supports Angela Reeder's 2026 cybersecurity job search, primarily Junior Cyber Threat Intelligence Analyst roles, though adjacent IT/security roles may also come through here. Use this file as standing instructions for every conversation in this Project.

## Background (for context, not to restate unprompted)

- Certifications: GIAC GFACT, GSEC, GCIH; (ISC)² CC; Google: Cybersecurity Professional; MAD20 Cyber Threat Intelligence Certification
- Organizations: Women in CyberSecurity (WiCys); Women + Cybersecurity = Women's Society of Cyberjutsu
- Mentorship: WiCyS Technical Mentor for Google Cybersecurity Professional Certificate cohort (2024, 2025, 2026)

## Master resume

The master resume is found at Job Search\Angela R Resume.docx (updated 2026-09-30). It is the single source of truth. Use it by default for any review or edit in this Project.

If Angela uploads a resume file in a given turn, treat that upload as the authoritative version for that turn. Use it instead of the stored master, and ask whether it should replace the stored master copy going forward. Don't overwrite the master file without confirmation.

## Standard workflow: reviewing a job description

When Angela shares a job description (pasted or attached) and asks for a review, fit check, or tailoring:

1. Use the `cyber-resume-reviewer` skill (`anthropic-skills:cyber-resume-reviewer`). Follow its truth and scope invariants strictly: no invented metrics, employers, dates, tools, or experience; unresolved facts go to Open Questions, not into the resume.
2. **Give the candid fit verdict first, on its own, before producing the full report.** State plainly whether this looks like a strong, moderate, or weak match, and name the one or two biggest reasons why. Then ask whether Angela wants the full prioritized-findings-and-exact-edits report, or wants to skip this one.
   - Only skip straight to the full report without asking if Angela has already indicated in that message that she wants the complete treatment regardless of fit (e.g., "review this one fully," "give me the whole report").
3. If she wants the full report, deliver it in the same structure used so far: Fit Verdict, Strongest Evidence to Preserve, Prioritized Findings, Exact Edits (with current/suggested text), Open Questions.
4. **Deliverable format: Markdown only**, delivered as a file. Do not render a PDF unless asked.
5. **Save each full report in this Project** at `Job Search\reviews\YYYY-MM-DD-company-###.md`, using the company's ID from `Job Search\job-search\company-map.md` (assign one first if it's a new company), never the real company name, in the file name or in the report text. Reports stay private to the Project; never suggest putting them in a public repo. Quick verdicts that don't get a full report are logged only, with notes in the log if useful.
6. After the review is delivered (whether full report or just the quick verdict), log it. See Application Log below.

## Application log

This repo is public, so `Job Search\job-search\applications-log.md` never contains real company names. Company identity lives only in `Job Search\job-search\company-map.md`, which is gitignored and stays local.

Keep a running log at `Job Search\job-search\applications-log.md` in this Project (create it if it doesn't exist yet). After each JD review:

1. Check `Job Search\job-search\company-map.md` for this company. If it's already there, reuse its ID. If not, assign the next sequential ID (zero-padded, e.g. `001`, `002`) and add a row to `Job Search\job-search\company-map.md`: `| ID | Company |`.
2. Append a row to `Job Search\job-search\applications-log.md` using the ID in place of the company name:

| Date       | Company     | Role       | Verdict                                        | Status                                                         |
| ---------- | ----------- | ---------- | ---------------------------------------------- | -------------------------------------------------------------- |
| YYYY-MM-DD | Company ### | Role title | Strong / Moderate / Weak fit + one-line reason | Reviewed / Applied / Skipped / Interviewing / Rejected / Offer |

3. If the review has a Notes section (e.g. for a legitimacy check, or anything with prose detail), use the same "Company ###" form there too instead of the real name. Don't let it leak into free text either.
4. When a full report is saved, add a line under Notes pointing to its `Job Search\reviews` path.

- Set "Status" to "Reviewed" by default when logging a new review. Update it later if Angela says she applied, heard back, got an interview, etc. She'll need to tell you the status change; don't infer it.
- Don't create a new log file per review. Always append to the same one.

- If Angela asks for a summary of her search (e.g., "how many have I reviewed," "what's my pipeline look like"), read this file rather than reconstructing from conversation history. If she asks which company an ID refers to, check `Job Search\job-search\company-map.md`.

## Cover letters

When asked to draft a cover letter for a specific JD:

- Base it only on experience already established in the master resume or stated directly by Angela in conversation. Same truth invariants as the resume work (no invented achievements, metrics, or enthusiasm-driven claims not grounded in fact).
- Match tone to the target role: for security-analyst-style roles, technical and direct; for process/governance-style roles, lean into the transferable documentation/process/stakeholder-communication experience.
- If the JD review surfaced a real gap (e.g., no ITIL cert, no formal process-mapping experience), don't paper over it in the cover letter. Address it honestly if it's a named requirement, or simply don't claim it.

## House style (applies to all drafted writing in this Project)

- No em dashes. Use a period and a new sentence instead. Semicolons are fine, sparingly.
- Avoid writing that reads as AI-generated: no generic corporate filler, no inflated enthusiasm, no formulaic "I am excited to apply..." openers unless Angela's own voice would actually say that. Write plainly, the way she'd say it herself.
- Never invent or round up metrics, dates, employers, or scope of responsibility. If something needs a number and none exists, leave it out or flag it as an open question. Don't estimate.
