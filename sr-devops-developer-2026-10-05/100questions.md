# 100 Interview Questions — Sr. DevOps Developer (SDD00001) — 2026-10-05

Target stack: Kubernetes, Docker, Ansible, Jenkins, Ubuntu OS, GitHub, ELK, SSH, version control, pipeline creation & maintenance, deployment/build scripts, code QC & reporting, Agile, AWS/Azure/GCP basics.

## Docker (1–15)

1. Explain Docker architecture: daemon, images, containers, registries.
2. How do you write an optimized Dockerfile for Node.js/Go apps?
3. What are multi-stage builds and when do you use them?
4. How do you reduce Docker image size and CVE surface?
5. Explain Docker volumes vs bind mounts with use cases.
6. How do you manage Docker networking (bridge, host, overlay)?
7. What is Docker Swarm? How does service scaling and rolling update work?
8. How do you troubleshoot a container that exits immediately?
9. How do you handle logs for many Docker containers in production?
10. Explain ECR/Docker Hub image tagging, versioning, and cleanup strategy.
11. How do you scan Docker images for vulnerabilities?
12. What is the difference between CMD and ENTRYPOINT?
13. How do you limit CPU/memory for containers?
14. How do you back up and migrate Docker volumes?
15. Walk through dockerizing a Node.js + PostgreSQL app.

## Kubernetes (16–32)

16. Explain Kubernetes architecture: API server, scheduler, kubelet, etcd.
17. What are Pods, Deployments, Services, Ingress? How do they fit together?
18. How do you expose an app inside Kubernetes to the internet?
19. Explain ConfigMaps vs Secrets. How do you manage secrets safely?
20. What are liveness, readiness, and startup probes?
21. How do rolling updates and rollbacks work in Deployments?
22. How do you troubleshoot CrashLoopBackOff and ImagePullBackOff?
23. Explain resource requests vs limits with an example.
24. What is HPA and Cluster Autoscaler?
25. Explain namespaces, RBAC Roles vs ClusterRoles with an example.
26. How do you manage persistent storage (PV, PVC, StorageClass)?
27. What are Helm charts? How do you version and roll back a release?
28. How do you do blue/green or canary releases in Kubernetes?
29. How do you collect logs and metrics from Kubernetes workloads?
30. Explain Kubernetes networking: CNI, ClusterIP, NodePort, LoadBalancer.
31. How do you upgrade a Kubernetes cluster safely?
32. Design a small Kubernetes setup for 3 backend services + Postgres.

## Ansible (33–44)

33. What is Ansible and how does agentless execution over SSH work?
34. Explain inventory, playbooks, roles, tasks, handlers.
35. How do you manage inventory for dev/staging/prod?
36. Explain idempotency in Ansible with an example.
37. How do you handle secrets in Ansible (Ansible Vault)?
38. What are roles vs collections? How do you structure a reusable role?
39. How do you configure Ubuntu users, SSH keys, and packages with Ansible?
40. Write a playbook to install Docker and deploy a container on Ubuntu.
41. How do you do rolling updates with Ansible?
42. How do you test Ansible playbooks before production?
43. Ansible vs Terraform vs Bash scripts — when do you pick each?
44. How do you debug a failing Ansible task?

## Jenkins + Pipelines (45–62)

45. Explain Jenkins architecture: controller, agents, executors, Jenkinsfile.
46. What is a declarative vs scripted Jenkins pipeline?
47. How do you configure Jenkins on Ubuntu (users, SSH agents, credentials)?
48. How do you create a CI pipeline: checkout, build, test, code QC, artifact?
49. How do you create a CD pipeline: deploy to staging/prod with approvals?
50. How do you manage Jenkins credentials and SSH keys securely?
51. Explain shared libraries for reusable pipeline code.
52. How do you trigger pipelines (webhooks, polling, scheduled, upstream)?
53. How do you implement pipeline creation and maintenance best practices?
54. How do you add code QC gates (SonarQube, lint, unit tests) to Jenkins?
55. How do you generate build/test/QC reports in Jenkins?
56. How do you speed up slow Jenkins pipelines (caching, parallel stages)?
57. How do you back up Jenkins and migrate jobs safely?
58. Jenkins vs GitHub Actions vs GitLab CI — pros/cons?
59. How do you implement Blue Ocean / multibranch pipelines?
60. How do you handle pipeline failures and automatic rollback?
61. How do you audit who deployed what and when in Jenkins?
62. Design a Jenkins pipeline for Docker build → push → deploy to Kubernetes.

## GitHub & Version Control (63–72)

63. Explain Git branching models: GitFlow vs trunk-based development.
64. How do you handle version control maintenance (branch cleanup, protection rules)?
65. How do you write good commit messages and PR descriptions?
66. How do you resolve merge conflicts safely?
67. Explain GitHub Actions basics: workflows, jobs, steps, runners.
68. How do you manage secrets and environments in GitHub Actions?
69. How do you do code review for DevOps repos (Dockerfile, Jenkinsfile, playbooks)?
70. How do you version artifacts and tag releases in GitHub?
71. How do you use GitHub webhooks to trigger Jenkins?
72. How do you recover a deleted branch or bad merge?

## Ubuntu / Linux / SSH (73–82)

73. How do you harden an Ubuntu server (users, SSH, firewall, updates)?
74. Explain SSH key authentication, ssh-agent, and config best practices.
75. How do you manage users, groups, and sudo on Ubuntu?
76. How do you troubleshoot disk full, high CPU, OOM on Ubuntu?
77. Explain systemd services: how do you create and debug one?
78. How do you manage logs on Ubuntu (journalctl, logrotate)?
79. How do you automate Ubuntu patching across 20 servers?
80. Explain firewall setup with UFW / iptables for a backend server.
81. How do you write Bash deployment scripts (build, deploy, rollback)?
82. Write a Bash script to check disk usage and alert/report via email.

## ELK & Monitoring (83–90)

83. Explain ELK stack: Elasticsearch, Logstash, Kibana — what does each do?
84. How do you ship Ubuntu/Docker logs to ELK (Filebeat/Logstash)?
85. How do you create a Kibana dashboard for error rates and latency?
86. ELK vs Prometheus + Grafana + Loki — when do you use each?
87. How do you manage ELK retention and disk growth?
88. How do you set up alerts from Elasticsearch/Kibana?
89. How do you do code QC reporting and build reporting with dashboards?
90. Walk through debugging a production outage using ELK logs.

## DevOps Process, Agile & Cloud (91–100)

91. Explain CI vs CD vs continuous deployment with examples.
92. How do you work in Agile (sprints, standups, retros) as a DevOps engineer?
93. How do you multitask and work under pressure during an outage?
94. How do you document Jenkins setup, runbooks, and onboarding guides?
95. Explain AWS basics for this role: EC2, S3, IAM, security groups.
96. What is the difference between AWS, Azure, and GCP for DevOps hiring?
97. What DevOps certifications are valuable and why?
98. How do you handle disagreement with developers over a deployment freeze?
99. How do you prioritize 5 pipelines broken on the same morning?
100. Why are you a good fit for this Sr. DevOps Developer role? What would you improve in your first 90 days?
