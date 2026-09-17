# Design Warmup

A five-minute design judgment exercise, packaged as a Claude skill.

You get an invented product scenario — context, a flow diagram, one UX principle, three facts, and a constraint. You commit to **two questions you'd ask and two actions you'd take**. Then a board comes back with the strongest questions and actions, and any of yours that hit are marked.

No Figma. No deliverable. No score.

The skill it trains is the one that usually gets skipped: deciding what the problem actually is before solving anything.

Includes a bank of 30 scenarios, so there's a new one every day of the month.

---

## What a round looks like

**Context** — A chain of pet urgent care clinics has a check-in app. You check in from your phone before driving over, pick your pet's symptoms from a list, and the app shows an urgency estimate.

**The flow** — Pre-check-in → symptom picker (shows estimate) → *branch*: arrives and waits for tech triage, exam, discharge / never arrives, goes elsewhere.

**UX principle** — Urgency is judged by the clinic, never by the owner.

**Tuesday** — Your PM sends these over. She thinks the picker is working and the drop-off is a marketing problem. You're not sure.

- Time to exam for true emergencies is down 20%
- Among owners shown a low urgency estimate, the share who never arrive has roughly doubled
- Two of those pets turned up at a competitor's overnight ER the same week

**The constraint** — Legal has ruled the app can never state or imply a medical assessment. The estimate copy is locked behind a six-week review.

> Two questions you'd ask, two actions you'd take.

Then the board. One of its six entries is a dud — a question that sounds smart and isn't. Naming the dud yourself is worth more than the top slot.

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
| [`RATIONALE.md`](RATIONALE.md) | Why it's shaped this way, and what got cut. Read this one if you only read one. |

`SKILL.md` is a generator, not a set of examples. That's the reason it's a skill and not a blog post — you get the thing that makes scenarios, not the four I happened to write.

---

## Take it and change it

Fork it, rewrite the rules, cut the dud, add your own problem shapes. If you find a shape that works better than mine, I'd like to hear about it — open an issue.

Built by [Ernest Leeson](https://ernestleeson.com).

MIT licensed.
