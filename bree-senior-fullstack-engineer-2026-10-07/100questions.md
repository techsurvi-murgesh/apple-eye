# 100 Interview Questions — Senior Fullstack Engineer, Bree

## Fullstack & TypeScript Fundamentals (1-14)
1. Walk through how you own a feature end-to-end, from discovery to production follow-up.
2. What makes TypeScript code "expert-level" and how do you enforce types across a stack?
3. How do you share types between a TypeScript frontend and backend safely?
4. How do you structure a fullstack TypeScript monorepo?
5. How do you approach technical design docs and get buy-in from Product/Design?
6. How do you decide service boundaries and data ownership?
7. When do you refactor versus extend an existing system?
8. How do you modernize a legacy part of a platform without breaking customers?
9. How do you balance speed of shipping with long-term maintainability?
10. How do you mentor engineers through design and code review?
11. How do you make pragmatic engineering decisions under regulatory constraints?
12. How do you handle ambiguity when Product doesn't define every requirement?
13. How do you communicate technical tradeoffs to non-engineering stakeholders?
14. How do you take ownership of outcomes, not just code?

## Backend — Node.js & Serverless (15-30)
15. How do you design a serverless API with Lambda and API Gateway?
16. Explain cold starts and how you mitigate them for latency-sensitive endpoints.
17. How do you design event-driven systems with SQS/SNS?
18. What are the tradeoffs of serverless vs containers for this kind of product?
19. How do you make Lambda functions idempotent for payment events?
20. How do you handle retries, dead-letter queues, and poison messages in SQS?
21. How do you bound concurrency to protect downstream systems?
22. How do you design REST vs GraphQL APIs for a fintech product?
23. How do you version APIs without breaking mobile/web clients?
24. How do you design authentication and authorization for regulated products?
25. How do you handle partial failures across multiple service calls?
26. How do you manage stateful workflows in an event-driven architecture?
27. How do you handle timeouts and cancellation across Lambda invocations?
28. How do you keep Node.js Lambda functions fast and small?
29. How do you handle background jobs and scheduled tasks serverlessly?
30. How do you debug a failing Lambda in production?

## Data & Database Design (31-44)
31. How do you model eligibility rules and product/pricing rules in a database?
32. How do you design a schema for loans, advances, repayments, and transactions?
33. Why is monetary precision important and how do you store money correctly?
34. Explain transactions, isolation levels, and locking for money movement.
35. How do you avoid double-charging or double-disbursing on retries?
36. How do you design idempotent writes with idempotency keys?
37. How do you handle schema migrations with zero downtime?
38. How do you model audit trails for regulated financial systems?
39. How do you handle multi-region data and regulatory data residency?
40. How do you ensure consistency across event-driven services (outbox/saga)?
41. How do you scale a relational database as volume grows?
42. How do you handle data retention and PII/PCI concerns?
43. How do you detect and fix N+1 queries?
44. How do you choose between SQL and NoSQL for different Bree data?

## Frontend & Full-Stack Product (45-56)
45. How do you build a React experience consuming a serverless API?
46. How do you manage server state vs client state in a React app?
47. How do you keep frontend and backend contracts in sync?
48. How do you handle auth/session management securely in a web app?
49. How do you build internal tools for CX/operations teams?
50. How do you handle loading, error, and edge cases in financial UIs?
51. How do you optimize performance for data-heavy screens?
52. How do you approach accessibility and responsive design pragmatically?
53. How do you do optimistic UI for actions with money implications?
54. How do you debug a bug that spans UI, API, and database?
55. When would you reuse vs extract a shared component across products?
56. How do you work with Design to iterate quickly without rework?

## Payments & Fintech Domain (57-68)
57. How does a cash-advance / short-term credit product work end to end?
58. How do you integrate with a payment provider safely?
59. What are idempotency and reconciliation in payments, and why do they matter?
60. How do you handle failed payments, chargebacks, and retries?
61. How do you design eligibility and underwriting rules as changeable configuration?
62. How do you prevent fraud and abuse in a consumer lending product?
63. How do you handle regulatory compliance (KYC/AML) in engineering?
64. How do you design auditability and traceability for every money movement?
65. How do you reason about money correctness under concurrency?
66. How do you test payment flows without moving real money?
67. How do you roll out a financial feature safely (guarded, reversible)?
68. How do you monitor financial health metrics and anomalies?

## AI-Native Development (69-78)
69. How do you use Claude Code/Cursor/Codex across your whole workflow?
70. How do you validate and own AI-generated code before it ships?
71. How do you use AI for debugging and root-causing production issues?
72. How do you use AI to write tests and improve coverage?
73. Where do AI coding tools fail in a complex codebase, and how do you catch it?
74. How do you keep AI-assisted changes consistent with team standards?
75. How do you safely give an AI tool context without leaking secrets/PII?
76. How do you measure the real velocity impact of AI tooling?
77. How do you onboard an AI-native workflow into a team's reviews and CI?
78. How do you apply judgement when AI suggests a quick fix that isn't correct?

## AWS, DevOps & Testing (79-92)
79. How do you design AWS infrastructure for a serverless Node.js backend?
80. How do you manage IaC with Terraform or Pulumi?
81. How do you build CI/CD for a fullstack TypeScript app?
82. What quality gates belong in the pipeline?
83. How do you wire Jest tests into CI pragmatically?
84. What should be unit vs integration vs end-to-end tests?
85. How do you do safe deploys and fast rollbacks?
86. How do you instrument what you ship (logs, metrics, traces)?
87. How do you alert on regressions without noisy false positives?
88. How do you control cost on AWS serverless?
89. How do you manage secrets and config across environments?
90. How do you handle a production incident affecting customers' access to money?
91. How do you set SLOs for critical financial flows?
92. How do you test event-driven/serverless systems locally?

## Senior Ownership, Modernization & Culture (93-100)
93. Describe a system you modernized and the outcomes.
94. How do you hold the line on stability without slowing releases?
95. How do you mentor engineers while staying hands-on?
96. How do you work across Product, Design, CX, and Ops to shape solutions?
97. How do you prioritize refactoring against new feature work?
98. Tell us about a time you took architectural ownership of a product area.
99. How do you keep product judgement sharp when code quality pressure rises?
100. Why Bree, why a senior fullstack role, and what would you own in your first 90 days?
