# 100 Interview Questions — DevOps Engineer (GoKwik) — 2026-11-02

Target stack: Kubernetes, Docker, Terraform, AWS/GCP, CI/CD (GitHub Actions, Jenkins), monitoring & observability, cloud security (IAM, encryption), Python/Go/Shell scripting, on-call incident response, infrastructure as code, chaos engineering. Target experience: 1-4 years in DevOps/SRE/CloudOps.

## Terraform (1–25)

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
21. How do you manage Terraform graph dependencies and parallelism?
22. Explain remote backend configuration (S3 + DynamoDB, Consul, etc.)
23. How do you handle Terraform version upgrades across a team?
24. What is Terraform Cloud/Enterprise and when would you use it?
25. How do you implement zero-downtime infrastructure updates with Terraform?

## AWS Core: EC2, VPC, RDS, EKS, S3 (26–55)

26. Design a production VPC: CIDRs, public/private subnets, AZs, NAT, route tables.
27. What is the difference between security groups and NACLs?
28. How do you troubleshoot EC2 instance unreachable (SSH, status checks, ENI, SG)?
29. How do you choose EC2 instance types and pricing models (on-demand, spot, reserved)?
30. Explain ALB vs NLB vs CLB. When would you use each with EKS?
31. How do you design highly available RDS (Multi-AZ, read replicas, backups)?
32. How do you handle RDS failover, backup restore, and point-in-time recovery?
33. Explain EKS architecture: control plane, node groups, Fargate vs managed nodes.
34. How do you upgrade an EKS cluster with zero downtime?
35. How do you manage EKS networking (VPC CNI, security groups for pods, IRSA)?
36. How do you provision EKS with Terraform (eks module, iam roles, addons)?
37. Explain IAM Roles for Service Accounts (IRSA) in EKS.
38. How do you manage EBS/EFS storage in EKS?
39. How do you secure S3 buckets used in provisioning workflows?
40. Explain VPC peering vs Transit Gateway vs PrivateLink for customer accounts.
41. How do you implement cross-account access for a platform like GoKwik?
42. How do you monitor AWS costs and prevent runaway provisioning?
43. How do you automate AMI baking and patching?
44. Explain CloudTrail, Config, and GuardDuty for compliance across accounts.
45. Walk through debugging a failed RDS connection from EKS pods.
46. How do you design a multi-account AWS organization structure?
47. How do you implement SCPs (Service Control Policies) for governance?
48. How do you manage AWS IAM identity center (SSO) integration?
49. Explain VPC Flow Logs and how you use them for debugging.
50. How do you design disaster recovery (RTO/RPO) for AWS workloads?
51. How do you handle NAT gateway redundancy and failover?
52. How do you configure and troubleshoot VPN connections in AWS?
53. Explain Route 53 routing policies (simple, weighted, latency, failover).
54. How do you implement WAF Web ACLs for application protection?
55. How do you manage AWS Secrets Manager vs Parameter Store vs Vault?

## Docker & Kubernetes (56–82)

56. Explain Docker image layers, caching, and multi-stage builds.
57. How do you optimize Docker image size and security?
58. What is the difference between CMD and ENTRYPOINT?
59. How do you manage Docker registries (ECR lifecycle, image scanning)?
60. Explain Kubernetes Pods, Deployments, Services, Ingress.
61. How do Deployments handle rolling updates and rollbacks?
62. Explain ConfigMaps vs Secrets in Kubernetes. How do you manage secrets in EKS?
63. What are resource requests/limits, probes (liveness/readiness/startup)?
64. How do you troubleshoot CrashLoopBackOff and ImagePullBackOff?
65. Explain HPA, VPA, and Cluster Autoscaler / Karpenter.
66. How do you manage persistent storage in Kubernetes (PV, PVC, storage classes)?
67. Explain RBAC in Kubernetes with an example.
68. How do you isolate tenants/namespaces in a shared cluster?
69. What are Helm charts / Kustomize? When would you use each?
70. How do you manage container logs and metrics at scale?
71. Explain service mesh use cases. Would you introduce one for GoKwik?
72. How do you secure container supply chain (image signing, admission controllers)?
73. Design a Kubernetes platform for provisioning customer workloads safely.
74. How do you implement PodSecurityPolicies / PSP equivalents in EKS?
75. How do you handle Kubernetes upgrade strategies (node pools, rolling)?
76. Explain NodePools, DaemonSets, and system pods in EKS.
77. How do you debug DNS issues inside Kubernetes clusters?
78. How do you configure and use EKS Fargate for serverless pods?
79. Explain health checks (liveness, readiness, startup) and their configuration.
80. How do you manage Kubernetes secrets across environments?
81. How do you implement pod disruption budgets (PDBs)?
82. How do you troubleshoot network policies and connectivity issues?

## CI/CD: GitHub Actions, Jenkins (83–105)

83. Design a CI/CD pipeline for Terraform modules: lint, plan, apply with approvals.
84. Compare GitHub Actions vs Jenkins vs GitLab CI. When would you pick each?
85. How do you implement GitFlow / trunk-based development for infra repos?
86. How do you safely run `terraform plan` in PRs and `apply` on merge?
87. How do you manage pipeline secrets (OIDC to AWS vs static keys)?
88. Explain reusable workflows / shared libraries in GitHub Actions.
89. How do you cache Docker layers to optimise pipeline speed?
90. How do you implement blue/green or canary deployments for backend services?
91. How do you roll back a bad deployment automatically?
92. How do you add quality gates (tests, tfsec, checkov, SonarQube) to pipelines?
93. How do you handle monorepo vs polyrepo CI for infra + app code?
94. How do you version artifacts and promote across environments?
95. Explain ephemeral Jenkins agents on Kubernetes / EC2.
96. How do you debug a flaky pipeline?
97. How do you audit who applied which infra change and when?
98. Design a customer-facing provisioning pipeline that is idempotent and observable.
99. How do you implement pull-based GitOps with Argo CD or Flux?
100. How do you handle database migrations in CI/CD pipelines?
101. How do you perform canary releases with Istio/Linkerd service mesh?
102. How do you implement progressive delivery (canary -> blue/green)?
103. How do you manage pipeline concurrency and parallelism?
104. How do you detect and prevent pipeline deadlocks?
105. How do you implement automated canary analysis and validation?

