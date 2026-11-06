# Take-home case: mock GEO audit

**Sample brand:** Brewlane, an invented coffee subscription that sells online. Swap in the brand they give you. **Timebox:** five working days. **Output:** a one-page summary, the tracking sheet and a ranked ticket list.

## Step 1. Agree the scope and write down what "good" looks like (half a day)

Which market, which products, three to five named competitors, and the business questions: are we named, are we cited, and what do engines say about us? Write the expected answers down before the first run. It stops the goalposts moving.

**Tools:** a Google Doc or Notion page.

## Step 2. Build the question set (half a day)

30 questions across four stages, typed the way a customer asks:

| Stage | Example |
|---|---|
| Category | "I want fresh coffee beans delivered every two weeks, which subscription is worth it?" |
| Comparison | "Is a coffee subscription cheaper per cup than supermarket beans?" |
| Problem | "Which coffee subscription has decaf that doesn't taste like decaf?" |
| Brand | "Is Brewlane any good, and how do I cancel?" |

**Tools:** Search Console queries (longest, question-shaped ones first), Google Keyword Planner, People Also Ask, related searches, Reddit threads in the niche, and the support inbox if it's shared.

## Step 3. Run the baseline (one and a half days)

Every question in ChatGPT (search on), Perplexity, Gemini, and Google AI Overviews / AI Mode. Logged out or in a clean profile, one fixed location. Three runs per engine in total, spread over two different days: 30 questions x 4 engines x 3 runs = 360 answers.

Run it in the apps, because that's what customers see; API answers without the search tool can differ. An AI coding agent can parse the saved answers and fill the sheet; spot-check a sample against the screenshots, because a parsing error is still an error.

**The sheet, one row per answer:**

| Question | Engine | Run | Date | Brand named? | Position in list | Brand URL cited? | Other cited URLs | Competitors named | Anything wrong about the brand? |
|---|---|---|---|---|---|---|---|---|---|

**Tools:** the four engines, Google Sheets, a coding agent for parsing and counting. Paid trackers can scale this; check one against the manual run before trusting its numbers.

## Step 4. Score it (half a day)

- **Appearance rate** and **citation rate**, per engine. Never one blended score.
- **Share of voice** against each named competitor.
- **Source mix:** own site, listicles, directories, review sites, Reddit, YouTube, news. For service and "best X" questions, expect listings and directories to dominate.
- **Accuracy:** anything an engine says about the brand that's wrong (prices, delivery areas, cancellation). These are often the fastest fix.

## Step 5. Technical check (one day)

- **Crawler access:** robots.txt and CDN bot rules for OAI-SearchBot, GPTBot, ChatGPT-User, PerplexityBot and Googlebot. Google-Extended controls whether Gemini can use the content (training and grounding); it doesn't control AI Overviews. Then the server or CDN logs: are these bots fetching the pages that matter?
- **Rendering:** a crawl with JavaScript rendering on and off. Content that only appears with JS is a risk for some crawlers.
- **Indexing:** Search Console page indexing report and Bing Webmaster Tools. Look for the ones tools miss: a noindex sent only in the HTTP header, a 302 that should be a 301.
- **Schema:** Rich Results Test and the Schema Markup Validator. Check it says what the page says (a schema price that doesn't match the page).
- **Speed:** PageSpeed Insights on the templates that matter. Check the tag manager isn't blocking in the head.

## Step 6. Content and entity check (half a day)

- For each question where a competitor is cited and the brand isn't: open the cited page. What does it give the model that the brand's page doesn't? Usually a direct answer in the first lines, a number, a comparison table.
- **Entity consistency:** is the brand described the same way on its site, Google Business Profile, LinkedIn, review sites and the cited directories?
- **What not to recommend** without current evidence: llms.txt, FAQ schema for rich results, rewriting every heading as a question.

## Step 7. Write it up (half a day)

- **One-page summary:** baseline rates per engine, the three biggest gaps, what to do first.
- **Ranked ticket list**, one row each: problem (measured), fix, owner (engineering, content or outreach), effort, the metric it should move, and when it'll be checked.
- **Off-site list:** each cited third-party page marked get listed, pitch, or ignore.
- **Measurement plan:** the same 30 questions re-run monthly in a dated window; AI Overviews impressions and AI referral sessions in GA4 (a channel group matching chatgpt.com, perplexity.ai, gemini.google.com, copilot.microsoft.com) beside them, in separate rows.

**A sample ticket:**

> **Problem:** In 4 of 12 ChatGPT runs on the cancellation question, the answer says Brewlane needs a phone call to cancel. The help page says it's one click in the account, but the steps load with JavaScript and the page has no clear answer in its first lines.
> **Fix:** Render the cancellation steps in the HTML. Open the page with one sentence: how to cancel and how long it takes.
> **Owner:** engineering (render), content (first lines). **Effort:** small.
> **Measure:** the cancellation question re-run in all four engines, 30 days after deploy.

(Brewlane and the ticket are invented for the exercise. Say so if you present it.)

## Presenting it (10 minutes)

Two minutes on the method, five on the three gaps and their fixes, two on how you'll measure, one on what you didn't check and why. Leave the sheet open; they'll want to scroll it.
