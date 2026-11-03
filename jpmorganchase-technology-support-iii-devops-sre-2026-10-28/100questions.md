# 100 SRE Interview Questions — Technology Support III, JPMorganChase

Target profile: Site Reliability Engineer supporting large-scale production application flows across on-premises and public cloud environments, with observability, ITIL-aligned incident/problem/change management, validated AI-assisted operations, automation, resiliency, security, and stakeholder communication.

## SRE and Production Reliability (1–15)

1. How do you define Site Reliability Engineering, and how does it differ from traditional production support?
2. How would you ensure operational stability, availability, and performance for a critical application flow?
3. Explain SLI, SLO, and SLA using a customer-facing payment flow as an example.
4. How do error budgets help balance delivery speed with production reliability?
5. Which availability and performance metrics matter most for an end-to-end application flow?
6. How do you distinguish a symptom, a contributing factor, and a root cause?
7. What is toil, and how do you identify and eliminate it in daily operations?
8. How would you apply a reuse-first approach to recurring production interruptions?
9. How do you measure whether a reliability improvement actually worked?
10. What belongs in an effective production-readiness review?
11. How do you assess the blast radius of an application or infrastructure failure?
12. How do you design graceful degradation for a critical user journey?
13. What is the difference between high availability and disaster recovery?
14. How do you prioritize reliability work against urgent feature delivery?
15. Describe a continuous-improvement loop you would establish for an SRE team.

## Incident, Problem, and Change Management (16–30)

16. Walk through your response to a P1 production outage from detection to closure.
17. How do you establish incident command and avoid duplicated investigation efforts?
18. What information do you gather before escalating an incident to another team?
19. How do you communicate with business and technology stakeholders during an outage?
20. How do you decide between restoring service quickly and preserving evidence for analysis?
21. Compare incident management and problem management under ITIL.
22. When should a known error be recorded, and what should its entry contain?
23. How do you conduct a blameless post-incident review?
24. How do you track corrective actions so they are completed rather than forgotten?
25. What makes a normal, standard, or emergency change under an ITIL-aligned process?
26. What should a production change plan include before approval?
27. How do you build and test a rollback plan for a risky release?
28. A change succeeds technically but increases application errors. What do you do?
29. How do you identify recurring interruption patterns across incident and change records?
30. How would you reduce repeat incidents without hiding alerts or lowering escalation standards?

## Observability and Monitoring (31–45)

31. Explain the four golden signals and how you would instrument them for an API.
32. How do metrics, logs, and traces complement one another during triage?
33. What would you monitor first in a Node.js production service?
34. How would you use Prometheus and Grafana to monitor SLOs?
35. How would you use Loki to investigate an intermittent production failure?
36. What is the difference between an actionable alert and monitoring noise?
37. How do you tune alerts without reducing coverage of genuine failures?
38. How would you design a dashboard for both engineers and business stakeholders?
39. How do you trace latency across application, database, and infrastructure layers?
40. Which health checks are appropriate for a containerized service?
41. How do synthetic checks help detect failures that infrastructure metrics miss?
42. How do you monitor batch jobs or asynchronous flows where latency is not request-driven?
43. What does high cardinality mean, and why can it harm a metrics platform?
44. How do you validate that monitoring remains reliable during an application outage?
45. A dashboard looks healthy but users report failures. Walk through your investigation.

## Application, Linux, Cloud, and Hybrid Troubleshooting (46–65)

46. How do you troubleshoot an application that responds intermittently with 5xx errors?
47. How do you investigate a sudden increase in API p99 latency?
48. What Linux commands do you use to inspect CPU, memory, disk, and network pressure?
49. How do you diagnose a process that repeatedly runs out of memory?
50. How do you investigate full disks or inode exhaustion without disrupting service?
51. How do you troubleshoot DNS, TLS, routing, and firewall issues systematically?
52. How do you diagnose PostgreSQL connection-pool exhaustion?
53. What do you check when a PostgreSQL query suddenly becomes slow?
54. How do you investigate a Docker container that restarts repeatedly?
55. What health signals matter for a Docker Swarm service during deployment?
56. How do you compare application behavior across on-premises and AWS environments?
57. How would you troubleshoot an AWS EC2 instance that appears healthy but serves no traffic?
58. How do you investigate an AWS RDS performance issue without immediately resizing it?
59. What is your approach to troubleshooting AWS Lambda timeouts?
60. How do you analyze a failure involving S3 or another external dependency?
61. How do you correlate an infrastructure change with an application regression?
62. How do you troubleshoot issues that occur only under production load?
63. What safeguards do you apply when reproducing a production issue in staging?
64. How do you perform capacity planning for a growing production workload?
65. Walk through a game day that tests the failure of a critical application dependency.

## Validated AI-Assisted Operations (66–76)

66. Where can enterprise-authorized AI responsibly accelerate incident triage?
67. How would you validate an AI-generated incident summary before sharing it?
68. What evidence would you require before acting on an AI-assisted remediation recommendation?
69. When must you reject or escalate an AI-generated recommendation?
70. How do you prevent sensitive operational data from being exposed to unauthorized AI tools?
71. Which operational data should be redacted or minimized before AI-assisted analysis?
72. How can AI help identify recurring interruption patterns without becoming the decision-maker?
73. How would you evaluate the accuracy and usefulness of AI-assisted triage over time?
74. What audit trail should an AI-assisted operational workflow retain?
75. An AI recommendation conflicts with a runbook. How do you proceed?
76. How would you design a human-approved, reuse-first AI workflow for incident and problem routines?

## Automation, Scripting, and Safe Delivery (77–87)

77. Describe a repetitive support task you would automate first and how you would measure the benefit.
78. How do you make Python or Bash operational automation idempotent?
79. What error handling, logging, and timeouts should a production script include?
80. How do you test an automation that restarts or repairs a production service?
81. How do you prevent an automated remediation from creating a larger outage?
82. How should automation handle secrets and privileged credentials?
83. How do you build a safe CI/CD pipeline for a production service?
84. What deployment checks should trigger an automatic rollback?
85. How do you manage configuration differences across development, staging, and production?
86. How do you version, review, and reuse operational runbooks and scripts?
87. Write the logic for a script that detects repeated service failures, validates recent changes, and opens a detailed escalation.

## Regulated Operations and Collaboration (88–95)

88. What additional operational discipline is required in financial services or similarly regulated industries?
89. How do you apply least privilege during production troubleshooting?
90. How do you preserve confidentiality and integrity when sharing logs for escalation?
91. What evidence should be retained for operational and security review after a change?
92. How do you balance rapid service restoration with security and compliance obligations?
93. How do you explain a technical outage to a non-technical business stakeholder?
94. Describe how you would resolve disagreement between application and infrastructure teams during triage.
95. How do you contribute operational best practices across teams rather than only closing tickets?

## Behavioral and Scenario Questions (96–100)

96. Describe a complex production issue you resolved end to end and what changed afterward.
97. Tell me about a time you escalated because the risk or uncertainty exceeded your authority.
98. How would you handle simultaneous P1 incidents affecting two critical application flows?
99. Describe a process improvement that reduced operational effort or improved availability.
100. Why are you a strong fit for this SRE-focused Technology Support III role, and what would you improve in your first 90 days?
