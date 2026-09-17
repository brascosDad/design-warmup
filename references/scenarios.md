# Scenario bank — 30 seeds

One seed per day of the month. Each is a skeleton: build the full scenario from it (five fields, flow, full board) following SKILL.md. All companies and people are invented. Rename them and change the figures every time you serve a seed.

Modes: **D** discovery · **I** interpretation (research is in; the constraint closes the research door) · **C** commitment (the decision is made and announced).

Each seed lists: product · mode · shape · colleague and their reading · three facts (at least one real win) · constraint · the planted gap · keystone question (Q1) · keystone action (A1) · pattern.

---

### 1. Showing requests (real estate)
- **Product:** Home-search app; buyers book showings from a listing calendar, listing agent confirms within two hours. · **I** · Approval in the wrong place
- **Colleague:** PM thinks agents are slow and wants auto-confirm; the researcher thinks agents hold on purpose.
- **Facts:** self-booked showings up 40%; 31% of requests expire, mostly on listings above $600K; 9 of 12 agents wait to check with the seller.
- **Constraint:** partner brokerages won't do research until spring; you present Thursday.
- **Plant:** the two-hour window has no stated basis; "open" slots were never seller-approved.
- **Q1:** Who sets the open slots, and has the seller agreed to them? · **A1:** Move seller sign-off to when the calendar is published.
- **Pattern:** The approval is in the wrong place.

### 2. Self-checkout weight alerts (grocery POS)
- **Product:** Self-checkout lanes that pause and call an attendant when bagged weight doesn't match. · **D** · A system took over human judgment
- **Colleague:** Loss-prevention lead says shrink is down, so the tighter tolerance is working.
- **Facts:** shrink down 18%; attendant calls per lane doubled; average basket size at self-checkout down 22%.
- **Constraint:** weight tolerance lives in the scale vendor's firmware; no changes this fiscal year.
- **Plant:** basket size is measured only on completed self-checkout transactions.
- **Q1:** Who stopped using self-checkout, and which lane did they move to? · **A1:** Watch a full-lane shift and log every attendant call by cause.
- **Pattern:** The cost landed where the metric can't see.

### 3. Maintenance requests (property management)
- **Product:** Tenant portal for repair tickets; a vendor gets dispatched by category. · **C** · Self-serve moved the work, not removed it
- **Colleague:** Ops director announced the phone line closes January 1; says the portal makes tenants self-sufficient.
- **Facts:** portal tickets up 60%; phone calls down 45%; repeat tickets for the same issue up 30%.
- **Constraint:** dispatch software accepts one category per ticket; owned by the vendor.
- **Plant:** "repeat ticket" never defined (same unit? same issue? within how long?).
- **Q1:** What did phone dispatchers ask before they filed a ticket? · **A1:** Put the dispatcher's clarifying questions into the portal before submit.
- **Pattern:** Self-serve moves the work; find out where it went.

### 4. School bus tracker (K-12)
- **Product:** Parent app showing live bus location and arrival times. · **D** · The metric improved because the population changed
- **Colleague:** Transportation manager credits the app for the on-time improvement.
- **Facts:** app rating up to 4.6; on-time rate up 12% since stops were consolidated; ridership down 9%.
- **Constraint:** routes are set by the bus contractor through June.
- **Plant:** "on-time" isn't defined — at the stop, or at school?
- **Q1:** Who stopped riding when the stops moved? · **A1:** Map former riders' addresses against the new stops.
- **Pattern:** The population changed, not the product.

### 5. Mobile check deposit (credit union)
- **Product:** Photo check deposit with a $2,500 per-check limit. · **I** · A threshold nobody can explain
- **Colleague:** Product lead reads support transcripts as "the limit is too low"; the support lead reads them as "members don't understand holds."
- **Facts:** mobile deposits up 25%; 1 in 5 checks above $2,500 are split across several deposits; branch visits for large checks flat.
- **Constraint:** the limit is set by the risk committee, reviewed in March; you present Monday.
- **Plant:** the $2,500 figure has no stated basis.
- **Q1:** Are members splitting to get around the limit, or around the hold? · **A1:** Show the hold date on the deposit screen before submit.
- **Pattern:** A threshold nobody can explain is a design decision nobody owns.

