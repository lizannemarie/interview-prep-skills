---
name: "interviewer-profile"
description: "Build an interviewer profile (background, how others describe them, what they value, expected style, how to show up, questions to ask) from LinkedIn recommendations and their LinkedIn PDF."
---

# Interviewer profile

Use when the user shares an interviewer's LinkedIn recommendations, LinkedIn profile PDF, or public comments and wants prep for that person. Also use when they say "profile" for a past or upcoming interviewer.

## Inputs to ask for or look for

1. The LinkedIn profile PDF (title, employer, dates, summary).
2. Recommendations the person wrote for others (what they praise is the best evidence of what they value).
3. Recommendations others wrote about them (how colleagues describe them).
4. Any recent public comments or posts.

If only some of these exist, build the profile from what is there and say so.

## Output: one markdown file per interviewer

Name it `<first-last>-interviewer-profile.md`. Sections, in this order:

1. **Title line**: `# Interviewer Profile: <Name>`, then an italic line stating the sources and counts (for example, recommendations written, recommendations received, comments).
2. **Data caveat**: a quoted block. State the sample size, the dates of the sources, and what the data cannot show (current role, seniority, how they interview today). Old or tiny samples must be called out plainly.
3. **Background**: current title and employer from the PDF, prior roles and dates, scope in their own words, education if relevant. Facts only.
4. **How others describe them**: short bullets with a bold lead phrase, each grounded in a recommendation.
5. **What they value in others**: ranked by emphasis. Draw from what they wrote about others and what colleagues praise. Add one "Key insight" line only if the evidence supports it.
6. **Expected interview style**: likely question types, tone, what they will probe. Mark this as inferred.
7. **How to show up**: concrete moves tied to the evidence, such as which story types to lead with, how to structure answers, and what to avoid.
8. **Comparison table** (only when profiling two or more interviewers in the same loop): center of gravity, what wins them over, leadership lens, likely probe. End with a common thread across them.
9. **Questions to ask them**: three or four, tied to their scope and the behavioral or strategic format of the round.

## Rules

- Separate verified facts (from the PDF) from inferences (from recommendations). Label inferences.
- Do not state a trait unless at least one recommendation or comment supports it. Do not pad.
- Keep to work style and values. Do not infer protected attributes, health, family, or personality types.
- Match the questions and prep to the actual round format the user describes. If the user says the round is behavioral and strategic leadership, do not prepare technical or domain quizzes; keep domain material as support inside stories.
- Pull the user's stories from their story bank by name or id. Do not invent stories, numbers, or outcomes.
- Run the prose through the humanizer rules: no em dashes, no not-X-but-Y contrasts, no forced triads, no bold labels inside sentences.
- Interview logistics, schedules, outcomes, and feedback go in the interview log, never in the user's career-facts file (Experience-Context).

## After building

Offer to fold the profile into the round's prep guide and flashcards, and note any gap (for example, a likely question with no matching story).