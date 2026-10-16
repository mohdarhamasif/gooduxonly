# Contributing to GoodUXOnly

Thanks for helping make Claude a better UX partner.

## Ground rules
1. **Paraphrase and link, never paste.** Don't copy articles, definitions, or case-study text from
   any source. Summarize in your own words and add the link to `references/sources.md` or inline.
2. **Every rule needs a "because".** New guidance should cite a principle, research, or a real
   product precedent.
3. **Ethics first.** No contributions that teach dark patterns, except as things to flag and avoid.
4. **Keep SKILL.md lean** (under ~500 lines). Put depth in `references/` and point to it from the
   table in SKILL.md.

## Making a change
1. Edit files under `skills/gooduxonly/`.
2. To test, zip the folder: `cd skills && zip -r ../gooduxonly.zip gooduxonly`. Release
   packages are built automatically by GitHub Actions when a release is published.
3. Test locally: copy `skills/gooduxonly` to `~/.claude/skills/` (Claude Code) or upload
   `gooduxonly.zip` in Claude.ai, then try the prompts in `examples/prompts.md`.
4. Open a PR describing what changed and which prompt it improves.

## Ideas we'd love
- More precedents for B2B SaaS, fintech, health and e-commerce
- Accessibility depth (WCAG 2.2 specifics)
- Pattern files for dashboards, data tables, settings, AI chat interfaces
- Translations of the reference files
