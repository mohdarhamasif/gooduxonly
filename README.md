# GoodUXOnly — an evidence-based UX skill for Claude

**GoodUXOnly** turns Claude into a UX reviewer and designer that backs every recommendation with a
principle, a piece of research, or a real product precedent. No "make it pop". Just ranked,
fixable issues with the *why* attached.

Built by [Legit Design Studio](https://x.com/m_arhamasif). Knowledge base distilled from six of the
best UX resources on the web:

| Source | What Claude learns from it |
|---|---|
| [Nielsen Norman Group](https://www.nngroup.com/) | 10 usability heuristics, severity rating, research methods, forms/navigation/writing/mobile guidelines |
| [Laws of UX](https://lawsofux.com/) | 30 psychological laws (Hick's, Fitts's, Jakob's, Peak-End…) with how to apply them and how they get misused |
| [Growth.Design](https://growth.design/case-studies) | Product psychology, ~80 cognitive biases, 45+ case studies on onboarding, trials, checkout, retention and offboarding |
| [Appcues GoodUX](https://goodux.appcues.com/) | Onboarding, product tours, tooltips, modals, feature announcements, NPS and upsell patterns |
| [UX Tools](https://www.uxtools.co/) | Modern design workflow, prototyping in code, taste |
| [Case Study Club](https://www.casestudy.club/) | Avoiding generic "zombie UI", design direction, writing portfolio case studies |

## What it does

Ask Claude naturally. The skill triggers on its own for design feedback and product-flow questions.

- **Audit / critique**: screenshots, URLs, Figma links, or a described flow. You get a verdict, what's working, issues ranked by severity (0–4) with the principle broken and a concrete fix, quick wins vs. bigger bets, and further reading.
- **Design / ideate**: new flows and onboarding mapped to the "aha moment", with patterns, precedent products and every state to design.
- **Explain**: "why does this work?" gives the principle, a real example, and the common misuse.
- **Case-study writing**: portfolio or client case studies structured around decisions and outcomes.

It also has built-in **ethics guardrails**. Claude flags dark patterns (fake urgency, hidden costs,
confirm-shaming, hard-to-cancel flows) and proposes honest alternatives that still convert.

### Example prompts

```
Audit this signup flow and rank the issues by severity. [screenshot]
Why is our pricing page underperforming? Here's the URL: https://...
Design an onboarding flow for a B2B invoicing SaaS. Users churn before sending their first invoice.
Which Laws of UX explain why this dashboard feels overwhelming?
Write a portfolio case study for my fintech app redesign. Here are my notes: ...
```

More in [`examples/`](examples/prompts.md).

## Install

### Claude.ai (web, desktop, mobile)
1. Download `gooduxonly.zip` from the [latest release](https://github.com/mohdarhamasif/gooduxonly/releases/latest).
2. Follow Anthropic's guide: [Using skills in Claude](https://support.claude.com/en/articles/12512180-using-skills-in-claude) to upload it as a custom skill.
3. Make sure Skills (and Code Execution) are enabled for your account.

### Claude Code
Add this repo as a plugin marketplace:
```
/plugin marketplace add mohdarhamasif/gooduxonly
/plugin install gooduxonly@gooduxonly
```
Or install manually as a personal skill:
```bash
git clone https://github.com/mohdarhamasif/gooduxonly.git
cp -r gooduxonly/skills/gooduxonly ~/.claude/skills/
```

### Claude API
Upload `skills/gooduxonly` as a custom skill. See the [Skills API guide](https://docs.claude.com/en/api/skills-guide).

## Repo structure

```
.claude-plugin/marketplace.json     Claude Code plugin marketplace manifest
skills/gooduxonly/
  SKILL.md                          Modes, core rules, output format
  references/
    audit-checklist.md              Full checklist + severity scale + output template
    nng-heuristics-and-research.md  NN/g heuristics, research methods, UI guidelines
    laws-of-ux.md                   30 laws: apply / misuse / symptom lookup
    product-psychology.md           Decision cycle, biases, ethics, case-study index
    onboarding-and-in-app-patterns.md  Onboarding & in-app pattern library
    craft-process-and-case-studies.md  Process, AI-era craft, case-study writing
    sources.md                      Links to every original source
.github/workflows/release.yml       Builds gooduxonly.zip and attaches it to every release
```

The skill uses progressive disclosure. Claude reads `SKILL.md` first and only loads the reference
files a task needs, so it stays fast.

## Content & attribution

This skill **does not contain copies of any source's articles**. Every reference file summarizes
principles in original wording and links back to the original page, so the creators get the
traffic and credit. Laws of UX is licensed CC BY-NC-ND 4.0 and the other sources are all rights
reserved. Please keep it that way in contributions: paraphrase and link, never paste.

GoodUXOnly is an independent project and is **not affiliated with or endorsed by** Nielsen Norman
Group, Jon Yablonski / Laws of UX, Growth.Design, Appcues, UX Tools or Case Study Club. Go read
them; they're excellent.

## Contributing

PRs welcome: new principles, better precedents, corrected guidance, new pattern categories. See
[CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE) © 2026 Legit Design Studio LLC. Applies to the original text and code in this repo.
Linked third-party content remains the property of its owners.
