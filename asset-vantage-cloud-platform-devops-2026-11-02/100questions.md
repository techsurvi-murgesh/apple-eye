# 100 Interview Questions — Cloud Platform & DevOps Engineer (Asset Vantage, Pune)

## AWS Core Services (1-15)

1. What are the key differences between EC2, ECS/Fargate, and EKS/Kubernetes, and when would you choose each?
2. How does Amazon RDS work, and what are the benefits of Multi-AZ deployments and read replicas?
3. What is a VPC, and how do you design subnets (public vs. private), route tables, and internet gateways?
4. How do Security Groups differ from Network ACLs in AWS?
5. How does AWS IAM work, and what is the principle of least privilege?
6. What is Amazon CloudWatch, and how do you use it for monitoring, metrics, and alarms?
7. What is Amazon S3, and how do you configure S3 bucket policies and lifecycle rules?
8. How does Amazon Route 53 work, and what routing policies are available?
9. What is AWS Lambda, and how do you handle cold starts and concurrency limits?
10. How do you design a highly available and fault-tolerant architecture on AWS?
11. What is the difference between a NAT Gateway and a NAT Instance?
12. How do you secure data at rest and in transit on AWS (KMS, SSL/TLS)?
13. What is AWS CloudTrail, and why is it important for audit and compliance?
14. How do you manage AWS service quotas and limits?
15. What is AWS Organizations, and how do you use SCPs (Service Control Policies)?

## Amazon Cognito & Identity/Access (16-25)

16. What is Amazon Cognito, and what is the difference between user pools and identity pools?
17. How do Cognito user pools handle user registration, authentication, and MFA?
18. What is federation in Cognito, and how do you integrate with social providers (Google, Facebook) and enterprise IdPs (SAML/OIDC)?
19. How do OAuth 2.0 and OIDC work in the context of Cognito?
20. What are JWT tokens, and how do you validate a Cognito JWT token in your application?
21. How do you implement role-based access control (RBAC) using Cognito groups and IAM roles?
22. What is a Cognito identity pool, and how does it grant temporary AWS credentials to unauthenticated/authenticated users?
23. How do you customize the Cognito authentication flow using Lambda triggers?
24. How do you handle token refresh and revocation in Cognito?
25. What security best practices do you follow when using Cognito (password policies, MFA, account recovery)?

## CI/CD Pipelines (26-35)

26. What is CI/CD, and why is it important for platform engineering?
27. How do you design a CI/CD pipeline using Jenkins (jobs, stages, agents, plugins)?
28. What is Bitbucket Pipelines, and how do you configure it (bitbucket-pipelines.yml)?
29. How do you integrate Git with CI/CD (branching strategy, pull requests, merge workflows)?
30. How do you implement automated deployment workflows (blue/green, rolling, canary)?
31. How do you manage secrets in CI/CD pipelines (Jenkins credentials, Bitbucket variables)?
32. How do you handle pipeline failures and rollbacks?
33. What is the difference between continuous integration, continuous delivery, and continuous deployment?
34. How do you speed up CI/CD pipeline execution (caching, parallel stages)?
35. How do you secure a CI/CD pipeline (service accounts, least privilege, audit logs)?

## Infrastructure as Code (36-45)

36. What is Infrastructure as Code (IaC), and what are its benefits?
37. How does Terraform work (providers, resources, state, modules)?
38. How do you manage Terraform state (local, remote, S3 + DynamoDB locking)?
39. What is AWS CloudFormation, and how does it differ from Terraform?
40. What is AWS CDK, and how does it allow defining infrastructure using programming languages?
41. How do you create and reuse Terraform modules?
42. How do you handle infrastructure drift in Terraform/CloudFormation?
43. How do you integrate IaC into CI/CD pipelines?
44. What is the difference between declarative and imperative IaC?
45. How do you manage multiple environments (dev, staging, prod) with IaC (workspaces, variable files)?

## Docker & Kubernetes (46-55)

