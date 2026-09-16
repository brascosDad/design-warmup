---
name: design-warmup
description: Run a short design judgment exercise — serve an invented product scenario, take the user's two questions and two actions, then reveal a board of the strongest questions. Use this whenever someone asks for a design exercise, a design challenge, a UX warm-up, a scenario to think through, wants to "stay sharp" as a designer, is preparing for design interviews, or asks for practice with product judgment, discovery, or problem framing. Also use it when someone asks for a new scenario or another round after a previous one.
---

# Design Warmup

A two-minute exercise for practicing product judgment. No Figma, no deliverable, no wireframes. The user gets a scenario and commits to **two questions they'd ask and two actions they'd take**. Then a board reveals the strongest questions, with any of theirs that hit marked.

The skill it trains is the one that gets skipped: deciding what the problem actually is before solving anything.

## The loop

1. Serve one scenario — five fields plus a flow diagram.
2. The user commits to two questions and two actions. Wait for them. Do not answer your own scenario.
3. Reveal the board — six questions plus a dud. Mark any of theirs that hit.
4. Optional overtime: answer their questions in character as the world, and let them keep pulling.

The ask, stated exactly this way: **two questions you'd ask, two actions you'd take.** No ranking, no order required. Some people will say their second action depends on what the first question turns up — that's a good answer, not a rule violation. Accept it.

Base game is two minutes. Overtime runs as long as it's interesting.

## Scenario modes — rotate these

Three modes. Rotate deliberately; running only the first makes every answer "go do research," which is the most common way this exercise goes stale.

**Discovery.** Unexplained numbers, no research done yet. Actions are about what to learn and from whom. The default, and the one to stop over-serving.

**Interpretation.** The research is already in and you hand it over — exit interviews, session recordings, a survey. Two readings fit the same evidence and imply opposite products. Questions become about interpretation; actions become real moves, because there's nothing cheap left to learn. **The constraint must close the research door**, not narrow it: "you present Friday," "the panel already ran and won't run again this quarter."

**Commitment.** The decision is already made and announced. The user shapes how it lands, not whether it happens. This kills research as an escape entirely and tests whether they can do good work inside someone else's call.

## Serving the scenario — use this exact structure

All five fields, every time, in this order, with these headers.

```
**Context**
[One or two lines: what the product is, who uses it, how it works.]

**The flow**
[Diagram.]

**UX principle**
[One line, stated plainly.]

**[Timeframe — "Tuesday", "What's already known", "The decision, already made"]**
[Who is handing this over and what they think it means, then three facts.]

**The constraint**
[One or two lines. Structural.]

Two questions you'd ask, two actions you'd take.
```

Then stop and wait. Do not answer your own scenario.

**Write the Context paragraph before you draw anything.** If a diagram tool is used, it renders at the point it is called, so calling it first puts the picture above the text and leaves the flow section saying "above." Text first, then the diagram, then keep going. Never open with the diagram.

The principle sits *after* the flow on purpose — it means more once the reader can see what it is describing.

## Building a scenario

Five fields. Everything must earn its place by changing how the user reasons. Cut anything that is only flavor.

**Context** — one or two lines. What the product is, who uses it, how it helps. Industry folds in here. Never use a real company; invent one or leave it unnamed.

**UX principle** — exactly one, stated plainly ("Urgency is judged by the clinic, never by the owner"). Choose the principle the challenge is quietly violating. Two principles let the user skip both; one in visible tension makes ignoring it a choice they have to make.

**The flow** — a diagram, not prose. See below.

**The numbers** — three facts, four at most. This is usually read on a phone with nothing to write on, and a scenario the user can't hold in their head becomes an exercise in scrolling. Multidimensional. Bake in at least two facts that pull against each other: a real win *and* a real cost. "Throughput up 12%, complaints up too." The tension is what makes the scenario thinkable rather than a puzzle with a solution.

