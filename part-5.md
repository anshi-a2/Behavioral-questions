# 21. Tell me about a time you put customer impact above technical preference

During a backend optimization discussion, there were multiple possible architectural improvements we could make.

Some options were technically cleaner, but they would have delayed the release significantly and impacted seller workflows.

Instead of over-engineering the solution, we focused on the changes that would solve the most critical customer pain points quickly while still keeping the system stable and maintainable.

We later improved the architecture incrementally after the immediate customer issues were resolved.

That experience taught me that engineering decisions should ultimately support customer value, not just technical perfection.

---

# 22. Tell me about a time you showed strong ownership

We were facing recurring staging instability because multiple dependent services were being deployed independently.

Although it was not officially assigned to me, I took initiative to coordinate deployment communication across teams.

I helped align deployment windows, tracked dependencies more carefully, and improved visibility around changes being merged.

As a result, staging became much more stable and debugging effort reduced significantly.

For me, ownership means proactively solving problems that affect the team or customers, even if they are outside strict task boundaries.

---

# 23. Tell me about a time you had to make a business-driven technical decision

During a system improvement discussion, there was an option to redesign a larger part of the architecture for long-term scalability.

However, the business priority at that time was delivering a critical seller-facing capability within a shorter timeline.

Instead of attempting a complete redesign immediately, we implemented a scalable intermediate solution that solved the immediate business need while still supporting future improvements.

This helped balance engineering quality with business urgency.

I’ve learned that good engineering decisions often involve understanding both technical and business tradeoffs.

---

# 24. Describe a situation where you had to earn trust from stakeholders

During one project involving backend workflow improvements, there were concerns about rollout safety because the changes affected important seller operations.

I made sure to communicate progress regularly, explain technical tradeoffs clearly, and provide visibility into testing and monitoring plans.

We also rolled out the changes gradually with proper observability.

Because stakeholders felt informed and confident in the rollout strategy, collaboration became much smoother and the deployment succeeded without major issues.

That experience showed me how transparency and communication help build trust.

---

# 25. Tell me about a time you took a difficult decision under pressure

During a production issue involving increased latency, we had to decide whether to continue investigating live or immediately roll back a recent configuration change.

Even though the root cause was not fully confirmed yet, the customer impact was increasing.

I supported rolling back first to stabilize the system and then continuing deeper analysis afterward.

The rollback reduced latency quickly, and later investigation confirmed the configuration was contributing to the issue.

That experience reinforced that during incidents, reducing customer impact should come before trying to prove technical assumptions.

---

# 26. Tell me about a time you improved something proactively before it became a bigger problem

While analyzing production metrics, I noticed growing thread utilization and increasing latency trends during traffic spikes.

The system was still functioning, but the patterns suggested future scalability issues.

I proactively investigated thread behavior and identified that the execution model was becoming inefficient for IO-heavy workloads.

We improved concurrency handling before the issue turned into a major production outage.

This helped improve long-term stability and prevented larger customer-facing problems later.

---

# 27. Describe a time when you had to influence people without authority

During deployment coordination improvements, I did not have formal ownership over all involved services or teams.

Instead of forcing process changes, I explained the operational pain points using examples from previous staging failures and debugging difficulties.

I also suggested practical improvements that would make everyone’s work easier rather than adding unnecessary process overhead.

Over time, teams adopted the coordinated deployment approach because they saw clear operational benefits.

That experience taught me that influence comes more from trust and practical value than formal authority.

---

# 28. Tell me about a time you balanced customer needs with system limitations

There was a request for additional flexibility in a seller workflow, but implementing it without limits could have significantly increased backend complexity and operational risk.

Instead of directly rejecting the requirement, we worked with stakeholders to identify the most important customer use cases.

We then designed a controlled implementation that solved the primary customer problem while keeping the system maintainable and scalable.

I believe strong engineering involves finding practical solutions that balance customer value with technical sustainability.

---

# 29. Tell me about a time you handled a situation where priorities suddenly changed

There have been situations where production incidents or urgent business requests suddenly shifted team priorities.

In such cases, I first reassess task urgency, dependencies, and customer impact.

I also communicate clearly with stakeholders about timeline adjustments and tradeoffs.

I try to remain flexible without losing focus on long-term stability and delivery quality.

Being adaptable while staying organized is very important in fast-moving engineering environments.

---

# 30. Tell me about a time you improved a system from a business perspective, not just technically

During navigation redesign work for seller workflows, the focus was not only technical modernization but also improving usability for sellers.

We redesigned information hierarchy and access patterns so sellers could find critical workflows faster.

This reduced search effort, improved workflow efficiency, and contributed to higher user retention.

The project reminded me that successful engineering is not only about backend performance, but also about improving actual user experience and business outcomes.
