# 100 Interview Questions — DevOps Engineer (QuickInfra) — 2026-10-05

Target stack: Terraform, AWS (EC2, VPC, RDS, EKS), Docker, Kubernetes, CI/CD (Jenkins / GitLab CI / GitHub Actions), monitoring & observability, cloud security (IAM, security groups, encryption), Python/Bash.

## Terraform (1–20)

1. Explain Terraform workflow: init, plan, apply, destroy. What happens in each step?
2. How do you structure production-grade Terraform modules for reusability?
3. How do you manage Terraform state in a team? Remote backends, locking?
4. What is state drift and how do you detect and remediate it?
5. Explain variables, outputs, locals, and data sources with use cases.
6. How do you handle multiple environments (dev/staging/prod) with Terraform?
7. What are Terraform workspaces vs. separate state files? Pros/cons?
8. How do you version and publish Terraform modules?
9. Explain `count` vs `for_each` with examples.
10. How do you handle sensitive values in Terraform (secrets, tfvars, vault)?
11. What is the difference between provisioners and configuration management? When would you avoid provisioners?
12. How do you test Terraform modules (terratest, tflint, tfsec, checkov)?
13. Explain Terraform import. When would you use it?
14. How do you manage provider version constraints and dependency locking?
15. How would you design a VPC + EKS + RDS module hierarchy for customers?
16. How do you roll out a breaking change to a shared Terraform module used by customers daily?
17. Explain dynamic blocks and how they simplify security group / IAM modules.
18. How do you implement compliance controls (e.g., encrypted S3, no open SGs) in Terraform?
19. What causes Terraform apply failures mid-run, and how do you recover safely?
20. How do you do code review for Terraform PRs? What do you check?

## AWS Core: EC2, VPC, RDS, EKS (21–40)

21. Design a production VPC: CIDRs, public/private subnets, AZs, NAT, route tables.
22. What is the difference between security groups and NACLs?
23. How do you troubleshoot EC2 instance unreachable (SSH, status checks, ENI, SG)?
24. How do you choose EC2 instance types and pricing models (on-demand, spot, reserved)?
25. Explain ALB vs NLB vs CLB. When would you use each with EKS?
26. How do you design highly available RDS (Multi-AZ, read replicas, backups)?
27. How do you handle RDS failover, backup restore, and point-in-time recovery?
28. Explain EKS architecture: control plane, node groups, Fargate vs managed nodes.
29. How do you upgrade an EKS cluster with zero downtime?
30. How do you manage EKS networking (VPC CNI, security groups for pods, IRSA)?
31. How do you provision EKS with Terraform (eks module, iam roles, addons)?
32. Explain IAM Roles for Service Accounts (IRSA) in EKS.
33. How do you manage EBS/EFS storage in EKS?
34. How do you secure S3 buckets used in provisioning workflows?
35. Explain VPC peering vs Transit Gateway vs PrivateLink for customer accounts.
36. How do you implement cross-account access for a platform like QuickInfra?
37. How do you monitor AWS costs and prevent runaway provisioning?
38. How do you automate AMI baking and patching?
39. Explain CloudTrail, Config, and GuardDuty for compliance across accounts.
40. Walk through debugging a failed RDS connection from EKS pods.

## Docker & Kubernetes (41–58)

41. Explain Docker image layers, caching, and multi-stage builds.
42. How do you optimize Docker image size and security?
43. What is the difference between CMD and ENTRYPOINT?
44. How do you manage Docker registries (ECR lifecycle, image scanning)?
45. Explain Kubernetes Pods, Deployments, Services, Ingress.
46. How do Deployments handle rolling updates and rollbacks?
47. Explain ConfigMaps vs Secrets in Kubernetes. How do you manage secrets in EKS?
48. What are resource requests/limits, probes (liveness/readiness/startup)?
49. How do you troubleshoot CrashLoopBackOff and ImagePullBackOff?
50. Explain HPA, VPA, and Cluster Autoscaler / Karpenter.
51. How do you manage persistent storage in Kubernetes?
52. Explain RBAC in Kubernetes with an example.
53. How do you isolate tenants/namespaces in a shared cluster?
54. What are Helm charts / Kustomize? When would you use each?
55. How do you manage container logs and metrics at scale?
56. Explain service mesh use cases. Would you introduce one for QuickInfra?
57. How do you secure container supply chain (image signing, admission controllers)?
58. Design a Kubernetes platform for provisioning customer workloads safely.

## CI/CD: Jenkins, GitLab CI, GitHub Actions (59–74)

59. Design a CI/CD pipeline for Terraform modules: lint, plan, apply with approvals.
60. Compare Jenkins vs GitLab CI vs GitHub Actions. When would you pick each?
61. How do you implement GitFlow / trunk-based development for infra repos?
62. How do you safely run `terraform plan` in PRs and `apply` on merge?
63. How do you manage pipeline secrets (OIDC to AWS vs static keys)?
64. Explain reusable workflows / shared libraries in Jenkins and GitHub Actions.
65. How do you cache Docker layers to optimise pipeline speed?
66. How do you implement blue/green or canary deployments for backend services?
67. How do you roll back a bad deployment automatically?
68. How do you add quality gates (tests, tfsec, checkov, SonarQube) to pipelines?
69. How do you handle monorepo vs polyrepo CI for infra + app code?
70. How do you version artifacts and promote across environments?
71. Explain ephemeral Jenkins agents on Kubernetes / EC2.
72. How do you debug a flaky pipeline?
73. How do you audit who applied which infra change and when?
74. Design a customer-facing provisioning pipeline that is idempotent and observable.

## Monitoring, Alerting & Observability (75–85)

75. What are the four golden signals / RED / USE methods?
76. How would you design monitoring for EKS + RDS + EC2 from scratch?
77. Compare Prometheus + Grafana + Loki vs CloudWatch vs Datadog.
78. How do you set up SLOs, SLIs, and alert thresholds without alert fatigue?
79. Explain PromQL with an example alert query.
80. How do you collect logs from EKS (Fluent Bit, Promtail, CloudWatch agent)?
81. How do you trace requests across microservices?
82. How do you monitor Terraform / provisioning failures?
83. Walk through an on-call incident: high CPU on RDS, pods OOMKilled. Steps?
84. How do you implement on-call rotations, runbooks, and postmortems?
85. How do you prove observability coverage for customer SLAs?

## Cloud Security & Compliance (86–92)

86. Explain IAM users, roles, policies, permission boundaries with least-privilege examples.
87. How do you audit over-permissive IAM across many customer accounts?
88. How do you enforce encryption at rest and in transit (RDS, S3, EBS, TLS)?
89. How do you manage secrets rotation (Secrets Manager, SSM Parameter Store, Vault)?
90. How do you implement SCPs, SSO, and centralized logging for compliance?
91. What CIS Benchmark controls would you enforce first on AWS accounts?
92. How would you respond to an exposed AWS access key?

## Scripting & Automation (93–96)

93. Write a Bash script to check EKS node health and cordon faulty nodes.
94. Write a Python script using boto3 to list unencrypted RDS instances across regions.
95. How do you decide between Ansible vs Terraform vs Python/Bash for a task?
96. Explain idempotency in automation scripts with an example.

## Collaboration & Scenarios (97–100)

97. How do you collaborate with product teams to automate a new infra pattern?
98. A customer provisioning workflow fails daily at scale. How do you debug and harden it?
99. How do you document a new Terraform module for customers and internal teams?
100. Why are you a good fit for QuickInfra's core automation platform with 2–4 years experience? What would you improve in your first 90 days?
