# 100 Interview Questions — Network Automation Engineer (Service Provider / Cisco)

## NMS Tools / Network Management (1-15)
1. What is an NMS and what core functions does it provide (discovery, monitoring, alerting, reporting)?
2. How does SNMP work (manager, agent, MIB, OID, traps vs polls)?
3. SNMPv2c vs SNMPv3 — what are the security differences?
4. How would you onboard a new device into an NMS?
5. How do you handle syslog and trap storms / alert fatigue?
6. Explain NetFlow / sFlow / IPFIX and what use cases they solve.
7. How do Prometheus + Grafana + Loki compare to traditional NMS tools?
8. How would you set up alerting rules and dashboards for interface errors and CPU/memory?
9. What are SLAs/SLOs for network availability and how do you measure them?
10. How do you monitor config drift or unauthorized changes on network devices?
11. Explain active vs passive monitoring (ping, SNMP poll vs syslog, traps, streaming telemetry).
12. What is model-driven telemetry (gNMI/gRPC, YANG) and why is it replacing SNMP?
13. How would you troubleshoot "device shows down in NMS but is actually reachable"?
14. How do you scale NMS for hundreds of SP nodes (pollers, HA, retention)?
15. How do you integrate NMS alerts with ticketing / ChatOps workflows?

## SQL / PostgreSQL (16-28)
16. Explain normalization and when you would denormalize.
17. Difference between INNER, LEFT, RIGHT, FULL OUTER JOIN with examples.
18. What are indexes and when do they hurt performance?
19. Explain EXPLAIN ANALYZE and how you tune a slow query.
20. How do you design a schema to store device inventory and interface stats?
21. How would you store time-series link-utilization data in Postgres efficiently?
22. What are transactions, ACID, and isolation levels?
23. How do backups work in Postgres (pg_dump vs PITR/WAL)?
24. How do you paginate large result sets efficiently?
25. Write a query to find top 10 interfaces by error rate in last 24h.
26. How do you handle connection pooling for backend services?
27. What is the difference between SQL and NoSQL for NMS data?
28. How do you prevent SQL injection in Node.js / Python backends?

## Python / YAML / JSON / GitHub Automation (29-45)
29. How do you use Python for network automation (Netmiko, Nornir, ncclient)?
30. How would you write a Python script to push config to multiple devices?
31. Explain virtualenv / pip dependency management for automation scripts.
32. How do you handle secrets in automation (vault, env vars, GitHub Secrets)?
33. YAML vs JSON — when to use each in automation?
34. How do you validate YAML/JSON before applying (lint, schema)?
35. Explain Git branching strategy for network config automation.
36. How do you do code review for an Ansible/Python change?
37. How do GitHub Actions workflows work (trigger, jobs, runners, secrets)?
38. How would you build a CI pipeline that lints, dry-runs, and applies network configs?
39. How do you implement rollback for a bad automated config push?
40. Explain idempotency and why it matters in automation.
41. How do you test automation code (pytest, mocks for devices)?
42. How do you parse CLI output vs structured JSON/XML APIs?
43. How do you schedule periodic automation jobs?
44. Explain REST API automation for controllers (headers, auth, pagination).
45. How do you handle retries with exponential backoff in automation?

## Ansible / Terraform / Orchestration (46-60)
46. How does Ansible work (control node, inventory, playbooks, modules)?
47. Difference between ad-hoc commands and playbooks?
48. Explain Ansible inventory (static vs dynamic) for SP networks.
49. What are Ansible roles and collections (e.g., cisco.iosxr)?
50. How do you make playbooks idempotent?
51. How do you handle vault-encrypted variables in Ansible?
52. How would you use Ansible to manage Linux hosts + network devices together?
53. What is Terraform state and why does it matter?
54. Explain Terraform plan/apply/destroy workflow.
55. How do you structure Terraform modules for reusable infra?
56. Terraform vs Ansible — when to use which?
57. How do you handle drift between real infra and Terraform state?
58. How do you manage Terraform remote state and locking?
59. What is orchestration vs configuration management?
60. How would you orchestrate VM + container + network provisioning end-to-end?

## Linux / Unix Administration (61-72)
61. How do you troubleshoot high CPU / memory / disk on Linux?
62. Explain systemd services, journalctl, and log rotation.
63. How do you manage users, SSH keys, and sudo securely?
64. How do you debug "service won't start" on Linux?
65. Explain networking troubleshooting on Linux (ip, ss, ping, traceroute, tcpdump).
66. How do you check open ports and firewall rules (iptables/nftables, firewalld)?
67. How do you analyze logs with grep/awk/jq and Loki?
68. How do you set up cron vs systemd timers?
69. How do you handle disk full / inode exhaustion?
70. Explain file permissions, ownership, and SELinux/AppArmor basics.
71. How do you upgrade/patch Ubuntu hosts with minimal downtime?
72. Walk through your Linux incident triage for "API latency spiked to 5s".

## Virtualization: VMware / Docker / Kubernetes (73-85)
73. Explain Type-1 vs Type-2 hypervisors and where VMware fits.
74. How do vSphere / ESXi / vCenter work at a high level?
75. How do you provision and snapshot VMs for automation labs?
76. Docker vs VM — differences in isolation, overhead, use cases?
77. Explain Dockerfile layers, multi-stage builds, image tagging.
78. How do you troubleshoot a crashing Docker container?
79. Explain Docker networking (bridge, host, overlay) and volumes.
80. What is Kubernetes architecture (control plane, kubelet, etcd, CNI)?
81. How do Deployments, Services, and Ingress work?
82. How would you containerize a Python NMS poller and deploy to K8s?
83. How do ConfigMaps, Secrets, and resource limits work in K8s?
84. How do you debug CrashLoopBackOff and ImagePullBackOff?
85. How would you run network automation tooling on K8s with persistent storage?

## Cisco SP / NCS / ASR / Consulting (86-95)
86. What is IOS-XR and how does it differ from IOS/IOS-XE?
87. What are NCS540 / NCS560 / NCS55xx use cases (aggregation, edge)?
88. What are ASR9k and Cisco 8000 roles in service-provider cores?
89. Explain MPLS, segment routing, and EVPN at a high level.
90. How do you handle Cisco config commits (commit confirmed, rollback)?
91. How would you automate IOS-XR config with NETCONF/YANG?
92. How do you articulate a technical outage to a non-technical customer?
93. How do you collaborate with TAC / delivery teams during escalations?
94. Describe your consulting approach when a customer resists automation.
95. How do you document delivery (HLD/LLD, MOP, rollback plan)?

## Agentic AI Tools (96-100)
96. What are Agentic AI tools and how do you use them for ops (triage, runbook generation)?
97. How do you validate AI-suggested configs before applying to production?
98. How would you build an AI assistant over NMS docs and runbooks (RAG)?
99. What are risks of using LLMs for network changes (hallucination, privilege)?
100. How do you combine Agentic AI with human approval gates for safe automation?
