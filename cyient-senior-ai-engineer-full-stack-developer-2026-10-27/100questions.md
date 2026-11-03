# 100 Interview Questions — Senior AI Engineer / Full-Stack Developer (Cyient)

Target profile: AI agentic applications, LLM/RAG, Python (FastAPI/Flask/Django), REST APIs, full-stack web apps, 3D CAD automation, engineering tool integration (CATIA V5, AVEVA E3D, Tekla Structures, STAAD.Pro, IDEA Statica), IFC/STEP/IGES, simulation and structural validation workflows.

## Python and Backend Fundamentals (1–15)

1. How does the Python GIL affect CPU-bound and I/O-bound workloads, and how do you work around it?
2. Compare asyncio, threading, and multiprocessing for a service that calls slow external APIs.
3. How do decorators work, and how would you use one for retries, logging, or authentication?
4. Explain context managers and a case where you would write your own.
5. How do generators and `yield` help when processing a large 3D model or a large API response?
6. How do type hints and Pydantic improve correctness at the boundaries of a Python service?
7. How do you manage dependencies and virtual environments across development, CI, and production?
8. How do you design exception hierarchies for an application that wraps external engineering software?
9. When would you use multiprocessing rather than asyncio for model processing jobs?
10. What causes memory growth in long-running Python services, and how do you diagnose it?
11. Explain the SOLID principles and give an example of applying one in Python.
12. Compare dataclasses and Pydantic models for configuration, domain objects, and API payloads.
13. How do you manage SQLAlchemy sessions and connection pooling safely in a web service?
14. How do Alembic migrations work, and how do you roll out a schema change without downtime?
15. How do you profile a slow Python endpoint and decide whether the bottleneck is CPU, I/O, or the database?

## APIs, FastAPI, Flask, and Django (16–30)

16. What makes an API RESTful, and which constraints matter most in a real service?
17. How do you implement idempotency for a request that triggers an expensive model-generation job?
18. Which HTTP status codes do you return for validation errors, auth failures, conflicts, and timeouts?
19. How do you design pagination and filtering for a large list of models or analysis results?
20. How do you version a public API without breaking existing clients?
21. How does FastAPI dependency injection work, and where would you use it?
22. What happens when a blocking call is made inside an async FastAPI endpoint, and how do you fix it?
23. How do you implement JWT or OAuth2 authentication and role-based access in FastAPI?
24. What belongs in middleware versus a dependency or a route handler?
25. Compare FastAPI background tasks, Celery, and a queue-backed worker for long-running simulation jobs.
26. What is the Flask application factory pattern, and why is it useful?
27. How does the Django ORM compare with SQLAlchemy for complex queries?
28. Explain WSGI versus ASGI and how the choice affects concurrency and deployment.
29. How do you add rate limiting and request quotas to an API that calls paid LLM or CAD services?
30. How do you keep OpenAPI documentation accurate as the API and models evolve?

## LLMs, Prompt Engineering, and RAG (31–45)

31. Walk through the architecture of a production LLM-powered application beyond the model API call.
32. What makes a prompt reliable for a structured engineering task?
33. Compare system, developer, and user prompts, and explain how you version them.
34. How do structured outputs or JSON schemas make LLM responses safe to feed into application logic?
35. How does tool or function calling work, and how do you validate the arguments a model produces?
36. Design a RAG pipeline for engineering standards, drawings, and project documents.
37. How do you choose chunk size, overlap, and metadata for technical documents?
38. What are embeddings, and how do you choose a vector store for a given workload?
39. How do you measure retrieval quality separately from generation quality?
40. When and why would you add reranking to a RAG pipeline?
41. How do you reduce hallucination when answers have structural or safety consequences?
42. How do you evaluate an LLM feature before and after a prompt or model change?
43. How do you control latency and token cost in a multi-step LLM workflow?
44. What happens when a document exceeds the context window, and how do you handle it?
45. How do you defend against prompt injection and data leakage in an agent that reads project files?

## AI Agents and Frameworks (46–58)

