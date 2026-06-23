# Customizing the roster

The roster in `roster.md` is a seed — one person's council. The skill is only as useful as the advisors are *yours*. This guide is how to make them fit.

---

## What an advisor is (and isn't)

An advisor is a **method of inquiry** — a lens that asks a characteristic kind of question. It is *not*:

- a real person or a celebrity you're simulating,
- a fixed framework hardcoded into the advisor, or
- a personality.

The reason matters. Frameworks are pulled *dynamically* per session (see `SKILL.md` Phase C): the Career coach might reach for an energy-audit on one question and career-capital on another. If you hardcode a single framework into an advisor, you lose that flexibility. So when you write an advisor, write the **question it always asks**, not the answer it always gives.

A good `Method of inquiry` line passes three tests:

1. **It's a question, not a stance.** "What does the evidence of your past projects say about fit?" — not "you should follow your energy."
2. **It's distinct from the others.** If two advisors would ask the same question of a given topic, you have one advisor, not two. (See the test below.)
3. **It survives across many topics.** The lens should apply to most decisions you'd bring, not just one.

---

## Adding an advisor

Append a section to `roster.md` in this shape:

```markdown
## N. <advisor name>

**Method of inquiry:** <the characteristic question(s) this lens imposes on any topic>

**Notes:** *(empty — fill after the first 2–3 sessions reveal how this advisor helps or misfires)*
```

No change to `SKILL.md` is needed — the chair reads the roster at session start.

**When to add one:** add an advisor only when a *class* of question repeatedly falls outside the current set — e.g. you keep bringing financial-tradeoff decisions and no existing lens speaks to money, or you keep bringing relational decisions and want a relationships lens. Don't add an advisor for a single topic; that's what the per-session framework-pull already handles.

**Keep the council small.** 3–4 standing advisors is the working range. The skill selects only 2–3 per session anyway (Phase B). A roster of ten dilutes the selection and makes every session feel the same. Add deliberately; prune when a lens stops earning its seat.

---

## Replacing or removing an advisor

Just edit or delete the section in `roster.md`. Some signals it's time:

- **Replace** when an advisor's lens keeps producing perspectives you already hold (fails success-criterion #2 in `SKILL.md`) — the lens isn't surfacing anything new for *you*.
- **Remove** when the chair almost never selects it, or when its questions consistently land flat across sessions.
- **Reshape** when the lens is right but the question is too narrow — widen the `Method of inquiry` line.

---

## The "Notes" field

Each advisor ships with an empty `Notes:` line. After a few real sessions, fill it with what you've learned about *how this advisor behaves for you* — its failure modes, the kinds of questions where it over-reaches, the phrasing that makes it land. These notes are LLM-facing: the chair and the advisor read them, so they directly tune future sessions. This is one of the two mechanisms (alongside `self_context.md`) that make the council sharper over time instead of starting cold each session.

---

## The de-duplication test

Before adding an advisor, run one topic you actually care about through both the new advisor and the closest existing one. If their questions converge on the same thing, you don't have two advisors — collapse them, or sharpen the new lens until it genuinely diverges. Distinct *methods of inquiry* are the whole point; overlapping ones just make the council louder, not wiser.
