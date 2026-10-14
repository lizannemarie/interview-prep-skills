---
name: "yoodli-interview-roleplay"
description: "Create copy/paste Yoodli personas for interviewers and fill in a Yoodli roleplay form (description, context, personas, rubric) for a behavioral or strategic interview."
---

# Yoodli personas and roleplay

Use when the user is practicing in yoodli.ai and wants personas for specific interviewers, or wants the roleplay form filled in. Also use when they say "Yoodli persona", "Yoodli roleplay", or share a Yoodli form screenshot.

## Step 1: gather evidence

- Interviewer name, title, employer: from the LinkedIn PDF or the prep guide. If an interviewer-profile file exists (LinkedIn recommendations summary), read it.
- For past interviewers, read the transcript or recap for how they actually behaved (questions asked, probes, tone, what they pushed on). Real behavior beats inference.
- The round format the user describes (behavioral, strategic leadership, people management). Match it. Do not build technical or domain quizzes unless the user says the round will have them.
- The role posting or the user's prep guide for context.

## Step 2: persona form (one per interviewer)

The Yoodli Create Persona form has these fields. Give each as a labeled copy/paste block.

1. **Name**
2. **Job Title**
3. **Company** (optional)
4. **Demeanor**: pick exactly one from Yoodli's list and give a one-line reason. Options: Friendly (easily approachable and pleasant), Critical (frequently points out flaws), Frightened (afraid, cautious, reactive to pressure), Empathetic (sensitive to others' feelings), Enthusiastic (intense excitement), Analytical (logic and detailed problem-solving), Curious (eager to learn, asks questions), Assertive (confident, self-assured), Aggressive (forceful, confrontational under pressure), Blunt (direct, to the point), Skeptical (wary of new ideas), Neutral (balanced, objective), Casual (relaxed, conversational), Rude (blunt and harsh, ignoring feelings). Choose from evidence. Default toward Friendly, Neutral, Analytical, Curious or Assertive. Use Skeptical or Blunt only when a transcript or recommendations support it. Avoid Rude, Aggressive and Frightened.
3. **Background**: up to 10 items, one line each, facts only (title, scope, prior employers, notable results, education). Pull from the LinkedIn PDF. Never put interview outcomes, feedback, or status in here.
4. **Persona Behavior**: how the persona acts. Cover question style, how they probe, what they listen for, speaking pattern, and objections or reframes they raise. Base it on the transcript or the recommendations. Mark nothing as fact that is only inferred; phrase inferred traits as how the persona behaves in the roleplay.

Keep each block short enough to paste into a single field.

## Step 3: roleplay form

The Yoodli roleplay form has these sections. Fill each one.

1. **Description** (shown to the person choosing the roleplay): one or two plain sentences on what the practice covers.
2. **Context** (instructions to the AI as the interviewer, not shown to the participant): write in second person, "You are...". Include the role and company, the round format, how many questions, the style (behavioral "tell me about a time" questions with follow-ups), what to probe (tradeoffs, what the candidate personally did, numbers), how to open and close, and to stay in character. Add the job description details if available. Keep it clear and under about 250 words.
3. **Persona**: list which personas to add and the order. Say whether to turn on multi-persona mode (on when practicing a back-to-back loop, off for a single interviewer).
4. **Rubric**: custom goal weighting. Provide goals as name, description, and weight. Weights add up to 100%. Replace the defaults (Actively listen 50%, Use the STAR method 50%) with goals tied to the user's known gaps. Typical goals: state the decision and the tradeoff early, give concrete ordered steps, use "I" for own decisions and "we" for team work, give one consistent number and one person, answer bottom line first and concisely, welcome a reframe and answer the follow-up.

## Rules

- Facts about people come only from the PDF, transcripts and profiles the user supplied. Do not invent.
- Run all prose through the humanizer rules: no em dashes, no not-X-but-Y contrasts, no forced triads, no bold labels inside sentences.
- Persona text goes in Yoodli, not in the user's career-facts file. Interview schedules and outcomes go in the interview log.
- Deliver as copy/paste blocks in the reply and, if the user wants to keep them, as one markdown file per round named `yoodli-<round>-personas.md`.
- After delivering, offer to adjust the demeanor or rubric weights.