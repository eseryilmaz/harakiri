# Example: SaaS Price Increase

## Input

```
Harakiri this:

Decision: We are increasing pricing from $29/month to $49/month across all plans,
effective in 30 days. Existing customers are automatically moved to the new price.
There is no grandfather period.

Sector: SaaS / project management tool
Audience: Existing paying customers, mostly indie hackers and small teams.
Average customer tenure: 14 months.

Framing: "We are investing heavily in the product and this pricing reflects
the value [Product] delivers today."

Context: We raised prices once before, 18 months ago ($19 → $29). A vocal
community exists on Reddit (r/projectmanagement, 40k members). Competitor X
is at $35/month with more features. We have not shipped a major feature
in the past 6 months.
```

---

## Output

```
HARAKIRI REPORT
SaaS pricing increase from $29/month to $49/month with no grandfather period,
30 days notice, positioned as reflecting delivered value.

─────────────────────────────────────────────────────────

VERDICT
Rewrite before launch

BACKLASH RISK SCORE
8.2 / 10 — Serious backlash risk

─────────────────────────────────────────────────────────

STRONGEST ATTACK VECTOR

The compounding increase pattern. This is not a price increase — in the market's
eyes, it is the second data point in a trend: $19 → $29 → $49 in 18 months, a 158%
cumulative rise, with no major feature shipped in the most recent cycle. Combined
with no grandfather period, the announcement framing ("reflecting the value we deliver")
will be read as the company telling loyal customers that their loyalty is not worth a
transition period. The competitor at $35 is the number that will appear in every thread.

─────────────────────────────────────────────────────────

PERSONA ATTACKS

[1] ANGRY EXISTING CUSTOMER
Long-tenure customer who survived the first increase and now faces a second.

  "They raised prices to $29 and I stayed. Now $49 with no warning
   and no grace period. How many times before I'm just a line item?"

I have been here since they were $19. I stayed through the first increase
because I believed in the product. I recommended it to my whole team.
I filed three bug reports that are still open. Now they want 69% more — no
grandfather period, 30 days notice, and a press release that talks about
the value they deliver. I cannot name a single major thing they shipped
in the past six months. This is not a product decision. It is an extraction.

Why this resonates: This customer has receipts. They reference specific timelines
and specific unfulfilled expectations. Other customers with similar tenure will
recognize themselves in this post.

What reduces the anger: A 6-month grandfather period at the current rate. One
sentence in the announcement that acknowledges the previous increase.

───

[2] COMPETITOR LOYALIST
Switched to Competitor X 3 months ago and has been watching this unfold.

  "Moved to Competitor X at $35/month three months ago.
   It was the right call. You are welcome."

I debated switching for almost a year. Every time I was close, they shipped
something that gave me hope. Now they are at $49 with no grandfather and my
replacement costs me $14 less per month with a better feature set. If you are
still sitting on the fence, here is your sign.

Why this resonates: The $35 competitor price is concrete and searchable.
This post gives undecided customers a destination, not just a grievance.

What reduces the anger: Hard to address directly. Shipping a visible feature
before the announcement reframes the context.

───

[3] SKEPTICAL JOURNALIST
Newsletter covering SaaS business models and pricing practices.

  "The phrase 'reflecting the value we deliver' is doing a lot of work
   in an announcement that delivers nothing new to existing customers."

The pattern here is familiar. Build dependency during the low-price phase.
Raise prices once when growth slows. Raise them again when the numbers need help.
Frame each increase as investment. Skip the grandfather period because the cost
of churn is lower than the cost of the discount. What is interesting about this
specific announcement is that it lands six months after the last meaningful
product update, which means the "value we deliver" language cannot be attached
to anything concrete. That is where the trust damage happens.

Why this resonates: This analysis gets shared by other SaaS founders and operators
who recognize the pattern. It reads as fair, not hysterical, which makes it more
credible and more damaging.

What reduces the anger: Specific investment commitments in the announcement —
not "we're investing in the product" but "we built X and are funding Y."

───

[4] BAD-FAITH COMMENTER
Has not used the product. Saw the announcement. Has 12,000 followers.

  "$19 → $29 → $49 in 18 months. 'Reflecting the value we deliver.'
   Screenshot this. They'll walk it back by Friday."

Another startup speedrunning the enshittification playbook.
The roadmap is: get them dependent, raise prices, blame value.

Why this resonates: Short, specific, cites real numbers. The $19 → $29 → $49
progression is devastating in a single line. Easy to retweet, easy to screenshot.

What reduces the anger: Nothing. Do not give them the screenshot opportunity.
Remove "reflecting the value we deliver" from the announcement copy.

───

[5] INTERNAL SKEPTIC
Former product lead who was in the room when this was decided.

  "The retention cohort data from the last price increase was shared
   with the team. This decision was made anyway."

I am not going to say who made the call. But I will say that the conversation
about grandfather pricing happened. There were people in that room who argued
for a 90-day transition. There was data on what the last increase did to
long-tenure cohorts. The outcome you are seeing is not the only option
that was available. It is the one that won the internal argument.
The framing in the announcement is the framing that won that argument too.

Why this resonates: This post is a journalist's gift. It validates every
suspicious customer's read and provides background for a follow-up story.
It frames the decision as deliberate, not accidental.

What reduces the anger: Transparency in the announcement about the tradeoffs
considered. One sentence acknowledging that you debated transition pricing
and chose not to offer it, with the reason, is more defensible than silence.

─────────────────────────────────────────────────────────

VIRAL NARRATIVE
"They raised prices on us once to survive. Now they're raising them again to profit.
The customers who kept them alive get no protection the second time around."

Likely platforms: Reddit, X, HN

─────────────────────────────────────────────────────────

WHO GETS ANGRY FIRST
Customers with tenure between 12–24 months who remember the first price increase
and stayed anyway. They have the longest memory, the strongest sense of betrayal,
and the most credibility in community spaces.

─────────────────────────────────────────────────────────

WHAT YOU ARE UNDERESTIMATING
The compounding effect of having no new feature to attach the price increase to.
If you had shipped something significant in the past 3 months, the "reflecting
the value we deliver" line is defensible. Without it, critics will point to the
feature gap and the price increase in the same sentence — and they will be right.
The timing is as damaging as the number.

─────────────────────────────────────────────────────────

MITIGATION PLAN

– Grandfather existing customers for 6 months at $29: Removes the loyalty penalty
  narrative. Costs less than the churn from skipping it.

– Remove "reflecting the value we deliver" from the announcement copy: This phrase
  is the screenshot the Bad-Faith Commenter is waiting for. Replace it with a
  specific list of what the pricing funds.

– Acknowledge the previous increase directly: One sentence. "This is our second
  pricing update in 18 months, and we know that is a lot to ask." Not acknowledging
  it makes you look like you hope no one remembers.

– Ship or announce one concrete thing before the price goes live: Even a roadmap
  commitment changes the framing from extraction to investment.

Safer framing:
"We are changing our pricing from $29 to $49 on [date]. Existing customers keep
their current rate until [date + 6 months]. This increase funds [specific thing].
If this doesn't work for you, here is how to manage your plan before the change."

─────────────────────────────────────────────────────────

KILL CRITERIA

Within 72 hours of announcement:

– Cancellation requests exceed 8% of active base → pause rollout, issue
  founder statement within 24 hours

– Reddit thread in r/projectmanagement reaches 200+ upvotes with competitor
  comparison as top comment → respond in thread directly, do not go silent

– Ex-employee or insider post surfaces on LinkedIn with internal detail →
  brief founder for transparent response; do not let it compound unanswered

─────────────────────────────────────────────────────────

CONFIDENCE LEVEL
High

Compounding SaaS price increases without grandfather periods are among the
most documented backlash patterns. High confidence in the loyalty penalty
and enshittification framings. The specific $35 competitor price differential
makes the Competitor Loyalist attack unusually concrete.

─────────────────────────────────────────────────────────

This report is a simulated red-team exercise. It reflects plausible criticism
patterns, not guaranteed public reaction. Do not treat it as legal, PR,
financial or crisis-management advice.
```
