# 100 Interview Questions — AWS Site Reliability Engineer (ITC Infotech) — 2026-10-07

Target stack: AWS (EC2, VPC, S3, IAM, RDS, Route 53, ELB/ALB/NLB, Auto Scaling, CloudWatch, Lambda, SNS/SQS, EKS/ECS, CloudFormation), Linux/Windows, Terraform, Ansible, Jenkins, Python/Shell/PowerShell, CloudWatch/Datadog/Splunk/Dynatrace, AWS Security Hub/GuardDuty/Config, ITIL, RCA, DR/backup, cost optimization.

## AWS Core & Compute (1-16)

1. Explain the AWS global infrastructure: regions, availability zones, edge locations.
2. Walk through launching a highly available EC2-based web tier across multiple AZs.
3. How do you choose between EC2 instance families and sizes for a workload?
4. Explain EC2 purchasing options: On-Demand, Reserved, Spot, Savings Plans.
5. How do you troubleshoot an EC2 instance that is unreachable over SSH?
6. Explain Auto Scaling groups, launch templates, and scaling policies.
7. How do you design a self-healing, highly available architecture on AWS?
8. What is the difference between ALB, NLB, and CLB, and when do you use each?
9. How do health checks and target groups work behind an ALB?
10. Explain Route 53 routing policies (simple, weighted, latency, failover, geolocation).
11. How do you implement a DNS failover for disaster recovery?
12. Explain Lambda: execution model, cold starts, concurrency, and limits.
13. When would you use Lambda instead of EC2/ECS for an operational task?
14. How do SNS and SQS differ, and how do you use them together for decoupling?
15. Explain SQS standard vs FIFO, visibility timeout, DLQs, and idempotency.
16. How do you automate an operational task end-to-end with Lambda + EventBridge + SNS?

## Networking & VPC (17-28)

17. Explain VPC components: subnets, route tables, IGW, NAT, and CIDR design.
18. How do you design a multi-tier VPC (public/private/data subnets)?
19. Difference between security groups and NACLs, and how they work together.
20. How do you troubleshoot connectivity between two subnets or to the internet?
21. What is VPC peering vs Transit Gateway vs PrivateLink?
22. How do you connect an on-prem data center to AWS (VPN vs Direct Connect)?
23. How do you debug DNS resolution inside a VPC (Route 53 resolver, DHCP options)?
24. Explain VPC endpoints (gateway vs interface) and why they improve security.
25. How do you capture and analyze network traffic (VPC Flow Logs, tcpdump)?
26. How do you implement a bastion host vs AWS Systems Manager Session Manager?
27. How do you design egress control and NAT gateway cost optimization?
28. Explain OSI layers with a real AWS connectivity debugging example.

## Storage, Databases & DR (29-42)

29. Explain S3 storage classes and lifecycle policies for cost optimization.
30. How do you secure S3 (bucket policies, Block Public Access, encryption, presigned URLs)?
31. How do you troubleshoot an S3 403 Access Denied for an application?
32. Explain S3 versioning, replication, and object lock for compliance.
33. Explain EBS volume types and when to use gp3, io2, or st1.
34. How do you take and restore EBS snapshots and AMIs?
35. Explain RDS Multi-AZ vs read replicas and failover behavior.
36. How do you perform an RDS major-version upgrade with minimal downtime?
37. How do you troubleshoot RDS connection exhaustion and slow queries?
38. How do you design a backup and disaster recovery strategy (RPO/RTO)?
39. Explain AWS Backup and cross-region backup/restore.
40. How do you test a disaster recovery plan without impacting production?
41. Explain difference between RPO and RTO with an example.
42. How do EFS, FSx, and S3 fit different storage needs?

## IAM & Security, Compliance (43-58)

