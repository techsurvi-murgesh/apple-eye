# 100 Interview Questions — Full Stack Java Developer, Angular + Spring Boot (Citi) — 2026-10-07

Target stack: Angular (v14+), TypeScript, RxJS/NgRx, HTML5/SCSS, Java 11/17, Spring Boot/MVC/Data/Security/Cloud, REST APIs, microservices, event-driven (Kafka/RabbitMQ), PostgreSQL/Oracle/MySQL, MongoDB/Cassandra, Hibernate/JPA, Docker, Kubernetes/OpenShift, CI/CD, JUnit/Mockito/Jasmine/Karma/Cypress, SonarQube/Snyk, SAST/DAST, Agile/Jira.

## Angular & Frontend (1-22)

1. Explain Angular architecture: modules, components, services, and dependency injection.
2. What is the difference between a component and a directive? Types of directives.
3. Explain Angular data binding types: interpolation, property, event, two-way.
4. How do lifecycle hooks work in Angular (ngOnInit, ngOnChanges, ngOnDestroy)?
5. Explain Angular change detection and OnPush strategy.
6. How does RxJS work? Explain Observables vs Promises.
7. Explain common RxJS operators (map, filter, mergeMap, switchMap, concatMap, catchError).
8. What is the difference between switchMap, mergeMap, concatMap, and exhaustMap?
9. How do you unsubscribe from Observables and avoid memory leaks?
10. Explain NgRx: store, actions, reducers, effects, selectors.
11. How do you manage state in a large Angular app without NgRx?
12. How do you build reactive forms vs template-driven forms?
13. How do you implement form validation in Angular (sync and async)?
14. How do you use Angular Router, lazy loading, and route guards?
15. How do you build a reusable service and share data between components?
16. How do you call a REST API from Angular with HttpClient and handle errors?
17. How do you implement an HTTP interceptor for auth tokens and error handling?
18. How do you optimize Angular app performance (trackBy, lazy loading, OnPush, AOT)?
19. How do you make an Angular app responsive and accessible?
20. How do you write unit tests in Angular with Jasmine and Karma?
21. How do you write end-to-end tests with Cypress or Protractor?
22. How do you structure a modular Angular project for maintainability?

## Java Core (23-38)

23. Explain OOP principles and SOLID with Java examples.
24. Difference between abstract classes and interfaces.
25. Explain the Java Collections framework and choosing implementations.
26. How do HashMap, ConcurrentHashMap, and Hashtable differ internally?
27. Explain multithreading: Thread, Runnable, Callable, ExecutorService.
28. What are synchronized, volatile, and atomic types?
29. Explain the Java memory model and happens-before.
30. Difference between `==` and `.equals()` and the hashCode contract.
31. Explain checked vs unchecked exceptions and best practices.
32. What are generics and type erasure?
33. Explain Java Streams and functional interfaces with examples.
34. Explain Java 11/17 features (var, records, sealed classes, text blocks).
35. How does garbage collection work and how do you tune the JVM?
36. How do you profile CPU/memory issues (JFR, jstack, heap dumps)?
37. How do you design immutable and thread-safe classes?
38. Explain Java concurrency utilities (locks, CountDownLatch, CompletableFuture).

## Spring Framework & Microservices (39-54)

39. Explain Spring Boot auto-configuration and starters.
40. Difference between @Component, @Service, @Repository, @Controller.
41. Explain dependency injection and bean scopes.
42. How does Spring MVC handle a request end-to-end?
43. How do you build and validate a REST API in Spring Boot?
44. Explain Spring Data JPA repositories and derived queries.
45. How do transactions work in Spring (@Transactional, propagation, isolation)?
46. How does Spring Security handle authentication and authorization?
47. How do you secure a REST API with JWT or OAuth2?
48. Explain Spring Cloud components (Config, Gateway, Eureka, Resilience4j).
49. How do you handle exceptions globally (@ControllerAdvice)?
50. How do you implement API versioning and backward compatibility?
51. Explain microservices vs monolith and decomposition strategies.
52. How do services communicate—REST vs messaging—and tradeoffs?
53. How do you implement resilience (circuit breaker, retry, timeout, bulkhead)?
54. How do you handle distributed transactions (Saga, outbox pattern)?

## Databases & Persistence (55-68)

55. Explain relational schema design and normalization vs denormalization.
56. How do indexes work and when can they hurt performance?
57. How do you read an execution plan and optimize a slow query?
58. Explain ACID and isolation levels with examples.
59. How do you handle deadlocks in a relational database?
60. Explain connection pooling and sizing (HikariCP).
61. Difference between Hibernate/JPA and raw SQL; when to use each.
62. Explain lazy vs eager loading and the N+1 problem in JPA.
63. How do you map relationships in JPA (OneToMany, ManyToMany)?
64. When would you use MongoDB or Cassandra instead of a relational DB?
65. How do you use Redis/Hazelcast for caching effectively?
66. Explain cache invalidation strategies.
67. How do you design a schema for high-write workloads?
68. How do you run safe database migrations in production (Flyway/Liquibase)?

## APIs, Messaging & Integration (69-76)

69. What makes a REST API RESTful? Verbs, resources, and status codes.
70. How do you design an OpenAPI/Swagger contract-first API?
71. How do you make APIs idempotent and handle retries?
72. Explain Apache Kafka: topics, partitions, consumer groups, offsets.
73. Compare Kafka, RabbitMQ, and ActiveMQ for enterprise integration.
74. How do you handle poison messages and dead-letter queues?
75. How do you implement at-least-once and exactly-once semantics?
76. How do you handle CORS and secure cross-origin frontend/backend calls?

## Testing, Security & DevOps (77-92)

77. Explain the testing pyramid for full-stack apps.
78. How do you write unit tests with JUnit 5 and Mockito?
79. Difference between mocks, stubs, spies, and fakes.
80. How do you write Angular unit tests with Jasmine/Karma?
81. How do you write end-to-end tests with Cypress?
82. How do you maintain meaningful high test coverage?
83. How do you apply SAST/DAST and remediate SonarQube/Snyk findings?
84. How do you prevent common web vulnerabilities (OWASP Top 10)?
85. How do you manage secrets and config across environments?
86. How do you build a CI/CD pipeline for an Angular + Spring Boot app?
87. How do you containerize frontend and backend (multi-stage, non-root)?
88. How do you deploy to Kubernetes/OpenShift with config/secrets?
89. How do you do zero-downtime and blue/green deployments?
90. How do you monitor a full-stack app (Prometheus, Grafana, OpenTelemetry)?
91. How do you roll back a bad deployment safely?
92. How do you handle database migration during deployment?

## Architecture, Agile & Behavioral (93-100)

93. Explain clean architecture and layered design in a Spring Boot app.
94. How do you design a scalable, cloud-native application end to end?
95. How do you ensure enterprise security, data privacy, and regulatory compliance?
96. How do you participate effectively in Agile ceremonies with Jira/Confluence?
97. How do you approach a peer code review constructively?
98. How do you debug a Level 3 production issue across frontend and backend?
99. How do you prioritize technical debt vs feature delivery?
100. Why are you a good fit for this Full Stack Java Developer role at Citi, and what would you improve in your first 90 days?
