# Nielsen Norman Group — Heuristics, Research Practice, Guidelines

Source: https://www.nngroup.com/articles/ (paraphrased; read originals for depth)

## Contents
1. The 10 usability heuristics (with audit questions)
2. Severity rating
3. Usability fundamentals
4. Research methods — what to use when
5. Interaction & UI guidelines (forms, navigation, errors, writing, mobile, visual design)
6. AI products

---

## 1. The 10 usability heuristics (Jakob Nielsen, 1994)
Broad rules of thumb, not rigid rules. Article: https://www.nngroup.com/articles/ten-usability-heuristics/

**H1 Visibility of system status** — Keep people informed about what's happening, quickly.
Ask: Is there feedback for every action? Loading/progress shown? "You are here" in nav?
Is save state, sync state, upload progress visible? Are selected/active states obvious?

**H2 Match between system and the real world** — Use the user's words and concepts, in a natural order.
Ask: Any internal jargon, error codes, database field names? Are icons and metaphors familiar?
Is information ordered the way users think about the task, not how the backend stores it?

**H3 User control and freedom** — Give an obvious way out of mistakes; support undo/redo.
Ask: Cancel/back/close always available? Undo for destructive or bulk actions? Can users
exit a tour, wizard or modal without losing work?

**H4 Consistency and standards** — Same thing looks and behaves the same everywhere; follow platform
and industry conventions (internal and external consistency).
Ask: Same button style for same action level? Same terms throughout? Matches iOS/Android/web norms?

**H5 Error prevention** — Design out the slip before writing the error message.
Ask: Constraints (date pickers, masks), sensible defaults, confirmations for high-cost actions,
disabled states with explanations, inline validation before submit?

**H6 Recognition rather than recall** — Make options and information visible instead of memorized.
Ask: Recent items, autocomplete, visible labels (not placeholder-only), context carried between
steps, help shown where it's needed?

**H7 Flexibility and efficiency of use** — Shortcuts for experts that don't burden novices.
Ask: Keyboard shortcuts, bulk actions, saved filters, templates, personalization, command palette?

**H8 Aesthetic and minimalist design** — Every extra element competes with the important ones.
Ask: Is there anything that could be removed without loss? Does visual hierarchy put the primary
action and key information first? Decoration that adds noise?

**H9 Help users recognize, diagnose, and recover from errors** — Plain-language errors that say what
went wrong and how to fix it, shown near the problem, with visual treatment that stands out.
Ask: Does every error message say what happened + why + what to do? Is user input preserved?

**H10 Help and documentation** — Ideally unnecessary, but when needed: searchable, task-focused,
concrete steps, shown in context.
Ask: Contextual help (tooltips, inline tips) at the point of need? Empty states that teach?

How to run one: https://www.nngroup.com/articles/how-to-conduct-a-heuristic-evaluation/
Several evaluators find far more problems than one; evaluate independently, then merge.

## 2. Severity rating (NN/g scale)
Weigh frequency (how many hit it), impact (how hard to overcome), persistence (one-time vs. every time).
- 0 — Not a usability problem
- 1 — Cosmetic; fix if time allows
- 2 — Minor; low priority
- 3 — Major; important to fix, high priority
- 4 — Catastrophe; must fix before release

