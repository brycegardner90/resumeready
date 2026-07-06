# ResumeReady

**Fill out your career profile once. Paste it into any AI, once per job hunt. Get a tailored resume or cover letter — no subscription, no lock-in, no lost history between applications.**

[Live demo →](https://brycegardner90.github.io/resumeready/)

## The problem this solves

Tailoring a resume to every job posting is tedious, even with AI — you end up re-explaining your whole background in every new chat. ResumeReady flips that: you do one structured "brain dump" of your entire career (messy, unpolished, in whatever order it comes), save it as a plain `.txt` file, and then reuse it across an entire job search. Paste it into a Claude, ChatGPT, or Gemini conversation once, then for every new posting you just paste the job description and ask again.

## How it works

1. **Brain dump your profile** — personal info, work history, education, skills, projects, references, and private context the AI should know but a resume never shows (career gaps, salary targets, companies to avoid, employers to never mention).
2. **Save it** — everything is stored in your browser only (`localStorage`) and/or downloaded as a portable `.txt` file. Nothing is ever sent to a server; this is a single static HTML file with no backend.
3. **Generate per job** — either copy a ready-to-paste AI prompt (profile + job posting bundled together) or download the `.txt` and paste it yourself into whatever AI you use.

## Why plain text

A `.txt` file is small enough to work on free AI plans, easy for any model to read closely, and fully portable — no vendor lock-in to one AI tool's paid tier.

## Built-in guardrails

The generated prompts explicitly instruct the AI to:
- Never invent numbers, metrics, skills, or employers not in your profile
- Respect an "always omit" list (jobs/employers that must never appear on any document)
- Frame career gaps honestly rather than papering over them
- Format output for PDF export and suggest a versioned filename, since PDF is what most employers expect

## Privacy

Everything runs client-side. Your data never leaves your browser unless you choose to download or copy it yourself. The only exception is anonymous, cookie-free page-view analytics ([GoatCounter](https://www.goatcounter.com/)) — no personal data, no profile content, ever included.

## Tech

Single-file HTML/CSS/vanilla JS — no build step, no dependencies. Open `index.html` directly or serve it from any static host.

## Feedback

Found a bug or have an idea? [Open an issue](https://github.com/brycegardner90/resumeready/issues) — that's the best way to make sure it doesn't get lost.

## License

© 2026 Bryce Gardner. All rights reserved — see [LICENSE](LICENSE). Viewing this repo and using the hosted app is welcome; copying or redistributing the source requires permission.
