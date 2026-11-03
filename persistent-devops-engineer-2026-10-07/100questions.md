# 100 Interview Questions — DevOps Engineer (Persistent Systems, Bengaluru) — 2026-10-07

Target stack: Jenkins CI/CD, AWS (Subnet/VPC, ElastiCache, MQ, MSK, RDS, S3, EKS), Terraform (IaC), NGINX, ELK/Dynatrace/Grafana/OpenSearch/Site24x7, Linux/Unix & automation scripting, Kubernetes/EKS, networking/firewall/Active Directory, P1/P2 incident handling.

## Jenkins & CI/CD Pipelines (1-18)

1. Explain the end-to-end CI/CD pipeline you would build for a microservice from commit to production.
2. How do you design Jenkins pipelines to deploy across production and non-production environments?
3. Declarative vs scripted Jenkins pipeline — when do you use each?
4. How do you manage Jenkins agents/executors and scale them dynamically for parallel builds?
5. How do you parameterize a Jenkins job for multi-environment deployments with approvals?
6. How do you store and use credentials (AWS keys, SSH, tokens) securely in Jenkins?
7. How do you implement shared libraries to reuse pipeline code across teams?
8. How do you add build, test, lint, and code-quality gates to a Jenkins pipeline?
9. How do you trigger Jenkins from GitHub webhooks and enforce status checks?
10. How do you implement blue/green or canary deployment in Jenkins to prod?
11. How do you make a Jenkins deployment automatically roll back on failure?
12. How do you speed up a slow Jenkins pipeline (caching, parallelism, incremental builds)?
13. How do you back up and restore Jenkins (JENKINS_HOME, plugins, credentials)?
14. How do you troubleshoot a Jenkins build stuck in the queue or a flaky stage?
15. How do you secure Enterprise Jenkins (RBAC, SSO, CSRF, script approval, agent isolation)?
16. How do you version artifacts and Docker images produced by CI to make deployments traceable?
17. Compare Jenkins with GitHub Actions and GitLab CI for a large enterprise.
18. How do you migrate pipelines from legacy freestyle jobs to declarative Jenkinsfiles safely?

## AWS Core Services (19-38)

19. Explain VPC design: subnets (public/private), route tables, NAT, IGW, and CIDR planning.
20. How do you troubleshoot a subnet with no internet or no route to an RDS instance?
21. What is ElastiCache (Redis/Memcached) and when do you use it vs application caching?
22. Explain Redis replication, cluster mode, and failover in ElastiCache.
23. How do you size, monitor, and optimize ElastiCache cost and performance?
24. What is Amazon MQ and when do you choose it over self-managed brokers or SQS/SNS?
25. Compare Amazon MQ with Kafka (MSK) and SQS for a messaging use case.
26. Explain MSK architecture: brokers, partitions, replication factor, and ZooKeeper/KRaft.
27. How do you size an MSK cluster and plan partitions for throughput?
28. How do you secure MSK (IAM, TLS, SASL, security groups, encryption at rest)?
29. How do you monitor MSK consumer lag and rebalance issues?
30. Explain RDS Multi-AZ vs read replicas; when do you use each?
31. How do you perform an RDS major-version upgrade with minimal downtime?
32. How do you tune RDS performance (instance class, parameter groups, storage, IOPS)?
33. How do you troubleshoot RDS connection exhaustion and slow queries?
34. Explain S3 storage classes, lifecycle policies, versioning, and cost optimization.
35. How do you secure S3 (bucket policies, Block Public Access, encryption, presigned URLs)?
36. How do you debug an S3 403/404 access issue for an application using IAM roles?
37. Explain IAM roles vs users, policies, and cross-account access for AWS services.
38. How do you use security groups, NACLs, and WAF to secure AWS workloads?

## Networking, Firewall & Active Directory (39-50)

