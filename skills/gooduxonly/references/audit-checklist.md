# GoodUXOnly Audit Checklist & Output Template

Use for any review of a screen, flow, site or app. Not every item applies — skip irrelevant sections,
but don't skip the 5-second test or states.

## Severity scale (NN/g)
- **4 Catastrophe** — blocks the task or causes loss (data, money, trust). Fix before release.
- **3 Major** — frequent or costly friction; many users stumble. High priority.
- **2 Minor** — slows people down or confuses some. Schedule it.
- **1 Cosmetic** — polish. Fix if time allows.
Raise severity if the screen is high-traffic or on the money path (signup, checkout, upgrade).

## A. 5-second test (first impression)
- [ ] Can you tell what this is and who it's for?
- [ ] Is the single primary action obvious? (Von Restorff, visual hierarchy)
- [ ] Does it look trustworthy and on-brand, not generic? (Aesthetic-Usability, point of view)

## B. Information & layout
- [ ] Clear visual hierarchy: one focal point, scannable headings (F-pattern awareness)
- [ ] Grouping via proximity/common region matches meaning (Gestalt)
- [ ] Nothing removable without loss (H8, Occam's Razor, Cognitive Load)
- [ ] Choices per step are limited; a default/recommended option exists (Hick's, Choice Overload)
- [ ] Important content doesn't look like an ad (Banner blindness, Selective Attention)
- [ ] Key items at start/end of lists (Serial Position)

## C. Interaction
- [ ] Every action gives feedback; loading states and progress (H1, Doherty)
- [ ] Clickable things look clickable; non-clickable things don't (Signifiers, Similarity)
- [ ] Targets large and reachable; primary actions in thumb zone on mobile (Fitts's)
- [ ] Undo/cancel/back available; can exit flows without losing work (H3)
- [ ] Consistent components, terms and placement; follows platform conventions (H4, Jakob's)
- [ ] Shortcuts/bulk actions for frequent users (H7)

## D. Forms & input
- [ ] Only necessary fields; optional/required marked consistently
- [ ] Persistent labels (not placeholder-only); single column
- [ ] Inline validation; input preserved on error; flexible formats accepted (Postel's)
- [ ] Smart defaults, autofill, appropriate keyboards/pickers (H5)
- [ ] Button labels describe outcomes

## E. Errors & edge states
- [ ] Error messages: what happened, why, how to fix, near the problem (H9)
- [ ] Destructive actions confirmed or undoable; visually separated (H5)
- [ ] Designed states: empty, loading, error, success, partial data, no results, offline, permission denied, long text/overflow

## F. Content & copy
- [ ] User's language, no jargon (H2)
- [ ] Front-loaded, concise, scannable; descriptive links
- [ ] Microcopy reduces anxiety at commitment points (pricing, payment, data sharing)

## G. Flow, onboarding & conversion
- [ ] Clear path to the aha moment; steps that don't serve it removed or deferred
- [ ] Value shown before friction (signup, card, permissions)
- [ ] Progress shown in multi-step flows; head start where honest (Goal-Gradient, Zeigarnik)
- [ ] Contextual, just-in-time help instead of front-loaded tours (Paradox of the Active User, H10)
- [ ] Success state at key completions with next step (Peak-End)
- [ ] Social proof, anchoring, scarcity used only truthfully

## H. Ethics & trust
- [ ] No dark patterns: fake urgency, hidden costs, pre-checked add-ons, confirm-shaming, hard-to-cancel
- [ ] Cancel/opt-out as easy as sign-up/opt-in
- [ ] Privacy and data use explained in plain language at the point of collection

## I. Accessibility
- [ ] Text contrast ≥ 4.5:1 (3:1 for large text and UI components)
- [ ] Touch targets ≥ 44×44pt (iOS) / 48×48dp (Android)
- [ ] Visible focus, logical tab order, keyboard operable
- [ ] Color not the only signal; alt text; readable type (16px+ body on mobile web)
- [ ] Reduced-motion respected

## J. Performance & responsive
- [ ] Perceived speed: skeletons, optimistic updates, < 400ms feedback
- [ ] Works at mobile, tablet, desktop breakpoints; no horizontal scroll; content parity

---

## Output template

**Verdict**
[2–3 sentences: overall state + the single most important fix.]

**What's working**
- [Thing] — [why it works / principle]

**Issues (ranked)**

| # | Sev | Where | Problem | Principle | Fix |
|---|---|---|---|---|---|
| 1 | 4 | Checkout, step 2 | … | H5 Error prevention | … |

(For long audits, group issues by screen. For short critiques, prose is fine — keep the severity,
principle and fix for each point.)

**Quick wins** (≤ 1 day) · **Bigger bets** (redesign/research needed)

**Test next**
[1–3 things worth validating with users, and the method — e.g., 5-user moderated test of the new
pricing page.]

**Further reading**
[2–4 links from sources.md tied to the top issues.]
