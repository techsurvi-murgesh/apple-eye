# 100 Interview Questions — Senior Software Engineer (Python Full Stack)

Target profile: Python (FastAPI) backend, React.js + TypeScript frontend, REST APIs and microservices on AWS (EC2, SNS, EMR, Bedrock), AI tools, Docker, CI/CD, PostgreSQL/MySQL/MongoDB, Agile delivery.

## Python Fundamentals (1–15)

1. What is the difference between mutable and immutable types in Python, and why does it matter for function arguments and default values?
2. Compare list, tuple, set, and dictionary. When would you choose each?
3. Explain shallow copy versus deep copy, with a case where the distinction caused a bug.
4. How do decorators work in Python? Give a practical use case such as authentication, logging, or retries.
5. What are generators and `yield`, and how do they help with memory when processing large datasets?
6. How does a context manager work, and when would you write your own with `__enter__` and `__exit__`?
7. What is the GIL, and how does it affect CPU-bound versus I/O-bound workloads?
8. Compare asyncio, threading, and multiprocessing. When do you use each?
9. Explain `*args` and `**kwargs`, including how they interact with keyword-only arguments.
10. How do you design exception hierarchies for a service, and when should an exception propagate to the API layer?
11. How do type hints, mypy, and Pydantic improve correctness in a large Python codebase?
12. Compare dataclasses and Pydantic models for request payloads, domain objects, and configuration.
13. What are the readability and performance trade-offs of list and dict comprehensions?
14. How do you manage Python dependencies and virtual environments across development, CI, and production?
15. How does Python manage memory and garbage collection, and what patterns cause memory leaks in long-running services?

## FastAPI, Django, and Flask (16–30)

16. Why would you choose FastAPI over Django or Flask for a new API service, and what do you give up?
17. How does Pydantic validation work in FastAPI for request bodies, query parameters, and response models?
18. Explain FastAPI dependency injection and give a real use case for a shared dependency.
19. What happens when a blocking call is made inside an async FastAPI endpoint, and how do you fix it?
20. How do you add middleware in FastAPI, and what belongs in middleware versus a dependency?
21. How do you implement JWT or OAuth2 authentication and role-based authorization in FastAPI?
22. How do exception handlers let you return consistent error responses across a FastAPI application?
23. Compare FastAPI background tasks with a Celery or queue-based worker for long-running work.
24. How do you use SQLAlchemy async sessions safely, including session lifecycle and connection pooling?
25. How does Alembic manage schema migrations, and how do you handle a destructive migration safely?
26. Compare the Django ORM with SQLAlchemy for complex queries and performance tuning.
27. How do Django middleware and signals work, and what problems can overusing signals create?
28. What is the Flask application factory pattern, and why is it useful for testing and configuration?
29. Explain WSGI versus ASGI and how that choice affects concurrency and deployment.
30. How do you version a public API and keep OpenAPI documentation accurate as the service evolves?

## REST APIs and Microservices (31–42)

31. What makes an API RESTful, and which REST constraints are most often ignored in practice?
32. Compare POST, PUT, and PATCH, including idempotency and partial updates.
33. Which HTTP status codes do you return for validation errors, auth failures, conflicts, and rate limits?
34. How do you design pagination, filtering, and sorting for a large collection endpoint?
35. What is an idempotency key, and how do you implement one for a payment or retried request?
36. How do you decide the boundary between two microservices rather than splitting a monolith arbitrarily?
37. How do services authenticate to each other, and how do you avoid long-lived shared secrets?
38. How do retries, exponential backoff, jitter, timeouts, and circuit breakers work together?
39. How do you handle a workflow that spans multiple services without a distributed transaction?
40. What problems do an API gateway and service discovery solve, and what new problems do they introduce?
41. How do you trace one request across multiple services in production?
42. How do you evolve an API without breaking existing consumers?

## React, TypeScript, and Frontend (43–57)

