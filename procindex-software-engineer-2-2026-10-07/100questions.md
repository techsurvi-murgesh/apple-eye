# 100 Interview Questions — Software Engineer 2, Procindex

## TypeScript / Node.js Backend (1-16)
1. How do you structure a Node.js/TypeScript backend for a multi-tenant SaaS product?
2. How does the Node.js event loop work and how do you keep services non-blocking?
3. How do you design clean service layers and dependency boundaries in TypeScript?
4. How do you handle async errors, retries, and timeouts in Node.js?
5. How do you make API endpoints idempotent for financial workflows?
6. How do you validate input and prevent injection at API boundaries?
7. How do you version APIs without breaking existing customers?
8. How do you handle authentication, API keys, and tenant isolation?
9. How do you design rate limiting and backpressure per tenant?
10. How do you bound concurrency when calling external services?
11. How do you design webhooks to ERPs/email systems reliably?
12. How do you handle partial failures across multiple external calls?
13. How do you write testable TypeScript (pure functions, DI, mocks)?
14. How do you structure a monorepo for backend + shared types?
15. How do you handle graceful shutdown without dropping in-flight jobs?
16. How do you profile and fix a slow Node.js endpoint?

## Backend System Design (17-32)
17. Design a system for invoice processing, approvals, and reconciliation.
18. How would you model the accounts payable (AP) lifecycle as a state machine?
19. How would you design accounts receivable (AR) and collections workflows?
20. How do you design a matching/reconciliation engine between records?
21. How do you ensure correctness and idempotency in money-handling systems?
22. How do you design multi-tenant data isolation?
23. How do you design for auditability and compliance in finance workflows?
24. How do you handle long-running workflows that span days/weeks?
25. How do you design a queue-based architecture for background jobs?
26. How do you choose between a queue, a cron, and a workflow engine?
27. How do you handle exactly-once vs at-least-once processing?
28. How do you design a schema for invoices, line items, and approvals?
29. How do you handle concurrency when two users act on the same invoice?
30. How do you design notifications and escalations for approvals?
31. How do you plan for reconciliation reporting and dashboards?
32. How would you design this platform to go from 0 to 1 quickly?

## PostgreSQL & Data (33-46)
33. How do you model financial records in PostgreSQL?
34. How do you use transactions and locking to keep balances consistent?
35. What isolation levels matter for money-handling and why?
36. How do you avoid deadlocks in concurrent financial writes?
37. How do you write efficient indexes and read query plans?
38. How do you handle large tables and pagination at scale?
39. How do you do zero-downtime schema migrations?
40. How do you handle soft deletes and audit history?
41. How do you design idempotent writes and dedupe?
42. How do you handle monetary precision (no floating point)?
43. How do you partition or archive old transaction data?
44. How do you back up and restore safely?
45. When would you add a cache or a search store alongside Postgres?
46. How do you detect and fix N+1 queries?

## Async Workflows, Queues & Background Jobs (47-58)
47. How do you design a reliable background job processor in Node.js?
48. What queues have you used (BullMQ, SQS, RabbitMQ) and how do you choose?
49. How do you handle job retries with exponential backoff and dead-letter queues?
50. How do you make jobs idempotent so retries are safe?
51. How do you handle poison messages and stuck jobs?
52. How do you schedule delayed and recurring jobs (approval reminders, reminders)?
53. How do you observe and monitor queue depth and job latency?
54. How do you handle ordering and dependencies between jobs?
55. How do you scale workers horizontally safely?
56. How do you handle long jobs without blocking the worker?
57. How do you recover jobs after a crash or deploy?
58. How do you balance synchronous vs asynchronous processing?

## Integrations — ERP, Email, Third-Party (59-70)
59. How would you integrate with ERPs (QuickBooks, NetSuite, SAP) via APIs?
60. How do you handle OAuth and token refresh across tenants?
61. How do you handle inconsistent or poorly documented third-party APIs?
62. How do you normalize data from many different ERP schemas?
63. How do you build an integration abstraction so new ERPs are easy to add?
64. How do you ingest and parse invoices from email (attachments, PDFs)?
65. How do you handle webhooks from external systems reliably and idempotently?
66. How do you deal with rate limits and quotas from third-party APIs?
67. How do you test integrations without touching live customer systems?
68. How do you surface integration failures to customers clearly?
69. How do you handle data synchronization and conflict resolution?
70. How do you debug a failed sync end-to-end?

## AI Agents / LLM Workflows (71-80)
71. How would you build an AI agent for accounting document processing?
72. How do you add guardrails so an AI agent can't take harmful actions?
73. How do you design retries, logging, and fallbacks around LLM calls?
74. How do you validate LLM output before it affects financial data?
75. How do you handle hallucinations in a high-stakes domain?
76. How do you control cost and latency of LLM calls at scale?
77. How do you design human-in-the-loop approval for AI decisions?
78. How do you evaluate and improve an agent's accuracy over time?
79. How do you handle PII/financial data privacy with LLM providers?
80. When would you not use an LLM and just write deterministic code?

## Reliability, Observability & Production (81-92)
81. How do you add observability (logs, metrics, traces) to a backend service?
82. How do you correlate a request across services with correlation IDs?
83. How do you alert on failures without noisy false positives?
84. How do you do safe deploys and fast rollbacks?
85. How do you debug a production issue with early customers?
86. How do you handle a third-party outage affecting core workflows?
87. How do you set SLOs for critical finance workflows?
88. How do you do load testing and capacity planning?
89. How do you manage secrets and config across environments?
90. How do you handle data migrations in production?
91. How do you build a CI/CD pipeline for a Node.js service?
92. How do you decide when to refactor vs ship the pragmatic fix?

## Ownership, Product & Startup Behavioral (93-100)
93. Describe a time you owned a feature end-to-end from 0 to 1.
94. Tell me about a messy real-world problem you solved pragmatically.
95. How do you make engineering decisions without overengineering?
96. How do you work directly with founders and early customers?
97. How do you handle ambiguity when requirements change weekly?
98. How do you prioritize when everything is urgent at a startup?
99. How do you debug production issues at speed with limited tooling?
100. Why Procindex, why a backend role, and what would you ship in your first 90 days?
