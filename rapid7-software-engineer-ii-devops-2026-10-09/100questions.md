# 100 Interview Questions — Software Engineer II, DevOps / Platform Ops (Rapid7) — 2026-10-09

Target stack: platform/infrastructure/SRE, public cloud (AWS/GCP/Azure), Linux performance tuning, Kubernetes/Docker, Terraform IaC, Grafana/Prometheus observability, Ansible, CI/CD, GitOps (ArgoCD/Atlantis), FedRAMP compliance, on-call/incident response/RCA, MTTR, runbooks, automation, microservices, agentic dev practices.

## Linux Systems (1-16)

1. Explain the Linux boot process and systemd service management.
2. How do you troubleshoot high CPU, memory, disk, and I/O on Linux?
3. How do you diagnose and fix a memory leak or OOM kill?
4. Explain how you tune Linux for high-throughput services (sysctl, ulimits, scheduling).
5. How do you analyze performance with top, vmstat, iostat, sar, perf?
6. Explain file descriptors/ulimits and how they cause production issues.
7. How do you use strace, lsof, and tcpdump to debug a process?
8. How do you manage users, permissions, sudo, and SSH at scale?
9. Explain filesystems, mounts, and disk troubleshooting.
10. How do you harden a Linux server for production?
11. How do you manage logs with journalctl, logrotate, and centralized logging?
12. How do you patch kernel/system packages with minimal downtime?
13. Explain cgroups and namespaces (containers foundation).
14. How do you troubleshoot DNS resolution failures?
15. How do you schedule jobs with cron vs systemd timers?
16. How do you debug a service that fails to start after reboot?

## Cloud Infrastructure (17-32)

17. Explain AWS core services: EC2, VPC, S3, IAM, RDS, ELB, Route 53.
18. How do you design a highly available, multi-AZ architecture?
19. How do you design and segment VPCs, subnets, and security groups?
20. Explain auto scaling and elasticity patterns.
21. How do you manage IAM roles and least privilege at scale?
22. How do you achieve cost efficiency across a large cloud estate?
23. Compare AWS, GCP, and Azure for a platform team.
24. How do you design multi-region/multi-cloud resilience?
25. How do you manage secrets and encryption in the cloud?
26. Explain S3 lifecycle, versioning, and access control.
27. How do you troubleshoot a cloud networking or security-group issue?
28. How do you use Managed Kubernetes (EKS/GKE/AKS)?
29. How do you manage DNS and certificates in the cloud?
30. How do you implement backups and disaster recovery?
31. How do you monitor cloud spend and capacity?
32. How do you evaluate a new cloud service for production use?

## Kubernetes & Containers (33-50)

33. Explain Kubernetes architecture: control plane, nodes, etcd, kubelet.
34. What are Pods, Deployments, StatefulSets, DaemonSets, Jobs?
35. How do Services, Ingress, and NetworkPolicies work?
36. How do you troubleshoot CrashLoopBackOff, ImagePullBackOff, OOMKilled, Pending?
37. Explain liveness, readiness, and startup probes.
38. How do rolling updates and rollbacks work?
39. How do you manage resource requests/limits and HPA?
40. How do you use ConfigMaps and Secrets securely?
41. How do you manage persistent storage (PV/PVC, StorageClass)?
42. How do you debug cluster networking and DNS (CNI, CoreDNS)?
43. How do you secure a Kubernetes cluster (RBAC, PodSecurity, network policies)?
44. How do you upgrade a cluster safely?
45. Explain operators and CRDs.
46. How do you write optimized Dockerfiles (multi-stage, non-root, minimal base)?
47. How do you scan container images for vulnerabilities?
48. How do you manage image registries and retention?
49. How do you do blue/green and canary deployments on Kubernetes?
50. How do you operate multiple clusters at scale?

## Terraform & IaC (51-64)

51. Explain Terraform workflow: init, plan, apply, state, providers.
52. How do you manage remote state with locking?
53. How do you structure reusable Terraform modules?
54. How do you manage multiple environments with workspaces or separate states?
55. How do you detect and remediate drift?
56. How do you import existing resources into Terraform?
57. How do you test Terraform (tflint, checkov, terratest)?
58. How do you protect production state from accidental destruction?
59. How do you handle secrets in Terraform?
60. Terraform vs CloudFormation vs Pulumi — tradeoffs.
61. What is Atlantis and how does it automate Terraform PR workflows?
62. How do you review and approve IaC changes safely?
63. How do you refactor a large monolithic Terraform codebase?
64. How do you pin and upgrade provider versions?

## CI/CD & GitOps (65-76)

65. Explain the stages of a robust CI/CD pipeline.
66. How do you build a pipeline for microservices?
67. How do you implement GitOps with ArgoCD?
68. Difference between push-based CI/CD and pull-based GitOps.
69. How do you handle environment promotion and approvals?
70. How do you implement fast, safe rollbacks?
71. How do you manage secrets in pipelines?
72. How do you cache dependencies and speed up builds?
73. How do you run automated tests and security scans in a pipeline?
74. How do you do progressive delivery (canary, blue/green)?
75. How do you manage configuration management with Ansible?
76. How do you integrate AI/agentic tools into development and operations?

## Observability & SRE (77-90)

77. Explain metrics, logs, and traces and how they complement each other.
78. How do you use Prometheus and PromQL for metrics?
79. How do you build effective Grafana dashboards and alerts?
80. How do you define SLIs, SLOs, and error budgets?
81. What are the four golden signals and how do you track them?
82. How do you reduce alert fatigue and define meaningful alerts?
83. How do you reduce MTTR across a platform?
84. How do you instrument a service with custom metrics and traces (OpenTelemetry)?
85. How do you monitor Kubernetes and cloud infrastructure at scale?
86. How do you capacity plan for a growing platform?
87. How do you design a runbook and operational workflow?
88. How do you run incident response and post-incident RCA?
89. How do you run an on-call rotation effectively?
90. How do you measure and improve platform reliability over time?

## Security, Compliance & Behavioral (91-100)

91. What is FedRAMP and what does an authorized environment require?
92. How do you implement least privilege across a cloud platform?
93. How do you manage vulnerability and patch management at scale?
94. How do you secure CI/CD and the software supply chain?
95. How do you approach compliance controls (auditing, evidence, boundaries)?
96. Describe a time you broke a large goal into smaller execution steps.
97. Describe a time you took ownership of an unfamiliar system or runbook.
98. How do you collaborate across teams to deliver platform improvements?
99. How do you communicate technical objectives and tradeoffs clearly?
100. Why are you a good fit for this Software Engineer II (DevOps) role at Rapid7, and what would you improve in your first 90 days?
