# Harakiri Angry Customer Skill

> Before you ship it, let the internet hate it.

Harakiri stress-tests product, brand, pricing, UX, marketing and launch decisions against five hostile market personas before you go public. It produces a structured red-team report with a backlash risk score, the strongest attack vector, quotable persona attacks, the viral narrative, a mitigation plan, and kill criteria.

---

## What it does

You describe a decision you are about to make public. Harakiri simulates how five different hostile audiences will react — specifically, personally, and without hedging.

The five personas:
1. **Angry Existing Customer** — feels betrayed, quotes what you promised
2. **Competitor Loyalist** — uses this to validate their switch
3. **Skeptical Journalist** — frames this as part of a pattern
4. **Bad-Faith Commenter** — finds the punchline and makes it viral
5. **Internal Skeptic / Ex-Employee** — exposes the gap between public messaging and internal reality

The output is a Harakiri Report: verdict, backlash risk score, persona attacks, viral narrative, mitigation plan, kill criteria.

---

## How it differs from a pre-mortem

A pre-mortem asks: "Why did our plan fail?"

Harakiri asks: "Who gets angry, what do they say, how does this become a backlash narrative, and what do we change before launch?"

Different question. Different output. Different use case.

---

## Installation

```bash
# Clone the repo (or download the skill directory)
git clone https://github.com/eseryilmaz/harakiri.git

# Copy the skill directory to your Claude skills folder
cp -R harakiri/skill ~/.claude/skills/harakiri-angry-customer
```

Restart Claude Code after installation. The skill is available immediately.

---

## Trigger phrases

Harakiri activates on any of these:

```
harakiri this
run a harakiri on [decision]
red team this [decision]
backlash test this
how will this get attacked
where could this create backlash
what will angry customers say about this
stress test this before I ship
talk me out of shipping this
```

---

## Usage

**Minimal input:**
```
Harakiri this: we are removing the free tier and requiring a paid plan for all new users.
```

**Better input (more specific output):**
```
Harakiri this:

Decision: We are increasing pricing from $29/month to $49/month for all plans, 
effective in 30 days. Existing customers will be moved to the new price automatically. 
No grandfather period.

Sector: SaaS / project management
Audience: Existing paying customers, mostly SMBs
Context: We raised prices once before 18 months ago. Competitor X is at $35/month.
Framing: "We are investing in the product and this reflects the value we deliver."
```

The more specific the input, the more specific and useful the attack.

---

## Example output

See `examples/` for full Harakiri reports across five decision types:

- `saas-price-increase.md` — pricing change with no grandfather period
- `mobile-app-redesign.md` — navigation overhaul that breaks muscle memory
- `removing-free-feature.md` — moving a free export feature behind a paywall
- `controversial-campaign.md` — bold brand claim that invites challenge
- `ai-feature-privacy-risk.md` — AI feature that reads user content

---

## Files in this package

```
skill/
├── harakiri.skill                    — main skill instructions for Claude
├── README.md                         — this file
├── examples/
│   ├── saas-price-increase.md
│   ├── mobile-app-redesign.md
│   ├── removing-free-feature.md
│   ├── controversial-campaign.md
│   └── ai-feature-privacy-risk.md
├── templates/
│   ├── decision-input-template.md    — fill-in template for giving context
│   └── harakiri-report-template.md  — blank report output format
├── evals/
│   ├── good-output.md                — what good Harakiri output looks like
│   └── bad-output.md                 — what bad output looks like and why
└── references/
    └── patterns/
        ├── pricing-change.md
        ├── feature-removal.md
        ├── product-launch.md
        ├── brand-campaign.md
        ├── ui-design-decision.md
        └── policy-change.md
```

---

## What it is not

- Not a prediction engine. It simulates plausible backlash — it does not guarantee it.
- Not legal, PR, financial or crisis-management advice.
- Not a tool to attack competitors or third parties. It is a self-risk analysis tool.
- Not a replacement for user research, customer interviews, or professional communications review.

---

## The disclaimer

Every Harakiri report ends with this:

> This report is a simulated red-team exercise. It reflects plausible criticism patterns, not guaranteed public reaction. Do not treat it as legal, PR, financial or crisis-management advice.
