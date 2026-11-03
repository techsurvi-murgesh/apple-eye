# 100 Interview Questions — Ubuntu Cloud Field Engineer (Canonical) — 2026-10-12

Target stack: intermediate-to-advanced Python, full Linux stack (kernel, networking, storage, applications), Kubernetes and operators, private cloud (OpenStack) and public cloud (AWS/GCP/Azure), Ceph and data platforms (Hadoop/Spark), Ansible/IaC, customer-facing solution architecture, presentations, training, handover, coaching.

## Python Programming (1-20)

1. Explain Python's object-oriented model, `__init__`, `self`, and instance vs class attributes.
2. What are dunder methods, and which ones matter most in infrastructure code (`__enter__`, `__exit__`, `__iter__`, `__repr__`)?
3. Explain decorators and how you'd write a retry/backoff decorator.
4. Explain generators and `yield`. How do they compare to lists for large data?
5. What is the difference between a list, tuple, set, and dict? When would you pick each?
6. Explain mutable default arguments and why they are a bug. How do you fix it?
7. Explain `*args` and `**kwargs`, and how you'd use them to build a flexible CLI.
8. Explain list/dict/set comprehensions and the `zip`, `map`, and `filter` builtins.
9. What are context managers and why are they used for files, locks, and DB connections?
10. Explain exception hierarchy, `try/except/else/finally`, and when to define custom exceptions.
11. How does Python's GIL affect multithreading? When do you use `multiprocessing` instead?
12. Explain `asyncio`, coroutines, `await`, and the event loop. When is async the right choice?
13. How do you type-hint a Python codebase, and what are `typing.Protocol`, `TypedDict`, and generics for?
14. Explain virtual environments, `pip`, `pyproject.toml`, and dependency pinning.
15. How do you package and publish an open-source Python library (PyPI, entry points, versioning)?
16. How do you structure a larger Python application into packages/modules?
17. Explain `logging` vs `print`. How do you configure structured logging for a service?
18. How do you write and run unit tests in Python? What are fixtures and parametrize?
19. Explain `pathlib`, `os`, and how you handle paths and permissions portably on Linux.
20. How do you profile and optimise a slow Python program?

## Kubernetes & Containers (21-38)

21. Explain Kubernetes architecture: control plane, kubelet, etcd, and the scheduler.
22. What are Pods, Deployments, StatefulSets, DaemonSets, Jobs, and CronJobs?
23. Explain Services (ClusterIP, NodePort, LoadBalancer) and how DNS works inside a cluster.
24. How do you write an optimized and secure Dockerfile for a Python service?
25. What is the Kubernetes Operator pattern and how do you write a simple operator?
26. Explain CRDs and how you define and version a custom resource.
27. Explain the operator SDK/controller-runtime reconcile loop and idempotency.
28. How do you manage configuration and secrets with ConfigMaps and Secrets?
29. Explain liveness, readiness, and startup probes, and how misconfiguring them causes outages.
30. How do you do rolling updates and rollbacks? What are risks?
31. How do you manage resource requests/limits, QoS classes, and autoscaling (HPA/VPA)?
32. Explain persistent volumes, storage classes, and dynamic provisioning.
33. How do you secure a Kubernetes cluster: RBAC, PodSecurity, network policies, admission control?
34. How do you troubleshoot a pod that won't start: Pending, CrashLoopBackOff, ImagePullBackOff, OOMKilled?
35. How do you collect logs and metrics from a cluster (kubectl, metrics-server, Prometheus)?
36. What is Helm? Explain charts, values, templating, and when you'd avoid it.
37. How do you manage multi-cluster environments and cluster add-ons?
38. How do you upgrade a Kubernetes cluster safely?

## Linux Systems Internals (39-55)

39. Explain the Linux boot process from firmware to a running systemd service.
40. Explain systemd units, targets, timers, and how to write and debug a service unit.
41. Explain processes vs threads, scheduling, and how `nice`/`renice` and cgroups control resources.
42. Explain virtual memory, paging, swap, and the OOM killer.
43. How do you diagnose high CPU, memory, disk, and I/O on a busy host?
44. Explain Linux file systems (ext4, XFS), inodes, and how to repair a filesystem.
45. How do you manage users, groups, sudo, and SSH key-based access securely?
46. How do you manage packages with `apt`/`dpkg` and handle dependencies and pinning?
47. Explain file descriptors, `ulimit`, and how fd exhaustion breaks services.
48. How do you diagnose a full disk, including deleted-but-open files?
49. Explain how containers use namespaces (pid, net, mount, uts) and cgroups.
50. How do containers differ from virtual machines?
51. Explain `journalctl`, logrotate, and central log collection on Linux.
52. How do you patch and upgrade Ubuntu hosts safely with minimal downtime?
53. Explain security hardening: AppArmor, SELinux, seccomp, and least privilege.
54. How do you use `strace`, `lsof`, `perf`, and `gdb` to debug a system-level problem?
55. Explain how to read `/proc` and `/sys` to understand system state.

