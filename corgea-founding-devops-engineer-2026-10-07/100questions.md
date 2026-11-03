# 100 Interview Questions — Founding DevOps Engineer, Corgea

## Cloud & Multi-Cloud (1-14)
1. How do you design cloud infrastructure for a high-availability SaaS platform?
2. How do you approach multi-cloud architecture, and when is it worth the complexity?
3. How do you design VPCs, subnets, routing, and egress for secure services?
4. How do you choose between AWS, GCP, and Azure for a given workload?
5. How do you implement least-privilege IAM across a cloud account?
6. How do you manage secrets across cloud environments (vault, KMS, rotation)?
7. How do you design networking for private services with controlled egress?
8. How do you set up account/tenancy isolation for enterprise customers?
9. How do you design for failure domains and multi-AZ resilience?
10. How do you control cloud cost without hurting reliability?
11. How do you tag, monitor, and govern resource usage across accounts?
12. How do you handle data residency and compliance requirements in the cloud?
13. How do you evaluate and adopt new cloud services pragmatically?
14. How do you keep infrastructure reproducible across environments?

## Infrastructure as Code — Terraform (15-26)
15. How do you structure Terraform for a growing startup with multiple environments?
16. How do you manage remote state, locking, and workspaces?
17. How do you review a Terraform plan to prevent outages?
18. How do you handle drift between state and real infrastructure?
19. How do you handle secrets in Terraform safely?
20. How do you refactor Terraform without destroying resources (moved/import)?
21. How do you test Terraform (validate, tflint, checkov, plan gates)?
22. How do you roll back a bad Terraform apply?
23. How do you manage provider and module version upgrades?
24. How do you structure reusable modules for common patterns?
25. How do you onboard a new service with Terraform quickly?
26. Terraform vs Pulumi vs CDK — how do you choose?

## CI/CD & Developer Velocity (27-40)
27. How do you build CI/CD pipelines that make deploys fast and safe?
28. How do you design a pipeline with quality gates (lint, test, scan, plan)?
29. How do you speed up slow builds and test suites?
30. How do you implement trunk-based development with feature flags?
31. How do you do progressive delivery (canary, blue-green, rollback)?
32. How do you manage secrets and permissions in CI/CD?
33. How do you secure CI/CD against supply-chain attacks?
34. How do you build internal developer tooling that removes toil?
35. How do you standardize how teams ship services?
36. How do you measure and improve developer velocity (DORA metrics)?
37. How do you handle monorepo CI efficiently?
38. How do you support PR preview environments?
39. How do you debug "pipeline passed but deployment broke"?
40. How do you keep release quality high without slowing releases?

## Containers & Kubernetes (41-54)
41. How do you containerize services securely for production?
42. How do you write minimal, secure Dockerfiles (multi-stage, non-root, pinned)?
43. Explain core Kubernetes objects and how a workload runs end-to-end.
44. How do you design a Kubernetes platform (namespaces, RBAC, policies)?
45. How do you secure a cluster (network policies, admission control, secrets)?
46. How do you debug CrashLoopBackOff, OOMKilled, ImagePullBackOff, Pending?
47. How do you configure probes, resources, and autoscaling?
48. How do you manage persistent storage and stateful workloads?
49. How do you do zero-downtime deploys and safe rollbacks on K8s?
50. How do you manage multi-tenant clusters for enterprise customers?
51. How do you scan and patch container images in the pipeline?
52. How do you control K8s cost (right-sizing, bin packing, autoscaling)?
53. How do you set up an ingress/service mesh safely?
54. How do you run Kubernetes across multiple clouds?

## Observability, Reliability & Incident Response (55-70)
55. How do you design monitoring, logging, and alerting for a platform?
56. How do you choose metrics vs logs vs traces for a problem?
57. What are SLIs, SLOs, and error budgets, and how do you set them?
58. How do you alert on real issues without noisy false positives?
59. How do you build dashboards that on-call actually uses?
60. How do you correlate deploys with error spikes?
61. How do you design incident response and on-call for a startup?
62. Walk through triaging a production outage systematically.
63. How do you run a blameless postmortem and drive action items?
64. How do you improve reliability without overengineering?
65. How do you load test and capacity plan for growth?
66. How do you handle a third-party provider outage?
67. How do you set up log aggregation and retention cost-effectively?
68. How do you monitor the CI/CD pipeline and infrastructure itself?
69. How do you implement health checks and graceful degradation?
70. How do you balance reliability work against feature velocity?

## Security & Compliance (71-84)
71. How do you strengthen security posture across cloud, app, and runtime?
72. How do you implement least privilege and audit access?
73. How do you manage secrets lifecycle (storage, rotation, revocation)?
74. How do you approach vulnerability management at a startup?
75. What are SAST, DAST, SCA, and how do you wire them into CI?
76. How do you secure the software supply chain (SBOM, signing, provenance)?
77. How do you secure runtime environments and detect threats?
78. How do you handle container security scanning and image policy?
79. How do you respond to a security incident?
80. How do you meet enterprise customer security requirements / questionnaires?
81. How do you handle compliance (SOC 2, ISO 27001) pragmatically?
82. How do you secure infrastructure as code and CI/CD?
83. How do you do threat modeling for a new service?
84. How do you encrypt data in transit and at rest?

## Linux, Networking & Scripting (85-94)
85. How do you debug a Linux production issue (CPU, memory, disk, network)?
86. Explain DNS, TCP/IP, HTTP/HTTPS in a request path.
87. How do you troubleshoot connectivity between services and databases?
88. How do you write robust Bash scripts (set -euo pipefail, logging, traps)?
89. How do you automate operational toil with Python or Go?
90. How do you parse APIs/JSON with jq, requests, or SDKs?
91. How do you manage systemd services, cron, and scheduled tasks?
92. How do you harden a Linux host?
93. How do you diagnose a load balancer / TLS issue?
94. How do you debug a slow network path or packet loss?

## Founding Startup Behavioral (95-100)
95. Why founding DevOps, and how do you operate with end-to-end ownership?
96. How do you make sound tradeoffs with limited time and headcount?
97. Describe a time you eliminated significant manual toil through automation.
98. How do you support enterprise-grade requirements without overengineering?
99. How do you prioritize across reliability, security, cost, and velocity?
100. Why Corgea, why a founding DevOps role, and what would you own in your first 90 days?
