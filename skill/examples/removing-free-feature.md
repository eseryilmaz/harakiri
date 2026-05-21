# Example: Removing a Free Feature

## Input

```
Harakiri this:

Decision: We are moving CSV export behind a paid plan. It is currently
available on the free tier. After the change, free users will only be
able to export their data as PDF. CSV will require the Pro plan ($19/month).

Sector: SaaS / note-taking / personal knowledge management
Audience: Free users (180,000 of them). Paid conversion rate is currently 4%.

Framing: "CSV export is a power-user feature and we're moving it to Pro
to better align features with the users who need them most."

Context: Several users have built personal automations and scripts that
depend on the CSV export. The feature was explicitly listed as free in
our original Product Hunt launch post from 2 years ago. A competitor
offers unlimited CSV export on their free tier.
```

---

## Output

```
HARAKIRI REPORT
Moving CSV export from free tier to paid Pro plan ($19/month), affecting
180,000 free users, including users who built automations that depend on it.

─────────────────────────────────────────────────────────

VERDICT
Rewrite before launch

BACKLASH RISK SCORE
7.8 / 10 — Serious backlash risk

─────────────────────────────────────────────────────────

STRONGEST ATTACK VECTOR

The Product Hunt post. Two years ago you told the world CSV export was free.
That post still ranks. People still link to it. Removing the feature while
that public record exists is not a business decision to the people affected —
it is a documented promise being broken. The automation dependency makes it
worse: this is not a "nice to have" for the affected users, it is a workflow
they built on the assumption that your free tier was stable. The framing
"better aligning features with users who need them most" will be read as
corporate language for "we are charging for something we said was free."

─────────────────────────────────────────────────────────

PERSONA ATTACKS

[1] ANGRY EXISTING CUSTOMER
Free user who built a weekly automation that exports notes to a spreadsheet.

  "I built my entire review workflow around their free CSV export.
   They advertised it as free. I have the Product Hunt post."

I chose this app over three alternatives specifically because CSV export was
free. I spent six hours building a script that runs every Sunday and exports
my weekly notes into a spreadsheet my team uses. That workflow is now broken
unless I pay $19 a month for a feature that was free when I committed to
the platform. The framing — "power-user feature, aligning with users who
need it most" — is remarkable. I am the user who needs it most. I am
a free user. I need it most and apparently that is the reason I should pay.

Why this resonates: This user has a documented dependency and a documented
promise. They are not making an argument — they are showing receipts.
Developers and automation users will amplify this heavily on HN and Reddit.

What reduces the anger: Grandfathering users who have downloaded a CSV export
in the past 90 days. Acknowledging the Product Hunt promise directly.

───

[2] COMPETITOR LOYALIST
Evaluating tools, now has a clear answer.

  "Made my decision. Competitor Y. Free CSV export, no gotchas."

I was down to two options. This announcement made it easy.
When a company gates data export, the question you have to ask is:
whose data is it, really?

Why this resonates: The data portability framing is powerful and principled.
It spreads beyond the immediate audience because it touches a values question,
not just a pricing question.

What reduces the anger: Hard to counter after the announcement. Before:
making data portability a visible value commitment.

───

[3] SKEPTICAL JOURNALIST
Writer covering product and indie tools.

  "Gating CSV export behind a paywall is not a feature alignment decision.
   It is a data hostage decision."

There is a recurring debate in the personal software space about whether
companies have an obligation to make data portability free. This announcement
is a useful test case. The framing — aligning features with the users who
need them most — makes a category error: data export is not a feature that
some users need and others do not. It is access to your own data. The
precedent this sets for the 180,000 free users is: your data is here,
but accessing it in a useful format now costs $19 a month.

Why this resonates: This argument travels beyond the company's own users.
It gets shared by product people and privacy advocates as a principles debate.

What reduces the anger: Framing the change as CSV export being enhanced
(not gated), or offering a one-time export before the paywall activates.

───

[4] BAD-FAITH COMMENTER
Finds the original Product Hunt post. Posts it.

  "[screenshot of original PH post listing CSV as free]
   Two years later:
   [screenshot of new pricing page]
   These people."

Product Hunt post said free. Pricing page now says Pro.
The classic arc.

Why this resonates: The screenshot comparison is a complete argument
in two images. No words needed. Highly retweetable.

What reduces the anger: Remove the original claim before it gets screenshotted,
or proactively acknowledge it in the announcement.

───

[5] INTERNAL SKEPTIC
Former growth team member.

  "The 4% paid conversion rate was the input to this decision.
   The output will be a lower number."

The logic here was: free users are not converting, so let's use CSV export
as a conversion lever. That is not wrong as a theory. What it misses is
that the users who rely on CSV export most heavily are the ones who have
integrated the product most deeply into their workflow — which usually means
they are the closest to converting on their own timeline. Gating their
workflow does not accelerate their decision. It reverses it.

Why this resonates: This is a credible business argument, not just an
emotional complaint. It gives the journalist a counter-narrative to the
company's own conversion logic.

What reduces the anger: Data on the conversion rate of CSV-heavy users
vs the overall base. If the internal data shows they convert at higher
rates, the decision becomes much harder to defend publicly.

─────────────────────────────────────────────────────────

VIRAL NARRATIVE
"They advertised CSV export as free two years ago.
 Here is the Product Hunt post. Here is the new pricing page."

Likely platforms: X, HN, Reddit (r/selfhosted, r/productivity)

─────────────────────────────────────────────────────────

WHO GETS ANGRY FIRST
Technical free users who built automations — developers, power users, and
the personal-knowledge-management community on Reddit and HN. They are small
in number but high in credibility and online presence.

─────────────────────────────────────────────────────────

WHAT YOU ARE UNDERESTIMATING
The Product Hunt post is an indexed public document. The screenshot comparison
— "they said free then, they say paid now" — requires zero argument and
will be made within hours of the announcement. The risk is not just current
users. It is every future user who searches for this tool and finds that post
before they find the current pricing page.

─────────────────────────────────────────────────────────

MITIGATION PLAN

– Grandfather users who have exported at least once in the past 6 months:
  These are the users with real dependencies. Protecting them removes the
  most credible attack vector.

– Acknowledge the Product Hunt promise in the announcement: Do not pretend
  the original post does not exist. One sentence: "We said CSV was free
  when we launched. We are changing that, and we know it is a significant shift."

– Offer a one-time full data export for all free users before the paywall
  activates: Reframes gating as "export your data now, then decide"
  rather than "pay or lose access."

– Do not use "aligning features with users who need them most" language:
  This phrase is the one the journalist will quote. Replace it with
  the honest reason: "We are moving CSV to Pro to fund ongoing development."

Safer framing:
"We are moving CSV export to our Pro plan on [date]. Before that date,
all free users can download a full CSV export of their data. Existing users
who export regularly will have 90 days at their current access level to decide."

─────────────────────────────────────────────────────────

KILL CRITERIA

Within 48 hours of announcement:

– Product Hunt post screenshot circulates with 500+ engagements → issue
  a direct public response acknowledging the original commitment

– HN thread reaches front page → founder posts in the thread directly,
  not through a PR statement

– Free user churn rate exceeds 15% in first week → grandfather all
  active free users, revisit paywall timeline

─────────────────────────────────────────────────────────

CONFIDENCE LEVEL
High

Feature removal with a documented prior promise is one of the most reliably
explosive backlash patterns. The Product Hunt post is a specific, locatable
vulnerability. High confidence in the data hostage and broken promise framings.

─────────────────────────────────────────────────────────

This report is a simulated red-team exercise. It reflects plausible criticism
patterns, not guaranteed public reaction. Do not treat it as legal, PR,
financial or crisis-management advice.
```
