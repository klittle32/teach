# teach

> **This is a fork of [Matt Pocock](https://github.com/mattpocock)'s `teach` skill.**
> The original work is by Matt Pocock; this repository adapts and extends it. All
> credit for the original concept and design goes to him.

An AI-agent skill that teaches you a new skill or concept over multiple
sessions, treating the current directory as a stateful **teaching workspace**.
It works with any coding agent that supports skills (Claude Code, and similar
agent tooling).

## What it does

When invoked, the skill grounds all teaching in a clear *mission* (why you want
to learn the topic), gathers high-trust resources, and produces short, beautiful,
self-contained HTML lessons tied to your zone of proximal development. It tracks
your progress across sessions using a set of workspace files:

- `MISSION.md` — the reason you're learning the topic; grounds all teaching.
- `RESOURCES.md` — curated, high-trust resources used to ground lessons.
- `GLOSSARY.md` — the canonical, opinionated vocabulary for the workspace.
- `./learning-records/*.md` — records of what you've learned (like ADRs).
- `./lessons/*.html` — the lessons themselves, the primary unit of teaching.
- `./reference/*.html` — compressed cheat sheets and reference material.
- `NOTES.md` — a scratchpad for your teaching preferences and working notes.

See [`SKILL.md`](./SKILL.md) for the full teaching philosophy and behavior.

## Attribution

This is a **fork** of Matt Pocock's original `teach` skill. See [`LICENSE`](./LICENSE)
for the MIT license, which retains the original copyright alongside the changes
made in this fork.
