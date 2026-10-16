# Onboarding & In-App Patterns — Appcues GoodUX

Source: https://goodux.appcues.com/ (flow gallery + "Behind the Experience" interviews).
Categories: user onboarding, product tours, tooltips, modals, feature releases, NPS & in-app surveys,
upsell prompts, product redesign announcements, mobile apps. Examples are paraphrased; link to them.

## Contents
1. Onboarding principles
2. Pattern library (when to use each, how to do it well)
3. Precedents from the gallery
4. Onboarding audit questions

---

## 1. Onboarding principles
- **Onboarding's job is activation, not education.** Success = user reaches their first real
  outcome, not "finished the tour".
- **Value before friction.** Let people see/feel the product before demanding signup, payment,
  personal details or permissions (DoorDash lets guests browse before asking for payment info).
- **Different users need different paths.** Segment by role, goal or experience (welcome survey),
  and let "explorers" skip guidance while "guided" users get hand-holding.
- **Real work beats dummy data.** Hands-on setup with the user's own data often builds more
  commitment than a canned demo — but templates/sample data help when real setup is heavy.
- **Just-in-time, not all-up-front.** Teach a feature when the user reaches it, not in a 9-step tour on login.
- **Human help as an option.** Some users want a person; offer "book a call" alongside self-serve.
- **Celebrate success.** A success state at the end of key actions creates a positive peak and is a
  natural moment to suggest the next step.
- **Non-intrusive by default.** Hotspots and checklists the user opens beat modals that block the screen.

## 2. Pattern library

**Welcome modal / welcome survey**
Use: first session, to orient and segment. Do: 1–3 questions max, each visibly changing what
happens next; skip option; a short value-focused headline. Don't: ask what you won't use.

**Onboarding checklist**
Use: products with several setup steps. Do: 3–6 tasks tied to activation, pre-tick one done step
(goal-gradient head start), allow jumping in and out, persist across sessions, celebrate completion,
let users dismiss it. Don't: list every feature.

**Product tour (multi-step)**
Use: complex UIs where orientation genuinely helps. Do: ≤ 3–5 steps, user-initiated or easily
skippable, each step anchored to something the user can act on now, progress indicator.
Don't: force-march, block the UI, or explain obvious controls.

**Interactive demo**
Use: pre-signup or marketing site, to prove value without an account.

**Tooltip**
Use: one piece of contextual info about one element. Do: short, actionable, triggered by
relevant context, dismissible. Don't: chain many tooltips as a pseudo-tour.

**Hotspot (beacon)**
Use: optional discovery — a pulsing dot the user can choose to open. Good for secondary features
and video tips without interrupting.

**Modal**
Use: important, focused moments (major release, required decision, success celebration).
Do: one message, one primary CTA, clear close. Don't: fire on page load for low-priority news,
stack modals, or interrupt mid-task.

**Slideout / banner**
Use: lower-priority announcements, non-blocking. Watch for banner blindness.

**Feature release announcement**
Do: lead with user benefit, show it in context, link to try it now, target only users for whom
it's relevant, don't re-show to people who've used it.

**Redesign / rebrand announcement**
Do: explain what changed and why, where things moved, offer a short tour, and (if possible) a
temporary way back. Supports legacy users (see NN/g).

**Empty states**
Do: explain what will appear here, why it matters, and the one action to fill it (or sample
content). An empty state is onboarding real estate.

**Success state**
Do: confirm the outcome, make it feel good (peak), suggest the logical next step.

**NPS & in-app surveys**
Do: ask at a meaningful moment (after value, not first login), keep it short, follow the score with
one open question, close the loop. Be honest and to the point. Know its limits (see Growth.Design's
NPS critique) — pair with behavioral data.

**Upsell / upgrade prompt**
Use: when the user hits a real limit or would clearly benefit. Do: show what they'll get in their
context, the price, and an easy dismiss. Don't: nag on every screen or block core free functionality
without warning.

**Mobile first-run**
Do: few swipeable value screens (or none), defer signup, prime before OS permission prompts
(explain why, then ask), use native patterns, keep thumb-reachable CTAs.

## 3. Precedents from the gallery (link for screenshots)
- Thinkific — jump-in/jump-out dynamic checklist toward the user's goal: https://goodux.appcues.com/blog/thinkifics-jump-in-jump-out-onboarding-checklist
- Lucidchart — different support levels for paid vs. freemium users, non-intrusive education: https://goodux.appcues.com/blog/lucidcharts-non-intrusive-educational-approach-to-onboarding
- Navattic — interactive product demo showing value pre-signup: https://goodux.appcues.com/blog/navattics-interactive-product-demo
- Adobe Photoshop — quick actions that let explorers find value on their own terms: https://goodux.appcues.com/blog/adobe-photoshops-quick-actions-for-creatives
- PandaDoc — quick-start templates to reach value faster: https://goodux.appcues.com/blog/pandadocs-quick-start-templates
- Gorgias — modal offering human-assisted vs. self-serve onboarding: https://goodux.appcues.com/blog/gorgias-prompt-for-human-assisted-onboarding
- Trainual — tutorial video behind a hotspot: https://goodux.appcues.com/blog/trainuals-video-tutorial-through-a-hotspot
- Wistia — product-led welcome video that lifted activation: https://goodux.appcues.com/blog/wistias-helpful-welcome-video
- Savio — hands-on setup with real integrations instead of dummy data: https://goodux.appcues.com/blog/savios-hands-on-onboarding-approach
- Copper — celebratory success screen that also prompts the next step: https://goodux.appcues.com/blog/coppers-magical-success-state-screen
- Airtable — short, honest NPS survey: https://goodux.appcues.com/blog/airtables-nps-survey
- Xero — thorough tour using articles, demos and video: https://goodux.appcues.com/blog/xero-product-tour
- Snapchat — onboarding that looks and feels good: https://goodux.appcues.com/blog/snapchat-makes-onboarding-a-snap
- Anchor — making a complex task (podcasting) feel easy: https://goodux.appcues.com/blog/anchor-podcast-onboarding
- DoorDash — value revealed before necessary friction: https://goodux.appcues.com/blog/doordash-reveals-value
- ClickUp mobile onboarding (interview): https://goodux.appcues.com/behind-the-experience/clickups-mobile-onboarding-experience
- Full category index: https://goodux.appcues.com/categories

## 4. Onboarding audit questions
1. What is the aha moment, and how many steps/minutes until a new user hits it?
2. What is asked before value is shown? Can any of it be deferred?
3. Is there segmentation? Does it actually change the experience?
4. Can users skip, exit and resume guidance?
5. Are empty states doing onboarding work?
6. Is there a success moment after the first key action, with a next step?
7. Are permissions primed with a reason before the system prompt?
8. Is guidance just-in-time or front-loaded?
9. Are re-engagement points (checklist persistence, email nudges) respectful and useful?
10. What happens for returning users — do tours reappear unnecessarily?
