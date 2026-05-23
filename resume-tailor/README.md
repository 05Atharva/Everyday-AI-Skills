# Resume Tailor Skill

`resume-tailor` is a surgical resume optimization skill.  
It tailors an existing resume to a target Job Description (JD) without inventing experience, tools, or metrics.

## What is included

- `SKILL.md`: The core engine, structured across 9 phases.
- `references/ats-keywords.md`: Domain-specific ATS keyword guidance.
- `references/bullet-rewriting.md`: Before/after bullet rewriting patterns.
- `references/domain-vocabulary.md`: Domain terminology support.
- `resume-tailor.skill`: Packaged skill bundle (for tools that support direct import).

## Core engine (`SKILL.md`)

`SKILL.md` is organized as a strict 9-phase workflow:

1. Knowledge Base Assembly (resumes, JD, portfolio, LinkedIn, certs, etc.)
2. JD Analysis with tiered keyword extraction (Must-Have / Strong Signal / Nice-to-Have)
3. Tailoring Strategy planning before any edits
4. Surgical Editing Rules with explicit "may do" and "must not do" constraints
5. Formatting Preservation Framework (bullets, spacing, hyperlinks, style, ATS safety)
6. Anti-Hallucination Framework with a hard checklist before every edit
7. ATS Optimization Strategy
8. Structured Output (Tailored Resume + Changes Summary + Optional Suggestions)
9. Dynamic Domain Detection across all professional fields

## Reference files (loaded on demand)

The skill uses these only when relevant to the current target role/domain:

1. `ats-keywords.md`: Keyword banks for 12+ domains
2. `bullet-rewriting.md`: Before/after surgical edit examples with anti-pattern warnings
3. `domain-vocabulary.md`: Cross-domain vocabulary mapping and detection signals

## Inputs this skill expects

Required:
- Existing resume
- Target job description (JD)

Optional:
- Portfolio/GitHub links
- LinkedIn profile
- Certifications
- Extra project/work details

## Add your Knowledge Base

In the same Claude project (or equivalent AI workspace), upload your supporting documents:

1. Your resume(s) (PDF or DOCX)
2. Portfolio descriptions (text or PDF)
3. Certifications list
4. Skills database
5. Any project write-ups

## Setup in Claude.ai (recommended workflow)

1. Open Claude and create a new **Project**.
2. Open `resume-tailor/SKILL.md` and copy all content.
3. In Claude Project Instructions, paste the full `SKILL.md` content.
4. Upload the reference files from `resume-tailor/references/` to the same project.
5. Start a chat in that project and provide:
- Your resume
- The exact JD text
- Any optional supporting files/details

Example prompt:

```text
Tailor my resume for this job description using the project instructions.
Keep edits surgical and ATS-friendly. Do not invent anything.
```

## Setup in other AI tools (ChatGPT, Gemini, etc.)

Use the same pattern:

1. Create a dedicated chat/project/custom GPT space.
2. Paste `SKILL.md` into system/custom instructions.
3. Upload files from `references/` if the tool supports file context.
4. Provide resume + JD in the chat.

If your tool does not support instruction memory or file uploads:
- Paste `SKILL.md` at the top of each session.
- Paste key reference snippets manually when needed.

## Using the `.skill` file

If your platform supports importing `.skill` bundles:

1. Import `resume-tailor.skill`.
2. Verify the imported skill includes `SKILL.md` and references.
3. Start tailoring using resume + JD inputs.

If `.skill` import is not supported, use the manual setup steps above.

## Best practices for good output

1. Provide full JD text, not just a job title.
2. Share your latest resume version (PDF/DOCX/text).
3. Add optional links/details for stronger alignment.
4. Ask for a "changes summary" so edits are transparent.
5. Review every claim before applying final resume updates.

## Important constraint

This skill is **not** a resume-from-scratch generator.  
It is designed to edit and optimize an existing resume using only user-provided facts.
