---
name: design-warmup
description: Run a short design judgment exercise — serve an invented product scenario in one of two formats (find what doesn't add up, or pick from candidate moves), reveal a board of what the scenario was built around, then offer an extra-credit prompt to say it to the stakeholder. Use this whenever someone asks for a design warmup, a design exercise, a design challenge, a UX warm-up, a scenario to think through, wants to "stay sharp" as a designer, is preparing for design interviews, or asks for practice with product judgment, discovery, or problem framing. Also use it when someone asks for a new scenario, another round, or names format B or C.
---

# Design Warmup

A five-to-ten-minute exercise for practicing product judgment. No Figma, no deliverable, no wireframes. The user gets a short scenario and answers it in one of two formats. Then a board reveals what the scenario was built around, with any of theirs that hit marked, and the round ends with an optional extra credit: say it to the person in the room.

The skill it trains is the one that gets skipped: deciding what the problem actually is before solving anything, and then saying so to someone who reads it differently.

**It has to be a small puzzle, not homework.** An earlier version asked for two questions and two actions. It was engrossing and it was too much: composing four answers, each one squeezing past the constraint, took longer than a warmup should, and the user stopped opening it. Every rule below protects the 5–10 minute round.

## The two formats

Each round is served in one of two formats. **Pick at random** unless the user names one ("give me a B", "C please") or the history check says the last two rounds were the same format, in which case serve the other. Say which format it is in the first line of the round.

**Format B — Find it.** The user names the one thing in the scenario that doesn't add up, then gives one action based on what they found. The answer is a plant: the undefined metric, the arbitrary threshold, the dead-end branch, the population measured wrong. It has a clear finish line, and it trains noticing.

Ask line, exactly: **What's the one thing here that doesn't add up?** Then give one action you'd take, based on what you found.

**Format C — Pick, then write.** The user gets five shuffled candidate moves, picks the strongest, calls out the decoy, then adds one move of their own. It's recognition over recall: faster, and it trains weighing trade-offs between options already on the table. The move they write themselves is where the most interesting thinking usually shows up, so never drop it.

Ask line, exactly: **Pick the strongest, call the decoy, then add one move of your own.**

Both formats share the same scenario structure, the same board logic, the same three-part close and the same extra credit.

## The loop

1. Pick a scenario using "Picking a scenario" below: check what this user has been served recently, then compose a setting, problem shape and mode that differ from it. Pick the format.
2. Serve the scenario, **in the order of operations below**.
3. The user answers. Wait for them. Do not answer your own scenario.
4. Reveal the board, marking any of theirs that hit. Then the three-part close, then the extra-credit prompt.
5. If they take the extra credit, give short feedback on what they wrote (see "Extra credit").
6. Optional overtime: answer their questions in character as the world, and let them keep pulling.

### Order of operations when serving — no exceptions

1. Write the opening line naming the format and the time ("Format B, about 5 minutes. First instinct counts, and fragments are fine."), then the **Context** paragraph, as plain text. This is the first thing in the reply.
2. Write the **The flow** header.
3. Only now call any diagram tool (including any silent setup call it needs). No tool call of any kind happens before the Context text exists.
4. After the diagram renders, write the remaining fields in full: the timeframe section (one-line handover, two facts, then the colleague's reading), the constraint, the moves list (format C only), and the ask line.

The most common failure is opening with a tool call: the diagram lands at the top, Context never gets written, and the fields after the diagram get thinned out because the scenario already feels delivered. Before ending the turn, check that every field is present.

### Written first is not the same as seen first

What matters is the order the user *sees*, not the order you write. Some surfaces (the Claude app among them) fold any text written between tool calls into a collapsed work summary, so a Context paragraph written before the diagram call never appears and the diagram becomes the first visible thing. That is exactly the failure above, even though you followed steps 1–3.

- If the session has a tool for sending a visible message mid-turn (for example `SendUserMessage`), send the opening line, the **Context** paragraph and the **The flow** header through it, *then* make the diagram calls, then write the remaining fields as the final reply.
- If any other tool work happens before or after serving (loading the skill, reading references, searching history), finish all of it first. Serving starts only when no tool call remains except the diagram.
- If you can't tell whether pre-tool text will show, assume it won't and use the visible-message tool.
- If no such tool exists and the surface collapses pre-tool text, put Context as the first line of the final reply, directly above the remaining fields, rather than skipping it.

A quick check before ending the turn: scroll the reply as the user will see it. The first thing on screen must be the format line and then **Context**.

## Scenario modes — rotate these

Three modes, independent of the format. Rotate deliberately; running only the first makes every answer "go do research," which is the most common way this exercise goes stale.

**Discovery.** Unexplained numbers, no research done yet. Actions are about what to learn and from whom. The default, and the one to stop over-serving.

**Interpretation.** The research is already in and you hand it over — exit interviews, session recordings, a survey. Two readings fit the same evidence and imply opposite products. **The constraint must close the research door**, not narrow it: "you present Friday," "the panel already ran and won't run again this quarter."

**Commitment.** The decision is already made and announced. The user shapes how it lands, not whether it happens. This kills research as an escape entirely and tests whether they can do good work inside someone else's call.

Format C pairs especially well with interpretation and commitment, where the candidate moves can all be real moves. Format B works in every mode; in discovery mode, its one action may legitimately be a targeted piece of learning, as long as it follows from the find.

## Serving the scenario — use this exact structure

```
[Format line: "Format B, about 5 minutes. First instinct counts, and fragments are fine."
 or "Format C, about 5 minutes. Pick the strongest move, call out the decoy, then add one of your own."]

**Context**
[Two or three lines: what the product is, who uses it, how it works.]

**The flow**
[Diagram.]

**[Timeframe — "Tuesday", "What's already known", "The decision, already made"]**
[One line on who handed this over. Then two facts. Then what they think the facts mean, and what they want to do.]

**The constraint**
[One or two lines. Structural.]

**The moves**            ← format C only
- **A.** …
- **B.** …
- **C.** …
- **D.** …
- **E.** …

[Ask line for the format, exactly as written above.]
```

Then stop and wait. Do not answer your own scenario.

**Write the Context paragraph before you draw anything** (see Order of operations above). Never open with the diagram.

## Building a scenario

Everything must earn its place by changing how the user reasons. Cut anything that is only flavor.

**Context** — two or three lines. What the product is, who uses it, how it helps. Industry folds in here. Never use a real company; invent one or leave it unnamed.

**The principle — built in, not served.** Choose one UX principle the scenario is quietly violating ("urgency is judged by the clinic, never by the owner") and build the plant around it. It no longer gets its own field; a stated principle hands the user half the answer and costs reading time. It usually surfaces in the named pattern at the close.

**The flow** — a diagram, not prose. See below.

**The numbers** — **two facts**. This is read on a phone with nothing to write on, and a round meant to take five minutes can't carry three or four data points. The two must pull against each other: a real win *and* a real cost. "Throughput up 12%, complaints up too." Usually one of the two is where the plant lives — in format B, it's often the fact the find depends on.

**The colleague's reading** — what they think the facts mean, plus the fix they want. That fix is the decoy.

**The constraint** — a structural obstacle, not a difficult stakeholder. A frozen budget, a locked legal review, a threshold owned by another department or a vendor, an agreement that can't change until renewal. It should block the obvious fix and force the good move sideways.

### Do not include

- **Scale.** Assume the product has users. If scale genuinely changes the answer, fold it into a sentence.
- **The user's title or seniority.** Level doesn't change the exercise. *Permission* does — and permission belongs in the constraint.
- **A third fact.** If the scenario needs one to work, the plant is in the wrong place. Move it into the flow or the colleague's reading.

### Plant the find on purpose

Every scenario has one primary plant, and in format B finding it *is* the round. In format C the plant is what makes the keystone move the keystone.

- A metric named but never defined. "Dwell time hasn't moved in eighteen months." Started when? Nobody said.
- A threshold with no stated basis, sitting visibly in the flow.
- A population measured wrong: a rate computed only on the people who made it through.
- An input the user supplies that also decides their route.
- A step whose logic doesn't follow from the one before it, or a branch with no way out.

**Findable in one read.** The plant has to be discoverable from what's on screen, without arithmetic and without outside knowledge. If it takes a second pass to see, it's too buried for a five-minute round.

**Undefined, not incorrect.** A wrong fact makes the user distrust every other fact, and they stop reasoning and start proofreading. Gaps produce the same head-scratch with none of that cost. If a user points at a gap, confirm it plainly — and if they catch something that was sloppy rather than planted, say that too.

### Building the five moves (format C)

Five candidates, shuffled so the keystone isn't reliably first or last. One line each, written as something the user could actually propose:

- **The keystone** — the move that gets past the constraint and fixes what the plant reveals.
- **A strong second** — a real move that helps, but less, or later.
- **The decoy** — the colleague's proposed fix, worded neutrally. Never mark it or make it sound dumb.
- **The tempting obvious** — a reasonable-sounding move that treats a symptom (a reminder, a tooltip, more copy).
- **The escape hatch** — a study or survey. In interpretation and commitment modes the constraint should make this visibly weak.

Every candidate must be plausible to a working designer. If the keystone is obvious at a glance, the other four are too weak; rewrite them before serving.

### Never state the problem

Nobody hands a designer a framed problem. They hand you numbers and somebody's opinion about what the numbers mean, and figuring out what's actually wrong is the job. Give the user a seat at the table and a colleague with a position — never a problem statement.

- Wrong: "The team's OKR is to reduce time-to-exam." Now everyone optimizes the same thing.
- Wrong: "This landed on your desk Monday." No one is attached to it; it reads as a slide.
- Right: "Your PM sends these over." Then the two facts. Then: "She thinks the picker is working and the drop-off is a marketing problem."

A named person with a stated position gives the user something to disagree with — and gives the extra credit someone to talk to.

**Facts before readings.** The handover line names who sent it and nothing else; the colleague's interpretation comes after the numbers, never before. Numbers first lets the user form their own impression, then meet the position they're being asked to agree or disagree with.

## The flow diagram

Not decoration. It is the thing the user points at, and a flow you can see is a flow you can poke holes in. In format B it is very often where the find lives.

- Show the real path end to end, **including the branch where people fall out**.
- Put decision points in the flow with **thresholds visible** — "Estimate under $1,500?" with both paths drawn. A threshold is a design decision sitting in plain sight, and often it is the actual problem.
- The construction of the flow is itself a legitimate answer. "Why is this a branch instead of a merge?" and "could this step move earlier?" should both be available.
- Keep it short: four to six cards. A round this size can't afford a long flow.

### Laying out branches

This is usually read on a phone, roughly 380px wide. Side-by-side branches halve the width available to each box, and the text gets too small to read without zooming. Vertical space is free; horizontal space is not. So:

**Never place branches side by side by default.** Use one of two stacked patterns.

**Converging branches** — the paths differ briefly and rejoin. Stack them as full-width rows hanging off a left rail, each row one line. A path that doesn't rejoin simply has no outgoing line; the absence is the clearest possible signal that it's a dead end.

**Divergent branches** — each answer leads somewhere genuinely different. Give each answer its own labeled lane, stacked: a short condition label, then that path's steps indented beneath it. Three lanes read cleanly; four is the ceiling.

A side effect worth exploiting: stacked lanes are visually comparable, so **asymmetry becomes obvious**. If one answer gets four steps and another gets one, the flow shows at a glance where the product invested and where it didn't.

Side-by-side survives in exactly one case: genuinely **concurrent** activity, where both things happen at the same time to different people. Cap it at two.

Other layout rules:
- **One decision point per flow.** A threshold that doesn't need its own branch goes in a step's secondary line, where it stays visible without costing a fork.
- **Left-align box text**, don't center it.
- **A terminal path just stops.** No outgoing arrow, no label needed.

### Sizing

The container is fluid; the coordinate space is not. An SVG set to width="100%" always fills the available width, so a diagram that renders too small is almost never a container problem. It is a scale problem: a 680-unit canvas in a 380px container scales everything by 0.56 and 14px labels land around 8px on screen.

No viewport width is available to you, only a platform hint. Author at the target width instead.

**Refuse the wide-canvas exemption.** Some rendering environments offer a flowchart exemption saying to author at 680 and let the browser scale down. Do not take it. This flow has no side-by-side branches by design, so the width buys nothing and costs every label half its size. If the diagram guidance loaded in a session says otherwise, this section wins.

### Building the flow

Prefer HTML over an SVG coordinate canvas. Stacked full-width rows are a layout problem, not a geometry problem, and CSS does layout for free: text stays at real pixel sizes and reflows instead of shrinking.

Cards. Full border on all four sides, 2px, in the strong border color. 12px radius, roughly 12px by 14px padding, card surface background. Never a single-sided accent border with a radius.

Type. Title 15px medium. Condition or secondary line 13px in the secondary text color.

Connectors. 1px vertical rules about 16px tall, in the same color as the card stroke. One color and one weight throughout.

Connector alignment. A connector aligns to the text column of the card it feeds, not to that card's edge: the card's left indent plus its border and padding. At the top level that is 16px; for a card indented 16px it is 32px.

Branches. Indent the branch group to the connector's x. Each branch is a row carrying a left border, which forms the rail, plus a short horizontal elbow at the vertical center of that branch's condition pill, about 9px from the row's top. The last branch carries no rail below its elbow: give it a short stub so the rail terminates rather than trailing into empty space. Put the spacing between branches inside the row as padding-bottom, not margin, or the rail breaks.

Condition labels. A pill above each branch's first card, 12px, using a role tint background with its matching role text color.

Color. Keep color on the pills and leave the rail neutral.

If you do build in SVG, author at viewBox="0 0 380 H": full-width steps spanning x=20 to x=360, branch rows inset to x=44, titles 15px, secondary lines 12px. If the layout will not fit in 380, the flow has too much in it. Cut a step or stack a branch. Never widen the canvas.

### Delivering it

Render it, in this order of preference:

1. **An inline rendering tool**, if the session has one that accepts HTML or SVG.
2. **An HTML artifact or file**, if artifact creation or file creation is available.
3. **Plain text with arrows and indented branches** — only if neither of the above exists. Say so in one short line, and keep the branches and thresholds intact.

Do not reach for the text version because it is quicker.

## The board

The board shows what the scenario was built around, ordered by what each entry unlocks given the constraint. Slot 1 in each group is the keystone. Number the slots.

**Format B board — two groups:**
- **What doesn't add up** — four finds, ordered. Slot 1 is the primary plant. Then the decoy, set apart below the four.
- **Actions** — four moves, ordered. Slot 1 is the keystone action.

**Format C board — one group:** the five candidates, re-ordered by what they unlock and kept with their letters ("C. Offer late spots as a claim"). The decoy goes last, set apart, marked ×. The user's own move goes in at the rank it earns, marked +.

**Build-time check:** if you can't fill four distinct actions for B, or five plausible candidates for C, the scenario is underspecified. Give it more before serving. And if every action is a study, it's a discovery scenario whether you meant it or not.

**Say what the board is, at the reveal.** One line: "Here's the board. These are the plants the scenario was built around, in order of what they unlock." Not crowd data, not the best answers a designer could give. Being upfront about that tells the user what a miss means: not a failure to think well, just a plant they didn't spot.

This construction is circular, and the rules below keep it honest.

- The user is never scored. Hitting any slot is a hit; hitting none is not a failure.
- **The decoy** is the move a stakeholder in the scenario has already endorsed. It isn't a dumb idea; it's a borrowed one. Say in one clause what in the evidence or the constraint undercuts it, pointing at the scenario, never at the user. In format C, calling the decoy correctly is itself a hit — mark it. In format B, quietly sidestepping it is worth naming in the close.
- **If an answer of theirs isn't on the board and it's good, add it and say so.** A board can only contain what its author thought of, so a genuinely novel angle would otherwise read as a miss. This is the release valve.
- **The decoy belongs in the solo version only.** If boards are ever built from other people's public answers, drop it.

### Delivering the board

**Render the board visually, on the same ladder as the flow.** A board delivered as a prose list falls flat: the whole point is that a hit is visible at a glance.

- **Every entry** carries its slot number in muted text on the left; the decoy carries ×; an added entry carries +.
- **A hit** — accent tint background, accent border, plus a caption beneath in the accent text color naming which answer landed ("your find", "your pick", "your action"). Four words, not a sentence.
- **A miss** — neutral card surface, standard border. No marking.
- **The decoy** — danger tint background and border, set slightly apart, with a one-clause reason beneath it in the danger text color. If the user called it in format C, also add the hit caption ("your decoy call").
- **An added entry** — accent tint like a hit, captioned "added to the board".

Same card spec as the flow: 2px border all round, 12px radius, roughly 12px by 14px padding, title 15px, caption 13px. Cards stacked full width, left-aligned text. Group labels in 13px secondary text.

### Keep it short

- **Each board entry is one line.** Around a dozen words.
- **Captions are four words**, not sentences.
- **After the board, exactly the three-part close, then the extra-credit prompt.** Nothing else.
- **Never re-explain the scenario.** They just read it.

## The close — three parts, this format

Each part is a bold lead, then one or two sentences. Keep the whole close to about one phone screen.

**1. Your hit.** Lead: **Your hit: [which answer].** (or **Your hits: …**). Name their strongest answer that landed and say in one clause *why it mattered*: the plant it found, the principle it tested, the assumption it refused.
- If their answer landed on the board as a new entry, say so plainly: "Good one, and not one the scenario planted. Added to the board." Then one clause on what it opens up.
- If nothing hit, lead with **Closest to the board: [their answer].** Say what it was reaching toward, without framing it as a miss.
- If their action bumps into the constraint, add one short practical note ("that changes how the waitlist is ordered, which is the vendor's — it's a next-term move"). One sentence, never a critique.

**2. The top slot you didn't get.** Lead with what it is and its slot: **Find I'd have added (#1):**, **Action I'd have taken (#1):**, or **Move I'd have picked (#2):**. Then the exact wording in quotes. Then **Why:** one or two sentences on what it unlocks *given the constraint*.
- Use the highest-ranked slot they missed. If they hit the keystone, use the next one down and label it.

**3. The named pattern.** Lead: the pattern name in bold, then how to spot it next time. Two sentences.

> **A queue stores stale intent.** A line records what people wanted when they joined, and that goes out of date. When a line moves slowly, check whether it's full of people who already got what they came for, and give them a cheap way to leave.

Name the pattern whether or not the user found it. Scenario facts expire; a named pattern travels.

## Extra credit — say it to the room

After the close, every round ends with one extra-credit prompt. It's a communication rep, not more analysis: the user has worked out the problem, and now they have to say it to someone who reads it differently. It is optional and it is meant to feel a little uncomfortable.

**The prompt.** One line, bold lead, aimed at the scenario's stakeholder by role and at the scenario's moment:

> **Extra credit:** Write the two sentences you'd say to the dean on Thursday that tell her the 6-hour window is the wrong fix without making her feel wrong.

- Always name the person and the occasion from the scenario ("the claims director in Monday's review", "your ops lead before Thursday").
- Always name the tension: what they have to say no to, and what they have to protect (her standing, the team's win, the relationship).
- Two or three sentences. Never a memo, never a deck.

**When they write it,** reply in this shape, short:

1. One line on what works and why — the move it makes ("It opens with her own data and turns the fix into a question, so she can agree without backing down").
2. **The catch**, if there is one — the thing a sharp stakeholder would notice first. Accuracy comes first: an overstated number, a percentage applied to the wrong population, a claim the scenario doesn't support. Then tone: blame, hedging, jargon, or a question that's really an accusation. One catch, maybe two. Never a list.
3. **A tightened version**, in quotes, keeping their idea and their voice. Fix the catch; don't rewrite their argument into yours.
4. Optionally, one more sentence they could have ready if the stakeholder pushes back.

Don't grade it and don't ask for a second draft. If they want to try again, they'll say so.

If they skip the extra credit, let it go. Don't mention it again that round.

## Never grade

Do not critique the user's answers after they've committed — the board is a comparison, not a verdict. Threads they didn't pull go in part 2 of the close, labeled and quoted, the way a colleague compares notes walking out of a meeting. The extra-credit feedback is the one exception, because the user asked for it by writing it — and even there it's one catch and a better version, not a score.

## Overtime

If the user wants to keep going, answer their question **as the world** rather than as a narrator.

- Reply as named people with jobs — a data scientist, an ops lead, a researcher. Short, in their voice, the way a Slack reply reads.
- **Let answers be inconclusive.** Real ones are.
- Volunteer the awkward limitation rather than hiding it. "That number is measured only on people who showed up."
- Never grade during overtime.

## Picking a scenario — variety rules

The scenario is built from three independent axes, picked separately, plus the format:

- **Setting** — the product and industry. `references/variety.md` holds a pool of 60.
- **Problem shape** — what is actually wrong underneath. `references/variety.md` holds 23. This is what the user is practicing, so it matters most.
- **Mode** — discovery, interpretation or commitment.
- **Format** — B or C, at random (see "The two formats").

### Step 1 — check what this user has already seen

You carry nothing between sessions, but some surfaces can search past chats. If a past-chat search tool exists (for example `conversation_search` or `recent_chats`), use it before picking:

- Search for the ask lines: `"doesn't add up"` and `"call the decoy"`, and if useful `"two actions you'd take"` for older rounds. One or two searches, at most two chats opened. Don't page through history.
- From the hits, note the **setting, shape, mode and format** of each round in roughly the last 30 days.
- Avoid every setting from that list, avoid the shapes of the last five rounds, use a different mode from the most recent round, and don't serve the same format three times running.

This is read-only. Do not write a log to the user's memory unless they ask you to.

Within one conversation, never repeat a setting or shape already served in it, and rotate the mode each round.

### Step 2 — compose

**With history**, pick any setting, shape and mode that pass the avoid-lists, favoring modes and shapes that have been served least.

**Without history**, pick by date so consecutive days differ. Let *N* be today's day of the year (1–366), from context or a time tool:
- Setting: entry `((N × 7) mod 60) + 1` in the settings pool.
- Shape: entry `((N × 5) mod 23) + 1` in the shapes list.
- Mode: `N mod 3` → 0 discovery, 1 interpretation, 2 commitment.
- If the setting and shape don't fit naturally, take the next shape down the list (wrapping) until one does. Never bend the setting into a cartoon to force a shape.
- Asked for another round in the same conversation → step every index forward by one, skipping anything already served here.

**If the user names an industry**, use it as the setting and still pick the shape and mode by the rules above.

### Step 3 — make the surface new

Invent the company name, the people, the figures and every sentence fresh. Nothing is copied from a reference file, including phrasing.

**Never serve the examples the user has already read.** Pet urgent care check-in (the worked example in this file), home-showing requests (the original bank) and course-section waitlists (the README example) are off the table as settings. If a pick lands on one, move to the next setting.

### The seed bank is a pattern library, not a menu

`references/scenarios.md` holds 30 worked seeds. Read it to see how a shape turns into a plant, a keystone question and action, and a named pattern. The seeds list three facts; serve the two that pull hardest against each other. A seed's plant and Q1 become format B's primary find; its A1 becomes the keystone action, or the keystone candidate in format C. Don't serve a seed as written: change the colleague, the constraint, the mode if possible, and every name and figure.

### Rotate the problem shape, not the industry

Settings are unlimited. Distinct problem shapes are maybe thirty or forty, and the shape is what the user is actually practicing. When the history check and the date pick disagree, protect shape variety first, then mode, then setting.

## Failure modes to avoid

- **Making it homework again.** More than two facts, a long flow, a hard-to-see plant, or a fat close all push the round past ten minutes. That is the failure that made the user stop using this skill.
- **Opening with the diagram.** Context text comes first, always, and must be seen first.
- **Repeating a scenario.** Run the history check when the tools exist, compose from the axes, and never serve the worked examples or a seed as written.
- **A plant you can't find in one read.** Format B depends on it.
- **A weak field of candidates.** In format C, if four of the five are obviously bad, the pick is free and nothing gets weighed.
- **Dropping the user's own move** in format C, or the action in format B. That's where they generate rather than recognize.
- **Skipping the extra credit**, or turning its feedback into a critique.
- **A vague close.** Part 2 always says find, action or move, quotes the exact wording, and says why.
- **Serving the scenario and the board together.** The commitment has to happen first.
- **Letting the constraint go unused.** It should change what the user can actually do.
- **Making the numbers all bad.** There must be a real win to protect.
- **A constraint that's just an annoying person.**
- **A flow with no branch.** A straight line has nothing to interrogate.
- **Grading.** The most common way this stops being fun.
- **Real companies with invented metrics.** Invent the company.

## Worked examples

Never served. They show the shape of each format.

### Format B

**Context** — A chain of pet urgent care clinics has a check-in app. You check in from your phone before driving over, pick your pet's symptoms from a list, and the app shows an urgency estimate.

**The flow** — Pre-check-in → symptom picker (shows estimate) → *branch*: arrives and waits for tech triage, exam, discharge / never arrives.

**Tuesday** — Your PM sends these over.
- Time to exam for true emergencies is down 20%.
- Among owners shown a low urgency estimate, the share who never arrive has roughly doubled.

She thinks the picker is working and the drop-off is a marketing problem. She wants a "we're here for you" campaign.

**The constraint** — Legal has ruled the app can never state or imply a medical assessment. The estimate copy is locked behind a six-week review.

**What's the one thing here that doesn't add up?** Then give one action you'd take, based on what you found.

*Board.* Finds: 1 the app gives an urgency verdict before anyone has seen the pet · 2 the drop-off is concentrated where the estimate is low · 3 the 20% win is measured only on pets that arrived · 4 legal's rule and the estimate contradict each other. **Decoy:** the marketing campaign — the drop-off sits exactly where the estimate is low. Actions: 1 show what happens after you arrive instead of an urgency estimate · 2 take the estimate out of the flow until legal's review · 3 have techs log what low-estimate no-shows had · 4 call a week of no-shows.

*Extra credit.* "Write the two sentences you'd say to your PM before she briefs marketing, telling her the drop-off isn't a reach problem without killing her campaign."

### Format C

Same scenario, with **The moves**:
- **A.** Add a line under the estimate: "Not sure? Come in anyway."
- **B.** Launch the "we're here for you" campaign.
- **C.** Replace the estimate with what happens after you arrive: triage, wait, exam.
- **D.** Send a follow-up text to owners who checked in but didn't arrive.
- **E.** Survey owners about the estimate.

**Pick the strongest, call the decoy, then add one move of your own.**

*Board.* 1 C (removes the assessment rather than rewording it, so it clears legal) · 2 D · 3 A (touches locked copy) · 4 E · × B — the drop-off is where the estimate is low, not where reach is.

*Close pattern.* **A rating is read as a verdict.** When an app shows a score before a professional has looked, people act on it as if it were the professional's call. To spot it, ask what a user would do differently if the number were hidden.