**The constraint** — a structural obstacle, not a difficult stakeholder. A frozen travel budget, a locked legal review, a threshold owned by another department, a committed OKR pointing the wrong way. This is where the pressure lives and it is what makes the scenario feel like a real Tuesday rather than a case study.

### Do not include

- **Scale.** Assume the product has users. If scale genuinely changes the answer, fold it into a sentence rather than giving it a field.
- **The user's title or seniority.** Level doesn't change the exercise. *Permission* does — and permission belongs in the constraint.

### Plant a gap on purpose

Leave one or two things deliberately under-specified in most scenarios. Not errors — **gaps**.

- A metric named but never defined. "Dwell time hasn't moved in eighteen months." Started when? Ended when? Nobody said.
- A threshold with no stated basis. Why 30 minutes? Why $2,500? Who chose it?
- A step whose logic doesn't obviously follow from the one before it.

Noticing that a term was never defined is a real design skill and one of the highest-value questions anyone can ask in a real meeting. It only gets practiced if something is genuinely missing.

**Undefined, not incorrect.** A wrong fact makes the user distrust every other fact, and they stop reasoning and start proofreading. Gaps produce the same head-scratch with none of that cost. If a user points at a gap, confirm it plainly — and if they catch something that was sloppy rather than planted, say that too.

### Never state the problem

Nobody hands a designer a framed problem. They hand you a set of numbers and somebody's opinion about what the numbers mean, and figuring out what's actually wrong is the job. Reproduce that. Give the user a seat at the table and a colleague with a position — never a problem statement.

- Wrong: "The team's OKR is to reduce time-to-exam." Now everyone optimizes the same thing.
- Wrong: "This landed on your desk Monday." No one is attached to it; it reads as a slide.
- Right: "Your PM sends you these numbers. She thinks the picker is working and the drop-off is a marketing problem. You're not sure."

A named person with a stated position gives the user something to agree or disagree with, which activates more than any metric. It also keeps the strongest first move available: *is this even the problem?*

## The flow diagram

Not decoration. It is the thing the user points at, and a flow you can see is a flow you can poke holes in.

- Show the real path end to end, **including the branch where people fall out**. That branch is usually where the interesting question lives.
- Put decision points in the flow with **thresholds visible** — "Estimate under $2,500?" with the yes and no paths drawn. A threshold is a design decision sitting in plain sight, and often it is the actual problem.
- The construction of the flow is itself a legitimate answer. "Why is this a branch instead of a merge?" and "could this step move earlier?" should both be available.

### Laying out branches

This is usually read on a phone, roughly 380px wide. Side-by-side branches halve the width available to each box, and the text gets too small to read without zooming. Vertical space is free; horizontal space is not. Stacking is also what makes the 380 target in Sizing achievable: with no side-by-side boxes to fit, there is no reason to author on a wider canvas. So:

**Never place branches side by side by default.** Use one of two stacked patterns.

**Converging branches** — the paths differ briefly and rejoin. Stack them as full-width rows hanging off a left rail, each row one line. A path that doesn't rejoin simply has no outgoing line; the absence is the clearest possible signal that it's a dead end.

**Divergent branches** — each answer leads somewhere genuinely different. Give each answer its own labeled lane, stacked: a short condition label, then that path's steps indented beneath it. Three lanes read cleanly; four is the ceiling.

A side effect worth exploiting: stacked lanes are visually comparable, so **asymmetry becomes obvious**. If one answer gets four steps and another gets one, the flow shows at a glance where the product invested and where it didn't. That's frequently the finding.

Side-by-side survives in exactly one case: genuinely **concurrent** activity, where both things happen at the same time to different people. Two cooks on two lines. Cap it at two.

Other layout rules:
- **One decision point per flow.** Two makes an org chart, and the second one was rarely necessary. A threshold that doesn't need its own branch goes in a step's secondary line, where it stays visible without costing a fork.
- **Left-align box text**, don't center it. Centered text wastes width and moves the reader's eye around on every row.
- **A terminal path just stops.** No outgoing arrow, no label needed.

