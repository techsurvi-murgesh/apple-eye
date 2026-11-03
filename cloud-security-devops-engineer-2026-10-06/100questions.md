# 100 Interview Questions — DevOps Engineer, Cloud Security (Cisco SSE Control Plane / Umbrella / Secure Access)

## SSE / Cloud Security / Microservices (1-12)
1. What is Cisco Umbrella / Secure Access (SSE) at a high level and what problems does it solve?
2. What is a cloud security control plane vs data plane?
3. How do microservices for network experience / traffic optimization communicate securely?
4. How would you design a reliable microservice for traffic insights (ingest, aggregate, serve)?
5. How do you handle multi-tenancy, rate limiting, and noisy neighbors in control plane services?
6. What is zero trust / secure access (ZTNA) in simple terms?
7. How do you secure service-to-service traffic (mTLS, service mesh, short-lived creds)?
8. How do you manage secrets for microservices (rotation, least privilege)?
9. How do you do safe rollouts for a control plane API serving many customers?
10. What reliability signals matter for control plane (availability, latency, error budget)?
11. How do you learn a large unfamiliar codebase and infra quickly as a new DevOps hire?
12. How do you collaborate with developers, sysadmins, and cross-functional teams on infra needs?

## CI/CD — Jenkins (13-28)
13. How do you build a Jenkins pipeline for Docker + Terraform + Helm deployments?
14. Declarative vs scripted Jenkins pipelines — when to use each?
15. How do you structure shared libraries to reuse pipeline code?
16. How do you troubleshoot a failing Jenkins build (stages, logs, agents, artifacts)?
17. How do you manage Jenkins agents (static, Docker, Kubernetes clouds)?
18. How do you handle credentials and secret masking in Jenkins?
19. How do you implement quality gates (lint, test, image scan, Terraform plan) in Jenkins?
20. How do you do branch/PR builds with GitHub, GitLab, or Bitbucket webhooks?
21. How do you speed up slow Jenkins pipelines (caching, parallelism, agent sizing)?
22. How do you back up Jenkins controllers and recover after failure?
23. How do you manage plugins without breaking pipelines?
24. How do you secure Jenkins (RBAC, SSO, agent-to-controller access, script approval)?
25. How do you compare Jenkins vs GitHub Actions vs GitLab CI for a new service?
26. How do you implement manual approvals and deployment windows in Jenkins?
27. How do you version pipeline changes with Git and code review?
28. Walk through debugging "pipeline passed but deploy is broken".

## Terraform IaC on AWS (29-40)
29. How do you structure Terraform modules for VPC, EKS, and RDS?
30. How does Terraform state work and how do you manage remote state + locking?
31. How do you integrate Terraform plan/apply into Jenkins pipelines safely?
32. How do you review a Terraform plan to prevent outages?
33. How do you handle drift between real AWS resources and state?
34. How do you manage multiple environments (dev/stage/prod) with Terraform?
35. How do you pass secrets to Terraform without leaking them?
36. How do you refactor Terraform code without destroying resources (moved blocks)?
37. How do you test Terraform (tflint, checkov, plan gates)?
38. How do you roll back a bad Terraform apply?
39. How do you manage Terraform versions and provider upgrades?
40. How would you provision a new EKS cluster + VPC from scratch with Terraform?

