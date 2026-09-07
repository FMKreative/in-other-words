# Talk the Talk

Talk the Talk helps you write, rewrite, summarize, and explain clearly. Use it to draft from a brief, improve human or AI writing, or make a difficult passage easier to understand.

It keeps the meaning, necessary detail, and an appropriate voice. It follows the requested language and its natural usage. Quality can vary by language and task.

## Install

Download [talk-the-talk.zip](https://github.com/FMKreative/talk-the-talk/releases/latest/download/talk-the-talk.zip) from the latest release. It contains one `talk-the-talk/` folder with the skill and its supporting files.

### Claude

Upload the ZIP without extracting it: open **Customize → Skills**, choose **+ → Create skill → Upload a skill**, then select `talk-the-talk.zip`. Enable the skill and ask Claude to use Talk the Talk. See [Claude's installation guide](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

### Claude Code

Extract the ZIP and place its `talk-the-talk` folder in `~/.claude/skills/` for personal use, or `.claude/skills/` inside a project. The resulting path should end in `talk-the-talk/SKILL.md`. Invoke it with `/talk-the-talk`. See [Claude Code's skill documentation](https://code.claude.com/docs/en/skills).

### Codex

Extract the ZIP and place its `talk-the-talk` folder in `~/.agents/skills/` for personal use, or `.agents/skills/` inside a project. Invoke it with `$talk-the-talk`. The personal installation has been checked locally in Codex.

### Other compatible agents

For tools supported by the third-party [Skills CLI](https://github.com/vercel-labs/skills), run:

```bash
npx skills add FMKreative/talk-the-talk --skill talk-the-talk
```

Choose your agent in the installer. This route requires Node.js and npm. The command follows the installer's documentation; it has not been tested with this repository. Claude's upload and Claude Code's installation paths are documented by Anthropic, but have not been tested with this skill. Other tools may use different locations or invocation syntax.

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
