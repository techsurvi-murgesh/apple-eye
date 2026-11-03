Created: 2026-11-02

# Integration Engineer (Go / Event-Driven / AWS EKS)

**Company:** Not specified
**Location:** Remote / Hybrid
**Posted:** 2026-11-02

## Key Responsibilities

- Design and build integration services and APIs in Go, applying appropriate integration and design patterns (message routing, transformation, idempotency, retry/backoff, circuit breaker, saga/compensation, outbox).
- Build event-driven flows using SQS, SNS, and Lambda — including ordering, deduplication, dead-letter handling, and replay strategy.
- Containerize services and deploy to EKS/Kubernetes; own Helm charts, resource sizing, health/readiness probes, autoscaling, and rollout strategy.
- Model and optimize data access against RDS (schema design, indexing, connection pooling, transaction boundaries, migrations).
- Translate integration requirements into interface contracts and sequence flows; document API and event schemas and drive versioning discipline.
- Build in observability from day one — structured logging, metrics, distributed tracing, alerting on integration SLAs.
- Use AI-assisted development tooling (e.g., Claude Code, GitHub Copilot, Cursor) to accelerate delivery, and enforce review discipline so AI-generated code meets the same quality and security bar.
- Contribute to CI/CD pipelines, automated testing (unit, contract, integration), and non-functional validation (load, failover, resiliency).
- Provide code review, mentoring, and technical guidance to mid-level developers; raise design risks early to the Tech Lead.

## Must-Have Qualifications

- **Go (hands-on, non-negotiable)**: 3+ years writing production Go; strong grasp of goroutines, channels, context propagation, error handling, and interface-driven design.
- Experience with Go web/API frameworks and gRPC or REST service development.
- Comfortable profiling and tuning Go services (memory, concurrency, latency).
- **Enterprise Integration**: Working command of enterprise integration patterns (Hohpe/Woolf) and their real trade-offs: sync vs. async, orchestration vs. choreography, guaranteed delivery, exactly-once vs. at-least-once, idempotent consumers.
- Strong understanding of canonical data models for integration — designing a canonical/common schema layer, mapping source and target payloads to and from it, and knowing when a canonical model is the right call versus point-to-point or a per-domain contract.
- Basic knowledge of one or more iPaaS platforms — MuleSoft, Boomi, Workato, Azure Logic Apps, Informatica, TIBCO, webMethods, or similar — including connector development, mapping/transformation, and orchestration.
- Practical experience with design patterns (creational/structural/behavioral) and clean architecture, SOLID, and domain boundaries — able to justify choices, not just name them.
- Experience with API contracts, schema evolution, and backward compatibility.

## Cloud & Platform (AWS)

- Hands-on with EKS and Kubernetes — deployments, services, ingress, config/secrets, HPA, troubleshooting live workloads.
- Understanding of containerization skills (Docker: multi-stage builds, image hardening, small runtime images).
- Knowledge about SQS, SNS, and Lambda in event-driven architectures.
- Understanding of RDS (PostgreSQL or MySQL) including performance tuning.
- Knowledge about IAM, VPC/networking basics, Secrets Manager/Parameter Store, and CloudWatch.

## AI in the Development Lifecycle

- Demonstrable experience using AI coding assistants in real delivery — able to describe what they accelerated, where the tooling failed, and how they validated output.
- Understanding of prompt/context practices for codebases, plus the guardrails: security review, licensing, and hallucination checks.

## Engineering Practice

- Git-based workflow, trunk/branching discipline, CI/CD (GitHub Actions, GitLab CI, Jenkins, or similar).
- Test automation habit — unit, contract, and integration testing as part of definition of done.
- Clear written and verbal communication with distributed teams and client stakeholders.