## Monitoring, Alerting & Observability (106–125)

106. What are the four golden signals / RED / USE methods?
107. How would you design monitoring for EKS + RDS + EC2 from scratch?
108. Compare Prometheus + Grafana + Loki vs CloudWatch vs Datadog.
109. How do you set up SLOs, SLIs, and alert thresholds without alert fatigue?
110. Explain PromQL with an example alert query.
111. How do you collect logs from EKS (Fluent Bit, Promtail, CloudWatch agent)?
112. How do you trace requests across microservices (OpenTelemetry, Jaeger, Zipkin)?
113. How do you monitor Terraform / provisioning failures?
114. Walk through an on-call incident: high CPU on RDS, pods OOMKilled. Steps?
115. How do you implement on-call rotations, runbooks, and postmortems?
116. How do you prove observability coverage for customer SLAs?
117. How do you design alert deduplication and noise reduction?
118. Explain the difference between push-based and pull-based monitoring.
119. How do you implement synthetic monitoring and uptime checks?
120. How do you correlate logs, metrics, and traces during an incident?
121. How do you set up and manage PagerDuty / OpsGenie escalations?
122. How do you implement chatOps for incident management (Slack, Teams)?
123. How do you monitor infrastructure as code changes and drift?
124. How do you design dashboard layouts for SRE/DevOps teams?
125. How do you handle alert fatigue and on-call burnout?

## Cloud Security & Compliance (126–138)

126. Explain IAM users, roles, policies, permission boundaries with least-privilege examples.
127. How do you audit over-permissive IAM across many customer accounts?
128. How do you enforce encryption at rest and in transit (RDS, S3, EBS, TLS)?
129. How do you manage secrets rotation (Secrets Manager, SSM Parameter Store, Vault)?
130. How do you implement SCPs, SSO, and centralized logging for compliance?
131. What CIS Benchmark controls would you enforce first on AWS accounts?
132. How would you respond to an exposed AWS access key?
133. How do you implement S3 bucket policies vs IAM policies for least privilege?
134. How do you scan container images for vulnerabilities (Trivy, Anchore, Clair)?
135. Explain supply chain security for containers (SBOM, SLSA, Sigstore)?
136. How do you implement network policies and zero-trust in Kubernetes?
137. How do you audit and monitor Kubernetes API server access?
138. How do you implement data residency and sovereignty controls in multi-region deployments?

## Scripting & Automation (139–145)

139. Write a Bash script to check EKS node health and cordon faulty nodes.
140. Write a Python script using boto3 to list unencrypted RDS instances across regions.
141. How do you decide between Ansible vs Terraform vs Python/Bash for a task?
142. Explain idempotency in automation scripts with an example.
143. Write a Python script to auto-scale EC2 instances based on CPU utilization.
144. How do you implement Infrastructure as Code testing (terratest, testinfra)?
145. Write a Shell script to rotate AWS access keys automatically.

## On-Call & Incident Response (146–150)

146. Walk through an on-call incident: high CPU on RDS, pods OOMKilled. Steps?
147. How do you implement on-call rotations, runbooks, and postmortems?
148. How do you prioritize incidents (P1, P2, P3, P4) and manage alert fatigue?
149. How do you conduct blameless postmortems and turn learnings into playbooks?
150. How do you document and share incident runbooks across teams?

## Distributed Systems & Linux (151–155)

151. Explain CAP theorem and how it affects distributed system design.
152. How do you troubleshoot network latency issues between microservices?
153. Explain Linux networking: netfilter, iptables, nftables, connection tracking.
154. How do you debug DNS resolution issues at scale?
155. Explain the difference between synchronous and asynchronous replication.

## Behavioral & Scenario-Based (156–160)

156. Why are you a good fit for GoKwik's DevOps team with 1-4 years experience?
157. What would you improve in your first 90 days as a DevOps Engineer at GoKwik?
158. Describe a time you resolved a difficult production incident. What was your approach?
159. How do you handle competing priorities between feature delivery and reliability improvements?
160. Describe your experience with chaos engineering and resilience testing.

## GoKwik-Specific (161–170)

161. How would you optimize GoKwik's checkout pipeline for reliability and scale?
162. How would you design self-healing infrastructure for GoKwik's eCommerce platform?
163. How would you approach RTO (Return to Origin) reduction through infrastructure improvements?
164. How would you design a post-purchase engagement infrastructure that scales?
165. How would you implement AI-powered infrastructure monitoring at GoKwik scale?
166. How would you design multi-region active-active infrastructure for GoKwik?
167. How would you approach capacity planning for GoKwik's GMV of $2B+?
168. How would you design disaster recovery for GoKwik's critical commerce workflows?
169. How would you implement progressive delivery for GoKwik's frequent deployments?
170. How would you collaborate with GoKwik's product team to embed reliability from day one?

## Bonus & Rapid-Fire (171–175)

171. Favorite Kubernetes resource and why?
172. Most useful Terraform module you've written?
173. Best automation you've built that eliminated manual toil?
174. What's the most interesting on-call incident you've handled?
175. What new DevOps tool or practice are you excited about right now?