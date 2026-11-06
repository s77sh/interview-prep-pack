# Claude Code interview prep skill: STAR method answers from your own resume

I built **interview-prep-pack** for my own job hunt in October 2026, getting ready for remote AI search lead roles.

It's a free [Claude Code](https://claude.com/claude-code) skill. It reads your resumes, your work and the job posting, then builds **one prep pack you can rehearse from**.

It's tuned for SEO, GEO/AEO, AI search and growth roles. Most of it works for any role.

| Part | What you get |
|---|---|
| Numbers sheet | Every number you can cite, with its company and period, the inconsistencies to fix before the next call, and the gap you'll be probed on |
| 25 likely questions | Screening, hiring-manager and case rounds, with the ones the posting names in bold |
| Answer outlines | A STAR outline per question, sized for 60 to 90 seconds out loud, with the one line to land |
| 30-60-90 day plan | Read and baseline, first fixes, re-measure and hand over |
| Take-home case | A mock GEO audit in seven steps, with the tools, a tracking-sheet layout and a sample ticket |
| Questions to ask | Eight, each with what the answer tells you |

One rule runs through all of it: **every story and number comes from your files.** With no real story, the outline gives a method instead.

A made-up client is exactly what the follow-up question finds.

## Install

Clone it into your personal skills folder and it works in every project:

```bash
git clone https://github.com/s77sh/interview-prep-pack ~/.claude/skills/interview-prep-pack
```

Or put it in one project only, at `.claude/skills/interview-prep-pack/`.

## Use

Open Claude Code in the folder with your resumes and work, and ask in plain words. Here are a few:

- "Prep me for the interview with [company], the posting is in jobs/[file]"
- "What will they ask me in the hiring manager round?"
- "Write me a 30-60-90 plan for an AI search lead"
- "Work through a take-home GEO audit for [brand]"

## What's inside

| File | What it does |
|---|---|
| `SKILL.md` | The procedure |
| `reference/seo-geo-questions.md` | What a strong answer covers for the SEO and AI search questions |
| `reference/30-60-90.md` | The plan frame |
| `reference/geo-audit-case.md` | The mock GEO audit, with an invented brand |
| `examples/example-pack.md` | A short filled pack for an invented candidate |

## Make it yours

Add a `personal.md` next to `SKILL.md` with your paths, voice notes and finished pack. **The skill reads it first** and it's gitignored.

## FAQ

### What is a Claude Code skill?

A folder Claude Code loads by itself when your request matches it.

### How is this different from asking ChatGPT or Claude for interview questions?

A plain prompt gives you generic questions with made-up examples. This one reads your files first, so **the stories and numbers come from your own work**.

It also flags where two of your resumes disagree, before an interviewer does.

### Does it write STAR method interview questions and answers?

Yes, 25 of them. Each outline runs **60 to 90 seconds out loud**, as beats you say in your own words.

### Does it work for roles outside SEO?

Mostly. **The numbers sheet, outlines, 30-60-90 plan and questions to ask fit any role.** The SEO questions and the GEO audit are extras.

### What's in the mock GEO audit?

A five-day case for an invented brand: 30 questions across four AI engines, scored per engine. It ends in **a ranked ticket list and a 10-minute talk**.

### Is my data sent anywhere?

Not by the skill. Claude Code reads your files like any project, and **the pack stays in your folder**.

## Related repos

| Repo | What it is |
|---|---|
| [claude-seo-skills-benchmark](https://github.com/s77sh/claude-seo-skills-benchmark) | 5 Claude Code SEO skill packs tested on 20 planted problems |
| [claude-random-numbers](https://github.com/s77sh/claude-random-numbers) | Which number Claude picks when you ask for a random one |
| [viral-reel-playbook](https://github.com/s77sh/viral-reel-playbook) | A Claude Code skill for Reels, TikTok and Shorts scripts |
| [bali-product-demand](https://github.com/s77sh/bali-product-demand) | Keyword Planner demand for 36 product niches in Bali |

What each one is for: [saeedseo.com/repos/](https://saeedseo.com/repos/).

## Author

Saeed Shahriar, senior SEO and growth marketer. [saeedseo.com](https://saeedseo.com)

## License

MIT