### 6. Digital discharge instructions (hospital)
- **Product:** Patients get discharge instructions and a question button in an app instead of on paper. · **C** · Success created a load nobody staffed
- **Colleague:** CNO announced all units go digital next month, citing satisfaction scores.
- **Facts:** patient satisfaction with discharge up 15 points; message volume to nurses tripled; average reply time 19 hours.
- **Constraint:** nurse staffing ratios are fixed by contract through next year.
- **Plant:** the 19-hour average — measured on which messages?
- **Q1:** What are patients asking that the instructions didn't answer? · **A1:** Route questions by type so pharmacy and scheduling take their share.
- **Pattern:** Success made a job nobody owns.

### 7. Desk booking (coworking)
- **Product:** Members book hot desks; a booking auto-releases 15 minutes after start if nobody badges in. · **D** · Two users share one interface and want opposite things
- **Colleague:** Community manager says ghost bookings are members gaming the system.
- **Facts:** occupancy up 20%; complaints about "no desks" up; 1 in 4 bookings auto-released.
- **Constraint:** badge-reader data can't be joined to bookings until the vendor upgrade in Q3.
- **Plant:** why 15 minutes?
- **Q1:** Who are the auto-released members, and what were they doing at minute 16? · **A1:** Let members extend the hold from their phone.
- **Pattern:** Two users, one screen: whose clock does it run on?

### 8. Volunteer shifts (food bank)
- **Product:** Volunteer shift signup app for a regional food bank. · **I** · The workaround is the spec
- **Colleague:** Volunteer director reads the survey as "people love the app"; the shift leads say they couldn't run a Saturday without their group chat.
- **Facts:** signups up 35%; no-show rate unchanged at 20%; shift leads fill gaps same-morning via a group chat.
- **Constraint:** no dev budget until the spring grant; board meeting Tuesday.
- **Plant:** "no-show" is counted how — didn't arrive, or arrived late?
- **Q1:** What does the group chat do that the app doesn't? · **A1:** Make the group chat official and link it from the shift page.
- **Pattern:** The workaround is the spec.

### 9. Auto-rebooking (airline)
- **Product:** When a flight is cancelled, the app auto-rebooks travelers onto the next available flight. · **C** · A default is doing the deciding
- **Colleague:** VP of customer care announced auto-rebook as the default for all cancellations.
- **Facts:** call volume down 35%; 80% keep the new booking; complaints from travelers moved to next-day flights when a same-day partner flight existed.
- **Constraint:** partner airline inventory isn't available by API until the contract renews next year.
- **Plant:** "keep the new booking" — measured how, and when?
- **Q1:** What would travelers have picked if they'd been asked? · **A1:** Show "we booked you on X — reply to request a same-day partner flight" instead of a silent confirmation.
- **Pattern:** A default is a decision someone else made for you.

### 10. Class waitlists (fitness studios)
- **Product:** Waitlisted members are auto-promoted into class up to two hours before start. · **D** · Fixing the bottleneck moved it
- **Colleague:** Franchise ops lead points at record class fill.
- **Facts:** fill rate up to 96%; late-cancel fees up 50%; front-desk fee disputes doubled.
- **Constraint:** the fee policy is set by franchise HQ.
- **Plant:** the two-hour promotion cutoff and the late-cancel window may not match.
- **Q1:** How many fees go to members who were promoted without seeing it? · **A1:** Require a one-tap accept before a promotion counts.
- **Pattern:** The bottleneck moved downstream.

### 11. Holds lockers (public library)
- **Product:** Patrons pick up held books from self-service lockers. · **D** · It only works at the good sites
- **Colleague:** Library director wants lockers at every branch.
- **Facts:** holds up 25%; pickup rate 95% at three branches, 60% at four others; expired holds up overall.
- **Constraint:** locker placement is fixed by the vendor lease for three years.
- **Plant:** the three good branches aren't named — what do they have in common?
- **Q1:** What is different about the branches where it works? · **A1:** Spend a day at a good branch and a weak one, same hours.
- **Pattern:** It only works at the good sites, and nobody asked why.

