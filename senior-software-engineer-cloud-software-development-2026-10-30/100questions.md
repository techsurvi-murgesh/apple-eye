# 100 Interview Questions — Senior Software Engineer, Cloud Software Development

Target profile: Go engineer owning distributed cloud services end-to-end, running cloud-native workloads on Kubernetes, modelling data in NoSQL stores, building event-driven and high-availability API surfaces (Kafka/MQTT), operating production systems, and applying AI tools and agents across the SDLC.

## Go Language and Runtime (1–18)

1. How do goroutines differ from OS threads, and how does the Go scheduler multiplex them?
2. Explain the G-M-P scheduler model and what happens during a blocking syscall.
3. When would you use a buffered channel versus an unbuffered channel?
4. How do you detect and prevent goroutine leaks in a long-running service?
5. How does `context.Context` propagate cancellation and deadlines across service boundaries?
6. What is the difference between `sync.Mutex`, `sync.RWMutex`, and channel-based coordination?
7. How do you reason about data races, and which tools do you use to find them?
8. Explain escape analysis and how it affects allocations and GC pressure.
9. How would you tune `GOGC` and `GOMEMLIMIT` for a latency-sensitive service?
10. What does the Go memory model guarantee about visibility of writes across goroutines?
11. How do `defer`, `panic`, and `recover` interact, and where should recover be used?
12. How do interfaces and implicit satisfaction shape service design in Go?
13. When would you use generics, and when do they hurt readability?
14. How do you implement graceful shutdown for an HTTP server and background workers?
15. How does `errgroup` simplify concurrent work with cancellation and error aggregation?
16. How do you profile CPU, heap, mutex, and block contention in production?
17. What are common causes of high tail latency in Go services?
18. How do you structure packages for a multi-service Go repository without circular dependencies?

## Kubernetes and Cloud-Native Platforms (19–38)

19. Walk through what happens in Kubernetes from `kubectl apply` to a running pod.
20. How do Deployments, ReplicaSets, and Pods relate?
21. How do readiness, liveness, and startup probes differ, and how do you design them?
22. What happens when a pod exceeds its memory limit versus its CPU limit?
23. Explain requests, limits, and Quality of Service classes.
24. How does the Horizontal Pod Autoscaler make scaling decisions, and what are its limits?
25. How would you design a service that must survive node drains during rolling updates?
26. What is a PodDisruptionBudget and when does it matter?
27. How do Services, EndpointSlices, and kube-proxy route traffic?
28. Compare ClusterIP, NodePort, LoadBalancer, and Ingress.
29. How do ConfigMaps and Secrets differ, and what are the risks of each?
30. How would you manage secrets for production workloads in Kubernetes?
31. Explain namespaces, resource quotas, and limit ranges for multi-team clusters.
32. How do network policies work, and how would you isolate a service?
33. What is the role of an admission controller or policy engine in a platform?
34. How do you debug a pod stuck in `CrashLoopBackOff` or `ImagePullBackOff`?
35. How do you investigate a pod evicted for resource pressure?
36. What strategies do you use for zero-downtime deployments and fast rollback?
37. How do you operate stateful workloads such as databases on Kubernetes?
38. How do you observe a Kubernetes platform end-to-end: metrics, logs, traces, events?

## Distributed Systems and NoSQL (39–58)

39. What does "own a service end-to-end" mean to you in practice?
40. How do you define SLIs, SLOs, and error budgets for a cloud service?
41. Explain the CAP theorem with a concrete example from your work.
42. How do you choose between strong and eventual consistency for a given feature?
43. What is idempotency, and how do you enforce it on retried writes?
44. How do you design for at-least-once delivery without duplicating side effects?
45. Compare optimistic and pessimistic concurrency control.
46. How would you model a one-to-many relationship in a document database?
47. When would you denormalize data in NoSQL, and what does it cost you?
48. How do you choose a partition key, and what is a hot partition?
49. How do secondary indexes work in NoSQL stores, and what are their trade-offs?
50. How do you handle schema evolution in an eventually consistent system?
51. Explain quorum reads and writes and how they affect latency and durability.
52. What is a distributed transaction, and when do you use a saga instead?
53. How do you detect and recover from partial failures across services?
54. What is backpressure, and how do you apply it to a consumer?
55. How do you design retries with exponential backoff and jitter without causing retry storms?
56. What is a circuit breaker, and where does it belong in the call path?
57. How do you approach cache invalidation and cache stampedes?
58. How would you run a production incident review and turn it into preventive work?

## API Design and High Availability (59–72)

59. What makes an API high-availability ready versus merely functional?
60. How do you version APIs without breaking existing mobile clients?
61. How do you design pagination for large, changing datasets?
62. How do you make write endpoints safe to retry?
63. How do you model errors so clients can act on them programmatically?
64. How do you set and enforce timeouts across a request chain?
65. What is the difference between rate limiting and throttling, and how do you implement each?
66. How do you design authentication and authorization for service-to-service calls?
67. How do you prevent request amplification and fan-out failures?
68. How do you test an API for availability, not just correctness?
69. How would you design a multi-region failover strategy?
70. What is the difference between active-active and active-passive, and what does each cost?
71. How do you safely deprecate an endpoint with live mobile traffic?
72. How do you document API contracts and keep them in sync with implementation?

## Kafka, MQTT, and Event-Driven Architecture (73–84)

73. How does Kafka achieve durability and ordering within a partition?
74. Explain consumer groups, rebalancing, and offset management.
75. What delivery guarantees does Kafka offer, and what must the producer and consumer do to get them?
76. How do you handle poison messages and dead-letter topics?
77. How do you choose the number of partitions for a topic?
78. What causes consumer lag, and how do you monitor and reduce it?
79. How would you design an exactly-once-ish payment or charging-session workflow?
80. Compare Kafka with a traditional queue for work distribution.
81. Where does MQTT fit for vehicle or device connectivity, and how does it differ from Kafka?
82. How do QoS levels 0, 1, and 2 behave in MQTT?
83. How do you handle retained messages, last-will, and reconnect storms in MQTT?
84. How would you design an event schema and evolve it without breaking consumers?

## AI-Native Software Engineering (85–93)

85. Which parts of your development workflow do you delegate to AI tools, and which do you keep yourself?
86. How do you verify AI-generated code before it reaches production?
87. How do you use AI for requirements and design exploration without outsourcing judgement?
88. How do you prompt an agent effectively for a multi-file refactor?
89. What are the risks of pasting production code or customer data into AI tools?
90. How do you use AI to generate tests, and how do you avoid tests that merely mirror the implementation?
91. How do you review an AI-authored pull request differently from a human-authored one?
92. How would you measure whether AI tooling is actually improving delivery quality?
93. What is your view on AI agents operating production systems, and what guardrails would you require?

## Frontend, Mentoring, and Leadership (94–100)

94. How do you design an API for both a React web client and a mobile app?
95. What frontend concerns should a backend engineer understand when collaborating with mobile and web teams?
96. How do you describe trade-offs to Product and QA without losing technical precision?
97. How have you mentored a less experienced engineer, and what changed as a result?
98. How do you lead a technical design discussion where the team disagrees?
99. Tell me about a production incident you owned end-to-end and what you changed afterwards.
100. Why this role, and what would you want to own in your first six months?
