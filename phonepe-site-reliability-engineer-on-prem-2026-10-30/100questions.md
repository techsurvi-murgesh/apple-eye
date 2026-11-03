# 100 Likely Interview Questions — PhonePe Site Reliability Engineer - On-Prem

## Linux / Unix Administration
1. How do you troubleshoot a Linux server with high CPU usage?
2. What tools do you use to investigate memory pressure and OOM kills?
3. How do you check disk I/O bottlenecks on a Linux host?
4. Explain the Linux boot process from BIOS to systemd.
5. How do you manage services with systemd and journalctl?
6. What is the difference between soft and hard links?
7. How do you find and kill runaway processes safely?
8. How do you manage users, groups, and sudo access?
9. What are file permissions, ACLs, and umask?
10. How do you tune kernel parameters with sysctl?
11. How do you handle log rotation and retention?
12. What is the difference between /proc and /sys?
13. How do you debug a service that fails to start?
14. How do you patch and reboot production Linux hosts with minimal downtime?
15. What is your approach to capacity planning for Linux hosts?

## Networking
16. Explain TCP three-way handshake and connection teardown.
17. How do you troubleshoot DNS resolution issues?
18. What is the difference between TCP and UDP?
19. How do iptables rules work and in what order are chains evaluated?
20. How would you configure NAT and port forwarding with iptables?
21. What is IPsec and how do you configure a tunnel?
22. How do you debug network connectivity with ping, traceroute, ss, and tcpdump?
23. What is MTU and how does fragmentation affect performance?
24. How do you configure VLANs and bonding on Linux?
25. What is ARP and how do you detect ARP spoofing?
26. How do routing tables work and how do you add static routes?
27. How do you troubleshoot high latency or packet loss?
28. What is the difference between stateful and stateless firewalls?
29. How do you secure SSH access on Linux servers?
30. How do you design network segmentation for on-prem services?

## MySQL / MariaDB / Galera
31. How do you install and secure a MySQL or MariaDB instance?
32. What is the InnoDB storage engine and its key features?
33. How do you tune MySQL performance using indexes and query plans?
34. How do you take consistent backups with mysqldump or Percona XtraBackup?
35. How do you monitor replication lag?
36. What is a Galera cluster and how does it provide high availability?
37. How do you handle split-brain scenarios in Galera?
38. What is wsrep and how does certification-based replication work?
39. How do you add or remove a node from a Galera cluster?
40. How do you troubleshoot a Galera node that fails to join?
41. What are the trade-offs between MySQL, MariaDB, and Percona?
42. How do you plan capacity and storage for a busy database?

## Scripting / Programming
43. How do you write robust Bash scripts with error handling?
44. What is the difference between $@ and $* in Bash?
45. How do you use Python for automation and system administration?
46. How do you parse logs and metrics with Python?
47. What is your experience with Perl for text processing and automation?
48. How do you write concurrent programs in Go?
49. How do you handle errors and retries in Go services?
50. How do you build and deploy a Go binary for production?
51. How do you schedule jobs with cron and systemd timers?
52. How do you make scripts idempotent and safe to rerun?

## SaltStack / Automation / Config Management
53. What is SaltStack and how does its master-minion architecture work?
54. How do you write Salt states and pillars?
55. How do you manage secrets in Salt?
56. How do you test Salt states before applying to production?
57. How do you handle configuration drift?
58. What is the difference between push and pull configuration management?
59. How do you orchestrate multi-step changes with Salt orchestration?
60. How do you integrate SaltStack with CI/CD pipelines?
61. How do you roll back a bad configuration change?
62. How do you monitor Salt job execution and failures?

## Virtualization / Private Cloud / KVM
63. How do you set up KVM and QEMU on a Linux host?
64. What is the role of libvirt in managing VMs?
65. How do you create and manage virtual networks and bridges?
66. How do you allocate CPU, memory, and storage to VMs?
67. How do you perform live migration of a VM?
68. How do you monitor VM performance and resource contention?
69. What are the differences between KVM, Xen, and VMware?
70. How do you back up and restore VMs?
71. How do you secure a private cloud environment?
72. How do you automate VM provisioning?

## Containers / Orchestration
73. How do Docker containers differ from VMs?
74. How do you write an efficient Dockerfile?
75. How do you troubleshoot a container that keeps restarting?
76. What is Kubernetes and how does it schedule pods?
77. How do you expose services in Kubernetes?
78. How do you handle rolling updates and rollbacks in Kubernetes?

## NoSQL / Aerospike
79. What is Aerospike and what are its key strengths?
80. How does Aerospike handle data distribution and replication?
81. How do you tune Aerospike for low latency?
82. What is the difference between strong and eventual consistency?
83. How do you monitor Aerospike cluster health?
84. How do you back up and restore Aerospike data?

## Observability / On-call / Reliability
85. How do you define SLIs, SLOs, and error budgets?
86. How do you set up Prometheus and Grafana for infrastructure monitoring?
87. What metrics would you collect from Linux hosts?
88. How do you reduce alert fatigue?
89. How do you conduct a post-incident review?
90. What is your on-call escalation process?
91. How do you perform root cause analysis?
92. How do you test disaster recovery procedures?

## Behavioral / General
93. Why do you want to work at PhonePe?
94. How do you prioritize tasks during an incident?
95. Describe a time you improved system reliability.
96. How do you communicate with non-technical stakeholders?
97. How do you keep your skills current?
98. What does "always-up, always-available" mean to you?
99. How do you handle disagreements within a team?
100. What questions do you have for us?
