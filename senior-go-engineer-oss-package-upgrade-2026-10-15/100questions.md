# 100 Interview Questions — Senior Go Engineer, OSS Package Upgrade — 2026-10-15

Target profile: Go engineer on a large monorepo, owning third-party OSS upgrades end to end.
Go modules, semantic versioning, dependency-tree analysis, breaking-API migration, `go build` /
`go test` / linker debugging, Git and patch management, Linux + Bash automation, CI presubmits,
migration reports.

Note on Bazel and Copybara: they are deliberately absent from the resume. Section 10 is a short
primer so you are not caught blank if the interviewer opens that door — answer honestly and pivot
to the equivalent you do know (`go build`, `go test`, Make, GitHub Actions).

## 1. Go fundamentals and the toolchain (1–14)

1. How does the Go build cache work, and what invalidates an entry?
2. What is the difference between `go build`, `go install`, and `go run`?
3. What does `GOFLAGS`, `GOOS`, `GOARCH`, and `CGO_ENABLED` do?
4. How do cross-compilation and build tags work in practice?
5. What are `GO111MODULE` and GOPATH mode, and why is GOPATH mode deprecated?
6. Explain the difference between a package and a module.
7. What is the `vendor/` directory and when should it be used?
8. How do you list and clean stale build artifacts, and what does `go clean -cache` cost?
9. What is `-race` and how is it implemented at a low level?
10. Explain `GOMAXPROCS` and how it interacts with containers and `GOMAXPROCS=auto`.
11. What is the difference between a workspace (`go.work`) and a module?
12. What does `-trimpath` do and why is it used for reproducible builds?
13. How does Go handle CGO, and what breaks when it is enabled in a static build?
14. What is a linker error vs a compile error vs a runtime error? Give one example of each.

## 2. Go modules, semver, and dependency resolution (15–31)

15. What are the files in a module cache and what does `go.sum` guarantee?
16. Explain Minimal Version Selection (MVS) with a concrete example.
17. Where does MVS over-conservatism hurt, and how does `go mod graph` reveal it?
18. What do the `require`, `exclude`, `replace`, and `retract` directives do?
19. When is a `replace` directive acceptable, and why is it dangerous in a shipped library?
20. What is a pseudo-version and when does Go generate one?
21. Explain semantic versioning precisely: what counts as a breaking change for a major version?
22. What is the `/v2` module path suffix, and what happens if you get it wrong?
23. How do you upgrade one dependency without disturbing the rest of the graph?
24. How do you downgrade a dependency, and what breaks if a transitive requirement is higher?
25. What is a module graph pruning change in Go 1.17+, and why did it exist?
26. How do you find every place in a codebase that imports a given module?
27. How do you detect a dependency that is required but no longer imported (dead dependency)?
28. What is the difference between a direct and an indirect requirement in `go.mod`?
29. How do you handle a dependency that pulls in an abandoned module?
30. What does `go mod tidy` actually do, and what can it break?
31. How do you verify a module checksum has not been tampered with?

## 3. Upgrade risk analysis (32–42)

32. Given a dependency bump from v1.4 to v2.0, what do you check before touching code?
33. How do you read an upstream CHANGELOG efficiently for breaking changes?
34. What is the difference between a source-compatible and a behaviour-compatible change?
35. How do you identify hidden API usage through interfaces or reflection?
36. What are deprecation warnings in Go, and do compilers enforce them?
37. How do you assess blast radius in a monorepo before merging a shared-library bump?
38. What are the risks of upgrading a package used by generated code?
39. How do you decide between upgrading in place and pinning an old version?
40. What is a "dependency conflict" in practice — give a real shape of the error.
41. How do you handle an upgrade that requires coordinated changes in several repositories?
42. What signals tell you a dependency should be forked or vendored instead?

## 4. Breaking API changes and downstream migration (43–54)

43. What is the standard workflow for migrating call sites after a breaking change?
44. How do you handle a renamed function across 300 call sites without manual editing?
45. What is `gofmt -r` and when is a plain rewrite safer?
46. How do you handle a struct field changing type in a widely used package?
47. What is the safest approach to changing an exported interface?
48. Explain Go's implicit interfaces and why adding a method to an interface is breaking.
49. How do you handle an upstream change from functional options to a config struct?
50. What do you do when the upstream removed an exported symbol you depend on?
51. How do you migrate a deprecated `io/ioutil` API and similar stdlib changes?
52. How do you handle error-wrapping changes that break `errors.Is`/`errors.As` chains?
53. What does it mean for an upgrade to be behaviourally breaking while still compiling?
54. How do you write a migration guide for downstream teams?

