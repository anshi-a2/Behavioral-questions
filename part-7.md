# 41. How are tasks usually distributed within a team?

In my experience, task distribution is usually a collaborative process during sprint planning or backlog discussions rather than tasks being assigned randomly.

The team reviews:
- business priority,
- complexity,
- dependencies,
- timelines,
- and ownership areas.

Tasks are generally distributed based on experience level, system knowledge, and current bandwidth.

For example:

- **SDE 1 / Junior Engineers** usually handle smaller scoped tasks such as:
  - API enhancements,
  - bug fixes,
  - unit tests,
  - UI/backend integration support,
  - smaller database changes,
  - or monitoring/dashboard updates.

  These tasks help them build system understanding while still contributing meaningfully.

- **SDE 2 Engineers** generally take ownership of medium-to-large features end to end. This includes:
  - designing APIs,
  - handling business logic,
  - coordinating with dependent services,
  - performance optimization,
  - rollout planning,
  - debugging production issues,
  - and mentoring junior engineers when needed.

  For example, in my experience I’ve handled backend design discussions, GraphQL migrations, concurrency optimization, and deployment coordination across services.

- **Senior Engineers** usually focus more on:
  - system design decisions,
  - architecture reviews,
  - scalability planning,
  - cross-team coordination,
  - risk management,
  - and guiding implementation approaches.

  They also help unblock teams during difficult technical situations.

- **Staff or Principal Engineers** are generally more involved in:
  - long-term technical strategy,
  - platform-wide architecture,
  - engineering standards,
  - organization-level scalability problems,
  - and major technical direction decisions.

For larger projects, work is often divided into components such as:
- backend APIs,
- database work,
- monitoring,
- testing,
- infrastructure changes,
- rollout planning,
- and observability improvements.

I also think task distribution should remain flexible because priorities and blockers can change during execution, so teams need to collaborate continuously rather than work in silos.

---

# 42. Who usually decides the LOE estimation in your team?

LOE estimation is generally a collaborative effort between engineers, senior engineers, tech leads, and sometimes product managers.

The engineer working closest to the implementation usually provides the initial estimate because they understand the technical details best.

Then the estimate gets refined through team discussions around:
- dependencies,
- unknowns,
- testing effort,
- production rollout risks,
- and operational considerations.

I think good estimation is less about exact prediction and more about aligning expectations and identifying risks early.

---

# 43. What would you do if a PM pushes for unrealistic timelines?

I would first try to understand the business urgency behind the request.

Then I would clearly explain the technical constraints, risks, dependencies, and potential quality impact of rushing the delivery.

Instead of only saying “this is not possible,” I prefer discussing tradeoffs and alternative approaches such as:
- phased delivery,
- reduced scope,
- MVP approach,
- or prioritizing critical functionality first.

I believe the best outcomes happen when engineering and product work together transparently rather than treating timelines as a conflict.

---

# 44. What if a PM asks for a feature that creates major technical debt?

I would first understand the business value and urgency behind the feature.

Then I would explain the long-term operational or scalability risks in simple terms without overcomplicating the discussion technically.

If the feature is still important from a business perspective, I would try finding a balanced solution — for example:
- a temporary implementation,
- feature flags,
- phased improvements,
- or scoped limitations.

I think engineers should help PMs make informed decisions rather than simply rejecting ideas.

---

# 45. What would you do if two high-priority tasks come at the same time?

I would first evaluate:
- customer impact,
- production risk,
- deadlines,
- dependencies,
- and business urgency.

If both tasks are important, I would communicate transparently with stakeholders about tradeoffs and available bandwidth.

Sometimes the best approach is splitting work across team members or handling immediate mitigation first while planning the second task carefully.

Clear prioritization and communication are extremely important in these situations.

---

# 46. What if your PM changes requirements after development has already started?

Requirement changes happen quite often in real projects.

I first try to understand whether the business problem itself has changed or only implementation details are evolving.

Then I evaluate:
- impact on timelines,
- existing work,
- dependencies,
- and technical feasibility.

I usually communicate the tradeoffs clearly and discuss whether we should:
- adjust scope,
- phase the change,
- or reprioritize tasks.

I think flexibility is important, but so is keeping stakeholders aware of the engineering impact of changes.

---

# 47. What would you do if your teammate is not delivering their part on time?

I would first try to understand whether they are facing technical blockers, unclear requirements, or bandwidth issues.

Instead of immediately escalating, I would try collaborating and helping where possible.

For example:
- clarifying dependencies,
- helping debug issues,
- or redistributing smaller tasks temporarily.

If delays start affecting larger project timelines, then I would communicate the risks transparently with the team so that expectations remain aligned.

I think supportive collaboration works better than blame-driven reactions.

---

# 48. What if your manager asks you to deliver faster but quality may get impacted?

I would explain the risks clearly and discuss possible tradeoffs openly.

Instead of framing it as “quality vs speed,” I usually try finding practical middle-ground solutions like:
- phased rollout,
- prioritizing critical functionality,
- adding monitoring safeguards,
- or reducing lower-priority scope.

I believe engineering teams should move fast, but not in ways that create avoidable operational instability or customer impact.

---

# 49. How do you handle situations where there is no clear ownership?

If ownership is unclear and the issue is affecting delivery or production stability, I usually step in proactively to help coordinate discussions.

I try to identify:
- affected systems,
- dependencies,
- responsible stakeholders,
- and immediate risks.

Even if I am not the official owner, I believe engineers should help move problems toward resolution instead of waiting indefinitely for ownership clarification.

Clear communication and collaboration usually help resolve such situations effectively.

---

# 50. What would you do if a PM rejects your technical recommendation?

I would first try to understand their reasoning and business priorities more deeply.

Then I would explain my concerns using practical examples around scalability, reliability, customer impact, or long-term maintenance costs.

If the final decision still goes in another direction, I would support the team decision professionally while ensuring risks are documented and mitigated as much as possible.

I think strong engineering collaboration requires balancing technical excellence with business realities.
