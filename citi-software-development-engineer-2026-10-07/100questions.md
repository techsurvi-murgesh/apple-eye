# 100 Interview Questions — Software Development Engineer, Python & Java (Citi C10) — 2026-10-07

Target stack: Python 3.x (FastAPI/Flask/Django, Pandas/NumPy, asyncio), Java 11/17+ (Core Java, Spring Boot/MVC/Data/Security), REST/OpenAPI, Kafka/RabbitMQ/JMS, PostgreSQL/Oracle/MySQL, SQLAlchemy/Hibernate/JPA, MongoDB/Redis/Elasticsearch, Docker, Kubernetes/OpenShift, Git, Maven/Gradle, pip/poetry, JUnit/Mockito/PyTest, SonarQube, CI/CD (GitHub Actions/Jenkins), Prometheus/Grafana/Splunk/OpenTelemetry, Agile/SDLC.

## Python Core (1-14)

1. Explain Python data structures: list, tuple, set, dict, and when to use each.
2. What is the difference between deep copy and shallow copy in Python?
3. Explain Python's GIL and its impact on CPU-bound vs I/O-bound work.
4. How does Python memory management and garbage collection work?
5. Explain decorators, generators, and iterators with examples.
6. What are *args and **kwargs, and how do you use them safely?
7. Explain list comprehensions vs generator expressions and their performance.
8. How do you handle exceptions properly in Python (try/except/else/finally, custom exceptions)?
9. Explain context managers and the `with` statement; how do you write one?
10. What is asyncio and how does async/await differ from threads/multiprocessing?
11. How do you write type hints and validate them (mypy, Pydantic)?
12. How do you profile and optimize slow Python code?
13. Explain virtual environments and dependency management (pip, poetry, uv).
14. How do you structure a Python package/project for maintainability?

## Python Web & Data (15-26)

15. Compare FastAPI, Flask, and Django and when to choose each.
16. How does FastAPI use Pydantic and dependency injection?
17. How do you build a REST API with FastAPI including validation and error handling?
18. How do you implement authentication/authorization in a Python web service?
19. How do you handle async database access in FastAPI (SQLAlchemy async, asyncpg)?
20. How do you manage database migrations (Alembic) in Python projects?
21. Explain ORM concepts with SQLAlchemy; lazy vs eager loading.
22. How do you avoid N+1 query problems in an ORM?
23. How do you use Pandas efficiently for large datasets (vectorization, chunking)?
24. Explain NumPy broadcasting and when to prefer it over loops.
25. How do you build a data pipeline in Python and handle failures/idempotency?
26. How do you test Python services (PyTest fixtures, mocking, parametrization)?

## Java Core (27-42)

27. Explain OOP principles and SOLID with Java examples.
28. Difference between abstract classes and interfaces in Java.
29. Explain the Java Collections framework: List, Set, Map and their implementations.
30. HashMap vs ConcurrentHashMap vs Hashtable internals.
31. Explain multithreading in Java: Thread, Runnable, ExecutorService.
32. What are synchronized, volatile, and atomic types?
33. Explain the Java memory model and happens-before relationship.
34. What is the difference between `==` and `.equals()`, and hashCode contract?
35. Explain exception hierarchy in Java: checked vs unchecked.
36. What are generics and type erasure in Java?
37. Explain Java Streams and functional interfaces (map/filter/reduce).
38. What is the difference between Optional misuse and proper usage?
39. Explain Java 11/17 features you use (var, records, sealed classes, text blocks).
40. How does garbage collection work in the JVM (G1, ZGC) and how do you tune it?
41. How do you profile a Java application for CPU/memory issues (JFR, jstack, heap dumps)?
42. Explain immutability and how to design thread-safe classes.

## Java Spring Ecosystem (43-54)

43. Explain Spring Boot auto-configuration and starters.
44. Difference between @Component, @Service, @Repository, @Controller.
45. Explain dependency injection and bean scopes in Spring.
46. How does Spring MVC handle a request end-to-end?
47. How do you build a REST API with Spring Boot and validate input?
48. Explain Spring Data JPA repositories and derived queries.
49. How do you manage transactions with @Transactional and propagation?
50. How does Spring Security handle authentication and authorization?
51. How do you secure a Spring Boot REST API with JWT?
52. How do you handle exceptions globally in Spring (@ControllerAdvice)?
53. How do you configure and use Spring profiles for multiple environments?
54. How do you write JUnit + Mockito tests for a Spring Boot service?

## APIs, Microservices & Messaging (55-68)

55. What makes a REST API RESTful? Explain resources, verbs, and status codes.
56. How do you version a REST API without breaking clients?
57. How do you write and maintain an OpenAPI/Swagger specification?
58. How do you design idempotent APIs and handle retries safely?
59. Explain microservices vs monolith and the tradeoffs.
60. How do services discover and communicate with each other?
61. Explain synchronous vs asynchronous communication in microservices.
62. Explain Apache Kafka: topics, partitions, offsets, consumer groups.
63. How do you guarantee at-least-once vs exactly-once processing in Kafka?
64. How do you handle a poison message and dead-letter topics?
65. Compare Kafka, RabbitMQ, ActiveMQ, and IBM MQ.
66. How do you implement an event-driven workflow reliably?
67. How do you handle distributed transactions (Saga, outbox pattern)?
68. How do you design for resilience (circuit breaker, bulkhead, timeout)?

## Databases & Persistence (69-80)

69. Explain relational schema design and normalization vs denormalization.
70. How do indexes work and when can they hurt performance?
71. How do you read a query execution plan and optimize a slow query?
72. Explain transactions and ACID isolation levels with examples.
73. How do you handle deadlocks in a relational database?
74. Explain connection pooling and how to size it (HikariCP).
75. Difference between Hibernate/JPA and raw SQL; when to use each.
76. Explain lazy vs eager fetching and the N+1 problem in JPA.
77. Explain caching strategies and how to use Redis effectively.
78. When would you use MongoDB or Elasticsearch instead of a relational DB?
79. How do you design a schema for time-series or high-write workloads?
80. How do you perform safe database migrations in production?

## Testing, Quality & SonarQube (81-88)

81. Explain the testing pyramid: unit, integration, component, e2e.
82. How do you write effective unit tests with JUnit 5 and Mockito?
83. How do you write effective tests with PyTest (fixtures, parametrize, mocking)?
84. Difference between mocks, stubs, fakes, and spies.
85. How do you maintain high code coverage meaningfully?
86. How do you fix SonarQube findings: code smells, bugs, vulnerabilities?
87. How do you apply SOLID and clean code in day-to-day reviews?
88. How do you perform a constructive peer code review?

## CI/CD, Containers & Cloud (89-95)

89. How do you build a CI/CD pipeline for a Java/Python service?
90. What stages would you include: build, test, scan, package, deploy?
91. How do you containerize Java and Python apps efficiently (multi-stage, non-root)?
92. How do you use Maven/Gradle and pip/poetry in a pipeline with caching?
93. How do you deploy to Kubernetes/OpenShift and handle config/secrets?
94. How do you do zero-downtime releases (rolling, blue/green, canary)?
95. How do you roll back a bad deployment safely?

## Observability, Production Support & Agile (96-100)

96. How do you instrument a service with Prometheus metrics and OpenTelemetry traces?
97. How would you debug a Level 3 production issue end to end?
98. How do you use Splunk/Grafana to perform RCA and reduce MTTR?
99. How do you work effectively in Agile ceremonies and estimate a task?
100. Why are you a good fit for this Python & Java SDE role at Citi, and what would you improve in your first 90 days?