39. Walk through the OSI model with a real packet-debugging example.
40. How do security groups differ from NACLs, and how do they work together?
41. How do you design least-privilege firewall rules between tiers (web/app/db)?
42. How do you debug a connectivity failure between two AWS subnets?
43. How does DNS resolution work end-to-end, and how do you debug with dig/nslookup/resolv.conf?
44. How do you configure Route 53 for internal and external name resolution?
45. How do you integrate Active Directory with AWS (AD Connector, Managed AD, SSO)?
46. How do you use AD groups for least-privilege access to Linux servers and AWS?
47. How do you troubleshoot authentication failures against Active Directory (Kerberos, LDAP, time skew)?
48. How do you implement LDAPS and secure directory traffic?
49. How do you load balance with NGINX/ALB and health-check backends correctly?
50. How do you troubleshoot TLS/SSL handshake failures (certs, SNI, ciphers)?

## Terraform (Infrastructure as Code) (51-64)

51. Explain Terraform workflow: init, plan, apply, destroy and providers.
52. How do you manage remote state with locking (S3 + DynamoDB) and why?
53. How do you structure reusable Terraform modules for VPC, EKS, and RDS?
54. How do you handle secrets and sensitive values in Terraform?
55. How do you manage multiple environments (dev/stage/prod) with workspaces or separate states?
56. How do you detect and remediate configuration drift?
57. How do you import existing AWS resources into Terraform safely?
58. Terraform vs CloudFormation vs Ansible — when do you pick each?
59. How do you review Terraform changes in a PR with plan output and policy checks?
60. How do you test Terraform code (tflint, checkov, terratest)?
61. How do you protect production state from accidental destroy?
62. How do you handle provider version pinning and upgrades?
63. How do you refactor a large monolithic Terraform configuration?
64. How do you use data sources and dependencies between modules?

## Monitoring, Logging & Observability (65-78)

65. Explain the ELK stack: Elasticsearch, Logstash, Kibana — what does each do?
66. How do you ship application and OS logs to ELK (Filebeat/Logstash) at scale?
67. How do you manage Elasticsearch index lifecycle, retention, and disk growth?
68. How do you create actionable Kibana dashboards and alerts?
69. What is OpenSearch and how does it compare with Elasticsearch?
70. How do you set up Grafana dashboards for infrastructure and application metrics?
71. How do you instrument metrics with Prometheus exporters and query with PromQL?
72. What is Dynatrace and how does APM differ from metrics/logs monitoring?
73. How do you use Dynatrace to find a slow transaction root cause?
74. What is Site24x7 and how do you configure uptime and synthetic monitoring?
75. How do you design alerting to avoid alert fatigue (thresholds, SLOs, routing)?
76. How do you implement centralized logging for Docker/Kubernetes workloads?
77. How do you trace a request across microservices using distributed tracing?
78. How do you monitor CI/CD and deployment health, not just the app?

## Kubernetes / EKS & Containers (79-90)

79. Explain Kubernetes architecture: API server, etcd, scheduler, controller manager, kubelet.
80. What are Pods, Deployments, Services, Ingress, and how do they fit together?
81. How do you deploy and expose an application on EKS end-to-end?
82. How do you manage EKS node groups, autoscaling, and cluster autoscaler?
83. How do you use IAM Roles for Service Accounts (IRSA) in EKS?
84. How do ConfigMaps, Secrets, and external secret managers work in EKS?
85. How do you troubleshoot CrashLoopBackOff, ImagePullBackOff, OOMKilled, and Pending pods?
86. Explain liveness, readiness, and startup probes with examples.
87. How do rolling updates and rollbacks work in a Deployment?
88. How do you use Helm to package and version Kubernetes applications?
89. How do you enforce resource requests/limits and HPA in EKS?
90. How do you debug networking issues inside a Kubernetes cluster (CNI, DNS, NetworkPolicy)?

## Linux, Automation & Incident Management (91-100)

91. How do you administer and harden Linux/Unix servers (users, SSH, sudo, patching)?
92. How do you troubleshoot high CPU, memory, disk, and OOM issues on Linux?
93. Explain systemd units, journalctl, and log management on Linux.
94. How do you write robust Bash/Python automation scripts (idempotency, error handling, logging)?
95. How do you automate routine toil (cleanup, patching, reporting) safely in production?
96. Walk through handling a P1 production incident from alert to postmortem.
97. How do you prioritize and communicate during multiple simultaneous P2 incidents?
98. How do you build runbooks and reduce MTTR for recurring incidents?
99. How do you understand an existing application's architecture before supporting its deployments?
100. Why are you a good fit for this DevOps Engineer role, and what would you improve in your first 90 days?
