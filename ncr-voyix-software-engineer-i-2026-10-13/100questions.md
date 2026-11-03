# 100 Interview Questions — Software Engineer (I), NCR Voyix — 2026-10-13

Target profile: Software Engineer (I), 1–3 yrs, entry-level but shipping. Go / TypeScript / React, AWS + Azure + GCP, Docker & Kubernetes, GitHub Actions CI/CD, Agile, testing, code review, documentation, AI-assisted development.

## Computer Science Fundamentals (1–16)

1. What are the main categories of data structures, and when would you pick each?
2. Explain the difference between an array and a linked list, including complexity trade-offs.
3. What is a hash table, and how does collision resolution work?
4. Explain stack vs queue. Where do you meet each in a real system?
5. What is a tree / binary search tree, and how does in-order traversal work?
6. Explain BFS and DFS, and give a use case for each.
7. What is the difference between a heap and a priority queue?
8. Explain time and space complexity. What is Big-O and why does it matter?
9. Explain common sorting algorithms and their complexities.
10. What is recursion, and when is it a bad idea in production code?
11. Explain the difference between pass-by-value and pass-by-reference.
12. What are closures, and why are they useful?
13. Explain immutability. What are the benefits and the cost?
14. What is memoisation and how does it differ from caching?
15. Explain the SOLID principles.
16. What is the difference between compilation and interpretation? Why does it matter for Go?

## OOP & Software Design (17–30)

17. What are the four pillars of OOP?
18. Explain inheritance vs composition. When would you prefer composition?
19. What is an interface / abstraction, and why is it useful?
20. Explain dependency injection.
21. What is the single responsibility principle? Give an example of a violation.
22. How do you decide where to put a boundary between modules or services?
23. Explain coupling and cohesion.
24. What is an anti-pattern? Describe one you have seen and how you fixed it.
25. Explain the difference between a library and a framework.
26. What is the Liskov Substitution Principle?
27. How do you handle errors: exceptions vs error codes vs result types?
28. What is a design pattern you'd use for retrying a flaky operation?
29. Explain the Repository pattern and when it earns its keep.
30. How do you design an API that other developers can use without reading your code?

## Go (31–44)

31. What is the difference between a Go slice and an array?
32. Explain `append` and what capacity means.
33. What are maps in Go, and what happens when you read a missing key?
34. Explain goroutines and how they differ from threads.
35. What is the difference between buffered and unbuffered channels?
36. Explain `select` and channel direction.
37. What is a race condition and how do you prevent it?
38. Explain `sync.Mutex` vs `sync.RWMutex` vs `sync.WaitGroup`.
39. What is context cancellation and why does every Go service need it?
40. How do you handle graceful shutdown with in-flight work?
41. What is an interface with a single method, and why is it idiomatic in Go?
42. How does Go's garbage collector affect performance?
43. What is `errgroup` and when would you use it?
44. How do you write a production-ready Go service: configuration, logging, errors, tests?

## TypeScript / Node.js (45–58)

45. What is TypeScript, and what problem does it solve?
46. Explain `interface` vs `type`.
47. What are generics in TypeScript and when do you use them?
48. Explain union types and type narrowing.
49. What is the difference between `any`, `unknown`, and `never`?
50. What are `readonly` arrays and how do they help?
51. Explain the Node.js event loop and why blocking matters.
52. What are promises and how does `async/await` change error handling?
53. How do you prevent unhandled promise rejections in a service?
54. What are streams in Node and when would you use them?
55. How do you structure a TypeScript codebase for a large team?
56. What is the difference between Express, Fastify, and NestJS?
57. How do you test a Node API — unit vs integration?
58. How do you handle a database connection pool in Node?

## React & Frontend (59–70)

59. What is a React component, and what are props vs state?
60. Explain the difference between controlled and uncontrolled inputs.
61. What is the virtual DOM and what problem does it solve?
62. Explain `useEffect` and the common mistakes people make with it.
63. What are React hooks rules?
64. How do you manage data fetching and server state in React?
65. What is memoisation in React (`memo`, `useMemo`, `useCallback`)?
66. How do you write accessible React components?
67. Explain code splitting and why it improves performance.
68. How do you handle forms and validation?
69. What is the difference between a controlled data flow and a global store?
70. How do you profile and fix a slow React page?

## Testing & Quality (71–82)

71. What is the difference between unit, integration, and system testing?
72. What makes a good unit test?
73. Explain test-driven development. Do you practise it, and how?
74. What is a test double — mock, stub, spy, fake?
75. How do you test code that calls an external service?
76. What is property-based testing?
77. What is a code coverage number, and what is a misleading one?
78. How do you test concurrency?
79. What is a regression test, and when do you write one?
80. How do you write tests for error paths?
81. What is flaky test, and how do you eliminate it?
82. How do you decide what to test and what not to?

## Docker, Kubernetes & Cloud (83–92)

83. What happens between `docker run` and a process starting in a container?
84. What is the difference between a container and a virtual machine?
85. Explain Docker image layers and why caching matters in CI.
86. What is a multi-stage Docker build?
87. What is Kubernetes and what problem does it solve?
88. Difference between a Deployment and a StatefulSet?
89. What are liveness and readiness probes?
90. What are the core AWS services you would use for a web application?
91. How would you deploy an application to Azure?
92. What is a managed Kubernetes service (AKS / EKS / GKE) and why use one?

## CI/CD, Agile & Git (93–100)

93. What happens in a CI/CD pipeline from push to production?
94. How would you set up a GitHub Actions workflow for a Node service?
95. How do you write a good commit message and a useful pull request description?
96. How do you handle a failed pipeline or a rollback?
97. What is Git flow vs trunk-based development?
98. What is Scrum, and how does it work day to day?
99. How do you take part in a code review well — as author and as reviewer?
100. How do you use AI to write code while keeping quality high, and how do you verify what it produces?

---