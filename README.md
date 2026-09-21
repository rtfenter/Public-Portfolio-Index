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

→ [View case study](https://github.com/rtfenter/Platform-Lifecycle-Controls) · [Launch interactive demo](https://rtfenter.github.io/B2C-Loyalty-Product-Study/#platform)

---

### 05 / Shipping Through Imperfect Systems

## When the Ideal Product Isn't the Shippable Product

A rewards product can have clear business rules and still depend on systems, data, and operational capabilities that weren't designed to support them.

**The challenge:** Decide what can be automated confidently, what needs controlled operations today, and what should preserve a path to automation later.

The work required balancing **Partner experience · Financial integrity · Legal requirements · Data reliability · Technical feasibility · Operational burden · Future extensibility** while moving from pilot toward broader launch.

**The principle:** Automation isn't the objective. Reliable execution is.

→ [View case study](https://github.com/rtfenter/Shipping-Through-Imperfect-Systems)

---

*These cases draw from product patterns I've encountered professionally. Companies, transactions, systems, and implementation details are generalized or fictionalized.*

---

# Selected Work

## Girl Dinner Mode

**0→1 Consumer Product · Personalization · Decision Support**

A personalized meal-decision app I designed, built, and shipped for iOS.

Girl Dinner Mode learns from user behavior and preferences to help answer a deceptively difficult question: **what should I eat?** The product includes personalized meal discovery, weekly planning, grocery organization, and lightweight daily experiences without calorie tracking, streaks, or guilt.

→ [Girl Dinner Mode](https://girldinnermode.com)

---

## Personalization & Discovery

**Profile Formation · Evolving Intent · Recommendations · ML & AI Product Decisions**

How should a personalization system learn about someone without treating its current understanding of them as permanent truth?

The study follows the same user from cold start through an established personalized experience, separating **what the user actually did, what the system inferred, and what the product decided to show next**.

It explores low-burden cold start, durable vs emerging interests, signal strength and scope, discovery and experience composition, then examines how a PM should reason about ML optimization, experiment tradeoffs, deterministic product policy, and where semantic AI actually adds value.

**The principle:** Evidence is fact. Inference is a hypothesis. Recommendation is a decision.

→ [View case study](https://github.com/rtfenter/Personalization-and-Discovery) · [Launch interactive demo](https://rtfenter.github.io/Personalization-Discovery-Lab/)

---

# Games

These studies use games and gaming platforms to explore player motivation, progression, accomplishment, audience behavior, and how evidence about behavior should inform product decisions.

### 01 / Player Accomplishment Product Study

## Who Decides What Represents a Player?

Xbox Achievements and PlayStation Trophies can record similar behaviors while making different aspects of accomplishment salient. The study started as a platform comparison and became a question about what gets lost when years of player behavior are compressed into a universal score.

**The product decision:** Preserve the verified accomplishment system, but let players curate a limited set of verified accomplishments that represent what matters to them.

**The principle:** The platform verifies what happened. The player decides what represents them.

→ [View case study](https://github.com/rtfenter/Player-Accomplishment-Product-Study)

---

### 02 / Progression & Player Agency

## How Progression Creates Meaningful Choice

*Hades II* gives players more power, options, and control over time without allowing progression to eliminate the uncertainty and tradeoffs that make individual runs meaningful.

**The product principle:** Progression can relax a constraint without eliminating the thing that made the constraint meaningful.

The study uses Arcana and Grasp to examine access, acquisition, capacity, resource economics, player agency, and how telemetry should be interpreted before changing progression balance.

→ [View case study](https://github.com/rtfenter/Progression-Player-Agency)

---

### 03 / Player & Audience Experience

## When Audience Evidence Should Change a Game Decision

Game telemetry describes the person holding the controller, but games can also have meaningful audiences who watch for mastery, narrative, suspense, community, discovery, or relaxation.

**The product decision:** Treat audience experience as an additional evidence set, not an optimization target.

The framework asks whether player and audience evidence align or diverge, then maps that to four responses: **Protect · Separate · Investigate · Improve.**

→ [View case study](https://github.com/rtfenter/Player-Audience-Experience)

---

### 04 / Access and Ownership Product Study

## When Ownership Doesn't Mean Usability

Xbox Game Pass can give a player access to a base game while allowing them to purchase add-on content separately. If access to the base game later disappears, the player can still own the add-on without being able to use it.

**The product decision:** Model acquisition, base-game access, and dependent-content usability separately, evaluating all applicable access grants before changing the player experience.

**The principle:** Losing one access grant should affect usability only when no other valid grant satisfies the prerequisite.

The study uses a bounded Game Pass scenario to examine subscription and purchase-based access, dependent content, recovery context, conflicting system states, and how to communicate an unusable purchase without implying that ownership was lost.

→ [View case study](https://github.com/rtfenter/Access-and-Ownership-Product-Study)

---

# Creators, Content & Community

### 01 / Account Onboarding & Intent

## Designing Onboarding Around User Intent

A solo founder can be the business owner, content creator, and person represented by the account at the same time. Using Instagram as the case environment, this study examines what happens when real-world intent doesn't map cleanly to a platform's account classifications.

**The product decision:** Capture lightweight, persistent intent before asking users to navigate the professional account model.

The proposed model separates **intent, next steps, and outcomes**, allowing the platform to use what someone is trying to accomplish as context while preserving whatever account classifications, eligibility rules, and policies still need to exist underneath.

**The principle:** Users shouldn't need to understand a platform's internal taxonomy before the platform can understand what they're trying to accomplish.

→ [View case study](https://github.com/rtfenter/Account-Onboarding-and-Intent)

---