### 12. Video inspections (car service)
- **Product:** Technicians send customers a video of recommended repairs to approve by text. · **I** · Right diagnosis, wrong owner
- **Colleague:** Service manager reads call recordings as "advisors aren't following up"; the dealer's consultant reads them as "techs over-recommend."
- **Facts:** repair approvals up 22%; 1 in 8 approved repairs are declined at pickup; average ticket up $140.
- **Constraint:** tech pay is flat-rate by repair, set by the dealer principal; you present Friday.
- **Plant:** "declined at pickup" — after work was done, or before?
- **Q1:** What changes the customer's mind between approving and paying? · **A1:** Add the total and the time estimate to the video approval.
- **Pattern:** Right diagnosis, wrong owner: you can't touch the part that's broken.

### 13. Residential permits (city government)
- **Product:** Online portal for fence and deck permits. · **C** · The thing that works isn't sanctioned
- **Colleague:** City manager announced the walk-in counter closes in 60 days.
- **Facts:** online applications up 50%; rejections for incomplete forms up 30%; clerks quietly pre-review drafts people email them.
- **Constraint:** state law fixes the application form's content.
- **Plant:** "incomplete" isn't defined — missing a field, or missing a drawing?
- **Q1:** What do clerks catch in those emailed drafts? · **A1:** Make the pre-review official: a draft upload a clerk checks before submit.
- **Pattern:** The thing that works isn't sanctioned.

### 14. Buy online, pick up in store (retail)
- **Product:** "Ready in 2 hours" pickup promise for online orders. · **D** · The metric counts the claim, not the outcome
- **Colleague:** E-commerce lead shows 97% on-time "ready" notices.
- **Facts:** pickup orders up 45%; ready notices on time 97%; 1 in 6 customers arrive to find the item isn't at the counter.
- **Constraint:** store inventory syncs nightly; merchandising owns that system.
- **Plant:** "ready" means the picker tapped a button.
- **Q1:** What does "ready" actually mean in the system? · **A1:** Stand at a pickup counter for a Saturday and log every miss.
- **Pattern:** The metric counts the claim, not the outcome.

### 15. Outage map (electric utility)
- **Product:** Public map of outages with an estimated restoration time. · **I** · An estimate became a promise
- **Colleague:** Comms lead reads social posts as "we need more updates"; the field ops lead reads them as "stop showing times we can't hit."
- **Facts:** map views up 3x; outage calls down 20%; complaints spike whenever an estimate slips.
- **Constraint:** estimates come from the field crew system, owned by operations; board briefing Friday.
- **Plant:** how often do estimates slip? Nobody has said.
- **Q1:** What do customers do on the strength of the estimate? · **A1:** Show a range and a confidence level instead of a single time.
- **Pattern:** An estimate gets read as a promise.

### 16. Furniture delivery (resale marketplace)
- **Product:** Buyers book a courier to collect used furniture from a seller. · **D** · Two users, opposite wants
- **Colleague:** Marketplace lead says sellers are flaky.
- **Facts:** completed sales up 30%; 1 in 5 pickups rescheduled; most reschedules are evening slots booked by buyers.
- **Constraint:** courier windows are fixed by the logistics partner.
- **Plant:** who initiates the reschedule is never stated.
- **Q1:** Does the seller see or approve the pickup window before it's booked? · **A1:** Have sellers set pickup windows when they list.
- **Pattern:** Two users, one calendar: whose time is it?

### 17. Course drops (university)
- **Product:** Students drop courses online; the advisor sign-off was removed. · **C** · Friction was doing a job
- **Colleague:** Registrar announced self-serve drops for all students this term.
- **Facts:** drops processed same day; drops up 30%; financial aid problems from dropping below full-time found weeks later.
- **Constraint:** aid eligibility rules are federal.
- **Plant:** "weeks later" — found by whom?
- **Q1:** What did advisors check during the sign-off? · **A1:** Show the aid impact on the drop screen before confirm.
- **Pattern:** The friction was doing a job.

