# In Other Words

Version 3.0.0

Write, rewrite, summarize, and explain in clear, natural language. In Other Words helps you draft from notes, improve your own writing, or “unslop” AI-generated text by removing filler, inflated wording, stale phrases, and needless repetition while keeping the meaning and voice.

Its main foundations are George Orwell, the Kansas City Star, and Digital.gov: respect the reader, use precise words, and make the message easy to follow. See [principles and sources](references/principles.md) for the sources and how they are adapted.

## Use it

Describe what you need, including the audience, tone, language, or length when they matter. For example:

- “Unslop this AI draft. Keep the substance and make it sound natural.”
- “Draft a short project update from these notes.”
- “Rewrite this email. Keep it warm, but make my request clearer.”
- “Summarize this report in three paragraphs. Keep the main limitations.”
- “Make this German text clearer while keeping it in German.”

In Codex, start your request with `$in-other-words`. In Claude Code, use `/in-other-words`.

The skill preserves facts, necessary qualifications, and an appropriate voice. It follows the requested language and its natural usage; otherwise it keeps the source language, or uses the language of your request for new writing. Quality can vary by language and task.

It briefly checks accuracy and clarity, then returns the requested text. Routine use needs no scripts, scores, or editing reports.

## Install

With Node.js and npm available, run the third-party [Skills CLI](https://github.com/vercel-labs/skills) and choose your agent:

```bash
npx skills add FMKreative/in-other-words --skill in-other-words
```

For a manual installation, clone this repository into the appropriate skill directory. The resulting path should end in `in-other-words/SKILL.md`.

| Tool | Personal installation | Project installation |
| --- | --- | --- |
| Codex | `~/.agents/skills/in-other-words/` | `.agents/skills/in-other-words/` |
| Claude Code | `~/.claude/skills/in-other-words/` | `.claude/skills/in-other-words/` |

The personal Codex installation has been checked locally. The [Claude Code path](https://code.claude.com/docs/en/skills) and Skills CLI command follow their documentation but have not been tested with this skill. Other agents may use different directories or invocation syntax.

## Renaming from Talk the Talk

In Other Words was previously published as Talk the Talk. Replace the old skill folder with `in-other-words` and use the new invocation. The skill still supports drafting, rewriting, summarizing, and guidance for other languages.

The instructions are in [SKILL.md](SKILL.md), and Codex display settings are in [agents/openai.yaml](agents/openai.yaml). See [LICENSE](LICENSE) for reuse terms.
