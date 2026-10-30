## 2026-10-29 — Setup Exercise: search/ personal layer built (yashika-lodh)

- **Recipe:** manual (Setup Exercise / Tutorial 00), agent-assisted intake in Claude chat
- **Inputs:** my resume (PDF), my public GitHub repos, intake interview, data/bls/compact/soc_occupation_compact.csv, three live job postings (Rillet Design Engineer, HappyRobot Forward Deployed Engineer, Coinflow Software Engineer; accessed 2026-10-29)
- **Outputs (local, gitignored — never committed):** search/resume.json (attested 2026-10-29), search/profile.yml, search/gaps.md
- **Privacy:** `git check-ignore -v search/private-notes.md` → `.gitignore:43:/search/*`. The handout's extra .gitignore line was redundant with the repo's existing `/search/*` rule, so I reverted it rather than touch a shared file.

**Attestation errors caught (resume.json):**
1. Buffett Intelligence corpus was misstated as "1K+ letters and Q&A pairs"; the repo shows one 1,010-page letters PDF plus 5,992 Q&A pairs.
2. Dynamic Pricing Engine read as solo with a stale "39 JUnit tests"; it was a 4-person team, the bullet is now scoped to my parts, and the test suite I wrote is now 46 tests (JUnit 5 + Spring Boot Test), 0 failures.
3. PawConnect's bullet claimed the whole platform; it was a 4-person team and my parts were two pages.
(Also corrected: NewEra IT title to offer-letter wording; "Redux Toolkit" → "Redux"; GraphQL moved to familiar_with_not_shipped, since its only appearance was a teammate's work.)

**SOC gate:** 15-1252 Software Developers (primary), 15-1254 Web Developers (secondary).

**Top gap:** Node.js backend depth — P2 lists React/TypeScript/Node.js as a must-have and P3 asks for TypeScript/Node; I have never built and owned a full Node/TypeScript API end to end. Plan: a tested, deployed TypeScript/Node API with a database by mid-December 2026.

**Killed row:** "One year of professional experience" (P3) — Reason: the agent treated my two internships as falling short of a year, but together they are about 14 months of engineering work (6 months NewEra IT, 8 months Aikreate as sole engineer).

**profile.yml field corrected from agent draft:** `visa.current_status` — the agent's prior record said "STEM OPT"; my documents say F-1, still in program, OPT filing in progress. EAD/OPT dates set to `uncertain` instead of guessed.

**Verification check:**
- resume.json: every job and project now traces to an offer letter or a public repo; employer-internal work is evidenced by offer letter only. Hardest to verify: the "50+ students" metric, which rests on my own knowledge.
- profile.yml: visa fields match my actual status; STEM eligibility is DSO-confirmed; no date was guessed. Buffer target 80 taken from Ch. 10 after the example personas showed 20/30.
- gaps.md: every evidence cell quotes P1–P3, but one row overstated demand: Go/Rust was listed as a gap when P3 calls it only "a plus" (and Python, which I have, satisfies that line) — removed. Rows 3 and 5 each cite two postings, but P1's line in row 5 is softer than a requirement.

- **Open issues:** EAD dates pending; sponsorship status of the three posting companies not yet checked with the scorer; P1/P2 likely past my Series C target.
