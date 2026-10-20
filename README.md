# Mentor Mode for Claude Code

A Claude Code plugin that turns Claude into a coding mentor. Instead of writing code for you, Claude guides you through problems with hints, questions, and code review.

## How it works

When you invoke `/mentor`, Claude switches into a fully pedagogical mode for the rest of the session. You write all the code. Claude coaches.

This is **not** Learning Mode. Anthropic's built-in Learning Mode has Claude build most of the code and pause at decision points for you to contribute 5–10 lines. Mentor Mode is the inverse: you drive, Claude navigates. 

## What Claude will do

- Ask what you've tried before hinting at anything
- Calibrate guidance to your level (from "completely lost" to "almost there")
- Review your code: strengths first, then questions about what's off
- Surface **★ Learning Insights** — brief reflections on the skill you just practiced
- Give you syntax reminders, doc pointers, and concept explanations freely

## What Claude won't do

- Write complete solutions
- Produce code blocks longer than ~5 lines (skeletons and pseudocode are fine)
- Say "just do X" — everything is framed as a question or suggestion

## Handling frustration

If you get stuck and explicitly ask for the answer, Claude will give it — but will follow up with "can I walk you through *why* this works?" If you want to exit mentor mode entirely, just say so. No judgment.

## Install

### From a GitHub marketplace

```
/plugin marketplace add YOUR_USERNAME/mentor-mode
/plugin install mentor-mode
```

### Local install

Clone this repo, then:

```
/plugin install --path /path/to/mentor-mode
```

### Manual install

Copy the `skills/mentor/` directory to `~/.claude/skills/mentor/`.

## Usage

Start a Claude Code session and type:

```
/mentor
```

That's it. Claude will introduce itself and the session begins.

## License

MIT
