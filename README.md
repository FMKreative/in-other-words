# Talk the Talk

Talk the Talk helps you write, rewrite, summarize, and explain clearly. Use it to draft from a brief, improve human or AI writing, or make a difficult passage easier to understand.

It keeps the meaning, necessary detail, and an appropriate voice. It follows the requested language and its natural usage. Quality can vary by language and task.

## Use it

Invoke the skill as `$talk-the-talk` and describe what you need:

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
