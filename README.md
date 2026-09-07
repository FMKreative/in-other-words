# Talk the Talk

Talk the Talk helps you write, rewrite, summarize, and explain clearly. Use it to draft from a brief, improve human or AI writing, or make a difficult passage easier to understand.

It keeps the meaning, necessary detail, and an appropriate voice. It follows the requested language and its natural usage. Quality can vary by language and task.

## Install

Install with the third-party [Skills CLI](https://github.com/vercel-labs/skills):

```bash
npx skills add FMKreative/talk-the-talk --skill talk-the-talk
```

Choose your agent in the installer. This requires Node.js and npm. The command follows the installer's documentation but has not been tested with this repository.

For a manual installation, clone this repository into your tool's skill directory, naming the folder `talk-the-talk`.

### Claude Code

Place the `talk-the-talk` folder in `~/.claude/skills/` for personal use, or `.claude/skills/` inside a project. The resulting path should end in `talk-the-talk/SKILL.md`. Invoke it with `/talk-the-talk`. See [Claude Code's skill documentation](https://code.claude.com/docs/en/skills).

### Codex

Place the `talk-the-talk` folder in `~/.agents/skills/` for personal use, or `.agents/skills/` inside a project. Invoke it with `$talk-the-talk`. The personal installation has been checked locally in Codex.

Other compatible agents may use different skill directories or invocation syntax. Claude Code's path is documented by Anthropic but has not been tested with this skill.

## Use it

Use the invocation for your tool and describe what you need. These examples use Codex syntax:

```text
Use $talk-the-talk to draft a short project update from these notes.
```

```text
Use $talk-the-talk to rewrite this email. Keep it warm, but make my request clearer.
```

```text
Use $talk-the-talk to summarize this report in three paragraphs. Keep the main limitations.
```

```text
Use $talk-the-talk to make this German text clearer while keeping it in German.
```

Specify the audience, tone, language, or length when they matter. The skill preserves the source language unless you request translation. For new writing, it uses the language of your request unless you specify another.

## How it works

The skill favors familiar words, concrete meaning, useful structure, and natural rhythm. It checks the result briefly for accuracy and clarity, then returns the text without a score or editing report unless you ask for one. Routine use needs no scripts or extra tools.

Its principles draw on George Orwell, the Kansas City Star, Digital.gov, and selected guidance from Simplified Technical English. Their emphasis on the reader guides the writing; language-specific rules follow the language being used. See [principles and provenance](references/principles.md) for the sources and how they are adapted.

## Updating from Clear English

Version 2.0.0 renames `clear-english` to `talk-the-talk`. Use `$talk-the-talk` in place of the old invocation, and replace the old installed skill folder with one named `talk-the-talk`.

This version adds drafting from a brief and support for other languages. It removes automatic readability scores, sentence-length targets, and the Python scoring tools.

The instructions are in [SKILL.md](SKILL.md), the display settings are in [agents/openai.yaml](agents/openai.yaml), and the version is in [VERSION](VERSION). See [LICENSE](LICENSE) for licensing terms.