## 3. Usability fundamentals
- **Usability = learnability, efficiency, memorability, errors, satisfaction.** Utility (does it do
  what's needed) + usability (is it easy) = usefulness. https://www.nngroup.com/articles/usability-101-introduction-to-usability/
- **UX is the whole relationship** with the company and product, not just the UI. https://www.nngroup.com/articles/definition-user-experience/
- **Test with ~5 users, many times.** Small, iterative tests find most issues per round; spend
  budget on more rounds, not bigger rounds. (Quant studies need far more participants.) https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/
- **Response-time limits:** ~0.1s feels instant; ~1s keeps flow of thought; ~10s is the limit of
  attention — beyond 1s show a spinner/skeleton, beyond ~10s show percent-done progress and allow
  the user to do something else.
- **Scanning patterns:** People scan in F-shapes and similar patterns on text-heavy pages; front-load
  headings, sentences and link text with the information-carrying words.
- **Legacy users** need change explained, familiar patterns preserved, and control over the switch.

## 4. Research methods — what to use when
Map: https://www.nngroup.com/articles/which-ux-research-methods/ · Cheat sheet: https://www.nngroup.com/articles/ux-research-cheat-sheet/

Three dimensions: **attitudinal vs. behavioral** (what people say vs. do), **qualitative vs.
quantitative** (why vs. how many), **context of use** (natural, scripted, decontextualized).

| Question | Method |
|---|---|
| Who are users, what jobs, what pain? | User interviews, contextual inquiry, diary studies |
| Can people use this design? | Moderated/unmoderated usability testing |
| How should content be organized/labeled? | Card sorting (generate IA), tree testing (validate IA) |
| Which version performs better? | A/B test, analytics |
| What do users feel/believe at scale? | Surveys (beware survey bias) |
| Fast expert check before testing | Heuristic evaluation |
| Shared understanding of users | Empathy maps, personas |
| End-to-end experience & backstage | Journey maps, service blueprints |

Notes:
- Interviews reveal perceptions and needs, not usability — watch behavior for that. https://www.nngroup.com/articles/user-interviews/
- Open-ended questions find the unexpected; closed questions clarify. https://www.nngroup.com/articles/open-ended-questions/
- **User journey** = broad, end-to-end, emotional, multichannel; **user flow** = specific steps in
  one product for one task. https://www.nngroup.com/articles/user-journeys-vs-user-flows/
- Reframe problems as "How might we…" to keep ideation on the right problem. https://www.nngroup.com/articles/how-might-we-questions/
- Affinity diagramming to cluster findings. https://www.nngroup.com/articles/affinity-diagram/
- Synthetic (AI) users can echo the headline conclusion of real people but flatten variety — don't
  substitute them for real participants. https://www.nngroup.com/articles/synthetic-users-vs-human-respondents/

## 5. Interaction & UI guidelines (NN/g positions, condensed)

**Forms**
- Single column; labels above fields; never placeholder-as-label.
- Ask only what's needed now; mark optional (or required) consistently.
- Inline validation after the field is left, not on every keystroke; keep input on error.
- Group related fields; match field width to expected input length.
- Primary button clearly distinguished; avoid "Reset/Clear" buttons.

**Navigation & IA**
- Visible navigation beats hidden (hamburger) on desktop; discoverability drops when hidden.
- Clear labels over clever ones; "you are here" indicators; breadcrumbs for deep hierarchies.
- Search is a must for large content sets; show the query in results; handle zero-results well.
- Use card sorting and tree testing rather than guessing the IA.

**Buttons, links, signifiers**
- Things that are clickable must look clickable (flat design weakens signifiers).
- Button labels say the outcome ("Create invoice"), not "Submit/OK".
- Destructive actions separated from and visually weaker than safe primary actions.

**Errors & confirmations**
- Confirmation dialogs only for consequential, irreversible actions — overuse trains auto-clicking.
  Prefer undo over "Are you sure?".
- Error messages: visible, near the field, plain language, constructive, polite, not blaming.

**Writing for the web**
- Users read ~20–28% of words on an average page. Write concise, scannable, objective copy.
- Inverted pyramid: conclusion first. Meaningful headings and descriptive link text (not "click here").
- Plain language helps experts too.

**Modals & overlays**
- Avoid modals that interrupt unprompted, especially immediately on page load. Use them for
  critical, focused, user-initiated tasks. Always provide a visible close.

**Mobile**
- Thumb-reachable primary actions; large touch targets; minimize typing (pickers, autofill).
- Content parity with desktop; don't hide key info behind extra taps.

**Visual design**
- Hierarchy via size, color, contrast, spacing; one clear focal point per view.
- Whitespace and grouping (Gestalt) communicate structure before words do.
- Aesthetic trends that reduce legibility or affordance (e.g., heavy translucency/glass over content)
  hurt usability — content must stay readable. https://www.nngroup.com/articles/liquid-glass/

**Accessibility**
- Good accessibility = good usability for everyone: contrast, text alternatives, keyboard access,
  focus order, captions, readable type sizes.

## 6. AI products (recent NN/g themes)
- Useful assistants need relevant personal context, the ability to act on it, and UI that makes
  their limits clear. https://www.nngroup.com/articles/ai-assistant-context/
- Show what the AI did and let users preview/approve before changes commit (H1 + H3).
- Set expectations about accuracy; make it easy to verify, edit, and undo AI output.
- Agentic systems grown piecemeal become fragile — design for inspectability. https://www.nngroup.com/articles/big-ball-of-mud-ai/
