Created: 2026-10-30

# 100 Likely Interview Questions for QAD Software Engineer (Python/Golang + Agentic Platform)

## Python, FastAPI & Async (1-15)
1. Explain async/await in Python and when to use it.
2. Differences between sync vs async I/O with examples.
3. FastAPI dependency injection - how and why?
4. Pydantic v2 validation patterns.
5. How to structure a scalable FastAPI project?
6. Exception handling and custom exception handlers.
7. Background tasks vs Celery/RQ?
8. Testing async endpoints with pytest-asyncio.
9. Type hints and their value in large codebases.
10. Managing config with Pydantic Settings.
11. Middleware in FastAPI use cases.
12. API versioning strategies.
13. Rate limiting approaches.
14. Handling large request/response payloads.
15. Connection pooling for DB in async apps.

## Golang Backend (16-30)
16. Goroutines vs threads.
17. Channels - buffered/unbuffered, select, deadlocks.
18. sync.Mutex vs sync.RWMutex.
19. Context usage for cancellation/timeouts.
20. Error handling idioms in Go.
21. Interfaces and composition.
22. Struct embedding vs inheritance.
23. Working with net/http or Chi framework.
24. Database access with sqlc/pgx.
25. Concurrency patterns (worker pools, fan-in/fan-out).
26. Testing in Go (table-driven tests).
27. Memory management/go GC basics.
28. Handling graceful shutdown.
29. Build tags and project layout.
30. When to use pointers vs values.

## MCP, A2A & Multi-Agent (31-50)
31. What is Model Context Protocol (MCP)? Architecture and use cases.
32. MCP vs function/tool calling differences.
33. Designing an MCP tool server.
34. What is Agent-to-Agent (A2A) protocol?
35. When to use A2A vs MCP?
36. Multi-agent patterns (router, supervisor, handoff).
37. Tool binding and scope enforcement.
38. Context injection for agents.
39. Managing agent state/memory.
40. Orchestration vs choreography in agents.
41. Human-in-the-loop patterns.
42. Handling tool failures and retries.
43. Agent authentication/authorization.
44. Preventing tool misuse/overreach.
45. Designing composable agents.
46. Tracing agent execution flows.
47. When to use single agent vs multi-agent.
48. Agent-to-tool vs agent-to-agent communication.
49. Schema design for tool inputs/outputs.
50. Versioning agent capabilities.

## Prompting, Evals & Observability (51-65)
51. System vs user vs assistant prompts.
52. Few-shot vs zero-shot prompting.
53. Prompt engineering best practices.
54. Context window management.
55. Reducing hallucinations.
56. Why evaluate agents (vs just prompts)?
57. DeepEval concepts and usage.
58. Designing eval datasets.
59. Metrics: task success, tool correctness, groundedness.
60. Tracing/observability for agents.
61. Logging prompts/responses safely (PII).
62. Cost/latency tracking.
63. Regression testing for prompts.
64. A/B testing agent versions.
65. Debugging failed agent runs.

## Platform, K8s, CI/CD, DX (66-85)
66. Trunk-based development vs GitFlow.
67. PR-gated merges and code review best practices.
68. Kubernetes basics: Pods, Services, Deployments, ConfigMaps.
69. Creating/managing K8s manifests.
70. LaunchDarkly feature flags for prompts/config.
71. Docker multi-stage builds.
72. GitHub Actions CI/CD patterns.
73. Database registration/migrations in platform.
74. Developer experience improvements (scaffolding).
75. Internal docs and onboarding paths.
76. Secrets management in K8s/CI.
77. Health checks, readiness/liveness probes.
78. Zero-downtime deployments.
79. Rollback strategies.
80. Monorepo vs multi-repo considerations.

## AWS, DB, Testing & Behavioral (86-100)
81. AWS ECR/EKS basics relevant to platform work.
82. PostgreSQL indexing/query optimization.
83. Migrations and schema evolution.
84. Connection management and transactions.
85. pytest patterns for backend services.
86. Mocking external services/tools.
87. Integration vs unit tests.
88. Security basics (authN/Z, input validation).
89. Handling errors and observability in prod.
90. Describe a time you improved developer experience.
91. How do you review agent implementations?
92. Pairing with other engineers approach.
93. Balancing platform work vs BU requests.
94. How do you ensure prompt quality in prod?
95. What interests you about QAD/Redzone/ChampionAI?
96. Experience with AI-native tools (Cursor/Claude Code)?
97. How do you stay updated on agentic AI?
98. Approach to debugging complex issues.
99. Why are you a good fit for this role?
100. Questions for the interviewer.
