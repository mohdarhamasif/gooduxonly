# Laws of UX — Applied

Source: https://lawsofux.com/ by Jon Yablonski (site licensed CC BY-NC-ND 4.0; these are
paraphrased summaries with original application notes — link users to each law's page).
Each entry: what it means → how to apply → common misuse.

## Perception & grouping (Gestalt)

**Law of Proximity** — Things near each other read as related.
Apply: tighter spacing within a group than between groups; keep labels close to their fields.
Misuse: equal spacing everywhere, so nothing groups. https://lawsofux.com/law-of-proximity/

**Law of Common Region** — A shared boundary (card, background, border) creates a group.
Apply: cards for list items, panels for settings sections. Misuse: boxes inside boxes inside boxes. https://lawsofux.com/law-of-common-region/

**Law of Similarity** — Things that look alike are read as belonging together/doing the same thing.
Apply: one style per action level; links look like links everywhere.
Misuse: styling a non-clickable label like a button. https://lawsofux.com/law-of-similarity/

**Law of Uniform Connectedness** — Visually connected elements (lines, shared frames) feel more related than mere proximity.
Apply: steppers, timelines, connected toggles. https://lawsofux.com/law-of-uniform-connectedness/

**Law of Prägnanz** — People read complex visuals as the simplest possible form.
Apply: simple, recognizable icons and shapes; reduce visual complexity. https://lawsofux.com/law-of-pr%C3%A4gnanz/

**Von Restorff Effect** — The one item that differs is the one remembered.
Apply: make the primary CTA or recommended plan visually distinct. Misuse: highlighting many things
(then nothing stands out); relying on color alone (accessibility). https://lawsofux.com/von-restorff-effect/

**Aesthetic-Usability Effect** — Attractive designs are perceived as easier to use and earn more tolerance.
Apply: polish matters for trust and first impressions. Misuse: beauty masking real usability
problems in testing — watch behavior, not just praise. https://lawsofux.com/aesthetic-usability-effect/

## Decision-making & choice

**Hick's Law** — Decision time grows with the number and complexity of options.
Apply: fewer choices per step, recommended defaults, progressive disclosure, highlight one option.
Misuse: over-simplifying into many extra steps; it applies to choices, not to scanning familiar menus. https://lawsofux.com/hicks-law/

**Choice Overload** — Too many options overwhelms and can lead to no choice at all.
Apply: curate; offer comparison tools; filter; 3–4 pricing tiers max. https://lawsofux.com/choice-overload/

**Occam's Razor** — Prefer the simplest solution that works equally well.
Apply: remove elements until removing more would hurt. https://lawsofux.com/occams-razor/

**Tesler's Law (Conservation of Complexity)** — Some complexity can't be removed, only moved.
Apply: let the system absorb it (smart defaults, auto-detection) rather than pushing it onto users.
Misuse: "simplifying" by hiding needed controls, so users carry the burden. https://lawsofux.com/teslers-law/

**Pareto Principle** — ~80% of effects come from ~20% of causes.
Apply: design and test the critical 20% of flows hardest; prioritize fixes by usage. https://lawsofux.com/pareto-principle/

**Cognitive Bias** — Systematic thinking shortcuts shape judgment.
Apply: know the biases (see product-psychology.md) — in your users and in your own design decisions. https://lawsofux.com/cognitive-bias/

## Memory & attention

**Miller's Law** — Working memory holds roughly 7±2 items.
Apply: chunk content; don't rely on users remembering across screens.
Misuse: treating "7" as a hard limit for nav items — the real lesson is chunking. https://lawsofux.com/millers-law/

**Working Memory** — A small, temporary store for task info.
Apply: carry context forward (show what was chosen earlier), recognition over recall. https://lawsofux.com/working-memory/

**Chunking** — Group pieces into meaningful units.
Apply: phone/card number formatting, sectioned forms, headings, short paragraphs. https://lawsofux.com/chunking/

