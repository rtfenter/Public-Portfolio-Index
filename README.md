# Product Portfolio

This portfolio brings together product patterns from my professional experience, products I've shipped independently, and studies I'm using to build deeper fluency in new domains.

---

# Professional Product Cases

My professional experience spans B2C and B2B products, including scaling consumer loyalty across ecommerce and POS to building a 0→1 partner rewards platform.

These cases use generalized examples to show some of the product decisions behind that work.

### 01 / B2B Commerce & Rewards

## Order ≠ Earned

In invoiced B2B commerce, an order can be completed with **$0 collected at checkout**. That means placing an order and earning usable reward value cannot safely represent the same event.

**Order → Invoice → Pending Validation → Available**

**The decision:** Separate recognition of qualifying activity from availability of usable value.

This gives the partner acknowledgement that qualifying activity occurred while giving the business time to validate the underlying financial activity before creating spendable value.

**What I'd measure:** straight-through validation rate, validation accuracy, time to availability, and exception rate.

→ [View case study](https://github.com/rtfenter/B2B-Commerce-and-Rewards)

---

### 02 / B2C Commerce & Loyalty

## Purchase ≠ Final Transaction

A customer's transaction doesn't necessarily end at checkout. They can redeem loyalty value, use it toward a purchase, and later reverse that transaction through a return or refund.

**Customer:** Points → Reward → Purchase → Return → New Purchase  
**System:** Redemption → Earning → Reversal → Restoration → New Earning

**The decision principle:** Customer-facing reward state and underlying financial state should remain explainable and reconcilable throughout the transaction lifecycle.

That means defining deterministic behavior for redeemed value, payment refunds, earning reversals, reward restoration, and the new purchase without making the customer experience feel like an accounting system.

**What I'd measure:** reconciliation accuracy, adjustment exceptions, incorrect reward balances, and reward-related customer contacts.

→ [View case study](https://github.com/rtfenter/B2C-Commerce-and-Loyalty) · [Launch interactive demo](https://rtfenter.github.io/B2C-Loyalty-Product-Study/)

---

### 03 / Engagement & Incentives

## Enrollment ≠ Activation

Enrollment gives someone access to a product or program. It doesn't mean they've experienced its value.

**Enrolled → Activated → Engaged → Retained**

**The decision principle:** Start with the behavior the product is trying to change, not the incentive.

A first qualifying action, repeat behavior, and re-engaging a lapsed user are different objectives. Each requires its own audience, eligibility, incentive, success event, and measurement window.

The distinction that matters is between **offer performance and behavior change**. Claims and clicks show interaction with an offer. They don't establish that the incentive created incremental engagement.

**What I'd measure:** incremental activation lift, activation rate, time to first qualifying purchase, incentive use, and subsequent engagement, with incentive cost, incremental contribution, cannibalization, and over-targeting as guardrails.

→ [View case study](https://github.com/rtfenter/Engagement-and-Incentives) · [Launch interactive demo](https://rtfenter.github.io/B2C-Loyalty-Product-Study/#engagement)

---

### 04 / Platform Lifecycle & Controls

## One Account State, Multiple Consequences

A customer can be restricted by an upstream account state, a loyalty-specific restriction, or their own participation choice. Those states can overlap, but they don't share the same owner, scope, or recovery path.

**Source → Authority → Scope → Product Effects → Recovery → Audit**

**The decision principle:** State propagates according to its source, authority, and scope. Recovery removes only the cause it actually resolves.

That means an upstream restriction can propagate into dependent products, while a loyalty-specific restriction or customer participation choice remains contained to Loyalty. Each authority can change only the state it owns.

**What I'd measure:** lifecycle integrity, state propagation accuracy, recovery accuracy, manual corrections, and lifecycle-related support volume, with unauthorized state changes, cross-product side effects, and audit gaps as guardrails.

→ [View case study](https://github.com/rtfenter/Platform-Lifecycle-and-Controls) · [Launch interactive demo](https://rtfenter.github.io/B2C-Loyalty-Product-Study/#platform)

---

*These cases draw from product patterns I've encountered professionally. Companies, transactions, systems, and implementation details are generalized or fictionalized.*

---

# Selected Work

## Girl Dinner Mode

**0→1 Consumer Product · Personalization · Decision Support**

A personalized meal-decision app I designed, built, and shipped for iOS.

Girl Dinner Mode learns from user behavior and preferences to help answer a deceptively difficult question: **what should I eat?** The product includes personalized meal discovery, weekly planning, grocery organization, and lightweight daily experiences without calorie tracking, streaks, or guilt.

→ [Girl Dinner Mode](https://girldinnertonight.com)

---

## Personalization & Discovery

**Recommendations · Behavioral Signals · Ranking · Experimentation**

How should a product decide what to show someone next?

This study will explore explicit preferences vs inferred behavior, cold start, recency and context, negative signals, familiarity vs discovery, feedback loops, and how to measure whether personalization is actually improving the experience.

**Status:** Next to build

---

# Games

These studies use games and gaming platforms to explore player motivation, progression, accomplishment, audience behavior, and how evidence about behavior should inform product decisions.

### 01 / Player Accomplishment

## Who Decides What Represents a Player?

Xbox Achievements and PlayStation Trophies can record similar behaviors while making different aspects of accomplishment salient. The study started as a platform comparison and became a question about what gets lost when years of player behavior are compressed into a universal score.

**The product decision:** Preserve the verified accomplishment system, but let players curate a limited set of verified accomplishments that represent what matters to them.

**The principle:** The platform verifies what happened. The player decides what represents them.

→ [View project](https://github.com/rtfenter/Player-Accomplishment-Product-Study)

---

### 02 / Progression & Player Agency

## How Progression Creates Meaningful Choice

*Hades II* gives players more power, options, and control over time without allowing progression to eliminate the uncertainty and tradeoffs that make individual runs meaningful.

**The product principle:** Progression can relax a constraint without eliminating the thing that made the constraint meaningful.

The study uses Arcana and Grasp to examine access, acquisition, capacity, resource economics, player agency, and how telemetry should be interpreted before changing progression balance.

→ [View project](https://github.com/rtfenter/Hades-II-Progression-System-Study)

---

### 03 / Player & Audience Experience

## When Audience Evidence Should Change a Game Decision

Game telemetry describes the person holding the controller, but games can also have meaningful audiences who watch for mastery, narrative, suspense, community, discovery, or relaxation.

**The product decision:** Treat audience experience as an additional evidence set, not an optimization target.

The framework asks whether player and audience evidence align or diverge, then maps that to four responses: **Protect · Separate · Investigate · Improve.**

→ [View project](https://github.com/rtfenter/Audience-Aware-Game-Product-Framework)

---

# Books, Audio & Community

## Dungeon Crawler Carl Product Study

**Discovery · Series Engagement · Audio · Community**

A planned consumer product study using *Dungeon Crawler Carl* to explore the product experience surrounding a series, not just the content itself.

The study will look at discovery, moving through a series, reading vs listening, fandom, spoiler-aware community, and the different product problems faced by platforms such as Audible, Everand, and Fable.

**Status:** Planned
