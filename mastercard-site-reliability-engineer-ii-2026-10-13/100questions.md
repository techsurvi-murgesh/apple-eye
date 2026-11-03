# 100 Interview Questions — Site Reliability Engineer II (Enterprise Monitoring), Mastercard — 2026-10-13

Target profile: Reliability Engineer II on an Enterprise Monitoring team. APM (Dynatrace strongly preferred), Digital Experience / synthetic monitoring, Linux, Python/Perl/bash automation, Kubernetes + AWS/Azure, on-call, incident resolution, internal-customer support and technical documentation.

## APM & Monitoring Platforms (1–18)

1. What is Application Performance Monitoring, and what problem does it solve that infrastructure metrics do not?
2. What is the difference between APM, infrastructure monitoring, and log management?
3. Explain the golden signals. Which one does APM surface that infrastructure monitoring misses?
4. How does APM auto-instrumentation work?
5. Explain distributed tracing: how is trace context propagated across service calls?
6. What is a span, a trace, and a transaction in tracing terms?
7. How do you measure end-to-end latency when a request crosses six services?
8. What is a service map and how is it built?
9. What are exemplars, and how do they link metrics to traces?
10. Explain RED vs USE for defining alerts.
11. How do you choose which metrics to alert on versus which to just display?
12. What is cardinality, and why can high cardinality break a monitoring system?
13. How do you monitor a queue-based system — which metrics matter?
14. Explain error budgets and how they connect monitoring to release decisions.
15. How do you reduce alert fatigue on a noisy service?
16. What is a dashboard that is actually useful during an incident?
17. How do you onboard a new service into a monitoring platform?
18. How do you monitor a Kubernetes cluster itself?

## Dynatrace Deep Dive (19–30)

19. Walk me through deploying the Dynatrace OneAgent in a Kubernetes environment.
20. Explain Dynatrace environment vs cluster vs tenant.
21. How does Dynatrace ActiveGate work, and when do you deploy more than one?
22. How do you define custom metrics and custom events in Dynatrace?
23. What is a custom service, and why would you create one?
24. How do you configure an availability check / synthetic monitor in Dynatrace?
25. Explain Dynatrace problem detection: event correlation and problem management.
26. How do you create a custom dashboard in Dynatrace and share it?
27. How do you write a maintenance window to suppress alerts?
28. Explain how Dynatrace handles third-party APIs and external services.
29. How do you use Dynatrace for Kubernetes application-only monitoring?
30. What Dynatrace concepts do new users most often get wrong?

## Datadog, AppDynamics, New Relic & Comparison (31–40)

31. What are Datadog's core concepts — metrics, traces, logs, and RUM?
32. How does Datadog correlate logs, metrics, and traces?
33. What is an APM span in AppDynamics and what is a Business iQ component?
34. How does New Relic do distributed tracing and what are its agent modes?
35. Compare Dynatrace, Datadog, and New Relic on pricing model. Why does that matter to a customer?
36. When would you recommend a customer move from one APM vendor to another?
37. How do you migrate from one APM tool to another without losing history?
38. What are the trade-offs of a SaaS APM tool vs an open-source stack?
39. How do you monitor a third-party SaaS dependency you do not control?
40. What is Real User Monitoring, and how does it differ from synthetic monitoring?

## Synthetic & Digital Experience Monitoring (41–52)

41. What is synthetic monitoring and why run it alongside RUM?
42. Explain HTTP, HTTPS, and multi-step synthetic checks.
43. How do you choose locations for synthetic probes?
44. What is a heartbeat check and what does it tell you?
45. How do you simulate authenticated user journeys in a synthetic test?
46. How do you detect a regional outage with synthetic monitoring?
47. What is the difference between availability monitoring and performance monitoring?
48. How do you measure page load time and Core Web Vitals?
49. Explain waterfall analysis in a synthetic or RUM result.
50. How do you avoid false positives from synthetic checks?
51. How do you measure end-user experience across devices and browsers?
52. How do you set and report an SLA using synthetic monitoring?

## Linux, Scripting & Automation (53–66)

53. How do you investigate high CPU usage on a Linux host?
54. How do you find a memory leak on a server?
55. Explain load average and what it actually tells you.
56. How do you trace a file descriptor leak?
57. How do you find which process is listening on a port?
58. How do you check network connectivity and DNS resolution from a host?
59. What is strace, and when would you use it?
60. How do you parse and aggregate large log files on the command line?
61. Explain bash arrays, functions, and error handling with `set -euo pipefail`.
62. How do you write an idempotent automation script?
63. How would you automate a Dynatrace or Datadog API configuration change in Python?
64. How do you schedule automation safely with cron or systemd timers?
65. How do you manage credentials in automation scripts?
66. How do you make an automation script safe to run repeatedly in production?

## Kubernetes, AWS & Azure (67–78)

67. How do you deploy a monitoring agent as a DaemonSet, and why a DaemonSet?
68. What is an init container and when would a monitoring agent need one?
69. How does a Kubernetes node expose metrics, and what is the Node Exporter?
70. How do you configure a metrics-server and what are the HPA limits it has?
71. Explain liveness vs readiness probes and what a monitoring agent must get right.
72. How do you monitor AWS — CloudWatch, and what would you use for cross-cloud?
73. How does an Azure Monitor agent or OpenTelemetry Collector get deployed?
74. How do you keep monitoring costs under control?
75. How do you monitor a Kubernetes cluster's control plane?
76. How do you handle a noisy neighbour in a shared cluster affecting your metrics?
77. Explain how container logs are collected and what the common failure modes are.
78. How do you monitor a serverless function?

## Operations, On-Call & Incident Response (79–92)

79. Walk me through your first 15 minutes on a SEV1.
80. How do you decide between rolling back, mitigating, and investigating?
81. How do you run a blameless postmortem?
82. How do you do root cause analysis when the symptom and cause are far apart?
83. How do you know an incident is truly resolved rather than just quiet?
84. How do you design a healthy on-call rotation?
85. What makes a runbook useful to someone who did not write it?
86. How do you handle an alert that fires at 3am and turns out to be nothing?
87. How do you prioritise when several alerts fire at once?
88. How do you manage operational maintenance alongside new-build work?
89. How do you handle a change that causes a monitoring blind spot?
90. How do you document a monitoring configuration so someone else can maintain it?
91. How do you manage alert ownership across teams?
92. What security responsibilities come with access to monitoring data?

## Stakeholders, Documentation & Communication (93–100)

93. How do you gather and prioritise requirements from an internal customer asking for a dashboard?
94. How do you explain a technical monitoring concept to a non-technical stakeholder?
95. How do you say no to a request that would create alert noise?
96. How do you write technical documentation that people actually read?
97. How do you partner with technical leads on a strategic project while handling daily support?
98. Tell me about a time you had to balance new-build work with operational maintenance.
99. Mastercard emphasises information security. How do you apply that in your day-to-day work?
100. Why do you want to work on Mastercard's Enterprise Monitoring team?

---