# 100 Interview Questions — Site Reliability Engineer II (Platform Engineer), SIXT

Target profile: Platform/SRE engineer owning developer experience and production agentic AI across an internal developer platform, with Kubernetes, AWS, CI/CD, observability, system engineering, secure tool execution, and reliable operation for hundreds of engineers across diverse technology stacks.

## Developer Experience and Platform Engineering (1–15)

1. What distinguishes an internal developer platform from a collection of infrastructure tools?
2. How would you measure developer experience and platform adoption without relying only on surveys?
3. Which developer workflows would you improve first to reduce friction at SIXT?
4. How do you design golden paths while still supporting different teams and technology stacks?
5. What makes a self-service platform capability safe enough for hundreds of engineers?
6. How would you design service templates that include CI/CD, observability, and security by default?
7. How do you balance platform standardization with team autonomy?
8. How do you version and roll out changes to shared developer tooling?
9. What is your approach to backward compatibility for internal platform APIs?
10. How do you gather and prioritize requirements from developers using the platform?
11. How would you reduce cognitive load for a developer onboarding a new service?
12. Which metrics would you track for build time, deployment frequency, lead time, and failed-deployment recovery?
13. How do you prevent an internal platform from becoming a ticket-driven bottleneck?
14. Describe taking a developer-tooling prototype into production. What changes at each stage?
15. How would you drive adoption of a new agentic capability across 800+ engineers?

## Agentic AI Architecture and Tool Use (16–35)

16. What makes a system agentic rather than a chatbot with a prompt?
17. Describe the architecture of a multi-step agent that investigates failed CI/CD pipelines.
18. How do you represent agent goals, plans, state, and completion criteria?
19. How would you design a tool interface that an LLM can call reliably?
20. Why should tool schemas be narrow and strongly typed, and how do you validate arguments?
21. How do you handle ambiguous instructions before allowing an agent to act?
22. What is the difference between short-term, episodic, and long-term agent memory?
23. What should and should not be stored in memory for a developer-platform agent?
24. How do you prevent stale or incorrect memories from influencing future decisions?
25. How do you make multi-step agent execution resumable after a crash?
26. How do you make tool operations idempotent or compensate for partial failures?
27. When would you use deterministic workflows instead of autonomous decision-making?
28. How do you bound an agent's steps, cost, execution time, and blast radius?
29. How do you design human approval for high-risk tool calls without blocking every task?
30. How do you implement a kill switch for an agent already executing a workflow?
31. How do you prevent prompt injection in repository content, logs, or pipeline output?
32. How do you scope credentials so an agent receives only the access required for one task?
33. How do you stop agents from leaking source code, secrets, or production data through tools?
34. What audit information should every agent decision and tool invocation record?
35. Compare single-agent and multi-agent designs for developer-platform automation.

## Agent Evaluation, Reliability, and Production Operations (36–48)

36. Which offline evaluations would you build before deploying an agent to production?
37. How do you create representative task datasets for CI/CD and observability agents?
38. How do you measure task success, tool-selection accuracy, and unsafe-action rates?
39. How do you evaluate multi-step reasoning without rewarding a lucky final answer?
40. How do you test agent behavior when tools time out, return malformed data, or contradict one another?
41. What online metrics would you monitor for a production agentic system?
42. How do you detect model, prompt, tool-schema, or memory regressions?
43. How would you canary an agent release and define rollback criteria?
44. How do you provide deterministic fallback behavior when a model is unavailable?
45. How do you control latency and token cost for multi-step agents at scale?
46. When would you use model routing or different model sizes for different steps?
47. How do you run AI workloads reliably on Kubernetes, including GPU or external-model dependencies?
48. Describe a production agent incident you might face and your triage approach.

## Kubernetes, AWS, and System Engineering (49–63)

49. How do you design a highly available platform workload on Kubernetes?
50. Explain requests, limits, quality-of-service classes, and their effect on reliability.
51. How do liveness, readiness, and startup probes differ, and how can they cause outages?
52. How do you troubleshoot CrashLoopBackOff, pending pods, and failed rollouts?
53. How do Horizontal Pod Autoscaler and cluster autoscaling work together?
54. What would you consider when autoscaling model-serving or agent-worker workloads?
55. How do you isolate tenants and workloads using namespaces, RBAC, policies, and network controls?
56. How do you safely upgrade a Kubernetes cluster supporting critical developer tooling?
57. Which AWS services would you use to run an internal developer platform, and why?
58. How would you design AWS networking and IAM for agents accessing CI/CD and observability systems?
59. How do you manage secrets for platform services and agent tools?
60. How do you design a queue-based agent worker system for concurrency and backpressure?
61. How do you handle distributed locks, duplicate work, and exactly-once expectations?
62. What caching strategies would you use for platform metadata, model responses, and repository data?
63. How do you capacity-plan a platform used by hundreds of engineers with bursty CI workloads?

## CI/CD and Software Delivery (64–73)

64. What does a secure, reusable CI/CD platform look like for polyglot engineering teams?
65. How do you design reusable GitHub Actions workflows without making them difficult to debug?
66. How do you implement artifact promotion across development, staging, and production?
67. Compare rolling, blue-green, and canary deployments for platform services.
68. How do health signals and error budgets drive automated deployment rollback?
69. How would an agent diagnose a failed deployment and recommend a safe remediation?
70. Which deployment actions should never be autonomously executed by an agent?
71. How do you protect CI/CD pipelines from compromised dependencies and untrusted repository input?
72. How do you use OIDC and short-lived credentials instead of static cloud keys?
73. How do you test changes to shared pipelines before rolling them out to every team?

## Observability and SRE (74–85)

74. How do SLIs, SLOs, and error budgets apply to an internal developer platform?
75. What SLOs would you define for CI/CD, deployment, and agent-assisted workflows?
76. How do metrics, logs, and traces help debug a multi-step agent execution?
77. Which agent-specific spans and attributes would you capture in distributed traces?
78. How would you correlate a code change, deployment, infrastructure event, and user-facing regression?
79. What would you put on a developer-platform health dashboard?
80. How do you alert on agent failures without paging for every model retry?
81. How do you monitor tool latency, model latency, queue depth, and task completion together?
82. How do you avoid high-cardinality observability data from repositories, teams, or agent sessions?
83. How do you protect sensitive prompts, logs, and traces while preserving debuggability?
84. Walk through a blameless postmortem for an agent that executed an unsafe remediation.
85. How do you turn repeated operational work into reliable platform automation?

## Scalability, Collaboration, and Behavioral (86–100)

86. How would you roll out an agentic capability gradually across teams with different maturity levels?
87. How do you support developers who distrust agent-generated recommendations?
88. Describe a developer pain point you would discover through shadowing or workflow analysis.
89. How do you distinguish a platform problem from a team-specific usage problem?
90. How do you prioritize platform reliability, developer requests, and new agent features?
91. Tell me about a complex system you owned from design through production operation.
92. Describe a time you simplified a workflow for other engineers.
93. How do you document an internal platform so teams can self-serve effectively?
94. How do you handle a critical incident caused by a shared platform change?
95. How do you push back on an AI feature that is impressive in a demo but unsafe in production?
96. Describe a difficult trade-off between autonomy, reliability, and delivery speed.
97. How do you keep up with agentic AI while maintaining engineering rigor?
98. What would your first 90 days on SIXT's Developer Experience & Agentic AI platform look like?
99. Which project best demonstrates your system engineering and production ownership skills?
100. Why are you a strong fit for building and operating agentic developer tooling at SIXT?
