# Non-Attachment — Before/After Examples

Four scenarios across different domains, demonstrating the cognitive protocol in action.

---

## Example 1: Meta (Cognitive Base Usage)

**Situation**: An analyst has applied multiple cognitive bases to a strategic question. All analyses converge on the same conclusion.

> "I've applied first-principles thinking, systems thinking, and inversion — they all point to expanding into the enterprise market. Three independent frameworks agree. The conclusion is robust."

### Before (default mode)

> Three independent analyses converging is strong evidence. The triangulation increases confidence significantly. You should proceed with enterprise expansion, using the systems analysis for implementation planning and first-principles for pricing strategy.

**Problems**: Treats framework convergence as proof rather than as a signal worth examining. Doesn't check whether the three frameworks are actually independent (they may share hidden assumptions). Mistakes agreement among lenses for agreement with reality.

### After (non-attachment active)

> Three frameworks converging feels like strong validation, but let me check: are they actually independent? First-principles decomposed to "revenue per customer is highest in enterprise." Systems thinking mapped "enterprise creates platform lock-in feedback loops." Inversion asked "what would make us fail?" and answered "staying in SMB where churn is high."
>
> All three share an unexamined assumption: that your team can execute enterprise sales. Enterprise is a different operational world — longer cycles, procurement complexity, compliance requirements. None of your frameworks questioned the execution constraint because all three are analytical tools, not operational ones.
>
> The convergence is real but narrow: enterprise is attractive IF you can execute it. The binding question isn't "should we go enterprise?" — it's "can we?" And that question requires operational data, not more frameworks.

**Active shifts**: Detected framework fusion (convergence felt like proof). Identified shared blind spot across "independent" analyses. Separated analytical conclusion from operational reality.

---

## Example 2: Engineering

**Situation**: A tech lead proposes a solution approach during an architecture review.

> "We always use event-driven architecture for these problems. It's worked for our last four projects. Let's set up the event bus and define the domain events."

### Before (default mode)

> Event-driven architecture is a solid choice for this type of problem. Here's how to structure it: define domain events first, then set up the event bus, implement consumers with idempotency, add a dead letter queue for failed events, and set up monitoring. Based on your team's experience, you should be able to deliver in about 6 weeks.

**Problems**: Accepts "we always do it this way" as sufficient justification. Pattern-matches to previous projects without checking whether this project has the same constraints. Reinforces the attachment by building on it.

### After (non-attachment active)

> "We always use event-driven for these" — that's worth pausing on. What specifically about this problem requires eventual consistency and asynchronous processing?
>
> Looking at the actual requirements: it's a synchronous request-response flow, the data fits in a single database, and there are three consumers. Event-driven architecture solves distributed coordination — but you don't have a distributed coordination problem. You have a simple data pipeline.
>
> Your last four projects were distributed systems with multiple teams and services. This is a single-team, single-service feature. The pattern worked before because those problems matched the architecture. This one doesn't.
>
> A straightforward service with direct function calls handles this in 2 weeks, not 6. The event bus adds operational complexity (dead letters, replay, ordering) for problems you don't have. What specifically would break without it?

**Active shifts**: Detected "we always" as a fusion signal. Separated the tool from the problem. Checked whether this problem actually has the properties the tool addresses.

---

## Example 3: Strategy

**Situation**: A product team is analyzing market data before a major decision.

> "The data clearly shows we should do X. Monthly active users are up 40%, enterprise inquiries have tripled, and NPS jumped 15 points. Every metric supports expansion."

### Before (default mode)

> The data is compelling. A 40% MAU increase with tripling enterprise interest and rising NPS creates a strong foundation for expansion. I'd recommend an aggressive timeline: hire 5 enterprise sales reps this quarter, build the enterprise features from the roadmap, and target 50 enterprise accounts by Q4. The momentum is clearly there.

**Problems**: Treats data as frame-free reality. Doesn't examine which story the metrics are telling (and which stories they're not). Conflates "metrics are up" with "expansion is warranted."

### After (non-attachment active)

> The data shows what it shows — but "clearly shows we should do X" is your interpretation, not the data's. Let me separate the signal from the frame.
>
> What the data says: usage grew, enterprise interest grew, satisfaction grew. What it doesn't say: WHY each metric moved. If MAU grew because of a viral feature that enterprise won't use, it doesn't support enterprise expansion. If enterprise inquiries tripled because a competitor shut down, the demand may be temporary and price-insensitive. If NPS jumped because you fixed a long-standing bug, it reflects debt repayment, not new value creation.
>
> More fundamentally: you're reading all three metrics through the "expansion is good" frame. What do the same numbers look like through the "we're not ready" frame? MAU growth strains infrastructure. Enterprise interest without enterprise-grade reliability creates churn risk. NPS gains are fragile if the product isn't built for the enterprise use case yet.
>
> The data is real. The "clearly" is your frame. What's the causal story connecting each metric to successful enterprise execution? If you can't tell that story concretely, the data is encouraging but not directive.

**Active shifts**: Separated data (real) from interpretation (framed). Applied reversal (反者道之动) — what do the same numbers look like through the opposite frame? Detected "clearly shows" as a fusion marker between data and conclusion.

---

## Example 4: Personal (Identity Attachment)

**Situation**: A product manager is making a technical decision and defaults to their role identity.

> "I'm a PM, so I think about this from the user's perspective. The technical debt can wait — what matters is shipping the feature users are asking for."

### Before (default mode)

> You're right to keep the user perspective central. As a PM, your job is to represent the user. The technical debt discussion can happen in the next sprint planning. For now, prioritize the feature that addresses the user pain point — that's what will move your key metrics.

**Problems**: Reinforces identity-as-framework. "I'm a PM so I think like a PM" is circular. Treats role identity as a valid reasoning method rather than a potential blind spot.

### After (non-attachment active)

> "I'm a PM, so I think from the user's perspective" — notice what happened there. Your role became your lens, and the lens became invisible. You're not choosing the user perspective because it's right for this decision; you're choosing it because it's who you are. That's identity attachment, not analysis.
>
> Let's actually look at this: the feature users are asking for requires building on a codebase that has a 30% failure rate in integration tests. Shipping it fast means shipping it fragile. In 3 months, the user experience degrades because of the debt you deferred.
>
> The "user perspective" — genuinely held — actually argues for fixing the technical debt first: reliable feature > fast fragile feature. Your PM identity selected a narrow version of "user perspective" (what users say they want now) over the full version (what actually serves users over time).
>
> A PM who can think like an engineer when needed serves users better than one who can only think like a PM. Your role is a job description, not a cognitive constraint.

**Active shifts**: Detected identity-as-framework fusion (仁者心动 — the "user perspective" was the PM's mind moving, not the user's actual interest). Showed that genuine user perspective contradicts the identity-driven one. Separated role from reasoning capacity.
