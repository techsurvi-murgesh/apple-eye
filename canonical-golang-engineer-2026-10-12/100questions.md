# 100 Interview Questions — Golang Engineer (Canonical) — 2026-10-12

Target stack: Go on Linux (Ubuntu/Debian), goroutines and tasteful concurrency, distributed systems and APIs (REST/gRPC/Protobuf), performance engineering and profiling, security, testing and documentation, containerised/CLI tooling, open-source community practices. Nice-to-have context: Juju, LXD, MicroK8s, Snapd, Ubuntu Core, Ubuntu Pro, MAAS, Livepatch.

## Go Language Fundamentals & Internals (1-15)

1. Explain Go's compilation model and how it differs from interpreted and JIT languages.
2. What is the difference between `:=` and `=`? Why can you use `:=` only in some places?
3. Explain slices versus arrays. What happens when you append to a slice and it reallocates?
4. Explain the difference between a slice header (`ptr`, `len`, `cap`) and the backing array.
5. What are maps internally, and what is the zero value of a map?
6. Why does deleting from a map during range not affect iteration, but adding does?
7. Explain value semantics vs pointer semantics. Give a case where pointer receivers are required.
8. What is an interface with zero methods? Why is it useful?
9. Explain type embedding and method promotion. What are the pitfalls?
10. What is the difference between a type assertion and a type switch? What happens on a failed assertion?
11. Explain `defer`, argument evaluation time, and common defer pitfalls in loops.
12. What are variadic functions and how are they implemented?
13. Explain struct tags and how reflection uses them (e.g., encoding/json).
14. What is the difference between `errors.New`, `fmt.Errorf` with `%w`, and sentinel errors?
15. Explain Go's garbage collector at a high level: tri-color marking, write barriers, and STW pauses.

## Concurrency, Channels & Parallelism (16-32)

16. What is a goroutine? How does it differ from an OS thread?
17. What does the `go` statement do, and what is a deadlock in Go?
18. Explain unbuffered vs buffered channels and how capacity affects blocking.
19. Explain directional channel types (`chan<-`, `<-chan`) and why they improve API design.
20. Explain `close()`, and how to safely detect a closed channel.
21. What happens if you send on a nil channel, close a nil channel, or receive from a nil channel?
22. Explain `select` with multiple ready cases. Is the choice random?
23. How do you implement a timeout pattern with `select` and `time.After`?
24. Explain `sync.WaitGroup` usage and common mistakes (Add inside goroutine).
25. Explain `sync.Mutex` vs `sync.RWMutex`. When is each appropriate?
26. What are data races? How does Go's race detector find them?
27. Explain `sync.Once`, `sync.Cond`, and `sync.Map`. When should you avoid `sync.Map`?
28. Explain the `context` package: `WithCancel`, `WithTimeout`, `WithDeadline`, and `WithValue`.
29. How do you correctly propagate cancellation across goroutines?
30. What are worker pools in Go, and how do you implement one?
31. Explain fan-out/fan-in patterns for concurrent work.
32. How do you bound concurrency? Explain `errgroup` (x/sync) and its benefits over `WaitGroup`.

## Performance, Profiling & Memory (33-45)

33. Explain CPU vs memory-bound workloads and how to tell them apart.
34. How do you profile a Go program using pprof? Which profiles are available?
35. Explain `go test -bench`, `-benchmem`, and how to read benchmark output.
36. How do you find and fix memory leaks and memory bloat in Go?
37. What causes high allocations, and how do you reduce them (sync.Pool, preallocation)?
38. Explain escape analysis. How do you check whether a variable escapes to the heap?
39. What is a `pprof` heap profile and how do you read `inuse_space` vs `alloc_space`?
40. How do you profile goroutines and detect goroutine leaks?
41. Explain false sharing and how padding/alignment affects concurrent performance.
42. How do you tune `GOMAXPROCS` for a containerised workload?
43. Explain what happens during GC cycles and how `GOGC` and `GOMEMLIMIT` affect memory.
44. How do you load-test and benchmark a Go HTTP/gRPC service?
45. Explain tail latency and p99. Why is p50 insufficient for service SLOs?

## Testing, Tooling & Engineering Practices (46-55)