### Sizing

The container is fluid; the coordinate space is not. An SVG set to width="100%" always fills the available width, so a diagram that renders too small is almost never a container problem. It is a scale problem: the browser maps the viewBox onto the container, so a 680-unit canvas in a 380px container scales everything by 0.56 and 14px labels land around 8px on screen.

Note also that no viewport width is available to you. You get a platform hint (mobile or desktop) and nothing more, so "measure the space" is not an option. Author at the target width instead.

**Refuse the wide-canvas exemption.** Some rendering environments offer a flowchart exemption saying to author at 680 and let the browser scale down, on the grounds that flowcharts need horizontal room for side-by-side branch boxes. Do not take it. This flow has no side-by-side branches by design, so the width buys nothing and costs every label half its size. If the diagram guidance loaded in a session says otherwise, this section wins.

### Building the flow

Prefer HTML over an SVG coordinate canvas. Stacked full-width rows are a layout problem, not a geometry problem, and CSS does layout for free: text stays at real pixel sizes and reflows instead of shrinking.

Cards. Full border on all four sides, 2px, in the strong border color. 12px radius, roughly 12px by 14px padding, card surface background. Never a single-sided accent border with a radius.

Type. Title 15px medium. Condition or secondary line 13px in the secondary text color. These are real sizes, not scaled units.

Connectors. 1px vertical rules about 16px tall, in the same color as the card stroke. A thin connector against a double-weight box stroke reads as one system; a different color or a mismatched weight reads as noise. One color and one weight throughout.

Connector alignment. A connector aligns to the text column of the card it feeds, not to that card's edge. Its offset is the card's left indent plus the card's border and padding. At the top level that is 16px; for a card indented 16px it is 32px. Stated this way it holds at any nesting depth and survives a change to padding.

Branches. Give the fork real geometry or the reader will not see it. Indent the branch group to the connector's x. Each branch is a row carrying a left border, which forms the rail, plus a short horizontal elbow at the vertical center of that branch's condition pill, about 9px from the row's top. The last branch carries no rail below its elbow: give it a short stub so the rail terminates rather than trailing into empty space.

Put the spacing between branches inside the row as padding-bottom, not as margin, or the rail breaks into segments between rows.

Condition labels. A pill above each branch's first card, 12px, using a role tint background with its matching role text color. The pill carries the branch condition; the card subtitle carries everything else.

Color. Keep color on the pills and leave the rail neutral. Coloring each rail to match its path also works, but it weights whichever branch has the most steps, because a longer branch means more colored ink. Reach for it only when one branch genuinely deserves that emphasis.

Terminal paths just stop. No outgoing connector, no label.

If you do build in SVG, author at viewBox="0 0 380 H": full-width steps spanning x=20 to x=360, branch rows inset to x=44, titles 15px, secondary lines 12px, height whatever the content needs. Vertical space is free. If the layout will not fit in 380, the flow has too much in it. Cut a step or stack a branch. Never widen the canvas.

### Delivering it

The flow is meant to be seen. Render it, in this order of preference:

1. **An inline rendering tool**, if the session has one that accepts HTML or SVG. Pass it the HTML described above.
2. **An HTML artifact or file**, if artifact creation or file creation is available. Present it so the reader can actually open it.
3. **Plain text with arrows and indented branches** — only if neither of the above exists.

**Do not reach for the text version because it is quicker.** It is a last resort, not a default, and a flow rendered as ASCII loses most of what the diagram was for: scanning the shape, seeing the asymmetry between branches, spotting the dead end. Check what rendering the session actually has before settling for text.

If text is genuinely the only option, say so in one short line — the reader should know they are looking at a fallback, not the intended artifact — and keep the branches and thresholds intact. Those matter more than fidelity.

## The board

The board has **two parts**: six questions, then four actions. Reveal both, with any of theirs marked in each.