43. How does React reconciliation work, and why is the virtual DOM not automatically faster than direct DOM updates?
44. What are the rules of hooks, and what bugs appear when they are violated?
45. Compare `useEffect` and `useLayoutEffect` with concrete examples.
46. When do `useMemo` and `useCallback` help, and when are they unnecessary?
47. Compare local state, Context, and Redux Toolkit for a growing application.
48. What is the difference between controlled and uncontrolled components, and when is each appropriate?
49. How does React Query or a similar library change how you manage server state, caching, and refetching?
50. How do you use code splitting and lazy loading to improve initial page load?
51. What do error boundaries catch, and what do they not catch?
52. Which accessibility practices do you apply to forms, modals, and keyboard navigation?
53. How do you build a responsive layout with Flexbox, Grid, media queries, and fluid sizing?
54. Compare TypeScript interfaces and type aliases, and explain when you prefer one.
55. How do generics improve a reusable React component or API client in TypeScript?
56. Why is `unknown` safer than `any`, and how does strict mode change your code?
57. How do you prevent XSS and CSRF in a React application that talks to a Python API?

## AWS (58–71)

58. How do you choose an EC2 instance family and size, and what does placement across Availability Zones give you?
59. How do Auto Scaling groups and load balancers work together for a highly available service?
60. Which S3 storage classes and security controls do you use for application assets and backups?
61. Compare IAM users, roles, and policies. How do you apply least privilege in practice?
62. How do you design public and private subnets, route tables, NAT, and security groups in a VPC?
63. Compare RDS Multi-AZ with read replicas, and explain when each is needed.
64. Compare SNS and SQS, and give a use case for each.
65. How does the SNS fan-out pattern work with multiple subscribers such as SQS queues and Lambda functions?
66. What is Amazon EMR, and when is it a better choice than a single application server for data processing?
67. How do you tune an EMR job for cost and performance, including instance selection and partitioning?
68. What is Amazon Bedrock, and how would you call a foundation model from a FastAPI service?
69. How do Bedrock guardrails, IAM permissions, and data-handling settings affect application security?
70. How do CloudWatch metrics, logs, alarms, and CloudTrail support production debugging and audit?
71. How do you identify and reduce AWS cost without hurting reliability?

## AI Tools and LLM Integration (72–78)

72. How do you use AI coding tools across design, implementation, testing, debugging, and documentation?
73. What is your process for reviewing AI-generated code before it reaches a pull request?
74. How do you write prompts that produce code matching an existing codebase's conventions and constraints?
75. What are the main risks of AI-generated code, including hallucinated APIs, leaked secrets, and license issues?
76. How would you integrate an LLM through Amazon Bedrock into a FastAPI endpoint with timeouts and fallbacks?
77. How do structured outputs and tool calling make LLM responses more reliable for application logic?
78. How do you evaluate an LLM feature and prevent a prompt change from silently degrading quality?

## Databases (79–87)

79. Compare PostgreSQL and MySQL for a new transactional web application.
80. How does a B-tree index work, and which queries does it accelerate or fail to accelerate?
81. How do you read an `EXPLAIN ANALYZE` plan and use it to fix a slow query?
82. Explain transaction isolation levels and the anomalies each one prevents.
83. What is the N+1 query problem, and how do you detect and fix it?
84. How do you model documents in MongoDB for read-heavy versus write-heavy access patterns?
85. How do compound, unique, and text indexes work in MongoDB, and how do you verify index usage?
86. When do you choose a relational database over a document database, and vice versa?
87. How do you size and configure connection pooling for an API service under load?

## Docker, CI/CD, and Git (88–94)

88. What is the difference between a Docker image and a container, and what makes a build reproducible?
89. How do multi-stage Docker builds reduce image size and attack surface?
90. How does Docker Compose networking work when several services need to talk to each other locally?
91. How do you design a CI/CD pipeline from commit to production, including tests and rollback?
92. How do you store CI/CD secrets safely, and how does OIDC federation remove static AWS keys?
93. Compare blue/green and canary deployments, including rollback behavior and cost.
94. How do you keep a Git history clean, and how do you resolve a complex merge conflict safely?

## OOP, Testing, Agile, and Behavioral (95–100)

95. Explain the SOLID principles and give an example of applying or violating one in Python or TypeScript.
96. How do you structure unit and integration tests with pytest, including fixtures and test isolation?
97. How do you mock an external HTTP service without making tests slow or flaky?
98. What do you look for in a code review, and how do you give feedback that improves the code without demoralizing the author?
99. How do sprint planning, estimation, daily standups, and retrospectives work in a healthy Agile team?
100. Walk through a production issue you diagnosed across frontend and backend components: how you found the cause, fixed it, and communicated with stakeholders.
