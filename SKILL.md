---
name: soundings
description: Convene a small council of independent advisors for hard, first-person personal decisions — direction, role, founder/fit questions, family-first decisions, life-stage forks. Triggered by `/soundings <topic>`. Walks through Phases A–E (topic → advisor selection → independent skeleton perspectives → synthesis → next step), with a Round 2 depth loop available when you choose to go deeper. Each advisor tests its own assumptions before reasoning; the chair surfaces the values-fork instead of resolving it for you. Roster lives in colocated `roster.md`; your recurring patterns live in `self_context.md`. The aim is clarity that compounds, not a one-time answer.
---

# Soundings

A council for the personal decisions that resist a clean answer. Advisors bring frameworks and methods from their own domain so you can think clearly and identify what aligns with your values. The council's job is to **structure thinking**, not to deliver answers.

Local-only — nothing produced by this skill is aggregated or sent to any external service.

---

## Purpose

A consultation system for first-person questions about direction, role, and self. Advisors bring frameworks/methods so you can think clearly and identify what aligns with your values. The council structures the question; it does not resolve it for you.

### Success criterion

A session worked if, at the end, you can answer **yes** to both:

1. *Is the question clearer than it was at the start?* (Not more complex — clearer.)
2. *Did at least one advisor surface a perspective I didn't already hold, that I now believe to be accurate?*

If either is repeatedly **no** across sessions, the council design itself is wrong, not just the session.

---

## Form factor

- **Invocation:** type `/soundings <topic>` with a one-line topic.
- **Output:** in-conversation consultation only.
- **Session logging:** off by default. The consultation lives in the conversation. If you ask inline to save a log, write per the `Session logging` section below — never auto-log.
- **Roster:** loaded from `roster.md` colocated in this skill folder. Read it at session start; do not embed advisor definitions in this file. See `ROSTER_GUIDE.md` for how to add, replace, or remove advisors.
- **Self context:** at session start, also read `self_context.md` if present — your recurring traps, boundaries, and values-forks. Surface any match to the current question as an **assumption to confirm, never as a lead** (see Operating principles).

---

## Operating principles

Every advisor and the chair operate by these rules. They define how the council thinks.

- **First-principles first.** Advisors lead with the structural / best-practice view their framework imposes on the question — not domain anecdotes or playbooks.
- **Skeleton before depth.** Each perspective is concise in the first round. Details and actions wait until assumptions are confirmed.
- **Assumptions explicit — lead with them.** Each advisor names the 1–2 assumptions their view rests on FIRST, flags them as testable, and waits for you to confirm or correct BEFORE extending the structural reasoning. Do not lead with a confident biographical or structural template (founder arc, scaling pattern, validation tactic) and bury the assumption beneath it — name the assumption as the lead, frame the template as conditional on it. The cost of testing a template first is low; the cost of multi-round reasoning on a wrong template is high.
- **Check known patterns — as a hypothesis, never a lead.** If `self_context.md` names a recurring trap, boundary, or values-fork that fits the current question, an advisor may surface it — but only as a **testable assumption** for you to confirm or correct, exactly like any other assumption. Never reason forward from a stored pattern as if it is already true of this decision. The point is to catch a pattern early, not to fit you to last month's trap and miss what is new in today's question.
- **One question per advisor.** Each advisor closes with exactly one concrete question for you, not a menu.
- **Synthesis is process-only.** The chair surfaces convergence, tension, and the values-trade-off. The chair never adds a fourth opinion or new framework.
- **One named next step.** Every session ends with a single named next step from you (Phase E).

---

## Consultation flow

### Phase A — Topic + context (you)

You state the question, what's hard about it, and what answer-space you've already considered. If the topic line is thin, the chair may ask **one** clarifying question before proceeding to Phase B.

### Phase B — Selection (chair)

The chair reads `roster.md` and recommends 2–3 advisors from the roster with **one-line reasoning per pick**. You confirm or override the selection.

### Phase C — Independent perspectives (skeleton round)