## 5. Build, test, and CI failure debugging (55–72)

55. `go build` fails in CI but passes locally — how do you start the investigation?
56. What causes a non-deterministic build and how do you make it hermetic?
57. Explain `go test ./...`, build tags, and why tests can silently not run.
58. How do you debug a test that passes locally and fails on CI?
59. What is a flaky test and what is your policy on quarantining one?
60. How do you read a panic stack trace efficiently?
61. What is a linker error like "duplicate symbol" and what causes it?
62. How do you reduce test binary size and test runtime?
63. What is `-count=1`, and why does it catch cached-test false positives?
64. How do you find data races in Go, and what does the race detector report mean?
65. How do you debug goroutine leaks?
66. What does a heap profile tell you that a CPU profile does not?
67. How do you use `pprof` to compare behaviour before and after an upgrade?
68. How do you identify memory growth after a dependency upgrade?
69. What is test caching in `go test` and when is it invalidated?
70. How do you run only the affected packages after an upgrade in a monorepo?
71. How do you handle test failures caused by shared global state or port conflicts?
72. What evidence do you attach to a change so a reviewer trusts it?

## 6. Git, patches, and review (73–82)

73. What is the difference between `rebase` and `merge` for a long-lived feature branch?
74. How do you resolve a merge conflict in `go.mod` correctly?
75. What is `git rerere`, and why is it useful in an upgrade-heavy workflow?
76. How do you produce a clean, minimal patch for review when the change is large?
77. When would you use `git bisect` to find the breaking commit?
78. How do you revert a bad dependency upgrade safely in production?
79. What is a patch stack, and how do you keep it reviewable?
80. How do you review a dependency upgrade PR as a reviewer, not an author?
81. What should a good upgrade commit message contain?
82. How do you split a 500-file upgrade into reviewable units?

## 7. Linux, scripting, and automation (83–91)

83. Which Linux tools do you reach for first when a build fails on a machine?
84. How do you find which process and file descriptor is holding a port?
85. What is a shell script's exit code contract, and how do you fail fast with `set -euo pipefail`?
86. How do you parallelise a slow validation script across packages?
87. How would you script a dependency audit across many repositories?
88. How do you detect which Go toolchain version built a binary?
89. What is the difference between a Make target and a shell script for build orchestration?
90. How do you make a build script reproducible on a clean machine?
91. How do you run something as a systemd service or a container entrypoint, and which do you pick?

## 8. CI/CD, presubmits, and monorepo practice (92–97)

92. What makes a good presubmit check, and what belongs after merge instead?
93. How do you design a pipeline so a failed upgrade blocks only the affected packages?
94. How do you cache Go modules and build artifacts correctly in CI?
95. How do you keep CI time low while adding more validation?
96. What is the difference between continuous integration and continuous delivery for an upgrade queue?
97. How do you prioritise upgrades across hundreds of dependencies?

## 9. Security, reporting, and collaboration (98–100)

98. How do you handle a CVE in a transitive dependency you cannot upgrade directly?
99. What goes into a migration report: versions, remediation, validation, outstanding issues?
100. How do you escalate a blocker you cannot solve alone, and what do you include in the message?

## 10. Bazel and Copybara — enough to not be caught blank

These are not on the resume. If they come up, answer honestly and redirect.

101. What problem does Bazel solve that `go build` does not?
102. What is a WORKSPACE file, a BUILD file, and a target?
103. What are the external dependencies (`go_repository`, `http_archive`) in Bazel?
104. How does `rules_go` / `gazelle` generate and maintain BUILD files?
105. What is a Starlark macro and why does Bazel use a Python-like language for config?
106. What are remote caching and remote execution, and what problem do they solve?
107. What is a hermetic build in Bazel terms?
108. How does Bazel model a monorepo differently from a plain `go build ./...`?
109. What is Copybara and what problem does source synchronisation solve?
110. How does a Copybara workflow (`.copybara/` config, labels, destinations) work at a high level?