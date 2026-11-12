# 100 Interview Questions — DevOps Engineer (Wolters Kluwer) — 2026-11-11

Target stack: AWS/Azure, Docker, Kubernetes, Terraform (IaC), Python/PowerShell/Shell scripting, CI/CD pipelines, full-stack monitoring, availability management, disaster recovery, change/release management, web app operations (IIS/Azure Service Environments/Service Fabric). Target experience: 2+ years IT, 2+ years cloud, 2+ years DevOps/AppOps.

## Availability & Service Management (1–12)

1. What is availability management and what tasks does it involve?
2. How do you analyse service and component availability, reliability, maintainability, and serviceability?
3. How do you ensure services meet agreed performance targets and service levels (SLAs)?
4. How do you implement disaster recovery arrangements and document recovery procedures?
5. How do you conduct testing of recovery procedures (DR drills)?
6. What is the difference between RTO and RPO?
7. How do you design highly available and highly scalable solutions?
8. How do you engage with project teams to confirm service acceptance criteria?
9. How do you feed into change management processes?
10. What is a change request and how do you apply change control procedures?
11. How do you track, log and correct information related to Configuration Items (CIs)?
12. How do you protect assets and components from unauthorized change, diversion, and inappropriate use?

## Release, Deployment & CI/CD (13–28)

13. What tools and techniques do you use for release and deployment activities?
14. How do you create, manage, and maintain DevOps pipelines?
15. How do you design a CI/CD pipeline (build → test → deploy)?
16. How do you handle rollback and release traceability?
17. How do you review system software updates and identify those that merit action?
18. How do you deploy web applications, web services, and applications on IIS?
19. How do you deploy applications on Azure Service Environments and Azure Service Fabric?
20. How do you manage environment promotion and approval gates?
21. How do you handle controlled artifact promotion?
22. How do you implement blue-green and canary deployments?
23. How do you secure CI/CD secrets and credentials?
24. How do you measure pipeline reliability (lead time, MTTR, deployment frequency)?
25. How do you handle pipeline failures and automated rollbacks?
26. How do you manage branching strategies and pull request gates?
27. How do you integrate automated testing into CI/CD?
28. How do you run SAST/SCA and container image scanning in CI?

## Cloud: AWS & Azure (29–44)

29. What AWS services have you used (EC2, VPC, IAM, S3, ELB, Route 53, CloudWatch, EKS, ECS, RDS, Lambda, ECR)?
30. How do you build and maintain systems in AWS?
31. What Azure services have you used (web apps, IIS, Service Environments, Service Fabric)?
32. How do you build and maintain systems in Azure?
33. How do you design VPC networking with public/private subnets and NAT?
34. What is the difference between ALB, NLB, and CLB?
35. How do you configure security groups vs. network ACLs?
36. How do you manage IAM roles and least-privilege access?
37. How do you use S3 with encryption and block public access?
38. How do you set up CloudWatch metrics, logs, and alarms?
39. How do you use Azure Monitor and Application Insights?
40. How do you handle multi-region HA/DR?
41. How do you manage Route 53 routing policies?
42. How do you use Azure Service Fabric for stateful/stateless services?
43. How do you deploy to IIS and configure application pools?
44. How do you handle cloud cost governance and billing alerts?

## Docker & Kubernetes (45–58)

45. What is the difference between a Docker image and a container?
46. How do you write an efficient, secure Dockerfile (multi-stage builds, non-root user)?
47. How do you reduce Docker image size and scan for vulnerabilities?
48. How do you push images to ECR/Azure Container Registry?
49. What are Kubernetes Pods, Deployments, Services, ConfigMaps, Secrets, and ServiceAccounts?
50. How do you configure Kubernetes resource requests and limits?
51. What is a NetworkPolicy and how do you restrict pod-to-pod traffic?
52. How do you troubleshoot CrashLoopBackOff, ImagePullBackOff, or Pending pods?
53. How do you configure liveness, readiness, and startup probes?
54. What is a HorizontalPodAutoscaler and how does it scale?
55. How do you use Helm charts and maintain a Helm repository?
56. How do you perform Helm rollback and history inspection?
57. What are init containers and sidecar containers?
58. How do you debug a running container with kubectl exec and logs?

## Terraform & Infrastructure as Code (59–70)

59. Describe the Terraform workflow: init, plan, apply, destroy.
60. How do you structure reusable Terraform modules?
61. How do you manage Terraform state in a team (remote backend, state locking)?
62. What is state drift and how do you detect and remediate it?
63. How do you handle multiple environments (dev/staging/prod) with Terraform?
64. What are Terraform workspaces vs. separate state files?
65. How do you version and publish Terraform modules?
66. Explain count vs. for_each with examples.
67. How do you handle sensitive values in Terraform (tfvars, Secrets Manager, Key Vault)?
68. What is `terraform import` and when would you use it?
69. How do you manage provider version constraints and dependency locking?
70. How do you test Terraform modules (tflint, Checkov, terratest)?

## Scripting & Automation (71–78)

71. How do you use Python, PowerShell, or Shell scripting to automate DevOps tasks?
72. How do you write idempotent scripts?
73. How do you handle error handling and logging in scripts?
74. How do you automate infrastructure provisioning with scripts?
75. How do you integrate scripts into CI/CD pipelines?
76. How do you manage secrets in scripts (environment variables, secret stores)?
77. How do you automate server configuration and patching?
78. How do you eliminate manual toil with automation?

## Monitoring & Observability (79–88)

79. How do you implement full-stack monitoring (infra, cloud platform, OS, apps telemetry)?
80. How do you use Prometheus, Grafana, Loki, and CloudWatch together?
81. How do you set up centralized logging and distributed tracing?
82. How do you define SLOs, SLIs, and SLAs?
83. How do you create dashboards and alerts to reduce noise?
84. How do you troubleshoot high latency or errors in a microservices architecture?
85. How do you monitor application performance (APM) on IIS/Azure?
86. How do you set up log aggregation and retention?
87. How do you define alerting thresholds and escalation paths?
88. How do you correlate infrastructure metrics with application telemetry?

## Incident & Problem Management (89–96)

89. How do you investigate and coordinate resolution of service problems?
90. How do you lead incident response and RCA (root cause analysis)?
91. How do you prepare and maintain operational documentation for system software?
92. How do you run blameless postmortems?
93. How do you define error budgets and SLO-based alerting?
94. How do you handle on-call rotations and incident severity levels?
95. How do you document recovery procedures and runbooks?
96. How do you balance incident response with planned project work?

## Technology Evaluation & Growth (97–100)

97. How do you explore new technologies and participate in pilots/POCs?
98. How do you evaluate development patterns and make recommendations?
99. How do you stay current with DevOps and cloud trends?
100. How do you balance routine technology tasks with increasing independence and complex responsibilities?
