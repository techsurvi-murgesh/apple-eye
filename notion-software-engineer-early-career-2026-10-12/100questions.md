# 100 Interview Questions — Software Engineer, Early Career (Notion) — 2026-10-12

Target stack: React, TypeScript, Node.js, PostgreSQL, Elasticsearch; data structures, algorithms and distributed systems fundamentals; product/frontend engineering, experiments and activation, AI-assisted development (Cursor, Claude Code), platform reliability. This is an early-career role — expect fundamentals, product judgement, and how you work rather than deep infrastructure specialisation.

## Data Structures & Algorithms (1-20)

1. What's the difference between an array and a linked list, and when would you pick each?
2. Explain hash maps: how they work, expected time complexity, and how collisions are handled.
3. Explain binary search. When is it applicable, and what is its complexity?
4. Explain merge sort and quicksort. When would you choose one over the other?
5. What's the difference between a stack and a queue? Give real product examples of each.
6. Explain breadth-first search and depth-first search. When do you use each?
7. How do you detect a cycle in a linked list and in a directed graph?
8. Explain a heap. How would you use one for "top K" problems?
9. What's dynamic programming? Give two problems where it applies.
10. Explain recursion and when converting to iteration matters in a product codebase.
11. What's the time complexity of common JavaScript array operations, and why does it matter?
12. Explain Big-O notation and how you'd reason about it in a code review.
13. How do you choose between sorting algorithms for a few thousand vs millions of records?
14. Explain graph representations (adjacency list vs matrix) and their trade-offs.
15. Explain two-pointer and sliding-window techniques with an example.
16. How do you detect and remove duplicates efficiently in a large collection?
17. Explain bit manipulation basics — when is it useful in systems code?
18. Explain memoization and how it differs from caching at the database layer.
19. How do you handle integer overflow, and why does it matter for things like money?
20. Explain how you'd test an algorithm for correctness beyond the happy path.

## Frontend, React & TypeScript (21-38)

21. Explain how React renders: what happens between `setState` and the DOM updating.
22. What is reconciliation, and how does React decide what to re-render?
23. Explain the difference between controlled and uncontrolled components.
24. When would you use `useMemo` and `useCallback`? When are they a pessimisation?
25. Explain `useEffect` and its dependency array. What are the common bugs?
26. Explain React context and when you'd reach for it versus a state library.
27. What are the trade-offs between client-side routing and server-side rendering?
28. Explain hydration and the common SSR pitfalls.
29. How do you prevent memory leaks from event listeners and subscriptions in React?
30. Explain React's reconciliation keys and what goes wrong with array indices as keys.
31. How would you profile and fix a slow render or a janky interaction?
32. Explain code-splitting, lazy loading, and how they affect perceived performance.
33. How do you approach accessibility in a component library? What do you actually test?
34. Explain TypeScript's type system: unions, generics, and narrowing.
35. When do you reach for `unknown` over `any`, and how do you type API boundaries?
36. Explain type inference and where explicit annotations help readability.
37. How do you model a complex domain (e.g. a database/block model) in TypeScript types?
38. What state management approach would you choose for a large collaborative editor, and why?

## Backend, APIs & Data (39-52)

39. Design a REST API for creating, updating, and sharing a document. What endpoints and status codes?
40. Explain pagination strategies (offset vs cursor) and when cursor wins.
41. How do you version an API without breaking existing clients?
42. Explain authentication vs authorisation, and how you'd implement session auth.
43. How do you design idempotent endpoints and prevent duplicate writes?
44. Explain transactions in PostgreSQL: ACID, isolation levels, and common anomalies.
45. How do you design and index a PostgreSQL schema for a documents table?
46. Explain N+1 queries and how you eliminate them.
47. How do you use indexes effectively? What is a covering index?
48. Explain connection pooling and why it matters for a Node.js service.
49. How do you handle schema migrations on a live table with millions of rows?
50. When do you denormalise, and what are the consistency costs?
51. How do you design for multi-tenancy, and what isolation do you need?
52. How would you search across documents? Explain inverted indexes and Elasticsearch basics.

## Distributed Systems & Scalability (53-68)

53. Explain the CAP theorem and what it means in practice for a product team.
54. Explain horizontal vs vertical scaling, and when each is appropriate.
55. What is a load balancer and what strategies does it use?
56. Explain caching layers (CDN, in-process, Redis) and how you avoid stale data.
57. Explain eventual consistency and where you can tolerate it in a product.
58. How do you design a rate limiter, and why do you need one?
59. Explain retries, exponential backoff with jitter, and idempotency together.
60. What are queues and how do you use them to smooth traffic spikes?
61. Explain how you would debug a latency spike in a service with many dependencies.
62. How do you measure and improve p50/p95/p99 latency?
63. Explain circuit breakers and bulkheads.
64. How do you handle a dependency being down without taking your service with it?
65. Explain how you'd think about database connection limits under sudden traffic growth.
66. What are the trade-offs of serverless (Lambda) versus always-on services?
67. Explain how you would scale a read-heavy workload versus a write-heavy one.
68. How do you design for observability: logs, metrics, traces, and what each is for?

## System Design (69-76)

69. Design a URL shortener with high read volume.
70. Design the "recently viewed" feature for a workspace app.
71. Design a notification system that handles email, in-app, and push.
72. Design a collaborative document with real-time editing.
73. Design a search experience with typo tolerance and ranking.
74. Design a rate-limited public API for a third-party integration.
75. Design an experiment/feature-flag system that supports gradual rollout.
76. Design a file/image upload pipeline with resizing and CDN delivery.

## Product, Growth & Experimentation (77-86)

77. How do you define activation for a product? What would you instrument?
78. Explain the difference between activation, engagement, retention, and revenue metrics.
79. How do you design an A/B test? What are the statistical pitfalls?
80. How do you avoid peeking at experiment results and p-hacking?
81. How do you run a gradual rollout and decide when to halt it?
82. How do you prioritise when many features compete for the same engineers?
83. How do you decide what to optimise first when a product feels slow?
84. How do you gather and use qualitative customer feedback alongside metrics?
85. How do you write a feature spec that engineers can act on?
86. Give an example of a feature you would remove, and how you'd justify it.

## AI-Assisted Development (87-93)

87. How do you use AI tools like Cursor or Claude Code day to day, concretely?
88. How do you review AI-generated code critically rather than accepting it?
89. What kinds of tasks are these tools good at, and where do you not trust them?
90. How do you keep context manageable in an AI-assisted workflow?
91. How do you make AI-generated work understandable to your teammates on review?
92. How would you use AI to understand an unfamiliar codebase quickly?
93. How do you avoid over-relying on AI and keep your own fundamentals sharp?

## Collaboration, Craft & Communication (94-100)

94. Describe a piece of work you owned end to end. What did you decide yourself?
95. How do you approach a problem you don't fully understand yet?
96. How do you decompose an ambiguous problem into shippable pieces?
97. Describe a technical disagreement. How did you resolve it?
98. How do you give and receive code review feedback?
99. How do you communicate technical trade-offs to non-technical partners like design?
100. Describe a time you shipped something imperfect. How did you handle the risk?

### Behavioural & Situational

- Tell us about something you built that users actually used. What did you learn?
- Describe a production bug you caused or caught. What did you change afterwards?
- How do you handle a project where requirements change halfway through?
- Describe a time you had to learn something quickly to unblock a deadline.
- How do you ask for help without appearing blocked?
- Tell us about a technical decision you made that you later reversed. Why?
- How do you stay current with new tools without chasing trends?
- Describe a time you improved something for your teammates rather than a user.