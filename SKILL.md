---
name: interview-prep-pack
description: Builds a complete interview prep pack for a job candidate from their own files (resumes, portfolio, published work, job posting, notes from earlier calls). The pack has a numbers sheet (every citable number with its company and period, the inconsistencies to fix, and the gap they'll be probed on), 25 likely questions across the screening, hiring-manager and case rounds, a STAR outline for each one sized for 60 to 90 seconds out loud, a 30-60-90 day plan, a take-home case worked through step by step, and 8 questions to ask the interviewer. Every story and number comes from the candidate's files; where none exists, the outline gives a method instead of a made-up story. Tuned for SEO, GEO/AEO, AI search and growth roles, and works for any role. Use when the user says "interview prep", "prep pack", "prep me for an interview", "I have an interview with X", "what will they ask me", "STAR answers", "30-60-90 plan", "take-home case", "mock audit", "questions to ask the interviewer", or pastes a job posting and asks how to get ready for it.
---

# interview-prep-pack

Builds one Markdown file the candidate can rehearse from and bring to every round. The point is not clever answers. It is answers that hold up when a hiring manager asks "on top of what?".

**First:** if `personal.md` exists next to this file, read it. It holds the candidate's own paths, their finished pack, their voice notes and their rules, and it overrides anything here.

## The one rule

**Every number and story comes from the candidate's files. Nothing is invented.** If a question has no real story behind it, the outline says so and answers with a method. A made-up client, conversation, or number is the one thing that can sink a candidate in the room, because the follow-up question finds it.

Before writing, list every source file used at the top of the pack. If a number isn't in the pack, the candidate shouldn't say it.

## Step 0: gather the sources

Ask for, or find in the project:

1. **Resumes**, every version (they disagree with each other more than people think).
2. **Portfolio and public work:** site pages, case studies, published posts, repos, experiment write-ups.
3. **The job posting(s)** they're preparing for. Pick the closest match and name it at the top.
4. **Notes from earlier calls** with this company or similar ones. A screener's questions repeat.
5. **Voice notes** if they have a style guide; the outlines should sound like them.

Read all of it before writing a word. Don't ask the candidate things the files already answer.

## Step 1: the numbers sheet

A table at the top of the pack:

| Number | What it is | Where and when |
|---|---|---|

Every citable number, each with its **company and period**. An unqualified number gets discounted by exactly the person the candidate wants to impress.

Then two short lists:

- **Things to fix before the next call.** Look for: the same metric reported differently in two places (often both true, at different dates; give one sentence that covers both), two numbers of the same size that are easy to swap mid-answer (two different "40%"s), and any big number with no baseline ("+300% from what?"). If the baseline isn't in the files, say so and tell them to pull it or offer to send it after the call.
- **The gap they will be probed on.** The one thing the role wants that the files can't prove. Name it, say what not to stretch, and give the honest answer plus what they could do before the interview to close it.

## Step 2: 25 likely questions

A table with three rounds:

- **Screening** (15 to 30 min, recruiter or ops): about 8 questions. Background, why this role now, relevant industry, handling several stakeholders, bad-news communication, KPIs owned, time zone and location.
- **Hiring manager** (45 to 60 min): about 14. The questions the posting signals by name come first; bold them. Then the role's core skills, a time AI or a tool got something wrong, biggest win, proving causation, a failure, a weak spot.
- **Case round** (live or take-home): about 3 method questions.

For SEO, GEO, AEO and AI search roles, always include: SEO vs GEO vs AEO, **how do you measure AI visibility**, **show us an AI workflow you built and how you checked it**, what you change on a site to get cited, "guarantee we show up in ChatGPT", clicks dropped but rankings held, llms.txt / FAQ schema / question headings, and one sprint vs a 40-item backlog. See `reference/seo-geo-questions.md` for what a strong answer to each covers.

## Step 3: the answer outlines

One outline per question. Each runs **60 to 90 seconds out loud, about 150 to 220 words**.

```
### N. The question.

(Optional one-line note: why they ask it, or which real call asked it.)

- **S:** the situation, with company and date.
- **T:** what they had to do.
- **A:** what they did, specific enough to be checked.
- **R:** the result, with its number, company and period.

(Optional: what to say if pressed, or the honest edge.)

**"The one line to land, in their voice."**
```

Rules for the outlines:

- **Beats, not a script.** The candidate says them in their own words and stops after the R unless asked for more.
- **Reuse the strongest stories,** but never tell the same one the same way twice. Two or three anchor stories carry most interviews.
- **No story? Say so.** Write "No client story for this one: it's a method question" and give the method as the A.
- **Honest edges in the outline,** not hidden: an NDA, a number that's organic and not AI, a channel they haven't run.
- **The bold line** is short, quotable and true. No slogans they couldn't defend.
- **Match their voice.** If they have a voice file, follow it. Otherwise: plain words, short sentences, no corporate filler.

## Step 4: the 30-60-90 day plan

One page that works for any company, because the first month is spent learning theirs. Use `reference/30-60-90.md` as the frame and adjust the nouns to the role. Days 1 to 30: read, get access, set the baseline. Days 31 to 60: deploy the first fixes and the workflow behind them. Days 61 to 90: re-measure, report honestly, plan the next quarter. End with "day 90 success, in their terms".

## Step 5: the take-home case

Pick the case this role is most likely to set and work it through in steps, each with its time, its tools and its output. For AI search roles, use the mock GEO audit in `reference/geo-audit-case.md`: an invented brand, a question set, a baseline run across engines, scoring, a technical check, a content and entity check, the write-up, a sample ticket, and a 10-minute presentation plan. Always mark invented brands as invented.

## Step 6: questions to ask them

Eight questions, each with one line on what the answer tells the candidate. Good ones expose the real metric, who owns what, how fast work deploys, the AI-content rules, and what failure at 90 days would look like. Say which to save for the hiring manager.

## Before handing it over: check

Go through the pack once more and confirm:

- [ ] Every number appears in a source file, with the same value, company and period.
- [ ] No invented client, conversation, quote or result anywhere. Invented example brands are labeled.
- [ ] Every outline is roughly 150 to 220 words of beats.
- [ ] The questions the posting names are bolded and have the strongest outlines.
- [ ] The gap is named once, honestly, with what not to stretch.
- [ ] The source list at the top is complete.

If a second model is available, ask it to fact-check the pack against the sources and list anything it can't trace. Fix those before handing it over.

## Output

Save the pack as `interviews/prep-<role>-<yyyy-mm>.md` (or wherever `personal.md` says) and tell the candidate the three things to fix before the next call.

See `examples/example-pack.md` for a short filled example with an invented candidate.
