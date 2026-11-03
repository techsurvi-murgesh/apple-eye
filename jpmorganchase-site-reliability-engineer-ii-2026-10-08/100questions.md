# 100 Interview Questions — Site Reliability Engineer II (JPMorgan Chase) — 2026-10-08

Target stack: SRE principles, SLO/SLI/error budgets, observability, incident triage & RCA, toil elimination, automation, Dynatrace/Grafana/Splunk/Geneos, AWS, Kubernetes, Kafka/MQ, relational DB (SQL Server/Oracle/DB2), capacity management, performance monitoring, CI/CD, Agile, Linux/Windows, AI/Copilot-assisted operations.

## SRE Principles (1-18)

1. What is Site Reliability Engineering and how does it differ from traditional ops?
2. Explain SLI, SLO, and SLA with a concrete example.
3. What is an error budget and how do you use it to make release decisions?
4. How do you choose good SLIs for a service?
5. How do you set an SLO when you have no baseline?
6. Explain toil and how you identify and eliminate it.
7. How do you balance reliability work with feature delivery?
8. What is the difference between MTTR, MTTD, MTBF, and MTTF?
9. How do you run a blameless postmortem and produce an RCA?
10. How do you build a culture of reliability within a team?
11. Explain the concept of risk and how you manage it in changes.
12. What is a "single point of failure" and how do you remove it?
13. How do you design for graceful degradation?
14. Explain idempotency and why it matters for reliability.
15. How do you approach capacity planning for a growing service?
16. What are the four golden signals of monitoring?
17. How do you define and monitor availability vs latency?
18. How do you prioritize reliability risks from operational signals?

## Incident Management & Troubleshooting (19-36)

19. Walk through triaging a P1 incident from alert to resolution.
20. How do you run an incident bridge and communicate with stakeholders?
21. Difference between mitigation and root cause fix; which comes first?
22. How do you systematically debug a distributed system failure?
23. Explain the "five whys" and when to use it.
24. How do you investigate a latency spike across a microservice chain?
25. How do you troubleshoot intermittent/flaky failures?
26. How do you use logs, metrics, and traces together during an incident?
27. How do you handle a noisy alert that keeps firing without cause?
28. What is a runbook and what makes a good one?
29. How do you reduce MTTR in a large enterprise?
30. How do you decide whether to roll back or roll forward?
31. How do you handle cascading failures and circuit breakers?
32. How do you debug a memory leak in production?
33. How do you debug a connection pool/thread pool exhaustion?
34. How do you investigate a database deadlock in production?
35. How do you handle an incident caused by a bad deployment?
36. How do you write a post-incident action plan that actually gets done?

## Observability & Monitoring Tools (37-52)

37. Explain the difference between monitoring and observability.
38. Explain instrumentation: metrics, logs, traces, and events.
39. How do you instrument an application with custom metrics?
40. Explain distributed tracing and span context propagation.
41. How do you use Dynatrace for APM and root cause analysis?
42. How do you use Splunk for log search and alerting?
43. How do you build Grafana dashboards that operators actually use?
44. What is Geneos and how does it fit enterprise monitoring?
45. How do you use Prometheus and PromQL for infrastructure metrics?
46. How do you design alerting to avoid alert fatigue?
47. How do you set up anomaly detection and dynamic thresholds?
48. How do you monitor Kafka consumer lag and broker health?
49. How do you monitor MQ queue depth and backlogs?
50. How do you implement SLO-based alerting (burn-rate alerts)?
51. How do you ensure monitoring covers dependencies and upstream/downstream systems?
52. How do you use AI/Copilot to speed up incident triage and post-incident analysis?

## Cloud, Kubernetes & Infrastructure (53-68)

53. Explain AWS compute, storage, networking, and managed services.
54. How do you design a highly available, fault-tolerant AWS architecture?
55. Explain IAM and least-privilege in a cloud environment.
56. How do you implement auto scaling and elasticity?
57. Explain VPC, subnets, security groups, and load balancers.
58. How do you use Terraform for reliable infrastructure provisioning?
59. How do you detect and remediate infrastructure drift?
60. Explain Kubernetes architecture and control plane components.
61. How do you troubleshoot a pod in CrashLoopBackOff or Pending?
62. Explain liveness, readiness, and startup probes.
63. How do you do rolling updates and rollbacks in Kubernetes?
64. How do you manage resource requests/limits and HPA?
65. How do you debug service-to-service networking in Kubernetes?
66. How do you manage persistent storage and stateful workloads?
67. How do you design for multi-AZ and multi-region resilience?
68. How do you manage secrets and configuration securely?

## Code, Automation & CI/CD (69-84)

69. What makes code "high quality, maintainable, and robust"?
70. How do you write reliable code for automation tooling?
71. Python vs Java for SRE tooling—when do you pick which?
72. How do you design a service to be observable from the start?
73. How do you eliminate toil with automation?
74. How do you write idempotent automation scripts?
75. Explain CI and CD and the stages of a good pipeline.
76. How do you test infrastructure and automation code?
77. How do you gate deployments on tests and checks?
78. How do you do blue/green or canary releases?
79. How do you implement fast, safe rollback?
80. How do you use Git branching and code review for reliability changes?
81. How do you manage configuration across environments?
82. How do you integrate security scanning into the pipeline?
83. How do you run chaos experiments and game days?
84. How do you measure the impact of an automation change?

## Databases, Capacity & Performance (85-94)

85. Explain relational database fundamentals and indexing.
86. How do you optimize a slow SQL query (SQL Server/Oracle/DB2)?
87. How do you monitor database performance and capacity?
88. Explain replication, failover, and high availability for databases.
89. How do you do performance testing and load testing?
90. How do you identify bottlenecks (CPU, memory, I/O, network, locks)?
91. How do you perform capacity management for large systems?
92. How do you plan for growth and cost efficiency?
93. How do you tune JVM/application performance?
94. How do you benchmark and set performance SLOs?

## OS, Agile & Behavioral (95-100)

95. How do you administer and troubleshoot Linux servers?
96. How do you troubleshoot Windows Server performance issues?
97. How do you work effectively in an Agile environment as an SRE?
98. How do you run small-to-medium projects independently?
99. Describe a time you eliminated toil or prevented a recurring incident.
100. Why are you a good fit for this Site Reliability Engineer II role at JPMorgan Chase, and what would you improve in your first 90 days?