46. What is Docker, and how do you write an efficient Dockerfile (multi-stage builds, small images)?
47. What is container security, and how do you harden container images (non-root user, scanning, minimal base)?
48. What is Kubernetes, and what are its core components (Pod, Deployment, Service, Ingress, ConfigMap, Secret)?
49. What is EKS, and how does it differ from self-managed Kubernetes?
50. How do you troubleshoot a failing Kubernetes pod (kubectl get, describe, logs, events)?
51. What is a Helm chart, and how do you use it to manage Kubernetes applications?
52. How do you configure resource limits and requests in Kubernetes?
53. What is a Kubernetes Service, and what are the types (ClusterIP, NodePort, LoadBalancer)?
54. How do you implement autoscaling in Kubernetes (HPA, VPA, Cluster Autoscaler)?
55. How do you secure a Kubernetes cluster (RBAC, network policies, pod security standards)?

## Linux, Networking & Scripting (56-62)

56. What are the key Linux concepts a DevOps engineer should know (processes, permissions, systemd, SSH)?
57. How do you troubleshoot networking issues in Linux (ping, traceroute, netstat, ss, dig, curl)?
58. What is the difference between TCP and UDP, and how do DNS and DHCP work?
59. How do you write Bash scripts for automation (loops, conditionals, functions, error handling)?
60. How do you use Python for DevOps automation (boto3 for AWS, subprocess, file handling)?
61. What is PowerShell, and when would you use it in a Windows/Linux hybrid environment?
62. How do you manage SSH keys and secure remote access to Linux servers?

## Monitoring, Logging & Observability (63-68)

63. What is observability, and what are its three pillars (metrics, logs, traces)?
64. How do you use AWS CloudWatch for monitoring (metrics, alarms, dashboards, logs)?
65. How does Grafana work, and how do you create dashboards with Prometheus data?
66. What is the ELK stack (Elasticsearch, Logstash, Kibana), and how do you use it for log aggregation?
67. How does Splunk/Datadog differ from open-source monitoring tools?
68. How do you define alerting thresholds and avoid alert fatigue?

## Security, VAPT & Compliance (69-80)

69. What is VAPT (Vulnerability Assessment and Penetration Testing), and how do you coordinate remediation of findings?
70. How do you assess and prioritize VAPT findings for remediation?
71. What are common security controls in cloud infrastructure (encryption, IAM, network security, logging)?
72. What is vulnerability management, and how do you track closure of vulnerabilities?
73. How do you manage secrets (AWS Secrets Manager, Parameter Store) securely?
74. What are access reviews, and how do you conduct them for IAM users and roles?
75. What are secure configuration baselines, and how do you enforce them?
76. What is SOC2, and what are its trust service criteria (security, availability, processing integrity, confidentiality, privacy)?
77. How do you prepare audit evidence for SOC2 internal controls?
78. What is encryption at rest and in transit, and how do you implement it using AWS KMS?
79. How do you handle authentication and authorization across microservices?
80. What is the shared responsibility model in AWS security?

## Disaster Recovery, Backup & Cost Governance (81-85)

81. What is a disaster recovery (DR) strategy, and what are RTO and RPO?
82. How do you design backup and restore procedures for RDS, S3, and EBS?
83. How do you implement environment management (dev, staging, prod) and promotion?
84. How do you support cloud-cost governance and optimization with FinOps stakeholders?
85. What AWS cost optimization tools do you use (Cost Explorer, Trusted Advisor, Budgets)?

## Incident Response & Operations (86-90)

86. How do you lead incident response (detection, triage, mitigation, postmortem)?
87. How do you perform root-cause analysis (RCA), and what goes into a postmortem report?
88. What are corrective actions, and how do you track them to closure?
89. How do you define operational improvements based on incident trends?
90. How do you handle on-call rotations and escalation policies?

## Leadership, Mentoring & Collaboration (91-100)

91. How do you mentor junior DevOps engineers (code reviews, troubleshooting sessions, learning plans)?
92. How do you set engineering standards and review technical designs?
93. How do you break down complex technical problems into practical, risk-based solutions?
94. How do you communicate with business, audit, and compliance stakeholders?
95. How do you partner with Engineering, Security, Compliance, QA, and Product teams on architecture and release decisions?
96. What does an ownership mindset mean to you during incidents?
97. How do you drive a continuous-improvement approach in a platform team?
98. How do you handle disagreements during architecture discussions?
99. How do you prioritize competing demands (security vs. speed vs. cost)?
100. Why do you want to work at Asset Vantage, and how does your experience match this Pune role?
