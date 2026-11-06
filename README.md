# interview-prep-pack

A [Claude Code](https://claude.com/claude-code) skill that turns your own files (resumes, portfolio, published work, the job posting, notes from earlier calls) into one interview prep pack you can rehearse from.

Built for SEO, GEO/AEO, AI search and growth roles, and works for any role.

| Part | What you get |
|---|---|
| Numbers sheet | Every number you can cite, with its company and period, the inconsistencies to fix before the next call, and the gap you'll be probed on |
| 25 likely questions | Screening, hiring-manager and case rounds, with the ones the posting names in bold |
| Answer outlines | A STAR outline per question, sized for 60 to 90 seconds out loud, with the one line to land |
| 30-60-90 day plan | Read and baseline, first fixes, re-measure and hand over |
| Take-home case | A mock GEO audit in seven steps, with the tools, a tracking-sheet layout and a sample ticket |
| Questions to ask | Eight, each with what the answer tells you |

One rule runs through all of it: **every story and number comes from your files.** Where no real story exists, the outline says so and gives a method instead. A made-up client is the thing the follow-up question finds.

## Install

Clone it into your personal skills folder, and it works in every project:

```bash
git clone https://github.com/s77sh/interview-prep-pack ~/.claude/skills/interview-prep-pack
```

Or put it in one project only, at `.claude/skills/interview-prep-pack/`.

## Use

Open Claude Code in the folder with your resumes and work, and ask in plain words:

- "Prep me for the interview with [company], the posting is in jobs/[file]"
- "Build an interview prep pack for senior SEO roles"
- "What will they ask me in the hiring manager round?"
- "Write me a 30-60-90 plan for an AI search lead"
- "Work through a take-home GEO audit for [brand]"

## What's inside

- `SKILL.md`: the procedure.
- `reference/seo-geo-questions.md`: what a strong answer covers for the SEO and AI search questions.
- `reference/30-60-90.md`: the plan frame.
- `reference/geo-audit-case.md`: the mock GEO audit, with an invented brand.
- `examples/example-pack.md`: a short filled pack for an invented candidate.

## Make it yours

Add a `personal.md` next to `SKILL.md` with your file paths, your voice notes, and your finished pack. The skill reads it first, and it overrides the general rules. It's in `.gitignore`, so it never gets pushed.

## Author

Saeed Shahriar, senior SEO and growth marketer. [saeedseo.com](https://saeedseo.com)

## License

MIT
