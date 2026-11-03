# 100 Interview Questions — DevOps Engineer (Linux / Jenkins / GitHub Actions / K8s / AWS)

## Linux/Unix Administration (1-18)
1. How do you troubleshoot high CPU, memory, and disk pressure on Linux?
2. Explain systemd units, journalctl, and service dependency management.
3. How do you manage users, groups, sudoers, and SSH key auth securely?
4. Walk through debugging a service that fails to start after reboot.
5. How do you use ip, ss, dig, traceroute, and tcpdump for network issues?
6. How do you configure firewalls with iptables/nftables or firewalld?
7. Explain file permissions, umask, setuid/setgid, and ownership.
8. How do you handle full disk / inode exhaustion in production?
9. How do you patch Ubuntu vs RedHat (apt vs dnf/yum) with minimal downtime?
10. How do you set up log rotation and centralized logging?
11. How do you schedule jobs with cron vs systemd timers?
12. How do you analyze logs with grep, awk, sed, and jq?
13. Explain LVM, mounts, and filesystem troubleshooting.
14. How do you tune kernel params with sysctl for high-traffic hosts?
15. How do you secure SSH (key-only, fail2ban, ports, banners)?
16. How do you diagnose DNS resolution failures on Linux?
17. Explain SELinux/AppArmor basics and troubleshooting denials.
18. How do you do bare-metal vs VM vs container host triage differently?

## Scripting: Python / Bash / Groovy (19-32)
19. How do you write robust Bash scripts (set -euo pipefail, traps, logging)?
20. How do you parse JSON/YAML in Bash vs Python?
21. Explain Python virtualenvs, pip, and requirements pinning for automation.
22. How do you handle secrets in scripts without hardcoding?
23. How do you implement retries with exponential backoff in Python/Bash?
24. How do you call REST APIs from Python and Bash (requests vs curl)?
25. What is Groovy used for in Jenkins pipelines (scripted vs declarative)?
26. How do you test Bash/Python automation (shellcheck, pytest)?
27. How do you parallelize work in Bash (xargs, &) and Python (asyncio, multiprocessing)?
28. How do you structure a reusable CLI tool in Python (argparse/click)?
29. How do you handle exit codes and idempotency in scripts?
30. How do you schedule and monitor script execution in production?
31. Explain regex log parsing for alerting.
32. How do you convert a manual runbook into an automated script safely?

## Git / GitHub / CI/CD Workflows (33-48)
33. Explain Git branching models (trunk-based vs GitFlow) for DevOps teams.
34. How do you resolve complex merge conflicts safely?
35. How do you write good commit messages and PR descriptions?
36. How do you protect branches and require reviews/status checks?
37. Explain GitHub Actions components: workflows, jobs, steps, runners, artifacts.
38. How do you manage GitHub Secrets, environments, and OIDC to AWS?
39. How do you cache Docker layers and dependencies in CI?
40. How do you design CI stages: lint, test, build, scan, push, deploy?
41. How do you implement manual approvals and environment gates?
42. How do you version artifacts and Docker tags (sha, semver, latest pitfalls)?
43. How do you roll back a bad deployment via CI/CD?
44. How do you run matrix builds for multiple Python/Node versions?
45. How do you audit CI/CD usage, cost, and runner hygiene?
46. Monorepo vs polyrepo for DevOps automation?
47. How do you handle large files/binaries with Git LFS?
48. How do you enforce conventional commits and changelog automation?

## Jenkins Administration & Security (49-62)
49. How is Enterprise Jenkins architected (controller, agents, executors)?
50. How do you provision static vs dynamic agents (SSH, Docker, K8s clouds)?
51. Declarative vs scripted Jenkins pipelines — when to use each?
52. How do you manage Jenkins credentials, vaults, and secret rotation?
53. How do you secure Jenkins (RBAC, SSO, agent-to-controller security, script approval)?
54. How do you harden Jenkins (disable CLI, CSRF, outdated plugins)?
55. How do you back up Jenkins home and recover after failure?
56. How do you manage plugins at scale without breakage?
57. How do you implement shared libraries for reusable pipeline code?
58. How do you troubleshoot slow/flaky Jenkins builds and queue starvation?
59. How do you implement build retention, log rotation, and disk management?
60. How do you integrate Jenkins with GitHub (webhooks, multibranch, status checks)?
61. How do you add SAST/DAST and image scanning gates in Jenkins?
62. Jenkins vs GitHub Actions — migration considerations?

## GitHub Actions Administration & Security (63-70)
63. How do you secure GitHub Actions (pin actions to SHA, least-privilege GITHUB_TOKEN)?
64. How do you prevent secret exfiltration in pull_request_target workflows?
65. How do you use environments, required reviewers, and deployment branches?
66. How do you build reusable workflows and composite actions?
67. How do you self-host runners securely (ephemeral, autoscaling)?
68. How do you audit Actions usage with audit logs and policies?
69. How do you do OIDC federation from Actions to AWS without static keys?
70. How do you harden third-party actions and Dependabot updates?

## Docker / Kubernetes / Cloud (71-86)
71. How do you write production Dockerfiles (multi-stage, non-root, minimal base)?
72. How do you scan and patch images (Trivy/Grype, distroless)?
73. Explain Docker networking and volumes for stateful services.
74. How do you debug a crashing container (logs, exec, inspect)?
75. Explain Kubernetes architecture (API server, etcd, scheduler, kubelet, CNI/CSI).
76. How do Deployments, StatefulSets, DaemonSets, and Jobs differ?
77. How do Services, Ingress, and NetworkPolicies work?
78. How do you manage config with ConfigMaps, Secrets, and external secret stores?
79. How do you do rolling updates, probes (liveness/readiness), and PDBs?
80. How do you troubleshoot CrashLoopBackOff, ImagePullBackOff, OOMKilled, Pending?
81. How do you handle persistent storage in K8s (PV/PVC, StorageClass)?
82. How do you deploy to EKS (IRSA, ALB controller, cluster autoscaler)?
83. How do EC2, ELB/ALB, RDS, and EKS fit together for a backend app?
84. How do you do blue-green vs canary releases on Kubernetes?
85. How do you set resource requests/limits and HPA?
86. How do you back up and restore K8s apps and RDS data?

## Config Management: Puppet vs Terraform (87-92)
87. How does Puppet work (agent, catalogs, manifests, Hiera) vs Terraform?
88. When would you use Puppet vs Terraform vs Ansible?
89. How do you manage Terraform state remotely with locking?
90. How do you structure Terraform modules for EC2/RDS/EKS?
91. How do you detect and remediate config drift?
92. How do you test infra code (tflint, checkov, terratest, puppet-lint)?

## Troubleshooting / Networking / REST / AI / Agile (93-100)
93. Walk through troubleshooting a 500-error spike across Linux, Nginx, app, RDS, and K8s.
94. Explain OSI layers with a real packet debugging example.
95. How does DNS work end-to-end and how do you debug it (dig, nslookup, resolv.conf)?
96. Compare Nginx vs HAProxy vs Apache as reverse proxies (TLS, load balancing, caching).
97. How do you design and consume REST APIs (auth, pagination, rate limits, idempotency)?
98. How do you use AI-assisted dev tools to accelerate automation while keeping code quality?
99. What guardrails do you put around AI-generated infra changes?
100. How do you work in agile/scrum as a DevOps engineer (standups, sprint planning, retros, on-call)?