## Networking & Troubleshooting (56-70)

56. Explain the OSI and TCP/IP models, and where real protocols actually sit.
57. Explain the TCP handshake, TIME_WAIT, and connection state changes.
58. How do you read `ss` or `netstat` output to diagnose a connectivity problem?
59. Explain DNS resolution end to end, and how you debug it with `dig` and `nslookup`.
60. Explain DHCP, ARP, and how a host gets onto the network.
61. How do you configure and troubleshoot routing between subnets?
62. Explain VLANs, trunks, and bridging.
63. How do you use `tcpdump` and `curl`/`nc` to isolate a network fault?
64. Explain MTU, fragmentation, and the classic "ping works, TCP hangs" problem.
65. How do TLS and certificates work, and how do you debug certificate errors?
66. Explain HTTP/1.1 vs HTTP/2 vs HTTP/3 and keep-alive.
67. How do you set up a reverse proxy and load balancer, and debug upstream failures?
68. Explain IPv4 vs IPv6 addressing and common migration issues.
69. How do you troubleshoot intermittent network problems (packet loss, high latency)?
70. How do you secure a network: firewalls, security groups, and network policy?

## Cloud Architecture & Public Cloud (71-85)

71. Explain IaaS, PaaS, and SaaS, and what "cloud" really means operationally.
72. Explain core AWS: EC2, VPC, S3, IAM, RDS, ELB, Route 53.
73. How do you design a highly available architecture across AZs and regions?
74. Explain shared responsibility and how it differs across IaaS/PaaS/SaaS.
75. Explain autoscaling and elasticity patterns for cost and resilience.
76. How do you manage IAM roles and least privilege at scale?
77. How do you design network segmentation: VPCs, subnets, security groups, NACLs?
78. How do you plan and control cloud cost for an enterprise?
79. Explain managed Kubernetes (EKS/GKE/AKS) and the shared responsibility model.
80. How do you design backups, snapshots, and disaster recovery (RPO/RTO)?
81. How do you manage DNS, certificates, and TLS in a cloud environment?
82. How do you evaluate a new cloud service for production adoption?
83. What is OpenStack, and what problem does it solve versus public cloud?
84. Explain how private cloud and public cloud are combined in a hybrid architecture.
85. How do you design for portability so customers aren't locked to one cloud?

## Storage & Data Platforms (86-92)

86. Explain block, file, and object storage, and when to use each.
87. Explain Ceph's architecture: OSDs, MONs, MGRs, RADOS, pools, and CRUSH.
88. How do you size and configure a Ceph cluster, and what are its failure modes?
89. Explain RAID levels and how software-defined storage (RAIDZ, Ceph) differs from hardware RAID.
90. Explain HDFS and the Hadoop ecosystem, and when it still makes sense.
91. Explain Spark's architecture and how it interacts with HDFS and object storage.
92. How do you design data durability, replication, and backup for customer data?

## Automation, IaC & Delivery (93-98)

93. Explain Ansible: inventories, playbooks, roles, modules, and idempotence.
94. How do you write idempotent automation, and why does idempotence matter?
95. Explain infrastructure as code (IaC) and the benefits over imperative configuration.
96. Explain CI/CD pipelines and how you make deployments safe and repeatable.
97. How do you write runbooks and hand over a solution to a support/managed services team?
98. How do you manage secrets and credentials in automation?

## Customer, Communication & Culture (99-100 + behavioural)

99. How do you translate a customer's business problem into a technical architecture?
100. How do you prepare and deliver a technical presentation to customer stakeholders?

### Behavioural & Situational

- Describe a customer problem you solved end to end, from discovery to handover.
- How do you handle a production issue at a customer site while remote?
- Tell us about a time you coached or mentored a colleague. What was the outcome?
- How do you learn a new technology quickly and keep up with continual learning?
- Describe a time you documented something so well that others reused it.
- How do you stay organised and reliably follow up on commitments across time zones?
- Describe a time a project changed scope mid-flight. How did you adapt?
- How do you hand over a solution to a support team and ensure they can operate it?
- Tell us about an open-source contribution you made or would like to make.
- How do you balance writing code with presenting and training?