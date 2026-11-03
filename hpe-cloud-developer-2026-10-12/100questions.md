# 100 Interview Questions — Cloud Developer, HPE Hybrid Cloud (Green Lake) — 2026-10-12

Target profile: early-career cloud developer (1-3 yrs) on a hybrid cloud platform team. Python / Golang / JavaScript, containers and Kubernetes, AWS + Azure, CI/CD on GitHub Actions, virtualization (KVM/OpenVZ), microservices, test-plan design and automated testing, production debugging and monitoring.

## Cloud Fundamentals & Architecture (1-16)

1. Explain the difference between IaaS, PaaS, and SaaS with an example of each.
2. What does "hybrid cloud" mean in practice, and what makes it harder than pure cloud?
3. How would you explain a consumable cloud service model (Green Lake style) to a customer?
4. What is the difference between a container and a virtual machine?
5. Explain shared kernel vs hypervisor isolation. What are the security trade-offs?
6. What is the twelve-factor app, and which factors break most often in practice?
7. How do you decide between a monolith and microservices for a given workload?
8. Explain stateless vs stateful services and why stateless scales easier.
9. What is a service mesh, and do you actually need one?
10. How do you handle schema/data evolution across independently deployed microservices?
11. Explain idempotency. Where must it hold in a distributed system?
12. How do you design an API that third parties will integrate against for years?
13. What is a circuit breaker, and how does it differ from a retry?
14. Explain the difference between orchestration and choreography in workflows.
15. How do you pass secrets to a workload running in a cloud environment?
16. How would you model a simple multi-tenant SaaS control plane?

## Containers & Kubernetes (17-38)

17. What happens between `docker run` and a process running in a container?
18. Explain Docker image layers. Why does layer caching matter for CI?
19. What is a multi-stage Docker build and why do you use it?
20. Why is a container image a bad thing to use directly in production?
21. What is the difference between a Deployment and a StatefulSet?
22. Explain Services, Ingress, and how traffic actually reaches a pod.
23. What are liveness, readiness, and startup probes, and what breaks if you reuse one probe for all three?
24. Explain ConfigMaps vs Secrets. What are the risks with each?
25. What are resource requests and limits, and how do they affect scheduling?
26. What is a Pod Disruption Budget and when do you need one?
27. Explain Horizontal Pod Autoscaling, including the metrics it needs.
28. Your pod is stuck in `CrashLoopBackOff`. Walk me through your debugging steps.
29. What is a custom resource (CRD) and why would you define one?
30. How do you expose a workload outside the cluster in a production setup?
31. What is the Kubernetes eviction problem, and how do you handle node pressure?
32. Explain rolling updates and what happens to in-flight requests during one.
33. What are namespaces for, and when do they stop being enough?
34. How do you manage Helm charts across many environments?
35. Explain RBAC. How would you give a CI pipeline deploy rights safely?
36. What is a sidecar, and what problems does it create?
37. How do you safely upgrade the Kubernetes version on a live cluster?
38. Explain how you would run a database inside Kubernetes, and why it is often a bad idea.

## Networking & Virtualization (39-52)

39. Explain KVM. How does it differ from a container runtime?
40. What is OpenVZ, and what problem does it solve that containers do not?
41. When would you choose KVM over containers for the same workload?
42. Explain bridge vs NAT networking in a virtualization host.
43. What is a CNI plugin, and where does it fit in the Kubernetes network path?
44. How does DNS resolution work inside a Kubernetes cluster?
45. Explain service-to-service networking, including network policies.
46. You have intermittent packet loss between two pods. How do you troubleshoot it?
47. What is MTU, and what causes MTU-related failures on overlay networks?
48. Explain TLS termination at the ingress controller vs the application.
49. How do you debug a network connectivity problem from the host down to the pod?
50. What is a VPC, and what security groups or network ACLs protect it?
51. Explain the difference between security groups and network ACLs.
52. How do you set up VPN or direct connect between an on-prem site and a cloud VPC?

## AWS & Azure Platforms (53-66)

53. What are the main compute options in AWS, and when do you use each?
54. Explain IAM. How do you design least-privilege policies?
55. What is an EC2 instance vs a Lambda function in terms of cost and behaviour?
56. What problem does an Auto Scaling Group solve?
57. Explain RDS vs DynamoDB. When would you choose either?
58. What is an availability zone, and why does it matter for design?
59. How do you design for high availability across three AZs?
60. What are S3 storage classes, and how do lifecycle policies work?
61. What is a VPC peering connection and what are its limits?
62. How do you move large amounts of data into a cloud provider cheaply?
63. Explain the equivalent Azure services: VMs, App Service, AKS, Blob, SQL.
64. What is Azure Resource Manager, and how does it differ from Azure CLI?
65. Compare managed identities in AWS (IAM roles) and Azure (service principals / managed identity).
66. How do you keep cloud costs under control in a growing environment?

## CI/CD & GitHub Actions (67-82)

67. What is the full flow of a CI/CD pipeline for a containerized service?
68. How do you structure a GitHub Actions workflow file?
69. What is a matrix build, and when do you use it?
70. How do you cache dependencies in a GitHub Actions runner?
71. Explain how you would pass secrets into a workflow without leaking them.
72. How do you build and push a Docker image from a pipeline?
73. How do you tag images, and how does that affect rollback?
74. What is a deployment strategy: recreate, rolling, blue/green, canary?
75. How do you implement blue/green deployment with a database schema change?
76. What is a pipeline as code, and why does it matter?
77. How do you gate a deploy on test results?
78. Your pipeline is flaky. How do you find and fix the cause?
79. How do you run integration tests against dependencies in CI?
80. What is infrastructure as code, and how does it fit into CI/CD?
81. How do you handle database migrations in a zero-downtime deployment?
82. How would you set up a pipeline that deploys the same artifact to dev, stage, and prod?

## Testing & Quality (83-92)

83. What goes into a good test plan?
84. Explain the test pyramid. Where do most tests belong, and why?
85. What is the difference between unit, integration, and end-to-end testing?
86. What is test coverage, and what does a high number not tell you?
87. How do you test a service that depends on a third-party API?
88. How do you write deterministic tests for concurrent code?
89. What is property-based or fuzz testing, and when is it valuable?
90. How do you decide what to automate in a test suite?
91. What is a regression, and how do you prevent one?
92. How do you make test suites fast enough that developers actually run them?

## Debugging, Operations & Monitoring (93-100)

93. Walk me through your approach to debugging a production issue at 2 a.m.
94. How do you read logs effectively when a request spans many services?
95. What is distributed tracing, and how do you implement it?
96. What metrics would you monitor for a containerized microservice?
97. How do you set up alerting without creating alert fatigue?
98. Explain the four golden signals.
99. How do you debug a performance regression that appeared after a release?
100. How do you write a clear bug report or post-mortem after resolving an incident?