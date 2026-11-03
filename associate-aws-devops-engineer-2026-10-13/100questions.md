# 100 Interview Questions — Associate AWS DevOps Engineer (Mumbai) — 2026-10-13

Target profile: associate/junior (2–4 yrs) AWS DevOps engineer on an advisory/infrastructure team. AWS core services, Terraform/CloudFormation, CI/CD (Jenkins, CodePipeline/CodeBuild), Docker/ECS/EKS, Python/Bash automation, Ansible, VPC networking, IAM/security, CloudWatch/CloudTrail/ELK observability.

## AWS Core Services & Architecture (1–16)

1. What are the main compute options in AWS and when would you pick EC2 over Lambda (and vice versa)?
2. Explain the difference between a security group and a NACL. Why do we need both?
3. Walk me through designing a highly available VPC for a 3-tier web app on AWS.
4. What is an Elastic Load Balancer? Difference between ALB, NLB, and GWLB?
5. How do you keep an RDS instance highly available? What is a Multi-AZ deployment vs a read replica?
6. What are S3 storage classes and how would you choose between them?
7. Explain Auto Scaling groups, launch templates, and health checks.
8. What is an Elastic IP and when is it a bad idea?
9. Explain Route 53 routing policies: simple, weighted, latency, failover, geolocation.
10. What is an AMI and how do you build one responsibly?
11. Explain the difference between public, private, and isolated subnets.
12. How does AWS PrivateLink / a NAT gateway differ from a public IP?
13. What are Availability Zones and why does it matter for a 99.9% SLA?
14. Explain VPC peering vs Transit Gateway vs VPC endpoints.
15. What is an AWS Outpost / edge service and when would you use it?
16. How would you decide between CloudFormation, Terraform, and CDK for a new team?

## VPC Networking & Connectivity (17–28)

17. What is DNS in the VPC context? How does Route 53 differ from a corporate DNS server?
18. Explain TCP/IP handshake and how it matters when debugging connectivity.
19. What is a VPN and how does it differ from a Direct Connect connection?
20. Walk me through troubleshooting an EC2 instance that cannot reach the internet.
21. What is a NAT gateway and why is it stateful?
22. How do NACLs differ from security groups in statefulness and ordering?
23. What is a VPC flow log and how do you use it for debugging?
24. Explain DNS resolution for an ELB — how does Route 53 health check work?
25. How would you connect an on-premises data centre to AWS VPC?
26. What happens to network traffic when a security group has no outbound rule?
27. Explain IPv4 vs IPv6 in VPCs and the implications for security rules.
28. What is a transit gateway attachment and how is it billed?

## IAM, Security & Encryption (29–42)

29. What is an IAM role and why prefer it over a long-lived access key?
30. Explain IAM policies: identity-based, resource-based, and trust policies.
31. What is the difference between an IAM user and an IAM role?
32. How do you grant least-privilege access in practice?
33. Explain permission boundaries vs IAM policies.
34. What is an OIDC provider role and why use it for CI?
35. How does AWS Organizations/SCP differ from an IAM policy?
36. What data encryption options does RDS support (at rest and in transit)?
37. Explain KMS: customer-managed vs AWS-managed keys.
38. How do you store and rotate secrets in AWS (Secrets Manager, SSM Parameter Store)?
39. What is the principle of "deny by default" in IAM evaluation?
40. Explain how CloudTrail helps in a security investigation.
41. What is AWS Config and how does it enforce security baselines?
42. How do you guard against an S3 bucket being made public by accident?

## Infrastructure as Code (43–54)

43. What problem does Terraform solve, and what are its main building blocks?
44. Explain the Terraform lifecycle: init, plan, apply, destroy.
45. What are providers, modules, state files, and workspaces?
46. How do you manage remote state safely (backend locking, encryption)?
47. Explain `terraform plan` output — what should you always review?
48. How do you manage secrets and sensitive values in Terraform?
49. What is drift detection and how do you handle it?
50. How do you promote infrastructure changes from dev to prod?
51. When would you use CloudFormation instead of Terraform?
52. What is a CDK app and how does it differ from a template-based approach?
53. How do you version and tag infrastructure resources?
54. How would you refactor a 500-line Terraform module safely?

## CI/CD (55–68)

55. What are the stages of a CI/CD pipeline?
56. Explain the difference between continuous delivery and continuous deployment.
57. How does CodePipeline differ from Jenkins?
58. What is CodeBuild and when is it a good fit?
59. How do you set up a Jenkins pipeline for a Dockerised application?
60. How do you manage credentials in a CI pipeline securely?
61. Explain blue/green, canary, and rolling deployment strategies.
62. How do you roll back a bad deployment quickly?
63. What is a GitOps workflow and how does it differ from push-based CI/CD?
64. How do you run tests in a pipeline before deployment?
65. Explain artifact storage and why you should never rebuild between stages.
66. How do you implement a manual approval gate before production?
67. What is a pipeline failure-rate notification and how do you configure it?
68. How do you make a CI pipeline faster?

## Containers: Docker, ECS, EKS (69–80)

69. What happens between `docker run` and a process starting in a container?
70. Explain Docker image layers and why layer caching matters in CI.
71. What is a multi-stage Docker build and why use it?
72. Explain the difference between ECS (Fargate vs EC2) and EKS.
73. What is a Kubernetes pod and what is a deployment?
74. Difference between a Deployment, StatefulSet, and DaemonSet?
75. What are Services vs Ingress in Kubernetes?
76. How do you configure resource limits and requests for a container?
77. What is a ConfigMap vs a Secret in Kubernetes?
78. Explain liveness vs readiness probes.
79. How would you expose an application outside the cluster?
80. What is the difference between ECS Task Definition and a Kubernetes deployment YAML?

## Automation & Scripting (81–88)

81. How do you choose between Bash and Python for an automation script?
82. What makes a script safe to run in production (idempotency, dry-run, logging)?
83. Explain idempotency and why it matters in IaC and config management.
84. How would you automate an EC2 instance provisioning with Ansible?
85. What are Ansible playbooks, roles, and inventories?
86. How do you pass secrets to an Ansible run?
87. How would you write a script to check the health of all running EC2 instances?
88. Explain crontab and how you'd schedule an automation safely.

## Monitoring, Logging & Alerting (89–95)

89. What is CloudWatch and what can you do with metrics, alarms, and logs?
90. How do you set up an alarm for high CPU on an EC2 instance?
91. What is a composite CloudWatch alarm?
92. What is CloudTrail, and what events does it record by default?
93. How would you set up centralized logging (ELK / OpenSearch) for AWS?
94. What metrics do you monitor for an ELB and an RDS instance?
95. How do you reduce alert fatigue?

## Serverless, Troubleshooting & Behavioural (96–100)

96. Explain an AWS Lambda function: triggers, concurrency, and cold starts.
97. What is API Gateway and how does it fit with Lambda?
98. A deployment just failed in production. Walk me through your troubleshooting process.
99. How do you prioritise when multiple infrastructure incidents occur at once?
100. Why do you want to work in a fast-paced advisory environment, and how do you document your work?

---