## Docker / EKS / Helm (41-58)
41. How do you containerize a Python backend and a React frontend for production?
42. How do you write secure Dockerfiles (multi-stage, non-root, minimal base, pinned tags)?
43. How do you migrate a legacy VM/EC2 app to EKS step by step?
44. Explain Kubernetes Pods, Deployments, Services, Ingress, ConfigMaps, Secrets.
45. How do you deploy, manage, and debug workloads on EKS (kubectl, events, logs)?
46. How do you troubleshoot CrashLoopBackOff, ImagePullBackOff, OOMKilled, and Pending pods?
47. How do you configure probes (liveness/readiness), resource requests/limits, and HPA?
48. How do Helm charts simplify Docker/Terraform/K8s deployments?
49. How do you manage Helm values per environment and secret handling?
50. How do you do rolling updates vs blue-green vs canary on EKS?
51. How do you handle persistent storage on EKS (StorageClass, PVC)?
52. How do EKS IRSA, cluster autoscaler, and ALB controller work?
53. How do you Debug "service reachable in cluster but not from outside"?
54. How do you right-size EKS nodes and control cost?
55. How do you back up EKS workloads and recover?
56. How do you scan and patch container images in the pipeline?
57. How do you manage image tags and registries (ECR) across envs?
58. How do you support developers with local Docker workflows that mirror EKS?

## Backend / REST APIs / Scripting (59-70)
59. How do you debug a Python backend issue end-to-end (logs, traces, repro)?
60. How do you integrate microservices via RESTful APIs (auth, pagination, retries)?
61. How do you design idempotent REST endpoints for safe retries?
62. How do you handle REST rate limits and backoff in automation?
63. How do you automate a routine deployment task with Bash vs Python?
64. How do you write robust Bash scripts (set -euo pipefail, logging, traps)?
65. How do you parse JSON APIs with jq in Bash and requests in Python?
66. How do you test automation scripts (shellcheck, pytest, dry-run)?
67. How do you convert a manual runbook into automation safely?
68. How do you use Git branching, merging, and PRs for automation repos?
69. How do GitLab vs Bitbucket vs GitHub workflows differ in practice?
70. How do you review infra/automation PRs for risk?

## GitOps — ArgoCD / Flux (71-76)
71. What is GitOps and how do ArgoCD/Flux reconcile desired vs actual state?
72. How would you bootstrap ArgoCD for an EKS cluster with Terraform + Helm?
73. How do you structure Git repos for app code vs GitOps manifests?
74. How do you handle secrets in GitOps without committing plaintext?
75. How do you do progressive delivery (canary/rollbacks) with ArgoCD?
76. How do you debug "ArgoCD says OutOfSync / degraded"?

## AWS Networking (77-86)
77. How do VPCs, subnets (public/private), route tables, and NAT gateways fit together?
78. How do security groups differ from NACLs?
79. How do you design EKS networking for private nodes with controlled egress?
80. How does load balancing work (ALB vs NLB) for EKS services and Ingress?
81. How do you troubleshoot EKS-to-RDS or EKS-to-external connectivity issues?
82. Explain DNS resolution inside VPC and Kubernetes (CoreDNS).
83. How do you expose a control plane API securely (private + public paths)?
84. How do you manage TLS termination at ALB vs Ingress?
85. How do you audit overly permissive security groups?
86. How do you plan IP addressing to avoid VPC/CNI exhaustion?

## Observability — Prometheus / Grafana / Splunk (87-94)
87. How do you monitor EKS cluster health vs application performance?
88. What are RED/USE metrics and which would you alert on first?
89. How do you build Grafana dashboards for latency, errors, and traffic insights?
90. How do you write Prometheus alerts that avoid noise (for/burn rate)?
91. How do you aggregate and search logs with Loki vs Splunk vs ELK?
92. How do you correlate a deploy with a spike in errors using metrics + logs?
93. How do you monitor Terraform/Jenkins pipeline health itself?
94. How do you set SLOs and error budgets for control plane services?

## Troubleshooting / Networking Phones / Security / Culture (95-100)
95. Walk through troubleshooting across platform and app: slow API on EKS + RDS.
96. Explain DNS, HTTP/HTTPS, TCP/IP, and firewalls using a real Umbrella-style request path.
97. How do you approach on-call for a control plane incident (triage, comms, postmortem)?
98. How do you balance speed vs safety when production is degraded?
99. How do you keep learning new DevOps tools quickly in a fast-changing org?
100. Why Cloud Security / SSE control plane work, and what would you ramp on in the first 90 days?