### 18. Mobile check-in and digital key (hotel)
- **Product:** Guests check in on their phone and use it as a room key. · **D** · The average hides two groups
- **Colleague:** GM says check-in is solved; the average time is down by half.
- **Facts:** average check-in time down 50%; key failures concentrated in the older wing; the 4pm front-desk line is unchanged.
- **Constraint:** lock hardware replacement is budgeted for two years out.
- **Plant:** the average mixes app users and desk users.
- **Q1:** Who is still in the 4pm line, and why? · **A1:** Assign app users to the new wing at booking.
- **Pattern:** The average hides two groups.

### 19. Daily site logs (construction)
- **Product:** Subcontractors submit a daily log from the job site. · **I** · A proxy became the goal
- **Colleague:** Project exec reads site visits as "compliance is great"; the site superintendent reads them as "the logs are copy-paste."
- **Facts:** on-time submission 98%; 40% of logs near-identical to the day before; two delays last month weren't in any log.
- **Constraint:** the lender requires the current log format; you present Wednesday.
- **Plant:** "on-time" means submitted by 6pm, whatever the content.
- **Q1:** Who reads the logs, and for what? · **A1:** Ask for one required change-from-yesterday field.
- **Pattern:** A proxy became the goal.

### 20. Pay-by-plate parking (city)
- **Product:** Drivers pay for street parking in an app by plate number. · **C** · The only door is one some people can't use
- **Colleague:** Parking director announced meters come out in January.
- **Facts:** 70% of payments already in-app; citations up among out-of-town plates; a 10-minute grace period applies to app payments only.
- **Constraint:** citation rules are set by city ordinance.
- **Plant:** why is the grace period app-only?
- **Q1:** Who can't pay in the app, and what do they do now? · **A1:** Put a text-to-pay number on every sign.
- **Pattern:** When there's one door, check who can't use it.

### 21. Substitutions (grocery delivery)
- **Product:** Shoppers substitute out-of-stock items; "allow substitutions" is on by default. · **D** · A preference captured too coarsely
- **Colleague:** Fulfillment lead celebrates the record fill rate.
- **Facts:** fill rate up to 98%; refunds for substitutions up 40%; ratings flat.
- **Constraint:** the shopper app is built by a third party; no changes until spring.
- **Plant:** refunds are counted per item, not per order.
- **Q1:** Which substitutions get refunded, and what do they have in common? · **A1:** Let customers mark "no substitutes" on specific items.
- **Pattern:** One switch can't hold a preference that varies by item.

### 22. Parent messaging (childcare centers)
- **Product:** Parents message teachers through the center's app. · **I** · Two populations, one number
- **Colleague:** Franchise marketing reads the survey as "messaging drives satisfaction"; the regional director reads it as "happy parents message more."
- **Facts:** parents who message rate the center 30 points higher; 45% of parents never message; teachers spend 40 minutes a day replying.
- **Constraint:** no new survey until spring; owners' meeting Monday.
- **Plant:** who received the survey?
- **Q1:** Did messaging make parents happier, or do happier parents message? · **A1:** Present both readings with what each would build.
- **Pattern:** Two populations, one number.

### 23. Applicant screening score (apartment leasing)
- **Product:** Leasing software scores rental applications; agents must follow the score. · **C** · A system took over human judgment
- **Colleague:** Regional VP announced the score is binding next quarter.
- **Facts:** time to lease down 5 days; appeals up 3x; 1 in 10 approvals were previously agent overrides of low scores.
- **Constraint:** screening criteria are locked by fair-housing counsel.
- **Plant:** how did those override tenants actually do? Unstated.
- **Q1:** How did the tenants agents overrode actually perform? · **A1:** Design an appeal path that goes to a person with a documented reason.
- **Pattern:** When a score replaces judgment, find where the judgment went.

### 24. Pick paths (warehouse)
- **Product:** Handheld app routes pickers along an optimized path. · **D** · Fixing the bottleneck moved it
- **Colleague:** Site GM reports picks per hour at an all-time high.
- **Facts:** picks per hour up 25%; packing station backlog up; late trucks up twice a week.
- **Constraint:** packing headcount is set by corporate labor planning.
- **Plant:** "twice a week" — which days?
- **Q1:** What changed at packing when picks sped up? · **A1:** Pace picking to packing capacity on peak days.
- **Pattern:** Speeding up one step only moves the queue.