43. Explain IAM users, groups, roles, and policies.
44. What is the difference between identity-based and resource-based policies?
45. How do you implement least privilege for an application on EC2/EKS?
46. Explain IAM roles for EC2 (instance profiles) and EKS (IRSA).
47. How do you troubleshoot an "Access Denied" IAM error systematically?
48. How do you rotate access keys and secrets safely?
49. Explain AWS KMS, SSE-S3, SSE-KMS, and envelope encryption.
50. What is AWS Secrets Manager vs Parameter Store?
51. Explain AWS Security Hub, GuardDuty, and AWS Config and how they work together.
52. How do you remediate a GuardDuty finding?
53. How do you use AWS Config rules for compliance and drift detection?
54. How do you implement centralized logging and Security Hub across accounts?
55. Explain AWS Organizations, SCPs, and multi-account strategy.
56. How do you handle patching across Linux and Windows fleets (SSM Patch Manager)?
57. How do you meet compliance requirements (CIS, SOC 2, PCI) on AWS?
58. How do you respond to a suspected compromised EC2 instance?

## Monitoring, Observability & SRE (59-72)

59. Explain CloudWatch metrics, logs, alarms, and dashboards.
60. How do you design actionable CloudWatch alarms to avoid alert fatigue?
61. What is CloudWatch Logs Insights and how do you query it?
62. Explain CloudWatch agent vs unified CloudWatch agent for custom metrics/logs.
63. How do you monitor application health beyond infrastructure metrics?
64. Compare Datadog, Splunk, Dynatrace, and CloudWatch for observability.
65. How do you implement distributed tracing for microservices?
66. What is an SLO, SLI, and error budget, and how do you apply them?
67. How do you reduce MTTR through better observability and runbooks?
68. How do you set up synthetic and uptime monitoring?
69. How do you monitor AWS costs and set budget alarms?
70. How do you build an on-call rotation and an incident escalation process?
71. How do you run a blameless postmortem and produce a solid RCA?
72. How do you monitor CI/CD and deployment health, not just the app?

## Automation, IaC & DevOps (73-88)

73. Explain Terraform workflow: init, plan, apply, state, providers.
74. How do you manage remote state with locking (S3 + DynamoDB)?
75. How do you structure reusable Terraform modules for VPC, EC2, RDS?
76. How do you detect and remediate Terraform drift?
77. Terraform vs CloudFormation — pros, cons, and when to choose each.
78. How do you import existing AWS resources into Terraform/CloudFormation?
79. How do you use Ansible for configuration management and patching?
80. Ansible vs Terraform vs script — when do you pick each?
81. How do you write idempotent, robust Python/Bash automation scripts?
82. How do you build a Jenkins pipeline to deploy infrastructure and apps?
83. How do you use Git/GitHub/GitLab for version control and CI/CD?
84. How do you manage secrets in pipelines without hardcoding?
85. How do you automate routine operational toil safely in production?
86. How do you test automation before running it against production?
87. How do you schedule and monitor automation jobs (cron, EventBridge, Jenkins)?
88. How do you write PowerShell for Windows Server administration tasks?

## Linux/Windows Admin & Troubleshooting (89-100)

89. How do you troubleshoot high CPU, memory, disk, and OOM on Linux?
90. Explain systemd, journalctl, and service management on RHEL/Amazon Linux.
91. How do you harden Linux servers (SSH, users, sudo, firewalls, patching)?
92. How do you manage users, groups, and permissions on Windows Server?
93. How do you troubleshoot a Windows Server that is slow or unresponsive?
94. How do you diagnose DNS and network issues on Linux vs Windows?
95. Explain ITIL Incident, Change, and Problem Management and how they differ.
96. Walk through handling a P1 production incident from alert to RCA.
97. How do you prioritize and communicate across multiple simultaneous P2 incidents?
98. How do you mentor L1/L2 engineers and raise overall team capability?
99. How do you optimize AWS resource utilization and reduce cloud cost?
100. Why are you a good fit for this AWS Site Reliability Engineer role, and what would you improve in your first 90 days?
