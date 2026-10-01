# Design Warmup

A five-minute design judgment exercise, packaged as a Claude skill.

You get an invented product scenario — context, a flow diagram, one UX principle, three facts, and a constraint. You commit to **two questions you'd ask and two actions you'd take**. Then a board comes back with the strongest questions and actions, in order of what they unlock, and any of yours that hit are marked.

No Figma. No deliverable. No score.

The skill it trains is the one that usually gets skipped: deciding what the problem actually is before solving anything.

Scenarios are composed from 60 settings, 23 problem shapes and 3 modes, and the skill checks your past rounds (where your Claude can search chat history) so it doesn't serve you the same story twice.

---

## What a round looks like

**Context** — A chain of pet urgent care clinics has a check-in app. You check in from your phone before driving over, pick your pet's symptoms from a list, and the app shows an urgency estimate.

**The flow** — Pre-check-in → symptom picker (shows estimate) → *branch*: arrives and waits for tech triage, exam, discharge / never arrives, goes elsewhere.

**UX principle** — Urgency is judged by the clinic, never by the owner.

**Tuesday** — Your PM sends these over.

- Time to exam for true emergencies is down 20%
- Among owners shown a low urgency estimate, the share who never arrive has roughly doubled
- Two of those pets turned up at a competitor's overnight ER the same week

She thinks the picker is working and the drop-off is a marketing problem. You're not sure.

**The constraint** — Legal has ruled the app can never state or imply a medical assessment. The estimate copy is locked behind a six-week review.

> Two questions you'd ask, two actions you'd take.

Then the board: six questions and four actions, in order of what they unlock, plus one decoy. The decoy is the move a stakeholder has already endorsed. It isn't a bad question, it's a borrowed one, and catching it is worth more than any hit.

The round closes in three parts: your strongest hit, the top slot you didn't get and why it matters, and a named pattern to carry into real work.

---

## Install

**Claude Code / Claude desktop**

```bash
git clone https://github.com/brascosDad/design-warmup.git ~/.claude/skills/design-warmup
```

**claude.ai**

Download the repo as a ZIP and upload it under Settings → Capabilities → Skills.

Then ask for a design warmup, a design exercise, or a scenario to think through.

---

## What's here

| File | What it is |
|---|---|
| [`SKILL.md`](SKILL.md) | The skill — modes, the five scenario fields, the flow spec, the board, the rules |
| [`references/variety.md`](references/variety.md) | 60 settings and 23 problem shapes that scenarios are composed from |
| [`references/scenarios.md`](references/scenarios.md) | 30 worked seeds — a pattern library showing how a shape becomes a scenario |
| [`RATIONALE.md`](RATIONALE.md) | Why it's shaped this way, and what got cut. Read this one if you only read one. |

`SKILL.md` is a generator, not a set of examples. The pools give it the raw material, the seed bank shows what good looks like, and the rules turn each pick into a fresh round. That's why it's a skill and not a blog post.

---

## Changelog

**October 2026**
- Variety: scenarios are now composed from three axes (setting, problem shape, mode) instead of mapping the day of the month to one of 30 fixed seeds, which served the same story on the same date every month. New `references/variety.md` holds the pools.
- History check: where past-chat search exists, the skill looks at your recent rounds and avoids their settings, shapes and mode.
- Context first, as seen: on surfaces that collapse text written before a tool call, Context and the flow header go out as a visible message before the diagram, so the round never opens on the picture.
- The examples you've already read (pet urgent care, showing requests) are never served.

---

## Take it and change it

Fork it, rewrite the rules, cut the decoy, add your own scenarios and problem shapes. If you find a shape that works better than mine, I'd like to hear about it — open an issue.

Built by [Ernest Leeson](https://ernestleeson.com).

MIT licensed.
