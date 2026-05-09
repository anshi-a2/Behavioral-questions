# 1. Do you do code reviews? What are the key points you focus on while reviewing?

Yes, I regularly participate in code reviews and I see them as collaborative engineering discussions rather than just approval steps.

Before manual review, I usually encourage running automated checks and AI-assisted review tools first. AI tools help catch basic issues like formatting problems, null handling issues, duplicate logic, simple optimizations, and common security concerns. This allows reviewers to focus more on design and business logic.

During the review, I mainly focus on:
- correctness of implementation,
- readability and simplicity,
- maintainability,
- scalability,
- edge cases and failure handling,
- logging and observability,
- performance impact,
- and test coverage.

I also try to understand the intent behind the change instead of reviewing only line by line.

When giving feedback, I try to keep it constructive and collaborative by explaining the reasoning behind suggestions instead of just pointing out issues.

I believe good code reviews improve both code quality and team learning.

---

# 2. If a PM comes with a very naive requirement, how will you handle it?

I first try to fully understand the business problem behind the requirement rather than directly rejecting the idea.

Sometimes requirements may sound technically unrealistic initially, but there is usually an actual customer or business pain point behind them.

I usually ask clarifying questions around:
- expected user behavior,
- scale,
- performance expectations,
- edge cases,
- and business priority.

Then I explain the technical challenges and tradeoffs in simple language instead of using too much technical jargon.

If needed, I suggest alternative approaches that achieve the same business goal in a more scalable or maintainable way.

I think the goal is not to say “this won’t work,” but to collaborate and find the best practical solution together.

---

# 3. When a senior questions your LOE estimation, what should you do?

If a senior engineer questions my LOE estimate, I treat it as a healthy discussion rather than taking it personally.

I first explain my assumptions clearly, including:
- dependencies,
- unknowns,
- testing effort,
- operational impact,
- and rollout considerations.

Sometimes differences happen because people are considering different levels of complexity.

I also listen carefully to their perspective because they may have historical context or system knowledge that I may not be fully aware of.

If needed, I break the task into smaller components and revisit the estimation collaboratively.

I think good estimation discussions are about alignment and risk understanding rather than proving who is right.

---

# 4. What is the dumbest production issue you caused? How did you resolve it?

Earlier in my career, I once pushed a configuration-related change that looked safe in lower environments but behaved differently under production traffic.

The issue increased downstream API retries and caused temporary latency spikes.

As soon as we noticed abnormal metrics and alerts in monitoring dashboards, I immediately started investigating logs and traffic behavior.

We quickly rolled back the configuration to stabilize the system and then performed detailed root cause analysis.

After that, I helped improve rollout validation, monitoring checks, and configuration review practices to reduce similar risks in the future.

That experience taught me the importance of gradual rollouts, production observability, and validating assumptions under real traffic conditions.

---

# 5. Explain any system that you designed end to end

One system I worked on was a centralized contact management platform for seller workflows.

The goal was to allow multiple teams and markets to manage and retrieve seller contact information efficiently.

The backend was built using Java and Spring Boot with REST and GraphQL APIs.

For storage, we used scalable cloud databases and optimized retrieval patterns to reduce latency.

The system supported:
- role-based access,
- filtering and search,
- validation,
- auditability,
- and secure access controls.

We also added monitoring and proactive alerting using Splunk and Catchpoint to track API health and user-impacting issues.

One key challenge was balancing flexibility in GraphQL queries while avoiding over-fetching and maintaining backend performance.

The platform improved operational efficiency and increased engagement for teams using the system.

---

# 6. Why do you want to leave Walmart?

I’ve had a very positive experience at Walmart and I’ve learned a lot there, especially around scalable backend systems, production ownership, and cross-team collaboration.

At this stage, I’m looking for opportunities where I can take on broader engineering ownership and work more deeply on SaaS and fintech-related engineering challenges.

What attracts me to Airbase by Paylocity is the combination of financial workflows, system reliability, scalability, and product impact.

I feel the role aligns strongly with the kind of backend engineering problems I enjoy solving and the direction I want to grow in professionally.

---

# 7. In thread optimization, how do you identify the root cause?

I usually start by observing production symptoms like:
- increased latency,
- request pileups,
- timeout spikes,
- CPU utilization,
- or thread saturation.

Then I analyze:
- thread dumps,
- request traces,
- pool utilization,
- queue sizes,
- downstream dependency timings,
- and blocking patterns.

For example, in one case we observed APIs slowing down during high traffic.

After analyzing thread dumps, we found worker threads blocked on IO-heavy downstream operations while using ForkJoinPool.

That helped identify thread starvation and improper execution model selection as the root cause.

We then redesigned execution handling using dedicated thread pools and controlled concurrency.

I’ve learned that thread issues are usually easier to diagnose when good observability and metrics are already in place.

---

# 8. Tell me about a time you handled ambiguity in requirements

There have been situations where requirements were not fully defined initially, especially for internal workflow systems.

In such cases, I usually start by clarifying the business goals, expected user behavior, and success criteria.

Then I break the problem into smaller functional areas and validate assumptions incrementally with stakeholders.

I prefer iterative alignment rather than making large assumptions upfront.

That approach helps reduce rework and ensures the solution evolves in the right direction.

---

# 9. How do you ensure reliability in backend systems?

I think reliability comes from a combination of good design and operational discipline.

While building backend systems, I focus on:
- proper timeout handling,
- retries with limits,
- monitoring and alerting,
- structured logging,
- graceful failure handling,
- scalability,
- and rollback planning.

I also think observability is extremely important because production systems cannot be improved if behavior is not visible.

In my projects, proactive monitoring using tools like Splunk and Catchpoint helped detect issues early and reduce customer impact significantly.

---

# 10. Tell me about a technical decision you influenced

During backend optimization discussions, there was a proposal to aggressively increase concurrency to reduce latency.

I raised concerns around downstream service pressure and thread exhaustion risks under heavy traffic.

Instead of relying only on assumptions, I suggested validating both approaches using load testing and staging metrics.

The results showed that beyond a certain point, additional concurrency actually degraded performance because downstream services became bottlenecks.

Based on the data, the team agreed on a more balanced concurrency model with better isolation and monitoring.

That experience reinforced the importance of data-driven technical decisions and collaborative discussions.
