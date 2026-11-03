# 100 Interview Questions — Azure SRE (SaaS Operations), Zensar

Target profile: Azure-based SRE for a large-scale enterprise SaaS platform, strong Microsoft SQL Server production support, PostgreSQL readiness, Windows/Linux, patching, automation (PowerShell/Python), Terraform/Puppet, GitHub/Jenkins, monitoring, incident response, RCA, and client-facing communication in a 24x7 environment.

## Azure and Cloud Operations (1–15)

1. How do Azure availability sets, availability zones, and regions differ, and how do they affect an HA design?
2. Which Azure storage redundancy option would you choose for a SaaS platform, and why?
3. How do Azure Monitor, Log Analytics, and Application Insights work together?
4. What signals would you collect from a production Azure VM and its application?
5. Compare Azure SQL Database with SQL Server running on Azure VMs for this platform.
6. How do VNets, subnets, NSGs, and route tables control traffic in Azure?
7. How would you design backup and disaster recovery for Azure VMs and databases?
8. How do you scale an Azure workload vertically and horizontally without downtime?
9. What are managed identities, and why are they safer than stored credentials?
10. How does Azure RBAC work, and how do you apply least privilege?
11. How do you investigate an Azure VM that is slow or intermittently unavailable?
12. How do you monitor and reduce Azure cost without reducing reliability?
13. What do Azure Policy and Azure Advisor contribute to operational governance?
14. How would you design a highly available SaaS platform across two Azure regions?
15. Walk through troubleshooting a service that is healthy in Azure but failing for a subset of customers.

## Microsoft SQL Server (16–32)

16. Compare full, differential, and transaction log backups, and explain the restore chain.
17. Which recovery models would you use for production and non-production, and why?
18. Compare clustered and nonclustered indexes, including included columns and covering queries.
19. How do you identify and handle index fragmentation?
20. Walk through tuning a slow query from symptom to validated improvement.
21. How do you read an execution plan and spot a bad join or missing index?
22. How do you diagnose blocking and deadlocks, and what changes prevent recurrence?
23. Explain SQL Server isolation levels and the anomalies each one prevents.
24. What is tempdb contention, and how do you investigate it?
25. How do you design and monitor SQL Agent jobs for reliability?
26. When would you use a stored procedure rather than application SQL?
27. How does Always On availability groups work, and what does failover involve?
28. How do you test that HA and DR actually work rather than assuming they do?
29. How do you patch SQL Server in a controlled production environment?
30. How do you troubleshoot high CPU, memory, and I/O on a SQL Server instance?
31. How do you perform a production data fix safely under change control?
32. Which SQL Server metrics and alerts would you put on a production dashboard?

## PostgreSQL (33–45)

33. Explain PostgreSQL process architecture and how it differs from SQL Server.
34. How does MVCC work, and why does vacuum matter?
35. Compare PostgreSQL index types and when you would use each.
36. How do you read `EXPLAIN ANALYZE` and use it to improve a query?
37. Which PostgreSQL settings would you tune first for a production workload?
38. Compare `pg_dump`, `pg_basebackup`, and continuous archiving for backup.
39. How does point-in-time recovery work with WAL archives?
40. How does PostgreSQL streaming replication work, and how do you monitor lag?
41. How would you design PostgreSQL high availability with Patroni or a managed service?
42. What are the main risks in migrating from SQL Server to PostgreSQL?
43. How do you handle data types, identity columns, and SQL dialect differences during coexistence?
44. Which PostgreSQL metrics and logs would you monitor in production?
45. How do you plan a PostgreSQL minor or major version upgrade with minimal downtime?

## Patching, Maintenance, and Change Control (46–55)

46. How do you build an annual and monthly patching plan for SQL Server and operating systems?
47. What goes into a maintenance window plan, including communication and validation?
48. How does change management affect how you execute a production patch?
49. What is your rollback plan if a patch causes an application regression?
50. How do you patch Linux servers safely across a fleet?
51. How do you patch Windows Server safely, including reboots and clustered services?
52. What checks do you run before and after a SQL Server patch?
53. How do you prove patch compliance to an auditor or client?
54. How do you minimize customer impact during mandatory security patching?
55. A patch succeeds technically but the application misbehaves. What do you do?

## Windows and Linux Operations (56–63)

56. How do you troubleshoot a Windows service that will not start?
57. Which Windows event logs and Performance Monitor counters do you check first?
58. How do you investigate IIS or Windows application errors in production?
59. How does systemd manage services, and how do you troubleshoot a failed unit?
60. Where do you look for Linux logs, and how do you correlate them with application logs?
61. How do Linux file permissions and ownership cause production failures?
62. Which Linux networking tools do you use to diagnose connectivity and latency?
63. A Linux server shows high CPU and memory usage. Walk through your investigation.

## Monitoring, SRE, and Incident Response (64–78)

64. Define SLI, SLO, and SLA with an example from a SaaS platform.
65. What is an error budget, and how would you use it in operations?
66. How do you tune alerts to reduce noise without missing real incidents?
67. What belongs on an SRE dashboard for a multi-tenant SaaS product?
68. Walk through P1 and P2 triage from alert to handoff.
69. How do you perform a root cause analysis when the incident involved several teams?
70. How do you use the five whys without oversimplifying the cause?
71. What do you communicate to clients during an active P1, and how often?
72. Which factors reduce MTTR most in a 24x7 SaaS operation?
73. What makes a runbook useful under pressure, and how do you keep it current?
74. How do you investigate an issue using logs from Azure, the OS, the database, and the application?
75. How do you use APM data to distinguish an application problem from an infrastructure problem?
76. How would you configure PagerDuty escalation for a follow-the-sun support model?
77. How do you reproduce a customer-reported issue safely in staging?
78. What belongs in a postmortem, and how do you ensure actions are completed?

## Automation, IaC, and DevOps (79–88)

79. Write a PowerShell script to check disk space and service status across Azure VMs. What would you add for production use?
80. How do you automate a repetitive SQL Server maintenance task in Python or PowerShell?
81. How do you structure Terraform for Azure infrastructure across environments?
82. How do you use Puppet for configuration management, and what does it not solve?
83. How do you manage code and reviews with GitHub in an operations team?
84. What does a reliable Jenkins pipeline look like for infrastructure or database changes?
85. How do you handle database schema changes in CI/CD safely?
86. Why must operational automation be idempotent, and how do you test that?
87. How do you store and rotate secrets used by automation?
88. How do you detect Terraform or Puppet drift and correct it without an outage?

## Containers and Microservices (89–92)

89. How do you operate Docker containers safely in production?
90. What do you monitor in a Kubernetes cluster from an SRE perspective?
91. What changes about incident response in a microservices architecture?
92. How would you troubleshoot a container that restarts repeatedly?

## SaaS, Client Communication, and Behavioral (93–100)

93. What is different about operating a multi-tenant SaaS platform compared with single-tenant systems?
94. How do you explain a complex database incident to a non-technical client stakeholder?
95. Are you comfortable with night shifts and US time zone coverage? How do you stay effective?
96. Describe how you have worked across database, platform, application, and support teams to resolve an issue.
97. What documentation do you leave behind after an incident or a platform change?
98. Walk through a production incident you owned end to end: detection, triage, communication, fix, and RCA.
99. How do you prioritize between a P1 incident, a scheduled patch, and a long-term reliability improvement?
100. Walk through an end-to-end reliability improvement you delivered across Azure, SQL Server/PostgreSQL, monitoring, automation, and incident response, and explain the trade-offs.
