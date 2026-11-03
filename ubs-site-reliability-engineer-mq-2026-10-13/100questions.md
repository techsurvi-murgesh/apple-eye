# 100 Interview Questions — Site Reliability Engineer - MQ (Infrastructure Engineer), UBS Pune — 2026-10-13

Target profile: infrastructure/SRE engineer on the UBS Middleware crew (Hosting stream, Pune). IBM MQ and enterprise messaging, Azure, Kubernetes/Docker, GitLab CI/CD, observability, agile/Scrum, automation, and AI-assisted delivery with validated outputs.

## IBM MQ & Enterprise Messaging (1–18)

1. What is IBM MQ and what problem does it solve?
2. Explain queue manager, queue, topic, and channel in IBM MQ terms.
3. What is a message queue vs a topic in IBM MQ?
4. Explain point-to-point vs publish/subscribe messaging.
5. What are delivery guarantees in IBM MQ — and what does MQ guarantee exactly?
6. How does IBM MQ handle poison messages? Explain backout queues and dead-letter queues.
7. What is queue depth, and how does queue depth affect throughput?
8. Explain MQ cluster vs queue manager sharing group.
9. How do you monitor IBM MQ health? Which metrics alarm first?
10. What causes a channel to go in retry, and how do you diagnose it?
11. Explain message persistence and how it trades off against throughput.
12. How do you do rolling upgrades of a queue manager cluster without downtime?
13. What is MQ transactionality, and when would you use it?
14. How do you migrate an application from direct DB writes to messaging via MQ?
15. Explain MQ's async logging (data logs) and why enabling it matters for recovery.
16. How do you benchmark an MQ workload and interpret throughput vs latency?
17. Explain the difference between IBM MQ and Kafka for a given workload.
18. How do you secure an MQ environment (TLS, authentication, authorisation, channel access control)?

## Cloud: Azure & Hybrid (19–30)

19. What are the main Azure compute options and when do you use each?
20. Explain Azure VMs, VM Scale Sets, App Service, and Container Apps.
21. What is AKS and how does it relate to Kubernetes?
22. Explain Azure Networking: VNet, subnet, NSG, and how they differ from on-prem firewalling.
23. How do you build a hybrid connectivity model between on-prem and Azure?
24. What are Availability Zones and Availability Sets, and when do you use each?
25. Explain Azure Storage and Blob tiers for a hosting platform.
26. What is Azure Monitor and what does it cover?
27. How do you manage secrets and identity in Azure (Key Vault, managed identities)?
28. How do you control cost of an Azure-hosted service?
29. Explain Azure Policy and Azure Landing Zones.
30. When would you choose Azure over AWS for a hosting platform, and why?

## Containers & Kubernetes (31–42)

31. What happens between `docker run` and a process running in a container?
32. Explain Docker image layers and why layer caching matters in CI.
33. What is a multi-stage Docker build?
34. Difference between a Deployment and a StatefulSet in Kubernetes?
35. What is a Kubernetes Service vs Ingress?
36. How do you configure resource requests and limits?
37. What are liveness and readiness probes, and what happens if you get them wrong?
38. Explain ConfigMaps vs Secrets, and how you should really handle secrets.
39. How do you achieve zero-downtime deployments on Kubernetes?
40. How do you autoscale a workload — HPA, VPA, and cluster autoscaling?
41. How do you manage images across clusters (registry, tagging, promotion)?
42. Explain rolling updates and how a failed rollout is rolled back.

## GitLab CI/CD & Release Engineering (43–54)

43. What are the stages of a GitLab CI/CD pipeline?
44. Explain `.gitlab-ci.yml` — jobs, stages, runners, and artifacts.
45. What is a GitLab Runner and how does executor type matter?
46. How do you define and reuse job templates (YAML anchors, `extends`, includes)?
47. How do you manage secrets in GitLab CI — protected variables, masked variables, environments?
48. Explain merge trains and why they matter for trunk-based development.
49. How do you do environment-specific deployment with manual gates?
50. How do you build and publish product packages/artifacts in a pipeline?
51. How do you run automated tests as a pipeline gate (unit, integration, security scan)?
52. How do you do blue/green and canary deployments from GitLab?
53. How do you roll back a bad release automatically?
54. How do you keep pipeline build time down as the codebase grows?

## Observability & Incident Response (55–68)

55. What are the three pillars of observability, and how do they differ from logging?
56. What are the four golden signals?
57. How do you define SLOs and SLIs for an infrastructure platform?
58. How do you build useful alerts that reduce noise rather than adding to it?
59. Explain RED vs USE methods for measuring services.
60. What metrics matter for a message queue versus an HTTP service?
61. How do you do distributed tracing across asynchronous messaging?
62. How do you build a useful dashboard for on-call?
63. Walk me through a SEV1: how do you triage in the first 15 minutes?
64. How do you run a blameless postmortem?
65. How do you do root cause analysis when the symptom and cause are far apart?
66. Explain error budgets and how they change release decisions.
67. How do you manage alert noise from a flaky dependency?
68. How do you prove an incident is resolved rather than just quiet?

## Linux, Networking & Automation (69–82)

69. How do you investigate high CPU on a Linux host?
70. How do you find a memory leak on a server?
71. Explain load average and what it actually tells you.
72. How do you troubleshoot a network connectivity issue between two hosts?
73. Explain TCP, DNS, and how they show up in a failed connection.
74. How do you find which process is using a port, and what is a file descriptor?
75. How do you write a production-grade Bash script?
76. How do you make automation idempotent?
77. Explain cron, systemd timers, and how you'd schedule jobs safely.
78. How do you manage configuration across a fleet (Ansible)?
79. How do you do zero-downtime host patching and reboots?
80. Explain Terraform state and why remote state must be locked.
81. How do you do capacity planning for a growing service?
82. How do you do performance tuning on a queueing system — what do you measure first?

## Agile, Quality & Compliance (83–92)

83. How do Scrum ceremonies fit into infrastructure engineering work?
84. How do you write a technical design document for an infra change?
85. What are functional vs non-functional requirements, and how do you test the latter?
86. How do you translate a compliance or risk requirement into an engineering control?
87. Explain zero-trust / least privilege for platform infrastructure.
88. How do you handle audit evidence for infrastructure changes?
89. How do you balance delivery speed with change safety?
90. How do you do a risk assessment for a new technology?
91. How do you make infrastructure self-service for developers?
92. How do you document a runbook that someone else can actually follow?

## AI-Assisted Delivery & Behavioural (93–100)

93. Where specifically does AI help you build, deliver, and optimize workflows?
94. How do you validate AI-generated output before using it in a regulated environment?
95. How do you keep an AI-assisted workflow aligned with policy, risk standards, and ethical use?
96. Describe an AI-assisted workflow you built and how you measured its benefit.
97. What are the risks of AI-generated code in infrastructure, and how do you control them?
98. A release went out and broke production. Walk me through what you did.
99. How do you explain a technical trade-off to a non-technical stakeholder?
100. Why do you want to work on the Middleware / IBM MQ hosting crew?

---