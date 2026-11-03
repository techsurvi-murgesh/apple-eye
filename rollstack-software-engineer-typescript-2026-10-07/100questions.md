# 100 Interview Questions — Software Engineer (TypeScript), Rollstack

## TypeScript & CS Fundamentals (1-14)
1. Explain TypeScript's type system and when to use interfaces vs types.
2. What are generics in TypeScript and how do you use them in a real API?
3. Explain union, intersection, and discriminated unions with a practical example.
4. How do you handle strict null checks and type narrowing?
5. How do you type async code, promises, and errors correctly?
6. How do you avoid `any` and type third-party libraries safely?
7. What's the difference between `unknown`, `any`, and `never`?
8. How do you structure a shared TypeScript package across frontend and backend?
9. Explain Big-O for common data structures you use daily.
10. How would you find duplicates / top-K elements in a large dataset efficiently?
11. Explain memoization and when it helps vs hurts.
12. How do you detect and resolve a memory leak in a Node.js service?
13. How do you write clean, testable TypeScript (pure functions, DI)?
14. What are the tradeoffs of monorepo vs polyrepo for a TypeScript product?

## React / Frontend (15-28)
15. Explain React hooks (useState, useEffect, useMemo, useCallback) and common pitfalls.
16. How do you build composable UI with custom hooks and Shadcn/UI?
17. How do you manage server state vs client state in React?
18. How do you avoid unnecessary re-renders in a data-heavy UI?
19. How do you build a native charts feature in React (data viz performance)?
20. How do you handle loading, error, and empty states cleanly?
21. How do you use Tailwind CSS effectively and keep components consistent?
22. How do you keep frontend and backend TypeScript contracts in sync?
23. How do you implement optimistic UI updates and rollback?
24. How do you handle auth/session in a React SPA?
25. How do you do pagination/infinite scroll for large result sets?
26. How do you test React components (unit + integration)?
27. How do you debug a frontend bug that spans UI, API, and database?
28. How do you keep fast iteration without accumulating UI tech debt?

## Node.js Backend & APIs (29-42)
29. How does the Node.js event loop work and how does it affect API design?
30. How do you design an async Node.js service that stays non-blocking?
31. How do you build a REST/RPC API in Node.js with clean architecture?
32. How do you handle errors, retries, and timeouts in a Node backend?
33. How do you design idempotent endpoints and webhooks?
34. How do you handle concurrency and race conditions in Node.js?
35. How do you bound concurrency when calling external APIs?
36. How do you structure a Node.js project for maintainability (layers, services)?
37. How do you handle background jobs and queues in Node.js?
38. How do you manage config and secrets across environments?
39. How do you version an API without breaking clients?
40. How do you profile and optimize a slow Node.js service?
41. How do you handle graceful shutdown without dropping requests?
42. How would you integrate a Generative-AI API into a product feature?

## Data, Prisma, Sync Engine & Temporal (43-56)
43. How does Prisma ORM work and what are its tradeoffs vs raw SQL?
44. How do you model a document/slide generation pipeline in PostgreSQL?
45. How do you write efficient Prisma queries and avoid N+1 problems?
46. How do you handle schema migrations safely with Prisma?
47. What is a sync engine and how would you design one for BI data?
48. How do you sync data incrementally and detect changes (deltas, cursors, watermarks)?
49. How do you handle conflicts and idempotency in a sync pipeline?
50. What is Temporal and how does it differ from a simple job queue?
51. Explain Temporal workflows, activities, retries, and durability.
52. How do you make a long-running sync workflow resumable after failure?
53. How do you handle rate limits and backpressure when pulling from BI tools?
54. How do you ensure exactly-once/at-least-once semantics in async workflows?
55. How do you store and version generated documents and their templates?
56. How do you optimize data synchronization with better protocols (batching, parallelism)?

## Integrations — BI Tools & Content Platforms (57-68)
57. How would you design a pluggable integration framework for many providers?
58. How do you integrate with Tableau, Looker, or Metabase APIs (auth, pagination, rate limits)?
59. How do you handle OAuth flows and token refresh per customer?
60. How do you abstract differences between BI tools behind one interface?
61. How do you integrate with Google Slides, PowerPoint, and Notion APIs?
62. How do you handle file formats and rendering for slides/documents?
63. How do you map arbitrary BI data into presentation templates?
64. How do you handle webhooks and change notifications from external platforms?
65. How do you make integrations resilient when a third-party API changes or breaks?
66. How do you test integrations without hitting live third-party systems?
67. How do you handle multi-tenancy and data isolation across integrations?
68. How do you debug a failed integration end-to-end?

## Generative AI Layer (69-78)
69. How would you add AI-generated insights to a reporting product?
70. LangChain vs direct OpenAI/Gemini API—when do you use each?
71. How do you manage prompts, versions, and evaluation in production?
72. How do you control cost and latency of LLM calls at scale?
73. How do you handle hallucinations and validate AI output before showing it?
74. What is Langfuse and how does it help observability of LLM features?
75. How do you stream LLM output to the frontend?
76. How do you handle PII and data privacy when sending data to LLM providers?
77. How do you design fallbacks across multiple model providers (OpenAI, Gemini)?
78. How would you A/B test an AI feature and measure its impact?

## Cloud, DevOps & Observability (79-90)
79. How do you containerize a TypeScript/Node.js app for production?
80. Explain Kubernetes objects and how you'd run this app on K8s.
81. How does Argo CD enable zero-downtime deploys and rollbacks?
82. How do you design CI/CD for a full-stack TypeScript monorepo?
83. What quality gates belong in the pipeline (lint, types, tests, scans)?
84. How do you manage secrets and config in K8s/AWS?
85. How do you autoscale and control cost on AWS K8s?
86. What is SigNoz and how do you use logs/traces for debugging?
87. How does Sentry help you triage production issues faster?
88. How do you use PostHog product analytics to drive decisions?
89. How do you alert on real regressions without noisy false positives?
90. How do you scale a sync engine as customer data grows?

## Debugging, Product & Culture (91-100)
91. Walk through debugging a broken slide update across the whole stack.
92. A deploy regressed production—how do you detect and roll back quickly?
93. How do you collaborate with PMs and designers to ship features fast?
94. How do you balance shipping fast with maintaining code quality?
95. Describe a time you optimized a slow system and the measurable result.
96. How do you approach an ambiguous feature with no clear spec?
97. How do you keep learning new tools (Temporal, Argo, LangChain) quickly?
98. How do you work effectively in a fully remote, autonomous team?
99. What would you build or improve at Rollstack in your first 90 days?
100. Why Rollstack, why a TypeScript full-stack role, and why now?