46. What is an AI agent, and how does it differ from a single LLM call or a fixed workflow?
47. Describe the agent loop: planning, tool selection, execution, observation, and stopping.
48. What does LangChain provide, and which parts would you avoid overusing?
49. How does LlamaIndex support retrieval-heavy applications?
50. How would you model roles and collaboration in CrewAI?
51. What kinds of problems suit AutoGen's multi-agent conversation model?
52. How do you decide between one agent with many tools and multiple specialised agents?
53. How do you give an agent memory without making it stale or unsafe?
54. What makes a good tool definition for an agent that must drive external software?
55. How would an agent interact with a CAD or simulation application through an SDK, API, or CLI?
56. Which guardrails do you put around an agent that can modify engineering models?
57. How do you handle partial failures, retries, and timeouts in a multi-step agent workflow?
58. How do you observe and debug an agent in production when the failure is in reasoning rather than code?

## 3D Geometry, CAD, and File Formats (59–72)

59. How is geometric data represented in software, and what are the trade-offs between representations?
60. Compare meshes, boundary representations, and NURBS surfaces.
61. What is the STEP format, and why is it used for exchanging CAD models?
62. What is IGES, and what are its limitations compared with STEP?
63. What is IFC, and how does it model building elements and relationships?
64. Which spatial data structures would you use for collision checks or nearest-part queries?
65. How do coordinate systems and transformation matrices affect model assembly and validation?
66. How would you programmatically generate or modify a 3D model from a specification?
67. How do you automate CATIA V5 through its API or scripting interface?
68. How do parts, products, and assemblies relate in CATIA V5?
69. What is parametric modelling, and how do parameters and constraints drive model changes?
70. How do you validate that a generated model is geometrically correct and manufacturable?
71. What are the common failure modes when converting between 3D file formats?
72. How would you store, version, and retrieve large 3D files efficiently in a web application?

## Engineering Tool Automation and Simulation (73–84)

73. What is AVEVA E3D used for, and how would you approach automating it?
74. What is Tekla Structures used for, and how does its data model support structural BIM?
75. How would you integrate with STAAD.Pro for structural analysis?
76. How would you integrate with IDEA Statica for connection design or code checks?
77. How do you design a plug-in architecture for an engineering desktop application?
78. How do you choose between an SDK, an API, and a CLI when automating a third-party tool?
79. Design a pipeline that takes a model from CAD through simulation and returns validated results.
80. What inputs and outputs would you expect from an automated stress analysis workflow?
81. How do you encode structural validation rules in software without losing engineering intent?
82. How do you schedule long-running model and simulation jobs without blocking the web application?
83. How do you detect and recover when an external engineering tool crashes mid-job?
84. How do you extract data from an engineering tool that has no clean API?

## Full-Stack, Frontend, and Delivery (85–94)

85. How would you structure a React application for reviewing models, jobs, and analysis results?
86. Compare local state, Context, and Redux Toolkit for a growing dashboard.
87. How do TypeScript types improve safety when consuming API responses?
88. How do you build a responsive interface for large tables, 3D viewers, and file uploads?
89. How do you handle secure file upload and download for large CAD assets?
90. How do you secure a full-stack application that connects users, AI models, and engineering software?
91. How do you structure pytest tests for a service that wraps external tools?
92. How do you mock a CAD or simulation tool in tests without making the suite slow or flaky?
93. How do you design CI/CD for an application with both Python services and a React frontend?
94. How do you package and deploy an application that depends on native engineering software?

## Collaboration, Problem Solving, and Behavioral (95–100)

95. How do you review code that mixes AI output, API logic, and engineering rules?
96. How do you work with domain-expert engineers to turn a manual workflow into software?
97. Describe a time you translated a complex physical or business rule into digital logic.
98. Walk through debugging an automation that produced the wrong model or analysis result.
99. How do you handle disagreement with a domain expert about what the software should do?
100. Walk through an end-to-end solution you built that combined AI, APIs, and external systems, and explain the trade-offs you made.
