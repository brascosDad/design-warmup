# Design Warmup

A five-to-ten-minute design judgment exercise, packaged as a Claude skill.

You get a short invented product scenario: context, a flow diagram, two facts, a colleague's reading of them, and a constraint. You answer in one of two formats, served at random:

- **Format B — Find it.** Name the one thing that doesn't add up, then give one action based on what you found.
- **Format C — Pick, then write.** Five candidate moves. Pick the strongest, call the decoy, then add one move of your own.

Then a board comes back with what the scenario was built around, in order of what it unlocks, with any of yours that hit marked. The round closes with an extra credit: write the two sentences you'd actually say to the colleague who reads it differently.

No Figma. No deliverable. No score.

It trains two things that usually get skipped: deciding what the problem actually is before solving anything, and then saying so to someone in the room.

Scenarios are composed from 60 settings, 23 problem shapes and 3 modes, and the skill checks your past rounds (where your Claude can search chat history) so it doesn't serve you the same story twice.

---

## What a round looks like

*Format B, about 5 minutes. First instinct counts, and fragments are fine.*

**Context** — Northgate Community College lets students join a waitlist when a class section is full. When a seat opens, the registration app offers it to the next student in line, who has 24 hours to claim it before it moves down the list.

**The flow** — Join waitlist → a seat opens → offer sent to next in line → 24 hours to claim → *branch*: claimed, enrolled / no response, offer moves to the next student.

**Tuesday** — Your associate dean sends these over.

- During add/drop week, an opened seat sat empty for 3.1 days on average before someone claimed it.
- Of the students who let an offer expire, 68% were already enrolled in that same course, just in a different section.

She says students are treating offers casually and wants to cut the claim window from 24 hours to 6.

**The constraint** — The student information system is run by a vendor. Your team owns the app's screens and notifications, but can't change how waitlists are stored or ordered this term.

> **What's the one thing here that doesn't add up?** Then give one action you'd take, based on what you found.

Then the board: four finds and four actions, in order of what they unlock, plus one decoy. The decoy is the fix a stakeholder has already proposed — here, the 6-hour window. It isn't a bad idea, it's a borrowed one, and catching it is worth more than any hit.

The round closes in three parts: your strongest hit, the top slot you didn't get and why it matters, and a named pattern to carry into real work. Here it's **a queue stores stale intent**.

Then the extra credit:

> Write the two sentences you'd say to the dean on Thursday that tell her the 6-hour window is the wrong fix without making her feel wrong.

Write it, and you get one catch (accuracy first, then tone) and a tightened version in your own voice.

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
| [`SKILL.md`](SKILL.md) | The skill — the two formats, modes, scenario fields, the flow spec, the board, the close, the extra credit |
| [`references/variety.md`](references/variety.md) | 60 settings and 23 problem shapes that scenarios are composed from |
| [`references/scenarios.md`](references/scenarios.md) | 30 worked seeds — a pattern library showing how a shape becomes a scenario |
| [`RATIONALE.md`](RATIONALE.md) | Why it's shaped this way, and what got cut. Read this one if you only read one. |

`SKILL.md` is a generator, not a set of examples. The pools give it the raw material, the seed bank shows what good looks like, and the rules turn each pick into a fresh round. That's why it's a skill and not a blog post.

---

## Changelog

**November 2026**
- Two formats replace "two questions, two actions," which took longer than a warmup should. **B** asks you to find the one thing that doesn't add up and give one action. **C** gives you five candidate moves to pick from, a decoy to call, and one move to write yourself. Each round is one or the other, at random, unless you ask for a specific one.
- Extra credit at the end of every round: write the two or three sentences you'd say to the scenario's stakeholder, and get one catch and a tightened version back.
- Shorter scenarios: two facts instead of three, and the UX principle is built into the plant instead of served as its own field.

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
