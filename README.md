# Story Doctor

A curated reference of narrative anti-patterns, craft conventions, and diagnostic methods for evaluating and revising fiction.

## What It Is

Story Doctor is a structured triage sequence for diagnosing what's broken in a story — and what to do about it. It draws from multiple craft traditions (Sol Stein's *Stein on Writing*, Gotham Writers' *Writing Fiction*, and others) to organize narrative problems into actionable categories: character, scene, conflict, motivation, and structure.

## The Sequence

Work through these steps in order. Stop at the first diagnosis that applies — that's usually the root cause.

1. **Autobiography Antipattern** — protagonist sounds too much like the writer
2. **Boring Protagonist** — competent and forgettable
3. **Protagonist Grill** — stress-test how well the writer knows their character
4. **Frozen Character** — protagonist ends unchanged
5. **Antagonist Check** — four sub-antipatterns (diffused, shallow, cartoon, bio trap)
6. **Minor Characters** — the one-thing trap
7. **Weak Conflict** — the story has no engine

Then: scene evaluation, motivation triage, second-pass plot review.

## Structure

```
story-doctor/
├── SKILL.md          — triage sequence + prompts + fix templates
└── references/
    ├── stein.md      — Sol Stein craft methods
    └── gotham.md     — Gotham Writers craft methods
```

## Sources

- **Stein on Writing** — Sol Stein. Character antipatterns, motivation, scene evaluation.
- **Writing Fiction** — Gotham Writers Workshop. Scene craft, dialogue, voice, point of view, structure, revision.

## Using With an AI Agent

This skill was built for use with AI coding agents (OpenClaw, Codex, etc.) as a creative partner. When an agent has the `story-doctor` skill loaded, it can run the triage sequence against a story you're working on, diagnose specific problems, and suggest fixes — without needing Sol Stein or Gotham Writers on your desk.

## Contributing

This is a living document. New craft sources, antipatterns, and patterns can be added to `references/` and cross-referenced from the main triage sequence. Open an issue or PR to add new material.