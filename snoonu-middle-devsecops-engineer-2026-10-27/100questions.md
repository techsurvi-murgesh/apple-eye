# 100 Interview Questions — Middle DevSecOps Engineer (Snoonu)

Target profile: AWS and GCP cloud security, IAM least privilege, VPC/network security, AWS security services (GuardDuty, Security Hub, Inspector, Config, CloudTrail, WAF), secure CI/CD and IaC (Terraform, CloudFormation), container and API security, security automation, incident response, and collaboration with development and operations teams.

## AWS and Cloud Security Foundations (1–15)

1. Explain the AWS shared responsibility model for IaaS, managed services, and serverless.
2. How would you structure AWS accounts for a growing company, and why use AWS Organizations?
3. What are service control policies, and how do they differ from IAM policies?
4. How does CloudTrail work, and what would you log to support security investigations?
5. How do you use AWS Config to detect and remediate non-compliant resources?
6. What does GuardDuty detect, and how do you triage a high-severity finding?
7. What is Security Hub, and how do security standards and findings work there?
8. When would you use Inspector, and how does it differ from a traditional vulnerability scanner?
9. How does AWS WAF protect an application, and what is the difference between a rule group and a web ACL?
10. When is AWS Shield Advanced justified, and what does it add beyond standard DDoS protection?
11. How does KMS envelope encryption work, and how do you design key policies safely?
12. Compare Secrets Manager and Systems Manager Parameter Store for secret storage and rotation.
13. How do you secure an S3 bucket against public exposure, accidental deletion, and data exfiltration?
14. What is your approach to encryption at rest and in transit across a multi-service AWS application?
15. Design a logging and monitoring architecture that gives both security and operations teams the signals they need.

## IAM and Least Privilege (16–28)

16. Compare IAM users, groups, and roles, and explain when each is appropriate.
17. What are identity-based, resource-based, permissions boundary, and session policies?
18. Walk through how AWS evaluates an IAM request when several policies apply.
19. How do permission boundaries help you delegate administration safely?
20. How do you design cross-account access with an assume-role pattern?
21. Describe your process for moving an existing over-permissive IAM policy to least privilege.
22. How does IAM Access Analyzer help, and what does it not catch?
23. What is attribute-based access control, and when would you use it?
24. How do you rotate access keys and credentials without breaking running workloads?
25. How does federation with OIDC or SAML remove long-lived credentials?
26. What is IRSA, and how does it let Kubernetes workloads access AWS securely?
27. Which IAM misconfigurations do you see most often, and how do you detect them?
28. How do service control policies and permission boundaries work together in a large organization?

## Network Security (29–40)

29. Design a VPC for a public web application and a private data tier. Which subnets, route tables, and gateways do you need?
30. Compare security groups and network ACLs, including statefulness and evaluation order.
31. When would you use VPC peering versus AWS Transit Gateway?
32. How do VPC endpoints and AWS PrivateLink keep traffic off the public internet?
33. Compare Site-to-Site VPN and AWS Direct Connect for hybrid connectivity, including security trade-offs.
34. What security controls apply to Route 53 and private DNS in a multi-account environment?
35. How do you enforce TLS across load balancers, services, and databases?
36. How do WAF, security groups, and NACLs complement each other rather than duplicate work?
37. How would you protect a public API from DDoS and application-layer abuse?
38. How do you segment a cloud network so a compromised workload cannot move laterally?
39. What do VPC Flow Logs tell you, and what do they miss?
40. A service cannot reach a private dependency. Walk through your troubleshooting steps, including security controls.

## AWS Security Services in Depth (41–53)

