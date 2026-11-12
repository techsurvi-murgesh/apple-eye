# 100 Interview Questions — AWS Cloud DevOps Lead (Deloitte) — 2026-11-11

Target stack: AWS (Organizations, SCPs, multi-account, VPC, Transit Gateway, Direct Connect, EC2, S3, IAM, KMS, Route 53, ELB), EKS/Kubernetes, Terraform/CloudFormation/CDK, Docker, Helm, ECR, CI/CD (CodePipeline/CodeBuild/CodeDeploy, Jenkins, GitLab CI, GitHub Actions), DevSecOps (Secrets Manager, Parameter Store, CloudTrail, Config, GuardDuty, Security Hub), observability (CloudWatch, X-Ray, Prometheus, Grafana, OpenSearch), FinOps, SRE/DR/HA, banking/regulated (RBI IT governance), team leadership. Target experience: 4-9 years, hands-on lead.

## AWS Architecture & Multi-Account (1–18)

1. What is AWS Organizations and how do you structure a multi-account landing zone?
2. What are SCPs and how do they differ from IAM policies?
3. How do you design VPC networking with Transit Gateway, VPC endpoints, NAT, VPN and Direct Connect?
4. How do you deliver HA/DR across Availability Zones and Regions?
5. What is the difference between an ALB, NLB, and CLB?
6. How do you configure security groups vs. network ACLs in a multi-tier VPC?
7. How do you peer VPCs across accounts and regions?
8. What is an Elastic IP and when would you use one?
9. How do you design subnets (public/private/isolated) and route tables for a banking platform?
10. How do you handle cross-account IAM roles and trust policies?
11. How do you enforce tagging and resource standards across accounts?
12. What is AWS Control Tower and how does it relate to landing zones?
13. How do you manage Route 53 routing policies (failover, geolocation, latency)?
14. How do you secure S3 buckets (block public access, encryption, bucket policies)?
15. How do you use KMS for envelope encryption and key rotation?
16. How do you set up CloudWatch cross-account observability?
17. What is AWS Resource Access Manager (RAM) and when is it used?
18. How do you design a disaster recovery strategy (pilot light, warm standby, multi-site)?

## EKS & Kubernetes (19–36)

19. What is Amazon EKS and how does the control plane differ from worker nodes?
20. How do you create an EKS cluster using eksctl and Terraform?
21. What are EKS node groups (managed, self-managed, Fargate) and when use each?
22. How does the Kubernetes Cluster Autoscaler work with EKS managed node groups?
23. How do you configure IRSA vs. EKS Pod Identity for pod IAM permissions?
24. What is the AWS Load Balancer Controller and how does it provision ALB/NLB for ingress?
25. How do you design EKS networking (CNIs, pod CIDR, service CIDR)?
26. How do you manage EKS storage (EBS, EFS, FSx, storage classes)?
27. How do you upgrade an EKS cluster version without downtime?
28. How do you drain and cordon nodes during maintenance?
29. What are Kubernetes Pods, Deployments, Services, ConfigMaps, Secrets, and ServiceAccounts?
30. How do you configure liveness, readiness, and startup probes?
31. What is a HorizontalPodAutoscaler and how does it scale?
32. What are NetworkPolicies and how do you restrict pod-to-pod traffic?
33. How do you use Helm charts and maintain a Helm repository?
34. How do you push and pull images from Amazon ECR?
35. How do you build standard deployment patterns (blue-green, canary, rolling) on EKS?
36. How do you enable developer self-service for EKS deployments?

## Terraform & Infrastructure as Code (37–50)

37. Describe the Terraform workflow: init, plan, apply, destroy.
38. How do you structure reusable Terraform modules for VPC, EKS, and RDS?
39. How do you manage Terraform state in a team (remote backend, state locking)?
40. What is state drift and how do you detect and remediate it?
41. How do you handle multiple environments (dev/staging/prod) with Terraform?
42. What are Terraform workspaces vs. separate state files — pros and cons?
43. How do you version and publish Terraform modules?
44. Explain count vs. for_each with examples.
45. How do you handle sensitive values in Terraform (tfvars, Secrets Manager, Vault)?
46. What is `terraform import` and when would you use it?
47. How do you manage provider version constraints and dependency locking?
48. How do you test Terraform modules (tflint, Checkov, terratest)?
49. How do you implement policy checks (OPA/Sentinel) and compliance in Terraform?
50. How does AWS CloudFormation/CDK compare to Terraform, and when would you use each?

