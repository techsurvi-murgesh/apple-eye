# 100 Interview Questions — AWS Kubernetes DevOps Engineer (VOIS) — 2026-11-11

Target stack: Amazon EKS, Kubernetes, Terraform, Argo CD, Helm, Docker, Git, AWS (VPC, EC2, S3, EBS, ELB, CloudWatch, CodeBuild, CodeCommit), GitOps, CI/CD, cloud security (RBAC, network policies, Secrets), observability, cost optimisation, ITIL/SOX compliance. Target experience: 3-5 years, business-critical cloud-native environments.

## Amazon EKS & Kubernetes (1–20)

1. What is Amazon EKS and how does it differ from self-managed Kubernetes?
2. Describe the EKS control plane vs. worker node responsibilities.
3. How do you create an EKS cluster using eksctl and Terraform?
4. What are Kubernetes Pods, Deployments, Services, ConfigMaps, Secrets, and ServiceAccounts?
5. How do you configure Kubernetes resource requests and limits, and why do they matter?
6. What is a NetworkPolicy and how do you restrict pod-to-pod traffic?
7. How do you handle Kubernetes service discovery and DNS?
8. What is an Ingress and how does an Ingress Controller work in EKS?
9. How do you upgrade an EKS cluster version without downtime?
10. How do you drain and cordon nodes during maintenance?
11. What is the Kubernetes scheduler and how does it place pods?
12. How do you use taints and tolerations, and node affinity/anti-affinity?
13. What are DaemonSets, StatefulSets, and Jobs/CronJobs used for?
14. How do you troubleshoot a pod in CrashLoopBackOff, ImagePullBackOff, or Pending state?
15. How do you configure liveness, readiness, and startup probes?
16. What is a HorizontalPodAutoscaler and how does it scale based on metrics?
17. How does the Kubernetes Cluster Autoscaler work with EKS managed node groups?
18. How do you manage etcd backups and disaster recovery for Kubernetes?
19. What are PriorityClasses and PodDisruptionBudgets?
20. How do you limit namespaces with ResourceQuotas and LimitRanges?

## Terraform & Infrastructure as Code (21–40)

21. Describe the Terraform workflow: init, plan, apply, destroy.
22. How do you structure reusable Terraform modules for VPC, EKS, and RDS?
23. How do you manage Terraform state in a team (remote backend, state locking)?
24. What is state drift and how do you detect and remediate it?
25. How do you handle multiple environments (dev/staging/prod) with Terraform?
26. What are Terraform workspaces vs. separate state files — pros and cons?
27. How do you version and publish Terraform modules?
28. Explain count vs. for_each with examples.
29. How do you handle sensitive values in Terraform (tfvars, Secrets Manager, Vault)?
30. What is `terraform import` and when would you use it?
31. How do you manage provider version constraints and dependency locking?
32. How do you test Terraform modules (tflint, Checkov, terratest)?
33. How do you roll out a breaking change to a shared Terraform module?
34. What are dynamic blocks and how do they simplify security group modules?
35. How do you implement compliance controls (encrypted S3, no open security groups) in Terraform?
36. How do you recover from a failed `terraform apply` mid-run?
37. What do you check when reviewing a Terraform pull request?
38. How do you configure a remote backend with S3 + DynamoDB?
39. How do you handle Terraform version upgrades across a team?
40. What is AWS CloudFormation and how does it compare to Terraform?

## GitOps, Argo CD & Helm (41–60)

41. What is GitOps and what are its core principles?
42. How does Argo CD implement declarative GitOps continuous delivery?
43. What is an Argo CD Application, and how does it sync from a Git repository?
44. What are Argo CD sync policies (automatic, manual, prune, self-heal)?
45. How do you manage Argo CD projects, applications, and repositories?
46. What are Argo Workflows and how do they differ from Argo CD?
47. How do you run automated testing in an Argo Workflow?
48. What is a Helm chart and what are its key files (Chart.yaml, values.yaml, templates)?
49. How do you template Kubernetes manifests with Helm?
50. How do you use Helm values files for multiple environments?
51. How do you create and maintain a Helm chart repository?
52. How do you perform Helm rollback and history inspection?
53. How do Argo CD and Helm work together in a GitOps pipeline?
54. How do you secure Helm chart signing and verification?
55. What are Helm hooks and when would you use them?
56. How do you automate Helm-based application deployments in CI/CD?
57. How do you handle secret injection in Helm/Argo CD without committing secrets to Git?
58. How do you drift-detect and self-heal with Argo CD?
59. How do you promote an application across dev → staging → prod with Argo CD?
60. What are AppOfApps and how do they simplify multi-app GitOps?

## Docker & Containers (61–70)

61. What is the difference between a Docker image and a container?
62. How do you write an efficient, secure Dockerfile (multi-stage builds, non-root user)?
63. What is Source-to-Image (S2I) and when is it used?
64. How do you reduce Docker image size and scan for vulnerabilities?
65. How do you push images to Amazon ECR and authenticate?
66. What are init containers and sidecar containers in Kubernetes?
67. How do you configure container security contexts (runAsNonRoot, readOnlyRootFilesystem)?
68. How do you manage image pull policies and image pull secrets?
69. What is a container runtime and which ones does EKS support?
70. How do you debug a running container with kubectl exec and logs?

## AWS Cloud Infrastructure & Networking (71–80)

71. What AWS services have you used (VPC, EC2, ECS, S3, EBS, Glacier, ELB, Elastic IP)?
72. How do you design a VPC with public/private subnets, NAT gateway, and route tables?
73. What is the difference between an ALB, NLB, and CLB?
74. How do you configure security groups vs. network ACLs?
75. How do you provision an EKS cluster in existing VPC subnets?
76. What is an Elastic IP and when would you use one?
77. How do you use AWS CloudWatch for metrics, logs, and alarms?
78. How do you use AWS CodeBuild and CodeCommit in a CI/CD pipeline?
79. How do you manage IAM roles for EKS worker nodes and IRSA for pods?
80. How do you handle AWS billing alerts and cost governance?

## CI/CD & Git (81–90)

81. How do you design a CI/CD pipeline (build → test → scan → deploy)?
82. What is the role of Git in infrastructure as code and GitOps workflows?
83. How do you handle branching strategies and pull request gates?
84. How do you integrate automated testing into a CI/CD pipeline?
85. How do you run SAST/SCA and container image scanning in CI?
86. How do you handle deployment strategies (blue/green, canary, rolling)?
87. How do you roll back a failed deployment in Kubernetes/Argo CD?
88. How do you manage environment promotion and approval gates?
89. How do you secure CI/CD secrets and credentials?
90. How do you measure CI/CD pipeline reliability (lead time, MTTR, deployment frequency)?

## Cloud Security, Compliance & Observability (91–100)

91. How do you implement Kubernetes RBAC (Roles, RoleBindings, ClusterRoles)?
92. How do you manage Kubernetes Secrets securely (Sealed Secrets, External Secrets, KMS)?
93. What security policies would you apply (PodSecurity, network policies, OPA/Gatekeeper)?
94. How do you meet ITIL, SOX, and security regulation requirements in the cloud?
95. How do you monitor cloud-resource consumption and optimise EKS cost?
96. How do you set up centralized logging (CloudWatch Logs, Loki, ELK) and alerting?
97. How do you trace distributed requests and define SLOs/SLIs?
98. How do you run incident response and blameless postmortems for business-critical systems?
99. How do you harden an EKS cluster (control-plane logging, encryption, private endpoints)?
100. How do you balance resilience, scalability, security, and cost in cloud-native infrastructure?
