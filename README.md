# Talk the Talk

Version 2.0.1

Write, rewrite, summarize, and explain in clear, natural language. Talk the Talk helps you draft from notes, improve your own writing, or “unslop” AI-generated text by removing filler, inflated wording, stale phrases, and needless repetition while keeping the meaning and voice.

Its main foundations are George Orwell, the Kansas City Star, and Digital.gov: respect the reader, use precise words, and make the message easy to follow. See [principles and sources](references/principles.md) for the sources and how they are adapted.

## Use it

Describe what you need, including the audience, tone, language, or length when they matter. For example:

- “Unslop this AI draft. Keep the substance and make it sound natural.”
- “Draft a short project update from these notes.”
- “Rewrite this email. Keep it warm, but make my request clearer.”
- “Summarize this report in three paragraphs. Keep the main limitations.”
- “Make this German text clearer while keeping it in German.”

In Codex, start your request with `$talk-the-talk`. In Claude Code, use `/talk-the-talk`.

The skill preserves facts, necessary qualifications, and an appropriate voice. It follows the requested language and its natural usage; otherwise it keeps the source language, or uses the language of your request for new writing. Quality can vary by language and task.

It briefly checks accuracy and clarity, then returns the requested text. Routine use needs no scripts, scores, or editing reports.

## Install

With Node.js and npm available, run the third-party [Skills CLI](https://github.com/vercel-labs/skills) and choose your agent:

```bash
npx skills add FMKreative/talk-the-talk --skill talk-the-talk
```

For a manual installation, clone this repository into the appropriate skill directory. The resulting path should end in `talk-the-talk/SKILL.md`.

| Tool | Personal installation | Project installation |
| --- | --- | --- |
| Codex | `~/.agents/skills/talk-the-talk/` | `.agents/skills/talk-the-talk/` |
| Claude Code | `~/.claude/skills/talk-the-talk/` | `.claude/skills/talk-the-talk/` |

The personal Codex installation has been checked locally. The [Claude Code path](https://code.claude.com/docs/en/skills) and Skills CLI command follow their documentation but have not been tested with this skill. Other agents may use different directories or invocation syntax.

## Updating from Clear English

Talk the Talk replaced `clear-english` in v2.0.0. Replace the old skill folder with `talk-the-talk` and use the new invocation. The update added drafting and guidance for other languages, and removed automatic readability scores, sentence-length targets, and Python scoring tools.

The instructions are in [SKILL.md](SKILL.md), and Codex display settings are in [agents/openai.yaml](agents/openai.yaml). See [LICENSE](LICENSE) for reuse terms.
