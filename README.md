# Product Portfolio

This portfolio brings together product patterns from my professional experience, products I've shipped independently, and studies I'm using to build deeper fluency in new domains.

---

# Professional Product Cases

My professional experience spans B2C and B2B products, from scaling consumer loyalty across ecommerce and POS to building a 0→1 partner rewards platform.

These cases use generalized examples to show some of the product decisions behind that work.

## 01 / [B2B Commerce & Rewards](https://github.com/rtfenter/B2B-Commerce-and-Rewards)

### Order ≠ Earned

In invoiced B2B commerce, an order can be completed with **$0 collected at checkout**. That means placing an order and earning usable reward value cannot safely represent the same event.

**Order → Invoice → Pending Validation → Available**

**The decision:** Separate recognition of qualifying activity from availability of usable value.

This gives the partner acknowledgement that qualifying activity occurred while giving the business time to validate the underlying financial activity before creating spendable value.

**What I'd measure:** straight-through validation rate, validation accuracy, time to availability, and exception rate.

---

## 02 / B2C Commerce & Loyalty

### Purchase ≠ Final Transaction

A customer's transaction doesn't necessarily end at checkout. They can earn rewards, redeem value, and later reverse some or all of the transaction through a return or refund.

**Customer:** Purchase → Earn → Redeem → Return  
**System:** Transaction → Reward Ledger → Adjustment → Reconciliation

**The decision principle:** Customer-facing reward state and underlying financial state should remain explainable and reconcilable throughout the transaction lifecycle.

That means defining deterministic behavior for partial returns, promotional earning, previously redeemed value, adjustments, and negative balances without making the customer experience feel like an accounting system.

**What I'd measure:** reconciliation accuracy, adjustment exceptions, incorrect reward balances, and reward-related customer contacts.

---

## 03 / Engagement & Incentives

### Enrollment ≠ Activation

Enrollment gives someone access to a product or program. It doesn't mean they've experienced its value.

**Enrolled → Activated → Engaged → Retained**

**The decision principle:** Start with the behavior the product is trying to change, not the incentive.

A first qualifying action, repeat behavior, and re-engaging a lapsed user are different objectives. Each requires its own audience, eligibility, incentive, success event, and measurement window.

The distinction that matters is between **offer performance and behavior change**. Claims and clicks show interaction with an offer. They don't establish that the incentive created incremental engagement.

**What I'd measure:** incremental qualifying behavior and progression through the engagement lifecycle, with incentive cost, cannibalization, margin impact, and opt-outs as guardrails.

---

## 04 / Platform Lifecycle & Controls

### One Account State, Multiple Consequences

A simple state like **Suspended** can affect commerce, billing, rewards, user access, and internal operations differently.

**Account State → Product Rules → User Access → Internal Operations → Audit**

**The decision principle:** Define lifecycle states by their effects, not just their names.

Suspension requires decisions about what a customer can still see and do, whether existing obligations or value remain accessible, which new actions are blocked, who internally can change the state, and what must be retained for audit.

It also requires separating **account state from user authority**. An account's lifecycle state and an individual user's permissions answer different product questions.

**What I'd measure:** state propagation failures, manual corrections, support escalations, unauthorized actions, and time to resolve lifecycle exceptions.

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

Product studies focused on player behavior, progression, accomplishment, and how product decisions change across different player audiences.

## Audience-Aware Game Product Framework

How differences between player audiences change the product decisions surrounding the same game or platform experience.

→ [View project](https://github.com/rtfenter/Audience-Aware-Game-Product-Framework)

## Hades II Progression System Study

A product study of progression, rewards, and player motivation in *Hades II*.

→ [View project](https://github.com/rtfenter/Hades-II-Progression-System-Study)

## Player Accomplishment Product Study

A study of how game platforms represent accomplishment and how those systems shape player motivation and behavior.

→ [View project](https://github.com/rtfenter/Player-Accomplishment-Product-Study)

---

# Books, Audio & Community

## Dungeon Crawler Carl Product Study

**Discovery · Series Engagement · Audio · Community**

A planned consumer product study using *Dungeon Crawler Carl* to explore the product experience surrounding a series, not just the content itself.

The study will look at discovery, moving through a series, reading vs listening, fandom, spoiler-aware community, and the different product problems faced by platforms such as Audible, Everand, and Fable.

**Status:** Planned
