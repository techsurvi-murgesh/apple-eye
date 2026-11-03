Created: 2026-10-30

# 100 Likely Interview Questions for MetLife AI Engineer (Azure-based)

## Python, FastAPI & Backend APIs (1-15)
1. Explain FastAPI vs Flask/Django and when you'd choose FastAPI.
2. How does async/await work in Python and when is it beneficial?
3. How would you design idempotent REST APIs?
4. Explain dependency injection in FastAPI.
5. How do you handle validation and serialization in FastAPI (Pydantic)?
6. Strategies for API versioning?
7. How to handle authentication/authorization (JWT/OAuth)?
8. How would you structure a large FastAPI microservice?
9. Explain CORS and how to configure it securely.
10. How do you handle rate limiting in APIs?
11. Difference between sync and async DB drivers?
12. How to implement pagination efficiently?
13. Error handling patterns in FastAPI?
14. How do you test FastAPI endpoints?
15. When would you use background tasks vs message queues?

## Agentic AI, LangGraph/LangChain (16-30)
16. What are agentic AI workflows and how do they differ from chains?
17. Explain LangGraph concepts (nodes, edges, state, tools).
18. How do you implement tool calling with LLMs?
19. Multi-step orchestration strategies and pitfalls.
20. Context and memory management in agents (short/long-term)?
21. How to implement retries and timeouts for tool calls?
22. Guardrails for agents (prompt injection, tool misuse)?
23. Human-in-the-loop patterns?
24. How do you debug agent traces?
25. When to use ReAct vs plan-execute patterns?
26. Managing agent state across turns?
27. Handling failures in multi-agent systems?
28. Cost/latency tradeoffs in agent design?
29. Evaluating agent reliability?
30. How would you prevent infinite loops in agents?

## LLMs, RAG, Vector Search (31-45)
31. Explain embeddings and vector similarity.
32. RAG architecture end-to-end.
33. Chunking strategies for documents.
34. When to use hybrid search vs pure vector?
35. Prompt engineering vs context engineering.
36. How to reduce hallucinations in RAG?
37. Evaluating RAG quality (faithfulness, relevance)?
38. Caching strategies for LLM calls?
39. Handling long context windows?
40. Fine-tuning vs RAG vs prompting?
41. Vector DB options and selection criteria.
42. Re-ranking in retrieval pipelines?
43. Managing prompt templates and versions.
44. Handling PII in prompts/RAG?
45. Cost optimization for embeddings and completions.

## Azure, AKS, Kubernetes, Docker (46-60)
46. Azure AKS architecture basics.
47. Docker multi-stage builds and optimization.
48. Kubernetes Deployments vs StatefulSets vs DaemonSets.
49. Helm charts - structure and best practices.
50. ConfigMaps/Secrets management in K8s.
51. Liveness/readiness/startup probes.
52. Resource requests/limits and autoscaling (HPA).
53. Service types (ClusterIP/NodePort/LoadBalancer).
54. Ingress controllers in AKS.
55. Debugging CrashLoopBackOff/ImagePullBackOff.
56. Network policies in K8s.
57. Azure Container Registry (ACR) integration.
58. Managing secrets with Azure Key Vault + CSI driver.
59. Pod security contexts/best practices.
60. Zero-downtime deployments in K8s.

## Event-Driven, Messaging, Reliability (61-75)
61. Event Hubs vs Kafka - differences and use cases.
62. Designing idempotent consumers.
63. Backfill and replay strategies.
64. Dead letter queues (DLQs).
65. Event ordering guarantees.
66. Handling schema evolution.
67. Exactly-once vs at-least-once semantics.
68. Retry with exponential backoff and jitter.
69. Circuit breaker pattern.
70. Bulkhead isolation.
71. SLO/SLI/SLA definitions and implementation.
72. Distributed tracing (OpenTelemetry concepts).
73. Logging strategies for microservices.
74. Incident triage and blameless postmortems.
75. Graceful shutdown in services.

## MLOps, CI/CD, Security & Behavioral (76-100)
76. MLflow vs LangSmith for LLM observability.
77. Model versioning and serving patterns.
78. Batch vs real-time inference tradeoffs.
79. CI/CD for services and model pipelines.
80. Release gating and canary deployments.
81. Security scanning in pipelines (SAST/DAST/dependency).
82. Secrets management best practices.
83. Principle of least privilege (RBAC/IAM).
84. Container image scanning.
85. API security (rate limiting, input validation, OWASP Top 10).
86. Observability: metrics, logs, traces correlation.
87. Cost monitoring for LLM workloads.
88. How would you optimize latency/cost for agents?
89. Tell me about a time you improved reliability.
90. How do you handle conflicting priorities?
91. Describe debugging a production incident.
92. How do you ensure code quality in reviews?
93. Experience collaborating with frontend (React/Next.js)?
94. How would you approach onboarding to MetLife's domain?
95. What interests you about MetLife's AI strategy?
96. How do you stay current with AI/LLM developments?
97. Describe a complex distributed system you built.
98. How do you balance speed vs reliability?
99. Give example of automation saving time.
100. Why should we hire you for this AI Engineer role?
