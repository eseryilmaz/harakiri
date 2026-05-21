# Good Harakiri Output

This file shows what high-quality Harakiri output looks like.
Use it to calibrate the skill and evaluate new outputs.

A good Harakiri report is:
- **Specific** — references the actual decision, not generic risks
- **Hostile** — uncomfortable to read if you are the one shipping
- **Quotable** — the dangerous quotes could actually spread
- **Useful** — the mitigation plan is actionable, not vague
- **Distinct** — each persona sounds different from the others

---

## Example: Good output for a price increase

**Input:** SaaS tool raising prices from $29 to $49 with no grandfather period, 30 days notice, framed as "reflecting the value we deliver."

---

```
HARAKIRI REPORT
SaaS pricing increase from $29/month to $49/month, effective in 30 days,
with no grandfather period for existing customers.

─────────────────────────────────────────────────────────

VERDICT
Rewrite before launch

BACKLASH RISK SCORE
8.2 / 10 — Serious backlash risk

─────────────────────────────────────────────────────────

STRONGEST ATTACK VECTOR

Price fairness combined with loyalty penalty framing. The 69% increase with
no grandfather period will be read as punishment for early adoption. The
announcement framing — "reflecting the value we deliver" — will be attacked
as tone-deaf because it centers the company's perspective, not the customer's.
Existing customers will not hear "we built more value." They will hear "pay more
or leave." This framing, on top of a previous price increase 18 months ago,
hands critics a compounding betrayal narrative.

─────────────────────────────────────────────────────────

PERSONA ATTACKS

[1] ANGRY EXISTING CUSTOMER
Long-tenured paying customer who has seen this movie before.

  "They raised prices 18 months ago. Now they are doing it again.
   How many more times before we are priced out?"

I have been paying since before they were cool. I have recommended this tool
to three colleagues. I have filed bug reports that sat unresolved for months.
And now they want 69% more money with 30 days notice and zero acknowledgment
of what loyal customers have put up with. "Reflecting the value we deliver" —
do you mean the value you have been slowly delivering less of while the
competitor across the street added features at the same price? This is not
a pricing update. It is a loyalty tax.

Why this resonates: Long-tenure customers feel disproportionate ownership of
the product. When they leave, they leave loudly and bring their referrals with
them. This archetype dominates Reddit and App Store reviews.

What reduces the anger: A grandfather period of at least 6 months for existing
customers. A specific acknowledgment of the previous increase in the announcement.

───

[2] COMPETITOR LOYALIST
Recently switched user who has been waiting for exactly this moment.

  "Moved to Competitor X three months ago. Paying $35/month for a better
   product. You are welcome."

I debated switching for a year. Every time I was about to, they shipped
something that gave me hope. Now I am glad I finally pulled the trigger.
Competitor X has everything this tool has, costs less, and does not
pull this. If you are still on the fence, this announcement is your answer.

Why this resonates: Competitor comparisons spread because they give
undecided users a destination, not just a grievance. The specific price
delta ($35 vs $49) is damaging because it is concrete and shareable.

What reduces the anger: Difficult to address directly. Shipping a
visible new feature before the price increase reframes the announcement.

───

[3] SKEPTICAL JOURNALIST
Newsletter writer covering SaaS business practices.

  "This is the third SaaS tool in my stack to raise prices this quarter.
   At some point, the value-inflation narrative stops working."

I have been watching the same pattern play out across the SaaS market.
Introduce a freemium product. Build dependency. Raise prices once.
Raise them again. Frame each increase as investment in the product.
Offer no protection to the customers who helped you survive the early years.
The interesting thing about this announcement is not the price. It is the
framing: "reflecting the value we deliver." That sentence is a tell.
It means the company has decided the customer's perception of value is
the problem, not the price.

Why this resonates: This framing gets shared by other SaaS founders who
are tired of seeing it, and by buyers who feel seen. It generates
discussion, not just outrage.

What reduces the anger: Announcing the specific features or investments
that justify the increase. Not vague value language — specific commitments.

───

[4] BAD-FAITH COMMENTER
Has not used the product. Has found a new episode.

  "Friendly reminder: 'we're doing this for you' means 'we're doing
   this to you.'"

69% increase. No grandfather. "Reflects the value we deliver."
Another startup speedrunning enshittification.

Why this resonates: This archetype does not need to be a customer
to do damage. They perform for their audience. The simpler and more
cutting the post, the more it spreads.

What reduces the anger: Nothing reduces it. Avoid giving them more
material. The announcement copy "reflecting the value we deliver" is
the quote they will screenshot.

───

[5] INTERNAL SKEPTIC
Former growth PM who knows how this decision was made.

  "The retention data on the last price increase was presented to
   leadership. This decision was made anyway."

I am not going to name names. But I will say that the decision to
skip grandfather pricing was debated internally. There was data on
churn risk from the last increase. There were people in the room
who argued for a transition period. The framing of this announcement
was workshopped for two weeks. The outcome you are seeing is not
the only option that was on the table. It is the one that won.

Why this resonates: This is the most credible attacker because it
surfaces the gap between what the company claims (data-driven,
customer-first) and what happened in the room. Journalists use this
as background. It validates every angry customer's suspicion.

What reduces the anger: Transparency in the announcement about the
decision-making process. Even a sentence acknowledging that the team
debated this reduces the narrative fuel.

─────────────────────────────────────────────────────────

VIRAL NARRATIVE
"They raised prices once to survive. Now they are raising them again
to profit. The customers who kept them alive during the first raise
get no protection during the second."

Likely platforms: Reddit, X, HN

─────────────────────────────────────────────────────────

WHO GETS ANGRY FIRST
Long-tenured customers on the original pricing tier who also lived
through the previous increase 18 months ago. They have the longest
memory and the loudest voices in the community.

─────────────────────────────────────────────────────────

WHAT YOU ARE UNDERESTIMATING
The compounding effect of two increases in 18 months. Each increase
on its own is defensible. Together, they form a pattern. The market
is not evaluating this announcement in isolation — it is evaluating
it as the second data point in a trend. The framing needs to
acknowledge this directly, or critics will do it for you.

─────────────────────────────────────────────────────────

MITIGATION PLAN

– Grandfather existing customers for 6 months at their current rate:
  Removes the loyalty penalty narrative. Gives customers agency.
  The cost is known; the churn risk from skipping this is not.

– Lead with a specific feature or investment, not value language:
  "We built X and Y, which cost us Z, and this pricing reflects that
  investment" is defensible. "Reflecting the value we deliver" is not.

– Acknowledge the previous increase directly in the announcement:
  Pretending this is the first time reads as dishonest to anyone
  with a memory. One sentence of acknowledgment defuses the pattern narrative.

– Give customers a clear downgrade path if they do not want the new price:
  Removing agency is what converts frustration into public anger.
  A documented option to cancel or downgrade before the increase
  reads as fair.

Safer framing:
"We have spent the last 18 months building [specific feature list].
Existing customers keep their current price until [date], after which
we will move to our new pricing that reflects these investments.
If this does not work for you, here is how to manage your plan."

─────────────────────────────────────────────────────────

KILL CRITERIA

If any of the following happen within 72 hours of announcement:

– Churn intent (cancellation requests + explicit threats) exceeds 8%
  of active customer base → pause rollout, issue founder statement

– Reddit thread exceeds 200 upvotes and top comment is a competitor
  comparison → respond directly in thread, do not go silent

– An ex-employee post on LinkedIn gains traction → brief the founder
  for a transparent response; do not let it sit unanswered

─────────────────────────────────────────────────────────

CONFIDENCE LEVEL
High

Strong historical evidence for this specific combination of pricing
increase + no grandfather period + compound increase. The complaint
patterns are well-documented and the framing risks are specific.

─────────────────────────────────────────────────────────

This report is a simulated red-team exercise. It reflects plausible
criticism patterns, not guaranteed public reaction. Do not treat it
as legal, PR, financial or crisis-management advice.
```

---

## Why this output is good

- **Specific:** References the 69% increase, the 18-month pattern, the "$35 competitor" — not generic pricing risk.
- **Hostile:** The Angry Customer's voice is personal and direct. The Bad-Faith Commenter is quotable. The Internal Skeptic is damning.
- **Distinct voices:** Each persona sounds different. The journalist is calm and analytical. The bad-faith commenter is short and punchy.
- **Useful:** The mitigation plan gives four specific actions, not vague suggestions. The safer framing is copy-ready.
- **Honest:** The confidence level is high, and the reason is specific.
