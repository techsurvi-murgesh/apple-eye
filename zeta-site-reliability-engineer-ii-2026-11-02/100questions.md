# 100 Interview Questions — Site Reliability Engineer II — Zeta Corporation (Hyderabad)

## Site Reliability Engineering Fundamentals (1-10)

1. What is Site Reliability Engineering (SRE), and how does it differ from traditional DevOps or operations?
2. What are the core principles of SRE (SLOs, SLIs, error budgets, toil elimination, automation)?
3. What is an SLO (Service Level Objective), and how do you define one for a banking platform?
4. What is an SLI (Service Level Indicator), and give examples relevant to payments/core banking.
5. What is an error budget, and how do you use it to balance reliability vs. feature velocity?
6. What is toil, and how do you identify and eliminate toil in SRE work?
7. How do you define availability, and how do you calculate it (e.g., 99.9%, 99.99%)?
8. What is MTTF, MTTR, MTBF, and how do they relate to system reliability?
9. How do you prioritize reliability work against new feature development?
10. What is the difference between reliability, scalability, and performance?

## System Reliability & Infrastructure (11-20)

11. How do you design scalable and reliable infrastructure for high-scale systems?
12. What is redundancy, and how do you implement it (active-active, active-passive)?
13. What is a single point of failure (SPOF), and how do you eliminate it?
14. How do you ensure high availability for critical banking services?
15. What is load balancing, and what are the common algorithms (round-robin, least connections, IP hash)?
16. How do you design auto-scaling for infrastructure based on demand?
17. What is circuit breaking, and how does it prevent cascading failures?
18. How do you implement graceful degradation and fallback mechanisms?
19. What is chaos engineering, and how do you use it to improve system resilience?
20. How do you conduct game days or failure injection tests?

## Automation & Scripting (21-30)

21. What automation tools have you used (Ansible, Puppet, Chef, custom scripts)?
22. How do you decide what to automate versus do manually?
23. How do you write idempotent automation scripts?
24. What is the difference between imperative and declarative automation?
25. How do you manage secrets in automation (passwords, API keys, tokens)?
26. How do you version control your automation code?
27. How do you test automation scripts before applying to production?
28. What is the difference between push-based and pull-based configuration management?
29. How do you handle drift detection in automated infrastructure?
30. How do you document your automation for other team members?

## Infrastructure as Code (IaC) (31-40)

31. What is Infrastructure as Code (IaC), and what are its benefits?
32. How does Terraform work (providers, resources, state, modules, workspaces)?
33. How do you manage Terraform state (local, remote, S3, state locking)?
34. What is the difference between `terraform plan`, `terraform apply`, and `terraform destroy`?
35. How do you use Terraform modules for reusability?
36. How does Ansible differ from Terraform?
37. What are Ansible playbooks, roles, and inventories?
38. How do you handle sensitive data in Terraform/Ansible?
39. How do you integrate IaC into CI/CD pipelines?
40. How do you manage multiple environments (dev, staging, prod) with IaC?

## Containerization & Orchestration (41-50)

41. What is Docker, and how do you write an efficient Dockerfile?
42. What is container security, and how do you harden container images?
43. What is Kubernetes, and what are its core components (Pod, Deployment, Service, Ingress, ConfigMap, Secret)?
44. How do you troubleshoot a failing Kubernetes pod?
45. What is a Kubernetes Service, and what are the types (ClusterIP, NodePort, LoadBalancer)?
46. How do you configure resource limits and requests in Kubernetes?
47. What is a Helm chart, and how do you use it to manage Kubernetes applications?
48. How do you implement autoscaling in Kubernetes (HPA, VPA)?
49. What is a service mesh, and when would you use one?
50. How do you secure container images in a CI/CD pipeline?

## Cloud Computing (51-60)

51. What cloud platforms have you used (AWS, Azure, GCP)?
52. What are the key AWS services for infrastructure (EC2, VPC, IAM, S3, RDS, Lambda, CloudWatch)?
53. How do you design a VPC (subnets, route tables, security groups, NAT gateway)?
54. What is the difference between a public and private subnet?
55. How do you manage IAM roles and policies for least privilege?
56. What is AWS CloudFormation, and how does it differ from Terraform?
57. How do you manage cloud costs and optimize spend?
58. What is multi-region architecture, and when would you use it?
59. How do you handle cloud service outages or degradation?
60. What is the shared responsibility model in cloud security?

## Monitoring & Logging (61-70)

61. What are the three pillars of observability (metrics, logs, traces)?
62. How does Prometheus work, and how do you query metrics (PromQL)?
63. How does Grafana work, and how do you create dashboards?
64. What is Loki, and how does it differ from Prometheus for logs?
65. What is the ELK stack (Elasticsearch, Logstash, Kibana), and how do you use it?
66. How do you set up alerting rules in Prometheus?
67. How do you avoid alert fatigue (alert grouping, silencing, thresholds)?
68. What is distributed tracing, and how do you use it in microservices?
69. How do you monitor SLOs and burn rates?
70. How do you correlate metrics, logs, and traces during incident investigation?

## Incident Response & On-Call (71-80)

71. How do you handle an on-call rotation, and what are best practices?
72. What is your incident response process (detection, triage, mitigation, postmortem)?
73. How do you perform root-cause analysis (RCA) after an incident?
74. What goes into a postmortem or incident review document?
75. How do you prioritize incidents (severity levels, business impact)?
76. How do you communicate during an incident (stakeholders, customers, status page)?
77. What is a runbook, and how do you create and maintain one?
78. How do you reduce mean time to recovery (MTTR)?
79. How do you handle incidents outside regular working hours?
80. How do you blamelessly conduct postmortems?

## Capacity Planning & Performance Optimization (81-90)

81. What is capacity planning, and how do you forecast future infrastructure needs?
82. How do you analyze system usage patterns (CPU, memory, disk, network)?
83. What is load testing, and how do you perform it?
84. How do you identify and address performance bottlenecks?
85. What is profiling, and how do you profile application performance?
86. How do you optimize database performance (indexing, query tuning, connection pooling)?
87. How do you plan for traffic spikes (flash sales, promotions, events)?
88. What is vertical vs. horizontal scaling, and when do you use each?
89. How do you set up and interpret monitoring dashboards for capacity?
90. How do you right-size cloud instances to balance cost and performance?

## Security & Disaster Recovery (91-100)

91. What security best practices do you follow for infrastructure (encryption, access controls, vulnerability management)?
92. How do you manage encryption at rest and in transit?
93. What is IAM, and how do you apply least privilege?
94. How do you collaborate with security teams on vulnerability management?
95. What is disaster recovery (DR), and what are RTO and RPO?
96. How do you design a disaster recovery plan for banking systems?
97. How do you test disaster recovery plans (DR drills, failover tests)?
98. How do you handle backup and restore for databases and file systems?
99. How do you ensure compliance with banking regulations (RBI, PCI-DSS, SOC2)?
100. Why do you want to work at Zeta, and how does your SRE experience match this Hyderabad role?
