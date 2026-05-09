# 11. Tell me about a time you improved reliability in a system

In one of our seller-facing systems, we noticed that some critical workflows were failing silently before users reported them.

To improve reliability, I worked on adding proactive monitoring using Splunk and Catchpoint.

We tracked API latency, failures, workflow completion rates, and user-impacting issues across critical flows.

This helped us detect problems much earlier and reduced customer impact significantly.

The experience taught me that reliability is not only about preventing failures, but also about detecting and responding to issues quickly.

---

# 12. Tell me about a time you had to balance speed vs quality

There was a feature that had aggressive delivery timelines, but some parts still needed better monitoring and edge-case handling.

Instead of delaying the entire release, we identified the most critical functionality needed for launch and implemented it with proper safeguards.

For lower-risk improvements, we planned phased follow-up releases.

This allowed us to deliver on time while still maintaining operational safety and system stability.

I think balancing speed and quality is usually about prioritizing risks intelligently rather than choosing one over the other.

---

# 13. How do you handle situations where requirements keep changing?

I try to stay flexible while keeping the overall business goal in focus.

When requirements change frequently, I first identify whether the core problem statement itself has changed or only implementation details are evolving.

I also prefer breaking work into smaller milestones so that changes can be absorbed without large rewrites.

Regular communication with PMs and stakeholders is very important in such situations because early clarification prevents unnecessary rework later.

---

# 14. Tell me about a time you optimized developer productivity

During platform upgrade and modernization work, we started leveraging tools like GitHub Copilot for repetitive implementation tasks and boilerplate generation.

This helped reduce manual effort for routine coding tasks and allowed engineers to focus more on logic, design, and debugging.

We also improved development workflows around dependency upgrades and service standardization.

As a result, development speed improved and technical debt reduction became much smoother across services.

---

# 15. Describe a situation where you had to debug an issue without much information

There was a production issue where APIs were intermittently slowing down, but logs initially did not show clear failures.

I started by narrowing the scope using request timing patterns, traffic correlation, and dependency analysis.

Then I checked thread dumps and identified blocking operations causing thread contention during peak traffic.

Even though the initial signals were unclear, systematically reducing possibilities helped isolate the root cause.

That experience reinforced the importance of structured debugging under uncertainty.

---

# 16. Tell me about a time you improved scalability

During REST to GraphQL migration work, one goal was improving backend efficiency and reducing unnecessary data transfer.

We redesigned API interactions to fetch only required fields instead of returning large fixed payloads.

This improved query flexibility, reduced backend load, and improved response times significantly.

The project helped improve scalability while also providing a better developer and user experience.

---

# 17. How do you handle feedback during code reviews?

I try to approach feedback with an open mindset because reviews are meant to improve both the code and engineering discussions.

Even if I initially disagree with feedback, I first try to understand the reasoning and broader concerns behind it.

Sometimes reviewers bring historical context, production learnings, or edge cases that may not be immediately obvious.

I think healthy engineering teams are built on respectful technical discussions rather than ego-driven debates.

---

# 18. Tell me about a time you had to coordinate across teams

During staging deployments, multiple services owned by different teams had dependencies on each other.

Lack of coordination was sometimes causing unstable environments and difficult debugging situations.

I proactively communicated with engineers across teams, aligned deployment timing, and increased visibility around dependency changes.

This significantly improved deployment stability and reduced confusion during validation.

It showed me how strong communication can directly improve engineering efficiency.

---

# 19. What do you do when you don’t know the answer to a problem?

If I don’t know something, I first try to clearly define what exactly is unknown instead of panicking.

Then I gather information through documentation, logs, code analysis, discussions with teammates, or experimentation.

I believe strong engineers are not people who know everything already, but people who can learn and troubleshoot efficiently.

I’m comfortable admitting when I don’t know something, but I also make sure I actively work toward finding the answer quickly.

---

# 20. Tell me about a time you reduced technical debt

During platform modernization efforts, we worked on decommissioning parts of a legacy seller platform and migrating functionality to modern microservices.

The older system had accumulated maintenance overhead and slower development cycles over time.

We gradually migrated traffic, removed obsolete components, and standardized newer service patterns.

This reduced long-term technical debt, improved maintainability, and made future development faster and more reliable.

It also improved operational stability by simplifying the overall architecture.