## CI/CD (51–65)

51. How do you design a CI/CD pipeline (build → test → scan → approve → deploy → rollback)?
52. How do you build reusable pipeline templates for Java/Spring Boot microservices?
53. How do you use CodePipeline, CodeBuild, and CodeDeploy together?
54. How do you integrate Jenkins, GitLab CI, and GitHub Actions in enterprise CI/CD?
55. How do you embed security scanning (SAST/SCA/container) in CI/CD?
56. What is controlled artifact promotion and how do you enforce it?
57. How do you implement blue-green and canary deployments?
58. How do you enforce approvals, rollback, and release traceability?
59. How do you manage CI/CD secrets and credentials securely?
60. How do you measure pipeline reliability (lead time, MTTR, deployment frequency, failure rate)?
61. How do you handle pipeline failures and automated rollbacks?
62. What is GitOps and how does Argo CD fit into CI/CD?
63. How do you promote applications across dev → staging → prod?
64. How do you handle environment-specific configuration in CI/CD?
65. How do you secure the CI/CD supply chain (signed artifacts, SBOM)?

## DevSecOps & Compliance (66–78)

66. How do you implement least-privilege IAM and federated identity?
67. How do you enforce MFA and privileged access controls?
68. How do you use Secrets Manager, Parameter Store, and KMS for secrets and encryption?
69. How do you rotate secrets and encryption keys?
70. How do you use CloudTrail, Config, GuardDuty, and Security Hub for posture management?
71. How do you ensure audit trails and compliance evidence for regulators and auditors?
72. How do you implement Kubernetes RBAC (Roles, RoleBindings, ClusterRoles)?
73. How do you manage Kubernetes Secrets securely (Sealed Secrets, External Secrets, KMS)?
74. What security policies would you apply (PodSecurity, network policies, OPA/Gatekeeper)?
75. How do you meet RBI IT governance and outsourcing requirements in banking?
76. How do you harden an AWS account (IAM, SCPs, GuardDuty, Security Hub baselines)?
77. How do you handle vulnerability management and container image scanning?
78. How do you run access reviews and privileged access governance?

## Observability, SRE & Incident Management (79–88)

79. How do you build monitoring with CloudWatch, X-Ray, Prometheus, Grafana and OpenSearch?
80. How do you define SLOs, SLIs, and SLAs?
81. How do you set up centralized logging and distributed tracing?
82. How do you lead incident response and RCA (root cause analysis)?
83. How do you run DR and resilience exercises (chaos, game days)?
84. How do you design alerting to reduce noise and avoid alert fatigue?
85. How do you create dashboards for leadership and engineering teams?
86. How do you troubleshoot high latency or errors in a microservices architecture?
87. How do you define error budgets and SLO-based alerting?
88. How do you run blameless postmortems?

## FinOps & Cost Optimisation (89–95)

89. How do you drive cost visibility through tagging, budgets and allocation?
90. How do you optimise through rightsizing and Auto Scaling?
91. How do you use purchasing strategy (Savings Plans, Reserved Instances, Spot)?
92. How do you apply storage lifecycle policies (S3 Intelligent-Tiering, Glacier)?
93. How do you report savings to leadership?
94. How do you set up AWS Cost Explorer, Budgets, and Cur reports?
95. How do you identify and eliminate idle or underutilized resources?

## Leadership & Banking Domain (96–100)

96. How do you mentor a team of DevOps, platform and automation engineers?
97. How do you set engineering standards and lead design reviews?
98. How do you handle complex troubleshooting across application, security, database and operations teams?
99. What is your experience in regulated environments, preferably banking/financial services?
100. How do you balance hands-on technical work with people leadership responsibilities?
