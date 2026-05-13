# Contributing to Story Doctor

Story Doctor is a curated reference — not a comprehensive encyclopedia. The goal is quality over quantity: every antipattern, diagnostic, and fix template should be something a writer or editor can actually use in a revision session.

## Adding Craft Sources

New sources can be added to `references/` as markdown files. Each reference file should:
1. Name the source (author, book, or tradition)
2. Organize content by topic — character, scene, dialogue, structure, etc.
3. Extract specific, actionable guidance (not general commentary)
4. Cross-reference from SKILL.md where relevant

**Format:**
```markdown
# Source Name — Book/Author

## Topic
### Specific technique or antipattern

**What it is:**
...

**Fix:**
...
```

## Adding Antipatterns

New antipatterns should follow this structure:
1. **Name** — descriptive, not just "the problem"
2. **What it is** — one clear paragraph
3. **Diagnosis prompt** — specific questions to ask
4. **Fix template** — concrete guidance, not vague encouragement
5. **Signal** — red/yellow/green criteria

Include a diagnosis table where possible.

## Adding Plot or Scene Tools

Scene-level and plot-level tools go in the appropriate sections of SKILL.md and can be expanded in `references/` if the content grows beyond SKILL.md.

## Open Issues

Current open work:
- [#5 — capture Chapter 15 motivation methodology](https://github.com/lux-sp4rk/marina/issues/5)
- [#6 — add Gotham Writers scene structure patterns](https://github.com/lux-sp4rk/marina/issues/6)
- [#7 — add dialogue and voice antipatterns from Gotham](https://github.com/lux-sp4rk/marina/issues/7)

Check the issue tracker before starting work — link issues to PRs where possible.