# 100 Interview Questions — DevOps Engineer (MBS Global, Bengaluru) — 2026-11-03

Target stack: CI/CD (Jenkins, GitHub Actions, GitLab CI, Azure DevOps), AWS/Azure/GCP, Terraform (IaC), Docker, Kubernetes, Linux administration, Shell/Python/Bash scripting, Git; Monitoring: Prometheus, Grafana, ELK, Datadog, CloudWatch; DevSecOps, networking (DNS, load balancers, SSL/TLS).

## CI/CD Pipelines (1-20)

1. What is CI/CD, and what is the difference between continuous integration, continuous delivery, and continuous deployment?
2. How do you design a CI/CD pipeline from commit to production for a microservice?
3. How do you use Jenkins to build, test, and deploy applications?
4. What are the differences between declarative and scripted Jenkins pipelines?
5. How do you manage Jenkins agents and scale builds dynamically?
6. How do you parameterize a Jenkins job for multi-environment deployments?
7. How do you store and use credentials securely in Jenkins (AWS keys, SSH, tokens)?
8. How do you implement shared libraries to reuse pipeline code across teams in Jenkins?
9. How do you add build, test, lint, and code-quality gates to a Jenkins pipeline?
10. How do you trigger Jenkins from GitHub webhooks and enforce status checks?
11. How do you implement blue/green or canary deployment in Jenkins to production?
12. How do you make a Jenkins deployment automatically roll back on failure?
13. How do you speed up a slow Jenkins pipeline (caching, parallelism, incremental builds)?
14. How do you back up and restore Jenkins (JENKINS_HOME, plugins, credentials)?
15. How do you troubleshoot a Jenkins build stuck in the queue or a flaky stage?
16. How do you secure Jenkins (RBAC, SSO, CSRF, script approval, agent isolation)?
17. Compare Jenkins with GitHub Actions, GitLab CI, and Azure DevOps for a large enterprise.
18. How do you migrate pipelines from legacy freestyle jobs to declarative Jenkinsfiles safely?
19. How do you version artifacts and Docker images produced by CI to make deployments traceable?
20. How do you implement approval gates for production deployments in CI/CD?

## GitHub Actions & GitLab CI (21-40)

21. How do you write a GitHub Actions workflow (triggers, jobs, steps, matrix builds)?
22. How do you store and use secrets in GitHub Actions?
23. How do you cache dependencies in GitHub Actions to speed up builds?
24. How do you implement reusable workflows and composite actions in GitHub Actions?
25. How do you enforce branch protection and required status checks in GitHub?
26. How do you write a GitLab CI .gitlab-ci.yml (stages, jobs, artifacts, caches)?
27. How do you use GitLab CI environments and protection rules for deployments?
28. How do you configure GitLab runners (shared, specific, autoscaling)?
29. How do you pass artifacts between stages in GitLab CI?
30. How do you implement manual approval jobs in GitLab CI?
31. How do you use GitLab CI pipeline schedules and triggers?
32. How do you compare GitHub Actions vs GitLab CI for an enterprise?
33. How do you set up Azure DevOps pipelines (YAML vs classic)?
34. How do you use Azure DevOps variable groups and secret variables?
35. How do you implement approval gates in Azure DevOps releases?
36. How do you integrate Azure DevOps with Azure services (AKS, ACR, App Service)?
37. How do you use Azure DevOps service connections for AWS/GCP?
38. How do you implement multi-stage pipelines in Azure DevOps?
39. How do you use pipeline templates and variable templates in Azure DevOps?
40. How do you compare Azure DevOps with GitHub Actions and GitLab CI?

## Cloud Platforms: AWS / Azure / GCP (41-60)