46. How do you write table-driven tests in Go, and what are subtests?
47. Explain test doubles: fakes, stubs, mocks, and when to use each.
48. How do you test code that has external dependencies (DB, HTTP, cloud)?
49. Explain `httptest` and how to test an HTTP handler.
50. How do you test gRPC services and clients?
51. Explain golden files / golden tests and when they are useful.
52. What is fuzzing in Go? How do you write and run a fuzz target?
53. How do you use the race detector in CI?
54. What linting and static analysis tools do you use for Go (go vet, staticcheck, golangci-lint)?
55. Explain Go modules: `go.mod`, semantic versioning, `go.sum`, vendoring, and workspaces.

## Distributed Systems, APIs & Networking (56-72)

56. Explain REST API design: versioning, pagination, filtering, and idempotency.
57. Explain gRPC and Protobuf. How does code generation work, and what are the trade-offs vs REST?
58. Explain unary vs streaming RPC, and when to use each.
59. What is a service mesh, and how does mTLS work?
60. Explain circuit breakers, bulkheads, and timeouts in distributed systems.
61. How do you implement retries safely? What is exponential backoff with jitter, and why jitter?
62. Explain idempotency keys and how they prevent duplicate side effects.
63. How do you design a rate limiter (token bucket vs leaky bucket vs sliding window)?
64. Explain how you handle partial failures and sagas vs two-phase commit.
65. How do you propagate a trace ID across services and what are the OTel concepts?
66. Explain leader election and consensus (Raft) at a high level.
67. How do you ensure backward compatibility when evolving a service API?
68. Explain connection pooling for HTTP clients and databases.
69. Explain DNS resolution, TLS handshakes, and where latency hides in a request path.
70. How do you design a rate-limited, authenticated public API?
71. How do you do canary and blue/green rollouts safely?
72. Explain backpressure and how you propagate it through a system.

## Linux Systems & Ubuntu (73-88)

73. Explain the Ubuntu boot process, from firmware to systemd and the login shell.
74. Explain systemd units, targets, `systemctl`, and how to write a service unit.
75. Explain how Linux schedules processes: states, nice/renice, and cgroups.
76. Explain memory management on Linux: virtual memory, paging, swap, and OOM killer.
77. How do you diagnose high CPU load (top, iostat, pidstat, perf)?
78. How do you debug a hung Go service on a Linux host?
79. Explain file descriptors, `ulimit`, and how fd exhaustion causes failures.
80. How do you debug disk space issues (df, du, lsof, deleted-but-open files)?
81. Explain Linux networking: interfaces, routes, DNS, and how to read `ss`/`netstat`.
82. How do you troubleshoot a service that cannot reach another host (curl, dig, nc, tcpdump)?
83. Explain namespaces and cgroups and how they underpin containers.
84. How do containers work (images, layers, overlayfs) and how is a container different from a VM?
85. How do you build a minimal, secure container image for a Go service?
86. How does `snap` work (monolithic squashfs, confinement via AppArmor/seccomp)?
87. Explain `apt`, `dpkg`, and packaging a service as a `.deb`.
88. How do you patch and upgrade a fleet of Linux hosts safely with minimal downtime?

## Security, Open Source & Canonical-Specific (89-100)

89. What are the most common vulnerabilities in Go services and how do you mitigate them?
90. Explain Go's cryptography packages and how to use them correctly (randomness, hashing, AEAD).
91. How do you securely manage secrets and credentials in Go applications?
92. Explain TLS/mTLS, certificate rotation, and how you automate it.
93. What is a supply-chain attack, and how do you protect your build and dependencies?
94. Explain SBOM, signed artefacts, SLSA, and why Go module verification matters.
95. How do you harden a Linux host and a Go service for production?
96. How do you apply least privilege, AppArmor/seccomp, and container confinement?
97. How do you write Go code that is easy to review, maintain, and hand off?
98. How do you contribute to an open-source project: issues, small PRs, code review etiquette?
99. How do you debug a bug users report — your process from report to root cause to fix?
100. Describe a time you took technical ownership of a system, improved engineering or operational practice, and what the measurable result was.

## Behavioural & Situational (for the "going above and beyond" and collaboration criteria)

- Tell us about a time you solved a hard technical problem nobody asked you to solve.
- Describe a production incident you were part of: detection, diagnosis, remediation, and follow-up.
- How do you keep up with a rapidly moving open-source ecosystem?
- How do you disagree in a code or architecture review, and how do you document the outcome?
- How do you work asynchronously across 80+ countries and time zones?
- Describe a piece of technical documentation you wrote that changed how others worked.
- How do you balance delivering to schedule with improving engineering practices?