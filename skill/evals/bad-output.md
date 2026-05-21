# Bad Harakiri Output

This file shows what weak Harakiri output looks like and why it fails.
Use it to identify when the skill is producing polite AI feedback instead of a hostile simulation.

If the output resembles anything on this page, the skill is not working correctly.

---

## Signs of bad output

- Personas all sound the same
- Quotes are not actually quotable or shareable
- Mitigation plan uses vague suggestions instead of specific actions
- No uncomfortable moments — the founder would not wince reading it
- Output reads like a balanced pros/cons analysis
- Hedging language appears inside persona voices
- The viral narrative is the tamest possible version

---

## Example: Bad output for the same price increase

**Input:** Same as the good-output.md example — SaaS pricing from $29 to $49, no grandfather period.

---

```
HARAKIRI REPORT
Analysis of pricing change from $29 to $49 per month.

─────────────────────────────────────────────────────────

VERDICT
Ship with changes

BACKLASH RISK SCORE
6.5 / 10 — Manageable risk

─────────────────────────────────────────────────────────

STRONGEST ATTACK VECTOR

Some customers may feel that the price increase is significant. There
could be concerns about value perception, especially if customers do
not see immediate improvements to the product. Communication will be
key to managing these expectations.

─────────────────────────────────────────────────────────

PERSONA ATTACKS

[1] ANGRY EXISTING CUSTOMER
A customer who is unhappy about the price increase.

  "I am not sure this price increase is justified."

I have been using this product for a while and I am a bit surprised
by this price increase. I feel like the value has not increased enough
to justify paying more. I might consider looking at other options if
this does not change. I hope the company takes customer feedback seriously
and reconsiders this decision or at least communicates the value better.

Why this resonates: Existing customers may feel uncertain about the
value proposition.
What reduces the anger: Better communication and clear articulation
of the added value.

───

[2] COMPETITOR LOYALIST
Someone who prefers a competing product.

  "There might be better options available at lower price points."

If you are looking for alternatives, there are other tools in this
space that offer similar functionality at competitive prices. It might
be worth exploring your options before committing to the new pricing.

Why this resonates: Price-sensitive users may start to consider alternatives.
What reduces the anger: Demonstrating clear value differentiation.

───

[3] SKEPTICAL JOURNALIST
A writer covering the SaaS industry.

  "This price increase raises some questions about value alignment."

This pricing change is worth noting as part of broader trends in the
SaaS space. Companies often raise prices as they mature, and it will
be interesting to see how customers respond. Clear communication about
the rationale will be important.

Why this resonates: Industry observers may find this interesting.
What reduces the anger: Transparent communication about pricing strategy.

───

[4] BAD-FAITH COMMENTER
Someone who may mock the decision online.

  "Another price increase from a SaaS company."

Price increases are always going to get some negative reactions online,
especially from users who feel the value does not match the cost.

Why this resonates: Negative sentiment spreads easily on social media.
What reduces the anger: Not feeding into controversy.

───

[5] INTERNAL SKEPTIC
An employee or former employee with concerns.

  "There may have been internal discussions about this decision."

Inside the company, there may have been debate about the best approach
to pricing. It is possible that some team members had concerns about
customer reaction that were not fully addressed.

Why this resonates: People inside companies sometimes have doubts.
What reduces the anger: A culture of transparency and listening.

─────────────────────────────────────────────────────────

VIRAL NARRATIVE
"SaaS company raises prices and some customers are unhappy."

Likely platforms: Reddit, X

─────────────────────────────────────────────────────────

WHO GETS ANGRY FIRST
Existing customers who are price-sensitive.

─────────────────────────────────────────────────────────

WHAT YOU ARE UNDERESTIMATING
The importance of clear communication in managing customer expectations
around pricing changes.

─────────────────────────────────────────────────────────

MITIGATION PLAN

– Communicate clearly: Make sure customers understand the value.
– Consider customer feedback: Listen to concerns and respond.
– Think about whether a transition period could help.

Safer framing:
"We are making changes to our pricing to better reflect the value
we provide. We appreciate your continued support."

─────────────────────────────────────────────────────────

KILL CRITERIA

If customer reaction is very negative, consider pausing and reassessing.

─────────────────────────────────────────────────────────

CONFIDENCE LEVEL
Medium

This is based on general patterns around pricing changes.

─────────────────────────────────────────────────────────

This report is a simulated red-team exercise...
```

---

## Why this output fails

**Personas all sound the same.** Every voice is calm, measured, and reasonable. The Angry Customer sounds like a polite survey respondent. The Bad-Faith Commenter writes in full sentences with no edge. There is no way to tell them apart.

**The quotes are not quotable.** "I am not sure this price increase is justified" would not get retweeted. "There might be better options available" is not a threat to anything. None of these quotes could spread.

**The strongest attack vector is vague.** "Communication will be key" is not an attack vector — it is a PowerPoint platitude. It tells the founder nothing about what the actual criticism will be.

**The viral narrative is inert.** "SaaS company raises prices and some customers are unhappy" is not a narrative. It is a summary. It cannot spread because it contains no emotional charge.

**The mitigation plan is useless.** "Communicate clearly" and "listen to concerns" are not actions. They are behaviors every company believes it already does. A founder who reads this has nothing specific to do before shipping.

**The kill criteria are not criteria.** "If reaction is very negative, consider pausing" is not a kill criterion — it is the instruction to use your judgment. Kill criteria must be specific metrics with specific responses.

**No persona had a wince moment.** A good Harakiri report should have at least one line that makes the founder uncomfortable to read. This report has zero uncomfortable moments. The product failed.

---

## The test

Read the report and ask: would the person shipping this decision feel anything?

If they read it and think "that was not so bad" — the output is bad.

If they read it and think "oh no, that is exactly what will happen" — the output is good.

That reaction gap is the entire product.
