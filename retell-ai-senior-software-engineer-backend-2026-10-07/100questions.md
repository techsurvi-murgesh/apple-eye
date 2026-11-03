# 100 Interview Questions — Senior Software Engineer, Backend (Retell AI)

## Real-Time Audio & Voice AI (1-14)
1. How does real-time audio streaming work end-to-end in a voice AI system (capture → transport → STT → LLM → TTS → playback)?
2. What transport do you use for low-latency audio (WebSockets, WebRTC, SIP/RTP) and why?
3. How do you keep end-to-end voice latency low enough for natural conversation?
4. How do you handle interruption/barge-in when a caller speaks over the agent?
5. How would you stream partial transcripts and tokens through the pipeline?
6. How do you manage jitter, buffering, and packet loss in audio transport?
7. How do you handle concurrency for thousands of simultaneous calls?
8. Where would you put a message queue or event bus in a voice pipeline, and why?
9. How do you make the LLM/prompt orchestration layer reliable under load?
10. How do you design fallbacks if STT, LLM, or TTS providers degrade mid-call?
11. How do you version and A/B test prompts and voice agent behavior?
12. How do you store and replay call audio/transcripts for debugging and QA?
13. What are the privacy/compliance considerations for recording calls (PII, consent, retention)?
14. How would you build an observability dashboard for live calls and call quality?

## Backend & APIs — Node.js / TypeScript (15-30)
15. Why is Node.js/TypeScript a good fit for real-time voice backends, and where does it struggle?
16. How does the Node.js event loop work, and how do you avoid blocking it?
17. How do you build a scalable REST and WebSocket API layer in Node.js?
18. How do you design APIs for customer onboarding and self-serve agent configuration?
19. REST vs WebSockets vs gRPC for different parts of a voice platform?
20. How do you version public APIs without breaking customers?
21. How do you design idempotent endpoints for call creation and webhooks?
22. How do you handle authentication, API keys, and tenant isolation?
23. How do you validate input and prevent abuse on telephony-facing endpoints?
24. How do you handle rate limiting and backpressure per customer?
25. How do you structure a TypeScript codebase for maintainability and speed (types, modules, DI)?
26. How do you manage async error handling and avoid unhandled promise rejections?
27. How do you design webhooks to carrier/CRM systems reliably?
28. How do you write prompt orchestration as maintainable code rather than spaghetti?
29. How do you build testing frameworks and contract tests for API behavior?
30. When would you drop to Python for a backend component, and how would you integrate it?

## Scalable / High-Performance Systems & Concurrency (31-44)
31. How do you design a backend to handle millions of calls per day?
32. Explain concurrency vs parallelism with a voice/backend example.
33. How do you avoid race conditions when multiple workers touch the same call state?
34. How do you bound concurrency to protect downstream providers?
35. How do you implement worker pools, queues, and backpressure?
36. How do you handle connection pooling for databases and HTTP clients at scale?
37. How do you keep p99 latency predictable under bursty load?
38. How do you do graceful shutdown without dropping in-flight calls?
39. How do you design caching (in-process vs Redis) for hot call metadata?
40. How do you handle memory growth / leaks in a long-running Node.js service?
41. How do you profile a slow endpoint and find the bottleneck?
42. How would you scale a stateful WebSocket service horizontally?
43. How do you balance latency vs correctness in a real-time system?
44. How do you reason about timeouts, retries, and cancellation end-to-end?

## Data & Storage — PostgreSQL / DynamoDB (45-58)
45. When do you choose PostgreSQL vs DynamoDB for a backend workload?
46. How do you model call, agent, and transcript data in PostgreSQL?
47. How do you model high-volume, time-series-like data in DynamoDB (partition/sort keys)?
48. How do you avoid hot partitions in DynamoDB?
49. How do you design GSIs/LSIs for common access patterns?
50. How do you handle DynamoDB consistency (eventual vs strong) in a real-time flow?
51. How do you manage transactions across multiple items/tables?
52. How do you tune PostgreSQL indexes and query plans for scale?
53. How do you handle schema migrations with zero downtime?
54. How do you store large blobs (audio) vs metadata — S3 + pointer pattern?
55. How do you cache and paginate large transcript datasets?
56. How do you back up, restore, and retain data per compliance rules?
57. How do you ensure data isolation between enterprise tenants?
58. How do you handle idempotent writes and dedupe in a distributed store?

## Distributed Systems & System Design (59-70)
59. Design the backend for a real-time AI voice agent platform end-to-end.
60. How do you make a voice pipeline highly available across regions?
61. Explain CAP and how it shapes your storage and call-state choices.
62. How do you handle partial failures and circuit breaking across providers?
63. How do you design an event-driven architecture for call lifecycle events?
64. How do you keep call state consistent across services (saga/outbox)?
65. How do you do service discovery and load balancing between microservices?
66. How do you correlate a single call across logs, metrics, and traces?
67. How do you design telephony provider failover (carrier A → carrier B)?
68. How do you set SLOs for call setup time and answer rate?
69. How do you scale from a few hundred to millions of concurrent calls?
70. How would you lead a complex backend project from architecture to production?

## Cloud, DevOps & Observability (71-84)
71. How do you design AWS infrastructure for a real-time backend?
72. How do you choose between EC2, ECS, EKS, Lambda, and Fargate for this workload?
73. How do you containerize and deploy a Node.js/TypeScript backend?
74. How do you write a secure, minimal Dockerfile?
75. Explain Kubernetes objects and how you'd run a WebSocket service on K8s.
76. How do you configure autoscaling for latency-sensitive services?
77. How do you do zero-downtime deploys and safe rollbacks?
78. How do you manage secrets and config across environments?
79. How do you build CI/CD workflows for fast, safe delivery?
80. What quality gates belong in the pipeline (lint, types, tests, scan)?
81. How do you monitor a real-time system (metrics, logs, traces, alerts)?
82. How do you alert on call quality without noisy false positives?
83. How do you control cloud cost while scaling globally?
84. How do you debug "service works locally but fails in production"?

## Telephony Integrations & Developer Tooling (85-92)
85. How do SIP, PSTN, and carriers fit into an AI voice platform?
86. How do you integrate and abstract multiple telephony providers behind one API?
87. How do you handle DTMF, call transfers, and hold/mute in an AI agent?
88. How do you build developer tooling and SDKs for quick customer onboarding?
89. How do you support testing of a voice agent before it goes live (simulation, sandbox numbers)?
90. How do you handle webhooks, retries, and ordering for call events?
91. How do you build an observability dashboard customers can trust?
92. How would you surface and act on customer feedback as product improvements?

## Debugging, Ownership & Startup Behavioral (93-100)
93. Walk through debugging a dropped or poor-quality live call end-to-end.
94. A provider outage is affecting calls — how do you triage and mitigate?
95. Describe a time you took founder-level ownership of a critical system.
96. How do you operate effectively in ambiguity and fast-changing requirements?
97. How do you balance shipping fast with correctness in a high-velocity startup?
98. How do you collaborate with product, design, and customer-facing teams?
99. How do you ramp up on an unfamiliar large codebase quickly?
100. Why Retell AI, why a senior backend role, and what would you ship in your first 90 days?
