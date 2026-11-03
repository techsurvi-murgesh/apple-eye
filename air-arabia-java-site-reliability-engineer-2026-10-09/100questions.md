# 100 Interview Questions — Java Site Reliability Engineer (Air Arabia) — 2026-10-09

Target stack: Java/Spring Boot enterprise & microservices support, JBoss/WildFly, incident response, RCA, monitoring/observability, CI/CD (Jenkins), Docker/Kubernetes, SQL/Oracle, Linux/networking, on-call, runbooks, patching/backups, Node.js/Next.js exposure.

## Java Core & JVM (1-18)

1. Explain OOP principles and SOLID with Java examples.
2. Difference between abstract classes and interfaces in Java.
3. Explain the Java Collections framework and choosing implementations.
4. How do HashMap and ConcurrentHashMap work internally?
5. Explain multithreading: Thread, Runnable, ExecutorService.
6. What are synchronized, volatile, and atomic types?
7. Explain the Java memory model and happens-before relationship.
8. Difference between `==` and `.equals()` and the hashCode contract.
9. Explain checked vs unchecked exceptions and best practices.
10. What are generics and type erasure?
11. Explain Java Streams and functional interfaces.
12. Explain Java 11/17 features (var, records, sealed classes, text blocks).
13. How does garbage collection work (G1, ZGC) and how do you tune it?
14. How do you diagnose a Java memory leak in production?
15. How do you troubleshoot high CPU in a JVM (thread dumps, jstack, JFR)?
16. How do you analyze a heap dump (jmap, MAT)?
17. Explain classloading and common ClassNotFound/NoClassDefFound errors.
18. How do you profile a Java application safely in production?

## Spring Boot & Microservices (19-36)

19. Explain Spring Boot auto-configuration and starters.
20. Difference between @Component, @Service, @Repository, @Controller.
21. Explain dependency injection and bean scopes.
22. How does Spring MVC handle a request end-to-end?
23. How do you build and validate a REST API in Spring Boot?
24. Explain Spring Data JPA repositories and derived queries.
25. How do transactions work in Spring (@Transactional, propagation, isolation)?
26. How does Spring Security handle authentication and authorization?
27. How do you handle exceptions globally in Spring (@ControllerAdvice)?
28. How do you configure Spring profiles for multiple environments?
29. Explain microservices vs monolith and deployment tradeoffs.
30. How do services communicate—REST vs messaging—and tradeoffs?
31. How do you implement resilience (circuit breaker, retry, timeout)?
32. How do you troubleshoot a Spring Boot app that fails to start?
33. How do you debug a NullPointerException or bean wiring failure?
34. How do you trace a request across microservices?
35. Explain JBoss/WildFly deployment and common issues.
36. How do you deploy a WAR/EAR vs a Spring Boot JAR?

## Databases & SQL (37-50)

37. Explain relational schema design and normalization.
38. How do indexes work and when can they hurt performance?
39. How do you read an execution plan and optimize a slow query?
40. Explain ACID and isolation levels with examples.
41. How do you handle deadlocks in Oracle/SQL databases?
42. Explain connection pooling and sizing (HikariCP).
43. How do you troubleshoot a DB connection leak or exhaustion?
44. Explain partition/table maintenance for large Oracle tables.
45. How do you monitor and tune a slow database?
46. Explain N+1 query problems in JPA and how to fix them.
47. How do you safely apply schema changes in production?
48. When would you use MongoDB or Redis instead of a relational DB?
49. How do you back up and restore a database (RPO/RTO)?
50. How do you write complex joins and subqueries efficiently?

## Incidents, Monitoring & Observability (51-68)

51. Walk through investigating a production incident from alert to resolution.
52. How do you analyze application logs to find a root cause?
53. How do you systematically perform root cause analysis?
54. How do you prioritize multiple simultaneous incidents?
55. How do you use metrics, logs, and traces together during an incident?
56. Explain SLI, SLO, and SLA with examples.
57. How do you set up alerting and avoid alert fatigue?
58. How do you use Grafana and Prometheus for application monitoring?
59. How do you use Splunk and Kibana for log analysis?
60. How do you monitor JVM metrics (heap, GC, threads)?
61. How do you monitor batch jobs and scheduled tasks?
62. How do you perform routine health checks and log reviews?
63. How do you proactively detect capacity/performance issues?
64. How do you turn an incident resolution into a runbook?
65. How do you write a good postmortem?
66. How do you reduce MTTR for recurring issues?
67. How do you participate effectively in an on-call rotation?
68. How do you escalate unresolved issues appropriately?

## CI/CD, Containers & Linux (69-84)

69. Explain the stages of a CI/CD pipeline.
70. How do you run and troubleshoot a Jenkins pipeline?
71. How do you manage deployment and release tasks safely?
72. How do you implement rollback on a failed deployment?
73. How do you do blue/green or canary releases?
74. How do you manage configuration across environments?
75. Explain Docker architecture and building optimized images.
76. How do you troubleshoot a container that exits immediately?
77. Explain Kubernetes: pods, deployments, services, probes.
78. How do you troubleshoot CrashLoopBackOff and ImagePullBackOff?
79. How do you operate and scale containerized apps in production?
80. How do you manage resource requests/limits?
81. How do you use Helm to deploy applications?
82. How do you patch and back up systems following change procedures?
83. How do you automate recurring operational tasks with scripts?
84. How do you manage secrets and certificates?

## Linux, Networking & Behavioral (85-100)

85. How do you administer Linux servers and use the command line effectively?
86. How do you troubleshoot high CPU, memory, disk, and I/O on Linux?
87. Explain systemd, journalctl, and service management.
88. How do you check open ports and process-to-port mapping (ss, netstat, lsof)?
89. Explain DNS resolution and how you debug it.
90. Explain OSI/TCP-IP with a real debugging example.
91. How do you debug connectivity between an app server and a database?
92. How do you analyze a packet capture (tcpdump, Wireshark)?
93. How do you manage users, permissions, and SSH securely?
94. How do you work in an Agile team as an SRE?
95. How do you document knowledge and mentor new team members?
96. How do you handle a production incident under pressure?
97. Describe a time you prevented an issue proactively.
98. How do you ensure compliance with policies and regulatory requirements?
99. How do you keep learning new reliability/Java technologies?
100. Why are you a good fit for this Java Site Reliability Engineer role at Air Arabia, and what would you improve in your first 90 days?
