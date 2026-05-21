# Example: AI Feature with Privacy Risk

## Input

```
Harakiri this:

Decision: We are launching "Smart Suggestions" — an AI feature that reads
the user's stored notes and documents to generate personalized productivity
recommendations. Examples: "You've been working on Project X for 3 weeks —
want to set a milestone?" or "You mentioned feeling overwhelmed on Tuesday —
here's a focus block suggestion."

The feature is opt-in but on by default. Users can disable it in Settings → Privacy.

Sector: Consumer app / productivity / personal notes
Audience: 400,000 users, mix of personal and professional users.
About 30% use the app for work-related notes.

Framing: "Smart Suggestions makes [App] the first productivity tool that
actually understands your work and your life."

Context: We had a minor data incident 14 months ago (a bug exposed some
user metadata to other users for 6 hours — no financial data, quickly fixed,
disclosed). We have not shipped AI features before. Our privacy policy
currently says we "do not use note content for any purpose other than displaying
it to you." We will need to update this policy to ship the feature.
```

---

## Output

```
HARAKIRI REPORT
Opt-in-by-default AI feature that reads user notes to generate personalized
suggestions, requiring a privacy policy update, launching to 400,000 users
including 30% professional users.

─────────────────────────────────────────────────────────

VERDICT
Do not ship as-is

BACKLASH RISK SCORE
8.8 / 10 — Serious backlash risk, approaching public narrative risk

─────────────────────────────────────────────────────────

STRONGEST ATTACK VECTOR

The privacy policy change combined with opt-out-by-default. Your current
policy explicitly states that note content is used only to display it to you.
Shipping a feature that reads note content for AI processing requires changing
that promise — and launching it opt-out-by-default means users who do not check
their settings have their content processed under a policy they never agreed to.
The 14-month-old incident is not forgotten by the users who experienced it.
This combination — prior incident, policy change, opt-out-by-default on a feature
that reads private notes — is the architecture of a trust catastrophe.

─────────────────────────────────────────────────────────

PERSONA ATTACKS

[1] ANGRY EXISTING CUSTOMER
Professional user who stores confidential client work in the app.

  "My client notes, my therapy notes, my financial planning documents —
   all being read by an AI I did not turn on. Because the opt-out
   is buried in Settings → Privacy."

I use this app for everything. Client meeting notes. Personal journaling.
Financial planning. I chose it specifically because their privacy policy
said note content was never used for anything else. Now, without asking me,
they have updated that policy and turned on a feature that reads all of it
to tell me I seem overwhelmed on Tuesdays. I do not want a productivity app
to know I seem overwhelmed. I want it to store my notes. This is not a
smart feature. It is a privacy violation dressed up as helpfulness.

Why this resonates: The professional user subset stores genuinely sensitive
material. "Client notes being read by AI" is not a hypothetical — it is
a real legal and reputational concern for lawyers, therapists, consultants
and executives.

What reduces the anger: Opt-in-by-default (not opt-out). Explicit consent
on first launch of the feature. A clear explanation of where and how content
is processed.

───

[2] COMPETITOR LOYALIST
Obsidian user who left every cloud note app on principle.

  "This is exactly why I moved to local-first apps.
   Your notes are not the product. Until they are."

I switched from cloud note apps to local-first storage two years ago
because I knew this was coming. AI features need training data or processing
targets. Your notes are the most convenient source. "Opt-out in Settings"
is not consent — it is the UX of a decision already made for you.
Obsidian does not read my notes. It stores them. The difference matters.

Why this resonates: The local-first and privacy-first communities are
vocal and principled. This spreads beyond the app's own users into a
broader values conversation about cloud software and AI.

What reduces the anger: Cannot recover this audience. The local-first
community will use this as a cautionary example regardless of mitigation.

───

[3] SKEPTICAL JOURNALIST
Tech writer covering AI privacy and consumer data practices.

  "The app's privacy policy previously said content was never used
   for any purpose other than display. The new AI feature requires
   changing that. The feature is on by default."

This story has several layers worth unpacking. First, a prior data incident
14 months ago — resolved quickly, but on the record. Second, a privacy policy
that explicitly promised content isolation, now being updated to enable AI
processing. Third, an opt-out default that means most of the 400,000 users
will have their notes processed before they know the feature exists.
Fourth: the marketing copy says the app "understands your work and your life."
That framing, applied to private notes, is either reassuring or alarming
depending on which side of the privacy debate you are on. I know which side
most of my readers are on.

Why this resonates: This is a documented, specific, multi-layer story.
The journalist does not need to speculate — every element is public and traceable.
It is the kind of story that gets filed to tech desks.

What reduces the anger: Opt-in-by-default. Privacy policy change announced
separately from the feature, with a comment period. No "understands your life"
language in the marketing.

───

[4] BAD-FAITH COMMENTER
Privacy Twitter. Sees the announcement. Posts.

  "Notes app that promised never to read your notes launches AI
   feature that reads your notes. Opt-out is in Settings → Privacy.
   Classic."

'Smart Suggestions makes [App] the first productivity tool that
actually understands your work and your life.'

Your notes were always the product. The AI just made it official.

Why this resonates: Short, quotable, and technically accurate. The quote
from the privacy policy next to the marketing copy is the screenshot.
This post writes itself from public information.

What reduces the anger: Impossible to prevent if the feature ships opt-out-by-default
with the current policy change. The screenshot exists the moment the policy updates.

───

[5] INTERNAL SKEPTIC
Engineer or product person with concerns about the prior incident.

  "We had a data incident 14 months ago. We resolved it.
   We disclosed it. Now we are shipping a feature that reads
   all user notes by default. I hope the incident response
   playbook is current."

I am not saying Smart Suggestions is a bad feature. I am saying the
sequence matters: prior incident, explicit privacy promise in the policy,
policy change to enable content processing, opt-out default, and marketing
copy that says the app "understands your life." Each of those decisions
is defensible individually. Together they form a narrative that will be
very hard to walk back if anything goes wrong. The question I would
want answered before we ship is: what is the plan if this becomes
a news story on a day when the product has a bug?

Why this resonates: The scenario described — a bad day combining a feature
issue with the prior incident being cited — is specific and plausible.
This is the kind of thinking that makes stakeholders ask hard questions.

What reduces the anger: Having a documented, rehearsed incident response
plan for this feature before it ships. Making it opt-in eliminates the
most urgent risk.

─────────────────────────────────────────────────────────

VIRAL NARRATIVE
"Notes app that promised to never read your notes updated their privacy
 policy and turned on an AI that reads your notes. Opt-out is in Settings."

Likely platforms: X, Hacker News, Reddit (r/privacy, r/selfhosted)

─────────────────────────────────────────────────────────

WHO GETS ANGRY FIRST
Privacy-conscious professional users — lawyers, therapists, consultants,
executives — who discover their confidential work notes are being processed
by AI without explicit consent. They are the loudest and most credible voices.

─────────────────────────────────────────────────────────

WHAT YOU ARE UNDERESTIMATING
The prior data incident. Fourteen months ago, your incident made some users
aware of how cloud-stored notes can be exposed. Those users have been watching.
When a follow-on privacy change happens — even a well-intentioned one — they
do not evaluate it in isolation. They evaluate it as the second entry in a pattern.

─────────────────────────────────────────────────────────

MITIGATION PLAN

– Change to opt-in-by-default: This is the only change that eliminates the
  strongest attack vector. "Users can enable it in Settings" is a completely
  different story than "Users must disable it in Settings."

– Announce the privacy policy change before the feature ships:
  Give users 30 days to read the new policy before anything changes.
  Consent that happens after the fact is not consent.

– Remove "understands your work and your life" from marketing copy:
  This phrase applied to private notes is alarming before it is reassuring.
  Replace with a functional description: "surfaces patterns from your notes
  to suggest what to work on next."

– Acknowledge the prior incident in the feature announcement:
  One sentence: "We know some of you remember our 2025 data incident.
  Here is how this feature is different." Not acknowledging it ensures
  someone else brings it up.

Safer framing:
"Smart Suggestions is a new opt-in feature that uses your note patterns
to suggest priorities and focus blocks. It is off by default. You can
enable it in Settings → AI Features. Here is exactly what it reads,
what it does not read, and where processing happens."

─────────────────────────────────────────────────────────

KILL CRITERIA

Before launch:
– If legal counsel flags the policy change as requiring user re-consent
  (common in GDPR jurisdictions) → do not ship opt-out; ship opt-in only

Within 7 days of launch:
– Any media inquiry citing the prior incident in connection with the
  new feature → hold a pre-planned founder response, do not respond ad hoc

– r/privacy thread reaches 500 upvotes → disable the feature for new users,
  hold for existing opted-in users, issue statement within 12 hours

– Any indication of content leakage between users (even minor) → kill switch
  immediately, full incident response protocol

─────────────────────────────────────────────────────────

CONFIDENCE LEVEL
High

Privacy policy changes combined with opt-out-by-default AI content processing
on a platform with a prior data incident is one of the highest-confidence
backlash patterns in consumer software. The specific risk vectors (policy
quote vs. feature behavior, prior incident citation, professional user exposure)
are documentable from the information provided.

─────────────────────────────────────────────────────────

This report is a simulated red-team exercise. It reflects plausible criticism
patterns, not guaranteed public reaction. Do not treat it as legal, PR,
financial or crisis-management advice.
```