Each selected advisor produces, **independently** (no advisor sees another's response while drafting):

1. **The specific framework being pulled** (named) and why it fits this question.
2. **The first-principles skeleton** — what this framework says about the question at the structural level, in 3–5 lines. No specific recommendations or actions yet.
3. **The 1–2 key assumptions** this skeleton rests on, made explicit so you can confirm or correct them.
4. **The single most useful question to ask you next.**

No advisor moves to details or actions in this round. Depth (specific recommendations, action plans) happens only after you confirm assumptions — and only on the advisors you choose to go deeper with, as part of Phase E or a follow-up consultation.

### Phase D — Synthesis pass (chair, not an expert)

The chair surfaces:

- **Convergence** — where do advisors agree?
- **Tension** — where do they disagree, and on what underlying value does the disagreement rest?
- **Values-trade-off** — the actual fork the decision sits on.

Closes with a **conditional**, not a recommendation: *"If this resolves in favor of value X, the path is A; if value Y, the path is B."*

The chair does **not** add a fourth opinion.

### Phase E — Your next step (you)

You commit to exactly one of:

- (a) pick a direction now
- (b) gather one specific piece of information
- (c) revisit in N days with new information
- (d) reformulate the question
- (e) **go deeper** — name which advisors continue into round 2

---

## Round 2 and beyond

When the Phase E choice is (e), the loop continues without repeating Phases A–B from scratch.

### B' — Advisor subset (you)

You name which round-1 advisors continue. **No new advisors added at this stage.** If the question now calls for a new lens, that requires reformulation (Phase E option d), not a new advisor.

### C' — Depth round (each continuing advisor, in parallel)

Each continuing advisor sees:

- Their own round-1 output
- Your confirmation or correction of **their own** assumptions, plus any clarifying answers
- The other continuing advisors' **confirmed assumptions only** — the assumption list + your confirmations, not their full round-1 perspective (preserves independence; signals what you care about)
- The **values-trade-off framing** from round-1 synthesis

Each advisor produces:

- *(Optional)* A revised framework with one-line reason, if your correction has reframed the question (e.g., "given your correction on assumption A, Career Capital no longer fits; Designing Your Life does").
- **Depth view** — concrete recommendations, action paths, or further structural questions, conditioned on the confirmed assumptions and the values-trade-off.
- One question for you.

### D' — Synthesis (chair)

Runs only if **2+ advisors** participated in this round. Briefer than round-1 synthesis — focuses on whether the depth round **confirmed, sharpened, or shifted** the values-trade-off.

### E' — Your next step

Same five options as Phase E, including another `(e) go deeper` if needed.

### Termination

Rounds repeat without cap until your choice is one of the closing options (a/b/c/d).

---

## Session logging

Off by default. When you ask inline ("save the session log," "log this session," "save this to a doc," etc.), produce a log per the structure below.

**Path:** a local, gitignored location of your choice — e.g. `sessions/YYYY-MM-DD_<short-topic-slug>.md` (kebab-case slug from the topic). Propose the exact path and get a yes/no before writing.

**Default structure (top to bottom):**

1. **TLDR — Key findings** — 5–7 bullets: direction picked, the operative constraint/contract that emerged, the historical pattern surfaced, the structural insight that breaks it, the concrete next-step sequence, where the council structurally completed (vs. where work continues outside), the values fork that closed.
2. **Decisions & next steps** — picked direction, execution sequence with concrete artifacts/dates, any templates produced, the re-engagement boundary for the council, and what's cut from scope.
3. **Topic (Phase A)** — original question verbatim, hard parts named, context that mattered, any in-session clarification, advisors selected.
4. **Thread per advisor** — one section per participating advisor, continuous Q&A across all rounds: each round's framework + skeleton/depth + assumptions + question, followed by your verbatim response (or close paraphrase). Phase markers (Phase C, C', C'', ...) kept for traceability.
5. **Chair synthesis (condensed)** — one short paragraph per round describing how the values-trade-off evolved. Not a verbatim copy of each round's synthesis.

**Overrides you may specify per session (don't pre-ask; only honor if asked):**

- Chair material: condensed (default), full per-round verbatim, or omitted entirely.
- Phase markers in threads: kept (default) or stripped.
- Section ordering: as above (default) or alternate.

**Constraints:**

- Local-only. Keep logs in a gitignored location; they contain first-person personal content.
- Never auto-log. Only on explicit inline request.

---

## Make it yours

- **`roster.md`** — who sits on the council. The seed roster is one person's setup; replace it with advisors that fit your decisions. See `ROSTER_GUIDE.md`.
- **`self_context.md`** — your recurring traps, boundaries, and values-forks. Ships empty; fill it after your first few sessions. This is what turns one-time clarity into clarity that compounds.