### 25. Pre-qualification tool (small business loans)
- **Product:** Online tool tells business owners if they're "likely approved." · **I** · The tool and the decider use different rules
- **Colleague:** Marketing reads loan officer interviews as "officers are too strict"; the credit lead reads them as "the tool is too generous."
- **Facts:** applications up 60%; approval rate down from 70% to 45%; officers spend more time on declines.
- **Constraint:** underwriting rules are set by the board; you present Thursday.
- **Plant:** "likely" has no stated threshold.
- **Q1:** Does the tool use the same criteria as underwriting? · **A1:** Show which criteria the tool can't check.
- **Pattern:** When the tool and the decider disagree, the user pays.

### 26. Ticket transfers (live events)
- **Product:** Rotating barcodes to stop screenshot tickets. · **C** · Killing the workaround kills what it did
- **Colleague:** Head of trust announced rotating barcodes for all events next season.
- **Facts:** fraud down 80% in pilot; gate delays up at pilot venues; "can't get in" complaints from groups where one person bought all tickets.
- **Constraint:** venue scanners can't be updated before next season.
- **Plant:** who in a group actually holds the tickets?
- **Q1:** What were screenshots doing besides fraud? · **A1:** Make group transfer a one-tap step at purchase.
- **Pattern:** Kill a workaround and you lose what it quietly did.

### 27. Fare capping (city transit)
- **Product:** Tap-to-pay fares cap at the monthly pass price. · **D** · Nobody owns the gap between two systems
- **Colleague:** Fare policy lead says capping made passes obsolete.
- **Facts:** tap riders up 40%; pass sales down 30%; employer-subsidized riders still buy passes and complain about double charges.
- **Constraint:** employer benefit programs run on a separate vendor system.
- **Plant:** "double charges" — how many, and on which days?
- **Q1:** Who owns the rider who uses both systems? · **A1:** Map one subsidized rider's month across both systems.
- **Pattern:** The gap between two systems belongs to nobody.

### 28. Booking deposits (salons)
- **Product:** Booking app requires a deposit for appointments. · **I** · The win and the loss hit different people
- **Colleague:** Owner reads stylist interviews as "deposits saved us"; the front-desk lead reads them as "new clients are gone."
- **Facts:** no-shows down 40%; new client bookings down 15%; repeat clients unaffected.
- **Constraint:** processor fees are fixed; present at Monday's staff meeting.
- **Plant:** "new client" isn't defined — first booking, or first visit?
- **Q1:** Who is the deposit filtering out? · **A1:** Waive deposits for first bookings made by referral.
- **Pattern:** Check who pays for the win.

### 29. Recurring gift default (nonprofit)
- **Product:** Donation page with "monthly" preselected. · **C** · A default is doing the deciding
- **Colleague:** Development director announced the monthly default sitewide.
- **Facts:** recurring donors up 50%; cancellations in month two up 3x; chargeback complaints appeared for the first time.
- **Constraint:** the payment CRM can't send pre-charge reminders until its upgrade.
- **Plant:** did the cancellers know they signed up for monthly?
- **Q1:** Did donors choose monthly, or miss that it was selected? · **A1:** Confirm "monthly" in plain words on the final step.
- **Pattern:** A default counts as consent only if people saw it.

### 30. Market tokens (farmers markets)
- **Product:** App and kiosks for EBT shoppers to buy market tokens. · **D** · It only works where a person is standing
- **Colleague:** Network director wants self-serve kiosks at every market.
- **Facts:** EBT sales up 50% at markets with a staffed booth; flat at kiosk-only markets; vendor complaints about token mix-ups.
- **Constraint:** token handling rules are set by federal program guidance.
- **Plant:** which markets have which setup isn't stated.
- **Q1:** What does the staffed booth do that the kiosk doesn't? · **A1:** Shadow a staffed booth for a morning.
- **Pattern:** It works where a person is standing.
