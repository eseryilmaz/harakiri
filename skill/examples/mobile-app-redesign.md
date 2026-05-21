# Example: Mobile App Redesign

## Input

```
Harakiri this:

Decision: We are shipping a complete navigation redesign for our mobile app.
The bottom tab bar is being replaced with a hamburger menu and a new sidebar.
All primary actions that were one tap away are now two or three taps away.
The change affects all 280,000 active users simultaneously with no opt-out.

Sector: Consumer app / personal finance tracker
Audience: Existing active users, daily users especially (about 40,000 DAU)

Framing: "A fresh, modern interface that gives you more space and flexibility."

Context: App has a 4.6 star rating with 12,000 reviews. Top review themes
are simplicity and speed. Users have been asking for a dark mode for 2 years
(not included in this release). Several power users have 3+ year streaks
they actively talk about in the community Discord.
```

---

## Output

```
HARAKIRI REPORT
Complete mobile navigation redesign replacing the bottom tab bar with a hamburger
menu and sidebar, affecting all 280,000 active users simultaneously with no opt-out.

─────────────────────────────────────────────────────────

VERDICT
Ship with changes

BACKLASH RISK SCORE
6.8 / 10 — Serious backlash risk

─────────────────────────────────────────────────────────

STRONGEST ATTACK VECTOR

Streak and habit destruction for the most vocal user segment. The users with
3+ year streaks have built daily rituals around muscle memory — they open the app,
tap the same place, log the thing, close. That workflow is being broken. When a
streak ends because the interface changed and they could not find the button in time,
the emotional response is not frustration — it is grief. These are your most
visible community members and they will be the loudest voices when the update drops.
The "more space and flexibility" framing will be mocked by anyone who used
the app for its speed, which is your top-reviewed attribute.

─────────────────────────────────────────────────────────

PERSONA ATTACKS

[1] ANGRY EXISTING CUSTOMER
Daily user with a 900-day streak and a practiced 12-second logging routine.

  "I had a 900-day streak. The update dropped overnight.
   I could not find the log button in time. It's gone."

I have used this app every single day for two and a half years. I recommended
it to my entire family. My 12-second morning routine — open, tap, log, close —
was the reason it worked for me. Now everything I tapped is gone or buried.
The hamburger menu takes three taps to reach things I used every day. I missed
my log yesterday because I could not find it fast enough. My streak is broken.
This is not a fresh interface. This is them deciding that their aesthetic vision
matters more than the habits of people who actually use the product.

Why this resonates: Streak loss has outsized emotional weight. This user has
a public presence in the community Discord and their experience will become
the reference story for the backlash.

What reduces the anger: A transition mode (old UI available for 30 days).
A streak protection mechanism for update-related misses.

───

[2] COMPETITOR LOYALIST
Switched from a competitor to this app specifically for the simple UI.

  "Left [Competitor] because their redesign made it unusable.
   Now this. Maybe simple apps just don't stay simple."

I moved to this app 18 months ago after [Competitor] buried everything under
new menus I never asked for. I explicitly chose this one because the reviews
said it was fast and clean. The reviews were right — until today. I am now
looking at the exact same problem I switched away from. Some product teams
really cannot leave well enough alone.

Why this resonates: This comparison is particularly damaging because it implies
a pattern across the industry — this is not one bad decision, it is every
productivity app eventually betraying its own value proposition.

What reduces the anger: A clear public statement about what specifically
the redesign enables that the old UI could not. "More space" is not enough.

───

[3] SKEPTICAL JOURNALIST
Tech writer covering mobile UX and product decisions.

  "The top review theme for this app is 'simple and fast.'
   The redesign adds taps to every primary action. Someone approved this."

The existing review corpus for this app tells you exactly why people chose it
over alternatives: it is fast, it is uncluttered, it does not get in the way.
The new navigation model adds between one and three taps to every action that
was previously one tap. The stated rationale — "more space and flexibility" —
is the language of a design team that fell in love with a visual direction and
worked backward to justify it. The more interesting story is what happens
to the 4.6 star rating in the next 30 days, and whether the team has a
rollback plan.

Why this resonates: The gap between what users chose the app for and what
was changed is documentable, specific, and makes for a clean narrative.

What reduces the anger: Shipping the dark mode alongside the redesign.
Answering the "why" with specifics. Providing a public rollback commitment.

───

[4] BAD-FAITH COMMENTER
Has 8,000 followers. Finance app connoisseur.

  "App was famous for being the one finance tracker that didn't
   ruin itself with a redesign. Past tense."

They finally did it. Hamburger menus. Buried actions. "Fresh and modern."
My streak is fine. My will to continue is not.

Why this resonates: Short, specific, nostalgic. "Past tense" is the knife.
This gets screenshotted and posted as a warning to anyone evaluating the app.

What reduces the anger: Nothing at this point. The screenshot is coming.
Mitigate by having a public transition plan ready before launch day.

───

[5] INTERNAL SKEPTIC
Product designer who raised concerns during the design review.

  "The usability testing was done with new users.
   The daily active users were not the test audience."

I am not saying the new design is bad. I am saying the decision to ship it to
everyone at once, with no opt-out, without testing it on the daily-habit segment —
the people who use this app in a 12-second window with one hand while doing
something else — was a choice that was made knowingly. The arguments for a
phased rollout were in the design review doc. They did not win the argument.

Why this resonates: This surfaces the exact fear every frustrated user has —
that the company knew, had the data, and shipped anyway. It is the most credible
attack because it does not sound emotional.

What reduces the anger: A phased rollout would prevent this. After launch,
a public acknowledgment of the feedback and a specific improvement timeline.

─────────────────────────────────────────────────────────

VIRAL NARRATIVE
"The one finance app that didn't ruin itself with a redesign finally did."

Likely platforms: X, Reddit (r/personalfinance), App Store reviews

─────────────────────────────────────────────────────────

WHO GETS ANGRY FIRST
Users with streaks over 365 days who lose their streak in the first 72 hours
due to navigation confusion. This is a small group with outsized community
presence and strong emotional attachment to the product.

─────────────────────────────────────────────────────────

WHAT YOU ARE UNDERESTIMATING
The relationship between "speed" and "trust" in a daily habit app. Users of
financial tracking tools have overcome habit barriers to use a tool every day.
That habit is fragile. When the interface breaks the habit — even temporarily —
the user's brain recategorizes the app as "unreliable." Winning that trust back
is orders of magnitude harder than not breaking it.

─────────────────────────────────────────────────────────

MITIGATION PLAN

– Offer the legacy UI as an opt-in for 60 days: Removes "no choice" from every
  angry post. Even users who do not use it feel better knowing it exists.

– Build streak protection for the first 7 days post-update: If a user misses
  a log in the 7 days after the update, it does not break their streak.
  This removes the most emotionally charged attack vector.

– Ship dark mode alongside the redesign: The top long-standing request
  being absent from a major UI update is a morale problem. It signals that
  the redesign was for the company, not the user.

– Publish the "why" with specifics before launch: Not "more space" — what
  specific things does the new navigation enable that the old one could not?
  If the answer is "it looks better," do not ship it like this.

Safer framing:
"We redesigned the navigation to [specific capability]. If you preferred
the previous layout, you can switch back in Settings → Display for the
next 60 days. We have also added streak protection during the transition period."

─────────────────────────────────────────────────────────

KILL CRITERIA

Within 7 days of launch:

– App Store rating drops below 4.2 → roll out legacy UI opt-in immediately,
  do not wait for the planned 30-day checkpoint

– Streak loss reports exceed 500 in community Discord → activate streak
  protection retroactively, post founder response in Discord directly

– Review volume in first 72 hours is more than 3x baseline with negative
  sentiment dominant → consider soft rollback for new installs, hold for
  existing users

─────────────────────────────────────────────────────────

CONFIDENCE LEVEL
Medium-High

Navigation redesigns in daily habit apps have a consistent backlash pattern,
especially when the prior UI was a competitive differentiator. Confidence is
slightly reduced because the severity depends heavily on whether the new UI
actually slows down the core workflow — that can only be confirmed with
real daily-user testing data, which is not included in the input.

─────────────────────────────────────────────────────────

This report is a simulated red-team exercise. It reflects plausible criticism
patterns, not guaranteed public reaction. Do not treat it as legal, PR,
financial or crisis-management advice.
```
