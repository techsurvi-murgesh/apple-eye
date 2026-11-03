# 100 Interview Questions — Senior Engineer, Infrastructure — The Hartford (GCC034)

## Cloud Database Infrastructure (1-15)

1. What are the key considerations when designing a cloud-native database architecture on AWS?
2. How do you choose between relational (RDS) and NoSQL (DynamoDB) databases for a given workload?
3. What is Amazon RDS, and what are the benefits of Multi-AZ deployments and read replicas?
4. How do you design a database schema for scalability and performance?
5. What are the trade-offs between vertical and horizontal scaling for databases?
6. How do you handle database connection pooling in cloud-native applications?
7. What is data modeling, and how does it differ for relational vs. NoSQL databases?
8. How do you design for high availability in a cloud database solution?
9. What is database sharding, and when would you use it?
10. How do you optimize query performance and indexing strategies?
11. What are the different RDS instance types and storage options, and how do you select them?
12. How do you manage database backups and point-in-time recovery?
13. What is database caching, and how do you use Redis or Memcached with cloud databases?
14. How do you handle database migrations with zero or minimal downtime?
15. What is change data capture (CDC), and how is it used in cloud database environments?

## Infrastructure as Code (Terraform & CloudFormation) (16-30)

16. What is Infrastructure as Code (IaC), and what are its benefits?
17. How does Terraform work (providers, resources, state, modules, workspaces)?
18. How do you manage Terraform state (local, remote, S3, state locking)?
19. What is the difference between `terraform plan`, `terraform apply`, and `terraform destroy`?
20. How do you create and reuse Terraform modules?
21. How does AWS CloudFormation differ from Terraform?
22. What are CloudFormation templates, stacks, and change sets?
23. How do you handle infrastructure drift in Terraform or CloudFormation?
24. How do you integrate IaC into CI/CD pipelines?
25. How do you manage multiple environments (dev, staging, prod) with IaC?
26. What is the difference between declarative and imperative IaC?
27. How do you handle secrets in Terraform/CloudFormation?
28. How do you version control IaC code using GitHub?
29. How do you perform code reviews for infrastructure code?
30. How do you test infrastructure changes before applying to production?

## CI/CD & Automation (Jenkins, Ansible, GitHub) (31-45)

31. What is CI/CD, and why is it important for database infrastructure?
32. How do you design a CI/CD pipeline using Jenkins (jobs, stages, agents, plugins)?
33. What is Ansible, and how do you use it for automation?
34. How do you write idempotent Ansible playbooks?
35. How do you manage secrets in CI/CD pipelines (Jenkins credentials, GitHub secrets)?
36. How do you integrate database provisioning into application CI/CD pipelines?
37. How do you handle pipeline failures and rollbacks?
38. What is the difference between continuous integration, continuous delivery, and continuous deployment?
39. How do you speed up CI/CD pipeline execution (caching, parallel stages)?
40. How do you secure a CI/CD pipeline (service accounts, least privilege, audit logs)?
41. How do you use GitHub for version control, pull requests, and code reviews?
42. How do you handle branching strategy for infrastructure code?
43. How do you automate database patching and upgrades?
44. How do you automate routine database maintenance (backups, performance tuning, capacity planning)?
45. How do you integrate ServiceNow with CI/CD or incident management?

## Networking & Security (46-55)

46. What is a VPC, and how do you design subnets (public vs. private), route tables, and internet gateways?
47. How do Security Groups differ from Network ACLs?
48. How do you secure database deployments using VPCs, subnets, and security groups?
49. How do you manage IAM roles and policies for least privilege?
50. How do you encrypt data at rest and in transit (KMS, SSL/TLS)?
51. What is AWS CloudTrail, and why is it important for audit and compliance?
52. How do you manage secrets (AWS Secrets Manager, Parameter Store)?
53. What are access reviews, and how do you conduct them?
54. How do you collaborate with security teams on vulnerability management?
55. How do you ensure compliance with data governance, security, regulatory, and privacy standards?

## Monitoring, Logging & Observability (56-65)

56. What are the three pillars of observability (metrics, logs, traces)?
57. How do you use AWS CloudWatch for monitoring (metrics, alarms, dashboards, logs)?
58. How does Prometheus work, and how do you query metrics (PromQL)?
59. How does Grafana work, and how do you create dashboards?
60. What is Loki, and how does it differ from Prometheus for logs?
61. How do you set up alerting rules for database performance and availability?
62. How do you avoid alert fatigue (alert grouping, silencing, thresholds)?
63. How do you monitor database performance (CPU, memory, disk, connections, query latency)?
64. How do you correlate metrics, logs, and traces during incident investigation?
65. How do you monitor SLOs and error budgets for database services?

## Disaster Recovery & High Availability (66-75)

66. What is disaster recovery (DR), and what are RTO and RPO?
67. How do you design a disaster recovery strategy for cloud databases?
68. How do you test disaster recovery plans (DR drills, failover tests)?
69. How do you handle backup and restore for databases (RDS snapshots, DynamoDB on-demand backups)?
70. What is high availability, and how do you achieve it (Multi-AZ, read replicas, auto-failover)?
71. How do you handle database failover and failback?
72. How do you plan for traffic spikes and capacity planning?
73. How do you right-size cloud instances to balance cost and performance?
74. How do you reduce complexity and cost in database environments?
75. How do you evaluate new database product releases and recommend implementation?

## Migrations & Consolidation (76-82)

76. How do you assist application and DBA teams with database migration from on-prem to cloud?
77. What is database consolidation, and how do you plan and execute it?
78. What is database conversion, and how do you handle schema and data type differences?
79. How do you perform end-to-end execution from roadmap to implementation of migrations?
80. How do you validate data integrity after migration?
81. How do you minimize downtime during database migrations?
82. How do you roll back a failed migration?

## AI & MLOps (83-90)

83. How do you use AI tools as a productivity accelerator in infrastructure work?
84. How do you critically evaluate and validate AI-generated output?
85. How do you apply AI responsibly within enterprise security, governance, and compliance boundaries?
86. How do you leverage AI to analyze logs, metrics, incidents, and configuration drift?
87. How do you accelerate root cause analysis using AI?
88. How do you explain what AI contributed, what was changed, and why?
89. What are MLOps-aligned practices (versioning, CI/CD integration, monitoring, lifecycle management)?
90. What are common model deployment patterns (batch processing, real-time APIs, event-driven architectures)?

## Leadership, Documentation & Collaboration (91-100)

91. How do you prepare deployment and operational procedure manuals?
92. How do you maintain documentation of standard operating policies and procedures?
93. How do you prepare evidence to support internal and external auditors?
94. How do you collaborate with application teams, Cloud Engineering, and SREs?
95. How do you manage multiple priorities and stay organized?
96. How do you communicate effectively with cross-functional teams?
97. How do you learn fast on the job by partnering with senior resources?
98. How do you demonstrate engineering excellence and continuous improvement?
99. How do you handle production incidents and provide second-level support?
100. Why do you want to work at The Hartford, and how does your experience match this Infrastructure role?
