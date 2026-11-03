# AGENTS.md — resume_builder

Single-page HTML resume tailored per Job Description (JD). Output is printed to PDF.

## Source of truth
- Root `resume.html` (to be added) is the canonical base resume. Per-JD resumes derive from it — never rewrite from scratch.
- Target roles only: cloud, DevOps, backend.

## Hard rules (never violate)
- The word **"Intern" / "Internship" must never appear anywhere** — not in `resume.html`, not in the root `resume.html`, not in `coldmail.md`, not in `coverletter.pdf`, not in `jd.md` or `100questions.md` prose you author. Present every role as a plain engineer title (e.g. "Full Stack Developer", never "Full Stack Developer Intern"). Internship-experience framing also bans hedges like "early-career", "trainee", "fresher", "fresher/junior" when used to imply internship status.
- This applies retroactively: when touching the repo, sweep **all** existing JD folders and the root `resume.html`, and regenerate any `ik_resume.pdf` you change.
- Grep before finishing: `grep -rin "intern" --include="*.html" --include="*.md" .` and fix every real hit.
  - Exception: legitimate English words that merely contain the substring — "internet", "internal", "internally", "internals" — are fine. Do not mangle them.

## Tailoring rules (per JD)
- Align resume to ~90% of JD. Do not over-fit / do not change it too much.
- NEVER change: projects section, years of experience.
- Add only dealbreaker skills missing from resume (e.g. Kubernetes, Docker, Python, ArgoCD, AWS if explicitly required).
- Skill frequency rule: collect repeating keywords from JD; repeat those core skills naturally in resume (summary + skills + experience bullets). Ignore very niche one-off tools.
- Must still fit a single PDF page with minimal top/bottom margins. Keep HTML print CSS (`@page`, single-page, compact spacing). No multi-page output.
- Change the about/summary section role as per JD but don't make it too specific (e.g. Golang Developer, Devops Engineer are good) (e.g. Golang + GraphDB developer, Devops + IAM Specialist are bad).

## Per-JD folder
- Create `<company>-<job-title>-YYYY-MM-DD/` (slugs, lowercase, e.g. `cisco-devops-engineer-2026-10-06/`). If JD has no company, fall back to `<job-title>-YYYY-MM-DD/`.
- Must contain exactly:
  - `jd.md` — full JD text + `Created: YYYY-MM-DD` header
  - `100questions.md` — 100 likely interview questions for that specific role/JD
  - `resume.html` — tailored single-page resume (copy of root adapted per rules above)
  - `ik_resume.pdf` - the pdf created from the html file
  - `coldmail.md` - a cold mail to send to recruiter. limit to 2-3 lines explaining why the candidate is the right fit
  - `coverletter.pdf` - a cover letter for the job explaining why the candidate it the right fit.
- Never edit other JD folders when adding a new one.

## Top-level project suggestions
- Maintain `suggested-projects.md` at repo root: one interviewer-impressing project idea per JD.
- Append entry per new JD: `## <company> <job-title> — YYYY-MM-DD` + 3–5 line project sketch linked to that JD's stack. Never replace prior entries.