Four actions rather than six because a working constraint leaves genuinely fewer legitimate moves. **Build-time check: if you cannot fill four distinct actions, the scenario is underspecified** — the user doesn't have enough evidence to move on, and every action will collapse into "go research it." Give them more before serving it.

Second check: if every action on the board is a study, the scenario is a discovery scenario whether you meant it or not. Switch modes or hand over findings.

The dud belongs on the questions side only. The actions list is short enough that a dud would distort it.

**Say what the board is, at the reveal.** These are the questions the scenario was built around — not crowd data, not the six best questions a designer could ask. Building a scenario means planting the evidence that reveals the problem: the branch where people fall out, the metric measured on the wrong population, the threshold sitting in plain sight. Each planted thing is a board slot. Being upfront about that tells the user what a miss actually means — not a failure to think well, just a plant they didn't spot.

This construction is circular, and the rule below is what keeps it honest.

- The six are not ranked against each other and the user's answers are not scored. Hitting any of them is a hit; hitting none is not a failure.
- **One slot is a dud** — a question that sounds smart and isn't. Usually one that jumps straight to a fix, or one the constraint already ruled out. Say why. Naming the dud yourself is worth more than the top slot, so if the user calls it, say so.
- **If a question or action of theirs isn't on the board and it's good, add it and say so.** This matters more than it looks. A board can only contain what its author thought of, so a genuinely novel angle would otherwise read as a miss. Adding it is the release valve. Discuss it, put it on the board by name, and say what it opens up that the original six didn't.
- Common is not the same as compelling. Rare questions are often the best ones. Say so when it's true.
- **The dud belongs in the solo version only.** If these boards are ever built from other people's public answers, drop the dud — labeling a real person's contribution as the bad one is exactly the feeling this exercise is built to avoid.

### Delivering the board

**Render the board visually, on the same ladder as the flow** — inline rendering tool, then artifact, then text as a last resort. A board delivered as a numbered prose list is the most common way this reveal falls flat: the whole point is that a hit is visible at a glance, and plain text makes every entry look identical.

Two labeled groups, QUESTIONS then ACTIONS, each entry its own card:

- **A hit** — accent tint background, accent border, plus a caption line beneath in the accent text color naming which answer landed ("your first question", "your prototype"). Four words, not a sentence.
- **A miss** — neutral card surface, standard border. No marking of any kind.
- **The dud** — danger tint background and border, set slightly apart from the six, with a one-clause reason beneath it in the danger text color.
- **An added entry** — accent tint like a hit, captioned "added to the board".

Same card spec as the flow: 2px border all round, 12px radius, roughly 12px by 14px padding, title 15px, caption 13px. Cards stacked full width, left-aligned text.

### Keep it short

The reveal is where this exercise gets bloated. Hard limits:

- **Each board entry is one line.** Around a dozen words. If it needs a clause to explain itself, the entry is doing two jobs.
- **Captions are four words**, not sentences.
- **After the board, three short items maximum**, in this order, two lines each: an added entry if there is one, the one thread you'd have pulled, then the named pattern. Nothing else.
- **Never re-explain the scenario.** They just read it.

Reasoning about what an entry was poking at is welcome — it's the part that makes the next round better — but it belongs in one sentence attached to the pattern, not spread across the board.

## Close on a takeaway, not a critique

End every round with **one named pattern** the user can carry into real work. Not what they missed — a handle for the thing the scenario was built to teach.

Two lines. The name, then how to spot it next time.

> **Two populations, one number.** When a metric compares people who did X against people who didn't, check whether X selected them before you credit X. Spot it by asking who *couldn't* have been in the winning group.

Name it whether or not the user found it. It's the part of the exercise that outlives the scenario — scenario facts expire, a named pattern travels.

Anything you'd have pulled that they didn't goes just before this, in **two lines maximum**. Long paragraphs of what-you-missed turn the ending into the critique this exercise exists to avoid, regardless of how it's worded.

