# Claude Code interview prep skill: STAR method answers from your own resume

**interview-prep-pack** is a free, open-source [Claude Code](https://claude.com/claude-code) skill that turns your own files (resumes, portfolio, published work, the job posting, notes from earlier calls) into one interview prep pack: STAR method answers to the 25 questions you're most likely to get, a 30-60-90 day plan, a worked take-home case and the questions to ask the interviewer.

Built for SEO, GEO/AEO, AI search and growth marketing roles, and works for any role.

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

## FAQ

**What is a Claude Code skill?**
A folder with a `SKILL.md` file that Claude Code loads when your request matches it. Once it's in `~/.claude/skills/`, say "prep me for my interview with [company]" and Claude uses it.

**How is this different from asking Claude or ChatGPT for interview questions?**
A plain prompt gives you generic questions and answers with made-up examples. This skill reads your resumes and work first, builds every answer from your real stories and numbers, and flags where your resumes disagree with each other before an interviewer does.

**Does it write STAR method interview questions and answers?**
Yes. Each of the 25 questions gets a Situation, Task, Action, Result outline sized for 60 to 90 seconds out loud, plus the one line to land. They're beats to say in your own words, not a script to memorize.

**Does it work for roles outside SEO?**
Yes. The numbers sheet, the outlines, the 30-60-90 plan and the questions to ask work for any role. The SEO and AI search questions and the GEO audit case are extras for those roles.

**What's in the mock GEO audit?**
A five-day take-home case for an invented brand: a 30-question set, a baseline run across ChatGPT, Perplexity, Gemini and Google AI Overviews, scoring per engine, a technical and entity check, a ranked ticket list and a 10-minute presentation plan. See `reference/geo-audit-case.md`.

**Is my data sent anywhere?**
The skill itself sends nothing anywhere: it reads the files in your folder and saves the pack there, like any Claude Code task. If you add a `personal.md`, it's gitignored, so it won't be pushed if you fork this repo.

## Related repos

- [claude-seo-skills-benchmark](https://github.com/s77sh/claude-seo-skills-benchmark): 5 Claude Code SEO skill packs tested on 20 planted problems.
- [claude-random-numbers](https://github.com/s77sh/claude-random-numbers): which number Claude picks when asked for a random one, 446 prompts.
- [viral-reel-playbook](https://github.com/s77sh/viral-reel-playbook): a Claude Code skill for Instagram Reels, TikTok and YouTube Shorts scripts.
- [bali-product-demand](https://github.com/s77sh/bali-product-demand): Google Keyword Planner demand for 36 product niches in Bali.

All of them, with what each one is for: [saeedseo.com/repos/](https://saeedseo.com/repos/).

## Author

Saeed Shahriar, senior SEO and growth marketer. [saeedseo.com](https://saeedseo.com)

## License

MIT
