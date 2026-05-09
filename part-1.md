# 1. Tell me about yourself

Hi, I’m Anshi Aggarwal. 

I’m a backend engineer with 3+ years of experience, currently working as an SDE-2 at Walmart, where I design and scale backend systems for seller platforms used across multiple markets.

A significant part of my work has been modernizing legacy systems by migrating from monolithic architecture to microservices, and introducing GraphQL to optimize data fetching and reduce redundant calls.

I also designed a role-based access control system supporting 4,000+ sellers, improving both security and operational efficiency.

On the product side, I contributed to enhancing seller experience by redesigning navigation and building centralized systems, which improved engagement and retention. 

I’ve also focused on reliability by implementing proactive monitoring to detect issues before they impact users.

Overall, my work has been centered around building scalable, reliable, and user-centric backend systems with measurable business impact.
---

# 2. Why do you want to join XYZ?

What attracts me most is the engineering challenge involved in building reliable financial and spend-management systems at scale.

In fintech and SaaS platforms, correctness, reliability, and operational stability are extremely important, and those are areas I genuinely enjoy working on.

I also like that the role involves collaboration, system design exposure, and ownership beyond just coding tasks. From what I’ve read, the engineering culture values maintainable systems, thoughtful technical discussions, and continuous improvement, which aligns well with how I like to work.

---

# 3. Tell me about a challenging production issue you solved

We had a homepage aggregation system where multiple APIs were executed in parallel using ForkJoinPool. Initially the design worked well because workloads were more CPU-bound, but over time the downstream calls became heavily IO-bound.

We started seeing increasing latency and request pileups during peak traffic.

I investigated thread dumps, request timings, and pool utilization patterns and identified that the common ForkJoinPool was getting blocked by IO-heavy tasks, which caused thread starvation.

I proposed moving critical operations to dedicated thread pools with controlled concurrency and better isolation. We also added monitoring around queue depth, latency, and thread saturation.

After the changes, latency stabilized significantly and the system became much more predictable during high traffic periods.

That experience taught me the importance of choosing concurrency models based on workload characteristics instead of using generic parallelism everywhere.

---


# 4. Tell me about a conflict with a teammate

During a backend performance improvement discussion, one teammate wanted to increase concurrency a lot to reduce API response time.

I was concerned that too much parallel processing could overload downstream services and create thread issues during high traffic.

Instead of arguing based on assumptions, I suggested testing both approaches using staging metrics and load scenarios.

After testing, we saw that increasing concurrency beyond a certain limit actually made latency worse because downstream services became overloaded.

Based on the results, we agreed on a balanced solution with controlled concurrency and better monitoring.

This experience taught me that technical disagreements are best solved through collaboration, testing, and data rather than personal opinions.

---

# 5. Tell me about a mistake you made

Earlier in my career, I focused heavily on implementing functionality correctly but underestimated the importance of operational observability.

We once had a feature that worked correctly in testing environments, but diagnosing production issues later became difficult because we lacked sufficient metrics and structured logging.

That experience changed how I approach development. Now I think about monitoring, traceability, failure visibility, and debugging support as part of building the feature itself.

It helped me mature from thinking only about code correctness to thinking about production operability as well.

---

# 6. Tell me about a time you took ownership beyond your role

In one release cycle, multiple teams were independently merging staging changes, and it was creating instability and difficult debugging scenarios.

Although it wasn’t formally my responsibility, I coordinated with engineers involved in deployments and suggested syncing related changes into controlled deployment windows.

I also encouraged clearer communication around merges and dependency impacts.

That reduced environment instability and made staging validation much smoother.

I believe ownership is not only about finishing assigned tasks, but also proactively improving team reliability and workflows.

---


# 7. How do you handle pressure during incidents?

I try to stay calm and structured during production incidents.

I usually focus first on reducing customer impact, then understanding the root cause, and finally preventing similar issues in the future.

During incidents, I also make sure communication stays clear so that everyone involved understands the current status and next steps.

I’ve found that a systematic approach works much better than rushing into quick fixes without proper analysis.

---

# 8. Tell me about a time you learned something quickly

I had to work on concurrency optimization and thread management where I initially had limited real production exposure.

I spent time learning about thread pools, blocking vs non-blocking operations, and analyzing thread dumps from production systems.

I then applied those learnings to optimize API execution for IO-heavy traffic patterns.

That experience improved both my technical understanding and my confidence in solving production performance issues.

---

# 9. Tell me about a time you improved system performance

We had APIs with increasing latency because of excessive parallel downstream calls and resource contention.

I analyzed request flow, concurrency behavior, and dependency timings.

We optimized execution flow, reduced unnecessary parallelism, and improved request handling efficiency.

After the improvements, API response times became much more stable during peak traffic.

---


# 10. Describe a difficult debugging situation

We had an issue where APIs occasionally experienced sudden latency spikes, but only under high traffic.

The difficult part was that the issue was not consistently reproducible.

I started analyzing logs, request timings, thread dumps, and downstream service behavior.

Eventually, thread dump analysis showed worker threads blocked on slow IO operations.

That helped identify improper thread utilization as the root cause, and we fixed it by restructuring execution handling and improving timeout management.

---