41. A GuardDuty finding reports credential exfiltration. What are your first five actions?
42. How do you select Security Hub standards, and how do you reduce finding noise?
43. How do you prioritize Inspector findings when everything looks critical?
44. Write the logic for an AWS Config rule that flags unencrypted EBS volumes.
45. How do you verify CloudTrail log integrity and protect the log archive account?
46. How would you write a WAF rule to block a credential-stuffing pattern without blocking real users?
47. What does Shield Advanced provide during an active attack, and how does the response team use it?
48. When would you use Macie, and how do you handle a sensitive-data finding?
49. How does Detective help after an incident, and how does it differ from GuardDuty?
50. Walk through an AWS security incident response from detection to containment, eradication, and recovery.
51. Design an automated remediation for a public S3 bucket using EventBridge, Lambda, and CloudTrail.
52. How do you run a vulnerability management program across EC2, containers, and dependencies?
53. How would you threat-model a new AWS service before it is deployed?

## CI/CD and Infrastructure-as-Code Security (54–65)

54. What does a secure CI/CD pipeline look like from commit to production?
55. How do you protect Terraform state, and why is state a security asset?
56. Which Terraform security controls do you enforce in code review and in CI?
57. What is policy as code, and how would you gate a deployment on security policy?
58. How do tools such as Checkov, tfsec, or Conftest fit into a pipeline?
59. Compare SAST, DAST, and dependency scanning, and explain where each belongs.
60. How do you handle a critical dependency vulnerability discovered during a release?
61. How do you protect the software supply chain, including artifacts and image signing?
62. Which branch protection and review controls do you require on a production repository?
63. How does OIDC federation improve CI/CD security compared with static cloud keys?
64. How do you detect and remediate infrastructure drift without breaking production?
65. How do you apply the same security review to CloudFormation that you apply to Terraform?

## Container and API Security (66–76)

66. How do you harden a Docker image and the runtime that executes it?
67. Where does image scanning belong in the build and deployment lifecycle?
68. How does Kubernetes RBAC work, and which roles are commonly over-permissive?
69. How do Kubernetes network policies reduce blast radius?
70. What does an admission controller enforce, and why is it useful for security?
71. What controls detect a compromised container at runtime?
72. How do you deliver secrets to containers without baking them into images?
73. How do you authenticate and authorize service-to-service API calls?
74. Compare session-based auth, JWT, and OAuth2 for a public API, including revocation.
75. Walk through the OWASP API Security Top 10 and how you would test for several of them.
76. How do rate limiting, quotas, and an API gateway protect both availability and cost?

## GCP and Multi-Cloud Security (77–84)

77. Compare GCP IAM with AWS IAM, including roles, bindings, and service accounts.
78. How do GCP VPC firewall rules differ from AWS security groups and NACLs?
79. What does Cloud Armor protect, and how does it compare with AWS WAF?
80. What is Security Command Center, and which findings would you act on first?
81. How do Cloud Audit Logs support detection and investigation in GCP?
82. How do organization policies enforce guardrails across GCP projects?
83. What security controls matter most for GKE clusters and workloads?
84. How would you maintain a consistent security baseline across AWS and GCP without duplicating everything?

## Automation, Incident Response, and Scripting (85–92)

85. Write a Python boto3 script to find and report public S3 buckets. What edge cases must it handle?
86. How do you design event-driven remediation that is safe and idempotent?
87. What would you automate first in a security operations backlog, and why?
88. Walk through the phases of incident response and the evidence you preserve at each stage.
89. What forensic data would you collect from a compromised EC2 instance, and how do you avoid destroying it?
90. How do you contain a compromised IAM principal without causing a wider outage?
91. How do you collect evidence for a compliance audit without manually gathering screenshots?
92. Which security metrics would you report to engineering leadership every month?

## Collaboration, Judgment, and Behavioral (93–100)

93. How do you balance security requirements with delivery speed when a team is under pressure?
94. How do you explain a high-risk finding to a developer who does not consider it urgent?
95. Describe a time you disagreed with an engineering decision on security grounds. What did you do?
96. Walk through a security incident or near miss you handled: detection, response, and what changed afterward.
97. How do you prioritize between a critical vulnerability, a noisy alert, and a long-term hardening project?
98. How do you get up to speed on a new cloud platform or security service quickly?
99. What documentation and runbooks do you leave behind so another engineer can operate the environment?
100. Walk through an end-to-end hardening project you delivered across cloud, CI/CD, containers, and APIs, and explain the trade-offs you made.
