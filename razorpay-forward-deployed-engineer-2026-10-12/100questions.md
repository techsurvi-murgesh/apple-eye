# 100 Interview Questions — Forward Deployed Engineer, Agent Studio (Razorpay) — 2026-10-12

Target profile: forward-deployed / applied-AI engineer in fintech. Python or TypeScript production engineering, customer-facing technical ownership, LLM agents (tool calling, RAG, evals, MCP), APIs/webhooks/auth, data pipelines, production debugging, outcome measurement, and writing crisp specs under ambiguity.

## LLM & Agent Engineering (1-22)

1. How do you write effective system prompts? What makes one robust and one brittle?
2. Explain tool / function calling end to end. How does the model know what tools exist?
3. How do you design tool schemas so the model calls them correctly?
4. When should an agent act autonomously, when should it only recommend, and when must a human approve?
5. Explain RAG. How do you decide what to retrieve, chunk, and re-rank?
6. How do you handle a RAG system that returns confidently wrong answers?
7. Explain retrieval vs generation trade-offs, and when you don't need RAG at all.
8. What is an MCP server and what problem does it solve for tool integration?
9. How do you design an eval harness for an agent? What do you measure?
10. Explain offline evals vs online/production monitoring. When do you need each?
11. How do you build a regression suite for prompt changes?
12. How do you debug a failure that is non-deterministic? What do you log?
13. How do you control cost per run? Where does cost actually come from?
14. Explain latency in agentic systems. How do you keep it acceptable?
15. How do you handle context-window limits in a long-running agent loop?
16. What is a multi-agent workflow, and when is it justified over a single agent?
17. How do you guard against prompt injection and unsafe tool execution?
18. Explain structured output / JSON mode and how you validate it reliably.
19. How do you version prompts, tools, and eval sets together?
20. How do you decide model choice per task (capability vs cost vs latency)?
21. Explain agent memory and state management across turns and sessions.
22. How would you take an agent from impressive demo to reliable production?

## Customer Discovery & Solution Consulting (23-38)

23. How do you run a discovery call with a customer who doesn't know what they need?
24. How do you uncover the real constraint behind a vague ask?
25. The business owner, ops lead, and dashboard disagree. How do you reconcile them?
26. How do you tell the difference between "what they asked for" and "what they need"?
27. How do you handle a customer who insists on a solution you think is wrong?
28. How do you say no to a customer's request while keeping the relationship?
29. How do you qualify a lead — when is this not a good fit to build?
30. How do you run a technical workshop with a mixed audience?
31. How do you present an architecture to non-technical stakeholders?
32. How do you explain cost and latency trade-offs to a business owner?
33. How do you handle scope creep during a customer engagement?
34. How do you decide what to prototype first when you have limited time?
35. How do you write a spec clear enough that product, engineering, legal, and the customer all agree?
36. What goes in a good agent spec? (success metric, data sources, tool calls, guardrails, human-in-the-loop, rollout plan)
37. How do you write crisp follow-ups and decision records?
38. How do you build trust quickly with a new stakeholder?

## APIs, Webhooks & Integrations (39-52)

39. Design a webhook system: payloads, signatures, retries, ordering, and deduplication.
40. How do you make webhooks idempotent on the receiver side?
41. Explain OAuth 2.0 flows. Which do you use for server-to-server vs user-facing?
42. How do you store and rotate API keys and credentials safely?
43. How do you handle third-party API rate limits in production?
44. Explain retries with exponential backoff and jitter. Why is jitter necessary?
45. How do you design a connector to a third-party system with no test environment?
46. How do you debug an integration that worked yesterday and fails today?
47. Explain circuit breakers, bulkheads, and how they protect your service.
48. How do you handle partial failure across multiple downstream systems?
49. How do you version an API without breaking existing clients?
50. Explain pagination strategies and when cursor-based beats offset.
51. How do you design an internal API that other teams will build against?
52. How do you handle schema drift in a third-party integration?

## Data & Pipelines (53-62)

53. Design a reconciliation pipeline between two systems of record.
54. How do you make a data pipeline idempotent and replayable?
55. Explain exactly-once vs at-least-once delivery and what you actually need.
56. How do you handle late-arriving or out-of-order data?
57. How do you design for data quality: validation, dedup, and quarantine?
58. Explain batch vs streaming and when each is right.
59. How do you track lineage — where did this number come from?
60. How do you build dashboards that people trust?
61. How do you debug a metric that disagrees with the source system?
62. How do you design schema migrations safely on live tables?

## Fintech Domain (63-74)

63. Explain the payments lifecycle: authorize, capture, settle, refund, and chargeback.
64. What causes an RTO (request to originate) decline and how do you reduce it?
65. How do checkout recovery and abandoned-payment recovery work?
66. How does dispute/chargeback management work, and what drives dispute win rate?
67. Explain idempotency keys in payment APIs and why they are mandatory.
68. How do you design for settlement delays and cashflow leakage visibility?
69. What are the compliance and audit constraints on storing payment data (PCI DSS, tokenisation)?
70. How do you handle sensitive financial data safely in an LLM agent pipeline?
71. Explain subscriptions (SIP) and failed-payment recovery.
72. How do you detect and prevent duplicate payouts?
73. What is fraud detection and where does an agent fit vs a rules engine?
74. How do you reconcile settlements against bank statements?

## Production Engineering & Debugging (75-86)

75. How do you debug a production issue with no stack trace and no logs?
76. Explain your incident process: detection, triage, mitigation, RCA.
77. How do you read a flame graph and identify a bottleneck?
78. How do you tune a slow SQL query?
79. How do you handle memory growth in a long-running service?
80. How do you roll back a bad deploy quickly?
81. How do you design feature flags and gradual rollout with safe kill switches?
82. How do you make a deployment observable before the rollout?
83. How do you manage secrets and config across environments?
84. How do you debug a network problem between two services?
85. How do you decide what to optimise when a service is slow?
86. How do you reduce MTTR for a customer-facing integration?

## Measurement, Ambiguity & Ownership (87-100)

87. How do you define the success metric before you build an agent?
88. How do you know an agent actually moved the metric rather than just looking good?
89. The agent didn't move the metric. How do you diagnose — and when do you kill it?
90. How do you design a rollout plan with quality gates?
91. How do you distinguish correlation from causation in a customer outcome?
92. How do you turn repeated field patterns into reusable platform capabilities?
93. You have one week and an ambiguous problem. How do you start?
94. How do you decompose a problem where the requirements are unknown?
95. How do you make a technical trade-off decision without complete information?
96. How do you handle a project that is failing and needs to be stopped?
97. How do you communicate bad news to a customer early?
98. How do you prioritise when three customers all need something urgent?
99. How do you give status updates that are genuinely useful?
100. Describe a time you owned a problem end to end that was not in your original remit.

### Behavioural & Situational

- Tell us about a customer problem you diagnosed that the customer had not correctly described.
- Describe a time you had to kill something you had built. How did you justify it?
- Tell us about a production incident you owned. What did you change afterwards?
- Describe a time you turned a one-off solution into a reusable capability.
- How do you handle a merchant who escalates angrily?
- Tell us about a technical decision you made under uncertainty.
- How do you balance shipping fast for a customer against platform quality?