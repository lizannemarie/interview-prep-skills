# interview-prep-skills

A Claude Code plugin with two skills for preparing for specific interviewers.

## Skills

### `interviewer-profile`

Builds a one-page profile of an interviewer from their LinkedIn profile PDF and the recommendations they wrote and received. The profile covers their background, how colleagues describe them, what they value, their likely interview style, how to show up, and questions to ask, with verified facts kept apart from inferences. Output is saved as `<first-last>-interviewer-profile.md`.

### `yoodli-interview-roleplay`

Turns interviewer evidence (a profile, a LinkedIn PDF, or past interview transcripts) into copy/paste blocks for [Yoodli](https://yoodli.ai): one Create Persona form per interviewer, plus a filled-in roleplay form with description, AI context, persona order, and a custom rubric weighted toward your known gaps. It targets behavioral and strategic interview rounds.

## Install

From inside Claude Code:

```
/plugin marketplace add lizannemarie/interview-prep-skills
/plugin install interview-prep-skills@interview-prep-skills
```

Or from your shell:

```bash
claude plugin marketplace add lizannemarie/interview-prep-skills
claude plugin install interview-prep-skills@interview-prep-skills
```

The repository is private, so you need GitHub access to it (for example through `gh auth login`) for the marketplace add to work.

To try it without installing, clone the repo and run `claude --plugin-dir ./interview-prep-skills`.

## Invoke

Claude Code prefixes plugin skills with the plugin name:

```
/interview-prep-skills:interviewer-profile
/interview-prep-skills:yoodli-interview-roleplay
```

Both skills also trigger on their own when you share the relevant material, such as a LinkedIn PDF with a request for interviewer prep, or a request for "Yoodli personas".

## Suggested workflow

1. **Build the profile.** Run `/interview-prep-skills:interviewer-profile` and attach the interviewer's LinkedIn PDF and their recommendations (given and received). Name the round format, for example behavioral or strategic leadership. You get `<first-last>-interviewer-profile.md`. Repeat for each person in the loop to get a comparison table.
2. **Build the roleplay.** Run `/interview-prep-skills:yoodli-interview-roleplay` in the same folder. It reads the profile files, plus any transcripts or recaps from past rounds, and produces the persona blocks and the roleplay form.
3. **Practice.** Paste the persona blocks into Yoodli's Create Persona form and the roleplay blocks into the roleplay form. Turn on multi-persona mode for a back-to-back loop.
4. **Adjust.** Ask Claude to change a persona's demeanor or the rubric weights after a practice run.

## License

MIT