41. What are the core AWS services you use for DevOps (EC2, Lambda, RDS, S3, ECR, CloudFront, IAM, VPC)?
42. How do you design a VPC (public/private subnets, route tables, NAT, IGW)?
43. How do you secure S3 (bucket policies, Block Public Access, encryption, presigned URLs)?
44. How do you manage IAM roles, policies, and cross-account access in AWS?
45. How do you use security groups and NACLs to secure AWS workloads?
46. What are the core Azure services for DevOps (AKS, ACR, App Service, Azure DevOps, Azure Monitor)?
47. How do you manage Azure subscriptions, resource groups, and RBAC?
48. How do you use Azure Key Vault and Managed Identities for secrets?
49. What are the core GCP services for DevOps (GKE, Cloud Run, Cloud Storage, Secret Manager)?
50. How do you manage GCP IAM roles and service accounts?
51. How do you choose between AWS, Azure, and GCP for a given workload?
52. How do you implement multi-cloud or hybrid-cloud deployments?
53. How do you manage cloud costs and set up billing alerts?
54. How do you handle cloud networking (VPN, peering, private endpoints)?
55. How do you implement infrastructure as code across multiple cloud providers?
56. How do you manage cloud provider authentication in CI/CD (OIDC, service accounts)?
57. How do you implement disaster recovery and backup in the cloud?
58. How do you handle cloud service limits and quotas?
59. How do you monitor cloud services (CloudWatch, Azure Monitor, Cloud Monitoring)?
60. How do you implement auto-scaling in AWS/Azure/GCP?

## Terraform & Infrastructure as Code (61-80)

61. What is Infrastructure as Code, and what are its benefits?
62. How do you write Terraform configuration (providers, resources, variables, outputs)?
63. How do you manage Terraform state (local, remote, state locking)?
64. How do you use Terraform workspaces for multiple environments?
65. How do you implement Terraform modules for reusable infrastructure?
66. How do you run `terraform plan`, `terraform apply`, and `terraform destroy` safely?
67. How do you import existing infrastructure into Terraform state?
68. How do you handle Terraform state drift and remediate it?
69. How do you use Terraform with AWS/Azure/GCP providers?
70. How do you provision a VPC, EKS/AKS/GKE, and RDS using Terraform?
71. How do you manage secrets in Terraform (AWS Secrets Manager, Azure Key Vault)?
72. How do you integrate Terraform with CI/CD pipelines?
73. How do you implement policy as code with Terraform (Sentinel, OPA)?
74. How do you version Terraform modules and providers?
75. How do you use `terraform import` and `terraform state` commands?
76. How do you handle Terraform parallelism and resource dependencies?
77. How do you use `terraform taint` and `terraform apply -target`?
78. How do you implement Terraform best practices (naming, tagging, modularity)?
79. How do you use Terraform with Kubernetes (helm provider, kubernetes provider)?
80. How do you troubleshoot Terraform apply failures?

## Docker & Kubernetes (81-100)

81. What is Docker, and how do containers differ from VMs?
82. How do you write a Dockerfile (multi-stage builds, small images, .dockerignore)?
83. How do you build, tag, push, and pull Docker images?
84. How do you manage Docker volumes, networks, and compose files?
85. How do you scan Docker images for vulnerabilities (Trivy, Snyk)?
86. What is Kubernetes, and what are its core components (Pods, Nodes, Control Plane)?
87. How do you use Kubernetes Deployments, Services, and Ingress?
88. How do you manage ConfigMaps and Secrets in Kubernetes?
89. How do you implement health probes (liveness, readiness, startup) in Kubernetes?
90. How do you use Horizontal Pod Autoscaler and PodDisruptionBudgets?
91. How do you deploy applications to Kubernetes using Helm charts?
92. How do you implement rolling updates and rollbacks in Kubernetes?
93. How do you manage namespaces, RBAC, and service accounts in Kubernetes?
94. How do you troubleshoot CrashLoopBackOff, failed rollout, and ImagePullBackOff?
95. How do you implement resource limits and requests in Kubernetes?
96. How do you use Kubernetes PersistentVolumes and StorageClasses?
97. How do you secure Kubernetes (network policies, pod security, admission controllers)?
98. How do you integrate Kubernetes with CI/CD (deploy, test, rollback)?
99. How do you monitor Kubernetes (metrics-server, Prometheus, kube-state-metrics)?
100. How do you implement a GitOps workflow with ArgoCD or Flux?