**Cognitive Load** — Mental effort needed to use the interface. Intrinsic load comes from the task;
extraneous load comes from bad design — cut the extraneous.
Apply: remove visual noise, reuse patterns, offload work (defaults, autofill). https://lawsofux.com/cognitive-load/

**Selective Attention** — People focus on what serves their goal and filter the rest (incl. banner blindness).
Apply: don't make important content look like ads; put key info in the task path. https://lawsofux.com/selective-attention/

**Serial Position Effect** — First and last items in a list are remembered best.
Apply: put key nav items at the start/end; important points first and last. https://lawsofux.com/serial-position-effect/

**Zeigarnik Effect** — Unfinished tasks stick in memory.
Apply: progress bars, profile-completion meters, checklists that show what's left. Misuse: guilt-based nagging. https://lawsofux.com/zeigarnik-effect/

**Peak-End Rule** — Experiences are judged by the peak moment and the end.
Apply: design memorable success states and graceful endings (checkout confirmation, offboarding);
fix the worst pain point first (negative peaks dominate). https://lawsofux.com/peak-end-rule/

## Motor & time

**Fitts's Law** — Time to hit a target depends on its size and distance.
Apply: big primary buttons, generous touch targets, place actions near the cursor/thumb, use screen edges.
Misuse: tiny close buttons; destructive actions right next to primary. https://lawsofux.com/fittss-law/

**Doherty Threshold** — Productivity soars when system and user respond within ~400ms.
Apply: optimistic UI, skeletons, instant feedback; perceived performance matters. https://lawsofux.com/doherty-threshold/

**Goal-Gradient Effect** — Motivation rises as the goal gets closer.
Apply: show progress, give a head start (pre-filled first step), short remaining steps. https://lawsofux.com/goal-gradient-effect/

**Parkinson's Law** — Tasks expand to fill the time allowed.
Apply: autofill, one-click flows, estimated time ("takes 2 minutes") to set expectations. https://lawsofux.com/parkinsons-law/

**Flow** — Full immersion when challenge matches skill and feedback is immediate.
Apply: remove interruptions, give clear goals and instant feedback; scale difficulty. https://lawsofux.com/flow/

## Expectations & behavior

**Jakob's Law** — Users spend most time on other products, so they expect yours to work the same way.
Apply: follow established patterns (cart top-right, logo links home); when redesigning, let users
transition gradually. https://lawsofux.com/jakobs-law/

**Mental Model** — Users' internal picture of how a system works.
Apply: research users' models (card sorting, interviews) and match them; close the gap between
designer and user models. https://lawsofux.com/mental-model/

**Paradox of the Active User** — People start using software right away instead of reading instructions.
Apply: in-context help, learn-by-doing onboarding, tooltips at point of need; never rely on a manual. https://lawsofux.com/paradox-of-the-active-user/

**Postel's Law** — Be liberal in what you accept, conservative in what you send.
Apply: accept many input formats (phone numbers with spaces, dates in various formats) and normalize;
output clean, predictable results. https://lawsofux.com/postels-law/

## Quick lookup: problem → law
| Symptom | Laws to cite |
|---|---|
| Users stall at a choice / pricing page | Hick's, Choice Overload, Von Restorff |
| Users miss the CTA | Von Restorff, Fitts's, Selective Attention, Serial Position |
| Screen feels cluttered | Cognitive Load, Occam's Razor, Prägnanz, Proximity |
| Users forget info between steps | Working Memory, Miller's, Chunking |
| Users abandon multi-step flow | Goal-Gradient, Zeigarnik, Parkinson's |
| "Feels slow" | Doherty Threshold |
| Users don't read onboarding | Paradox of the Active User |
| Unusual UI confuses people | Jakob's Law, Mental Model |
| Form rejects valid input | Postel's Law |
| Bad lasting impression | Peak-End Rule |
