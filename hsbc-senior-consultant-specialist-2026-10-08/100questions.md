# 100 Interview Questions — Senior Consultant Specialist, DevOps/Release (HSBC) — 2026-10-08

Target stack: CI/CD (Jenkins, UrbanCode Deploy), release management, multi-stage deployments, environment onboarding (dev/UAT/pre-prod/prod), ITRS Geneos/Splunk/Kibana, RCA, certificates/TLS, Autosys & shell scripting, AWS/Docker/Kubernetes, Ansible/Helm, Git/Gerrit/Bitbucket/Nexus Artifactory, config & change management, HA production support.

## CI/CD & Pipelines (1-18)

1. Explain the end-to-end CI/CD pipeline you would design for a critical banking application.
2. How do you build a single-click production deployment pipeline?
3. Declarative vs scripted Jenkins pipelines — when do you use each?
4. How do you design multi-stage deployments across dev, UAT, pre-prod, and prod?
5. How do you automate switching between production and pre-production servers?
6. How do you parameterize a Jenkins pipeline for many environments?
7. How do you implement approvals and gates before production deployment?
8. How do you manage Jenkins agents, credentials, and secrets securely?
9. How do you use shared libraries to standardize pipelines?
10. How do you make deployments idempotent and repeatable?
11. How do you troubleshoot a pipeline that fails intermittently?
12. How do you speed up slow pipelines (caching, parallelism, incremental builds)?
13. How do you implement rollback in a deployment pipeline?
14. How do you implement blue/green or canary deployments?
15. What is UrbanCode Deploy (UCD) and how do deployment processes/components work there?
16. How do you migrate deployments from manual to automated safely?
17. How do you audit who deployed what, when, and from which commit?
18. How do you version and promote build artifacts across environments?

## Release & Environment Management (19-34)

19. Explain the release management lifecycle in an enterprise.
20. How do you plan and coordinate a major production release?
21. How do you set up and onboard a new application environment from scratch?
22. What belongs in a deployment runbook and a handover document?
23. How do you manage configuration across multiple environments?
24. How do you keep dev/UAT/pre-prod aligned with production?
25. How do you handle environment drift and refresh?
26. How do you manage database changes during a release?
27. How do you handle hotfixes vs standard releases?
28. How do you do a go/no-go release decision?
29. How do you coordinate releases across engineering, testing, ops, and business?
30. How do you manage change management and CAB processes?
31. How do you track defects found during deployment and drive resolution?
32. How do you measure release quality and deployment frequency?
33. How do you ensure backward/forward compatibility during releases?
34. How do you document and transfer knowledge to new team members?

## Monitoring & Observability (35-50)

35. Explain ITRS Geneos and how it is used in enterprise monitoring.
36. How do you monitor multiple highly available environments?
37. How do you use Splunk for log analysis and alerting?
38. How do you use Kibana/ELK for operational dashboards?
39. How do you design alerts that reduce noise and catch real issues?
40. How do you monitor application vs infrastructure health?
41. How do you set up synthetic and uptime monitoring?
42. How do you monitor batch job success/failure (Autosys)?
43. How do you monitor certificates and their expiry?
44. How do you build automated operational reports from monitoring data?
45. How do you use metrics, logs, and traces together for diagnosis?
46. How do you monitor deployment health after a release?
47. How do you define and monitor SLIs/SLOs for critical services?
48. How do you investigate a monitoring gap after an incident?
49. How do you monitor middleware (MQ, Kafka) and databases?
50. How do you reduce MTTR using better observability?

## Troubleshooting & RCA (51-66)

51. Walk through triaging a failed production deployment.
52. How do you systematically perform root cause analysis?
53. How do you distinguish application, build, configuration, and environment issues?
54. How do you debug a build that works locally but fails in CI?
55. How do you troubleshoot a service that fails to start after deployment?
56. How do you debug connectivity issues between tiers?
57. How do you troubleshoot DNS and TLS/certificate problems?
58. How do you handle a certificate that has expired in production?
59. How do you debug performance degradation after a release?
60. How do you handle a failed rollback?
61. How do you troubleshoot resource exhaustion (CPU, memory, disk, connections)?
62. How do you use logs to reconstruct an incident timeline?
63. How do you handle an incident with masking/unknown root cause under pressure?
64. How do you write a blameless postmortem and action items?
65. How do you prevent recurrence of a repeated deployment failure?
66. How do you escalate appropriately during a critical incident?

## Containers, Cloud & Configuration (67-82)

67. Explain Docker architecture and how you build optimized images.
68. How do you write production-grade Dockerfiles (multi-stage, non-root)?
69. Explain Kubernetes architecture: control plane, nodes, pods, services.
70. How do you deploy and roll back a workload in Kubernetes?
71. How do you manage config and secrets in Kubernetes (ConfigMaps, Secrets)?
72. How do you expose a Kubernetes app (Service, Ingress, load balancer)?
73. How do you troubleshoot a pod in CrashLoopBackOff or Pending?
74. What is Helm and how do you version and template charts?
75. How do you manage Helm releases and rollbacks?
76. Explain Ansible: inventory, playbooks, roles, idempotency.
77. How do you use Ansible for environment setup and app deployment?
78. How do you manage secrets in Ansible (Vault)?
79. Explain AWS compute, storage, networking, and IAM for deployments.
80. How do you achieve high availability and resilience on AWS?
81. How do you manage certificates and TLS termination on AWS/load balancers?
82. How do you set up auto scaling for a production service?

## Shell, Batch & Source/Artefacts (83-92)

83. How do you write robust shell scripts (set -euo pipefail, traps, logging)?
84. How do you parse JSON/logs in shell and automate operational tasks?
85. How do you schedule and monitor batch jobs with Autosys?
86. How do you debug a failed batch job chain?
87. How do you implement retries and idempotency in scripts?
88. Explain Git branching strategies for release management (GitFlow, trunk-based).
89. How do you manage code review with Gerrit vs pull requests?
90. How do you resolve complex merge conflicts safely?
91. What is Nexus/Artifactory and how do you manage artifacts and retention?
92. How do you manage dependency and binary repositories securely?

## Linux, Networking & Behavioral (93-100)

93. How do you administer and harden Linux servers for production?
94. How do you troubleshoot high CPU, memory, disk, and I/O on Linux?
95. Explain systemd, journalctl, and service management.
96. How do you manage users, permissions, and SSH access at scale?
97. Explain OSI/TCP-IP and how you debug a network issue.
98. How do you work in an Agile team as a DevOps/release engineer?
99. How do you mentor junior engineers and document processes?
100. Why are you a good fit for this Senior Consultant Specialist role at HSBC, and what would you improve in your first 90 days?