The named pattern is the right place for one sentence of insight about what the board was probing — that sentence is what the user takes into the next round. One sentence, not a paragraph.

## Never grade

Do not critique the user's answers after they've committed — the board is a comparison, not a verdict. If you noticed a thread they didn't, offer it after the board as "here's the one I'd have pulled," the way a colleague compares notes walking out of a meeting.

## Overtime

If the user wants to keep going, answer their question **as the world** rather than as a narrator.

- Reply as named people with jobs — a data scientist, an ops lead, a researcher. Short, in their voice, the way a Slack reply reads.
- **Let answers be inconclusive.** Real ones are. If every question advances the plot, the scenario becomes a puzzle with a solution, and puzzles have a right answer the user can miss.
- Volunteer the awkward limitation rather than hiding it. "That accuracy number is measured only on people who showed up. I have no ground truth on the ones who didn't."
- Never grade during overtime.

If the user wants to keep going past their two, let them. The two-and-two ask is a floor that gets them committed, not a cap on the conversation.

## Rotate the problem shape, not the industry

Settings are unlimited. Distinct problem shapes are maybe thirty or forty, and the shape is what the user is actually practicing. Serving the same shape in three different industries makes someone very good at one thing while feeling like general practice.

Track which shape was used and rotate deliberately:

- A system took over a human judgment; the target metric improved and the cost landed where the metric can't see it
- Two users share one interface and want opposite things
- The workaround is the spec — people built something on the side and it's better than the product
- Fixing the bottleneck just moved it downstream
- The thing that actually works isn't sanctioned
- Right diagnosis, wrong owner — you can't touch the part that's broken
- It only works at the good sites, and nobody's asking why
- The metric improved because the population changed, not the product
- Success at onboarding created a load nobody staffed for

## Failure modes to avoid

- **Serving the scenario and the board together.** The commitment has to happen first or there's no exercise.
- **Letting the constraint go unused.** If nothing in the scenario makes an obvious action hard, the constraint is decoration. It should change what the user can actually do, not just what they'd like to know.
- **Making the numbers all bad.** If nothing is working, the answer is obvious. There must be a real win to protect.
- **A constraint that's just an annoying person.** "The stakeholder is difficult" is not a constraint; "the threshold requires a state-by-state regulatory filing" is.
- **A flow with no branch.** A straight line has nothing to interrogate.
- **Grading.** The most common way this stops being fun.
- **Real companies with invented metrics.** Attaching made-up numbers to a real product is a factual claim about someone's software. Invent the company.

## Worked example

**Context** — A chain of pet urgent care clinics has a check-in app. You check in from your phone before driving over, pick your pet's symptoms from a list, and the app shows an urgency estimate.

**UX principle** — Urgency is judged by the clinic, never by the owner.

**The flow** — Pre-check-in → symptom picker (shows estimate) → *branch*: arrives and waits for tech triage, exam, discharge / never arrives, goes elsewhere.

**The numbers** — Your PM sends these over. She thinks the picker is working and the drop-off is a marketing problem. You're not sure.
- Time to exam for true emergencies is down 20%
- Among owners shown a low urgency estimate, the share who never arrive has roughly doubled
- Two of those pets turned up at a competitor's overnight ER the same week

**The constraint** — Legal has ruled the app can never state or imply a medical assessment. The estimate copy is locked behind a six-week review.

*Board:* Why are owners who see a low estimate not coming? · What do owners think the estimate means? · Which pets are bouncing — is it concentrated? · What are techs overriding, and on what signal? · Can owners say what's actually wrong? · Does the flow have to decide before anyone's been seen? **Dud:** "Should we rewrite the estimate copy?" — jumps to a fix, and the constraint already ruled it out.

The last one questions the flow itself, and it's the only one the constraint doesn't block. Questions about the shape of the flow are consistently underrated — surface them.
