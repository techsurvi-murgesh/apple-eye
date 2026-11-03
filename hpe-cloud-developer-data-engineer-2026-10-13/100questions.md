# 100 Interview Questions — Cloud Developer / Data Engineer, HPE — 2026-10-13

Target profile: data/cloud engineer (2–4 yrs) on an HPE edge-to-cloud data platform team. Kafka, Spark, ClickHouse, ArangoDB, AWS, Python/Java/Scala, Linux + shell, CI/CD, Docker/Kubernetes, NoSQL, message queues, Elasticsearch, data quality, and GenAI/Agentic AI.

## Data Engineering Fundamentals (1–14)

1. What is the difference between a data engineer, a data analyst, and a data scientist?
2. Explain batch vs streaming processing, with an example of each.
3. What is a data pipeline, and what are its typical stages?
4. Explain ETL vs ELT. When would you choose one over the other?
5. What is data modelling? Explain star schema vs snowflake schema.
6. Normalisation vs denormalisation in a data warehouse — when do you denormalise?
7. Explain slowly changing dimensions (Type 1, 2, 3).
8. What is a data lake, a data warehouse, and a lakehouse?
9. How would you design a pipeline that ingests 50M events per day?
10. What is idempotency and why does it matter in data pipelines?
11. Explain backfilling: what is it and how do you do it safely?
12. How do you handle schema evolution on an events pipeline?
13. What is late-arriving data and how do you reconcile it?
14. Explain the difference between OLTP and OLAP workloads.

## Kafka & Streaming (15–30)

15. What problem does Kafka solve? Explain topics, partitions, and offsets.
16. What are producer acks and delivery semantics (at-most-once, at-least-once, exactly-once)?
17. What is a consumer group and why do you need one?
18. How does Kafka achieve ordering guarantees — and when does it not?
19. What are partitions and how do you choose the partition count?
20. Explain the Kafka replication factor and leader election.
21. What is a rebalance? How do you minimise the impact of one?
22. How do you handle a poison pill message in a consumer?
23. Explain consumer lag and how you alert on it.
24. What is a Dead Letter Queue (DLQ) in a streaming context?
25. What are Kafka Connect and Schema Registry used for?
26. How do you achieve exactly-once processing with Kafka?
27. How do you compact a topic and when?
28. What is backpressure in a consumer pipeline and how do you handle it?
29. How would you migrate from one Kafka broker/cluster to another with zero downtime?
30. Explain the difference between Kafka Streams and Spark Structured Streaming.

## Spark & Batch Processing (31–42)

31. What is Apache Spark and what problem does it solve?
32. Explain RDDs vs DataFrames vs Datasets.
33. What is a Spark job's execution flow (driver → executor)?
34. What is a shuffle and why is it expensive?
35. Explain partitioning in Spark and how skew causes problems.
36. What is broadcast join and when would you use it?
37. How do you tune Spark memory (driver vs executor, JVM heap, overhead)?
38. What is a narrow vs wide transformation?
39. How do you handle small files in a Spark job?
40. Explain checkpointing and why it matters for long-running jobs.
41. How do you make a Spark job idempotent?
42. When would you choose Spark over a simple Python script?

## OLAP & NoSQL Databases (43–55)

43. Why would you choose ClickHouse over a traditional RDBMS for analytics?
44. Explain the ClickHouse MergeTree engine and how data is stored on disk.
45. What are ClickHouse partitions and how do you pick partition keys?
46. Explain ORDER BY vs PARTITION BY in ClickHouse.
47. What is a materialized view in ClickHouse and when do you use it?
48. How do you deduplicate data in ClickHouse (ReplacingMergeTree, FINAL)?
49. What is ArangoDB's multi-model design (documents, graph, key/value)?
50. Explain AQL in ArangoDB and a typical traversal query.
51. When would you model a relationship as an edge in a graph database rather than a foreign key?
52. Explain eventual consistency vs strong consistency in NoSQL stores.
53. When would you choose MongoDB over PostgreSQL?
54. Explain sharding and how it differs from partitioning.
55. How do you migrate data from a relational database to a NoSQL store safely?

## Data Quality, Reliability & Performance (56–65)

56. How do you define and measure data quality? Name the dimensions.
57. How would you implement data validation at ingestion and post-load?
58. Explain data observability: freshness, volume, distribution, and lineage.
59. What metrics do you monitor on a data pipeline?
60. How do you set up alerting for a failing pipeline?
61. What causes a sudden spike in consumer lag, and how do you troubleshoot it?
62. How do you detect a silent data quality regression?
63. Explain SLA vs SLO for a data platform.
64. How do you make a pipeline cost-efficient?
65. What is a data contract and how does it prevent breaking changes?

## Cloud, Containers & CI/CD (66–78)

66. Which AWS services would you use to run a Spark job? Compare EMR, Glue, and ECS.
67. How do you store raw vs curated data in S3?
68. Explain the AWS Glue Data Catalog and its role in Athena.
69. When would you choose Redshift over ClickHouse on AWS?
70. How do you run containerised data jobs on Kubernetes?
71. Explain a CI/CD pipeline for a data engineering project.
72. How do you version and test dbt-style transformation code?
73. What is an Airflow DAG and why do schedulers need a scheduler?
74. Explain the difference between Airflow and a plain cron job.
75. How do you make an Airflow task idempotent and backfillable?
76. How do you manage secrets for data pipelines?
77. How would you run a Spark job on a Kubernetes cluster with dynamic allocation?
78. Explain the difference between Docker and a virtual machine for data workloads.

## Elasticsearch, Search & Visualisation (79–86)

79. What is an inverted index and how does it make search fast?
80. Explain near-real-time indexing in Elasticsearch.
81. How do you design an index for high-cardinality data?
82. What are mappings, and what happens with a mapping conflict?
83. How do you implement log analytics with the ELK stack?
84. Explain aggregations and how they differ from SQL GROUP BY in cost.
85. Which visualisation tools would you use for a data platform dashboard?
86. How do you build a dashboard that answers a business question rather than showing every metric?

## AI on Data Platforms (87–94)

87. What are Generative AI and Agentic AI? How do they differ?
88. What is RAG and when is it better than fine-tuning?
89. How would you use an LLM over a data warehouse without exposing raw data?
90. What is an AI agent and what makes an agent loop safe to run?
91. How do you evaluate the output quality of an LLM pipeline?
92. What are the data privacy concerns when calling an LLM API with customer data?
93. How would you build an agent that answers questions over a ClickHouse database?
94. Explain prompt injection and how you mitigate it in an agentic system.

## System Design, Linux & Behavioural (95–100)

95. Design an end-to-end pipeline: source → Kafka → Spark → ClickHouse → dashboard. Explain every choice.
96. You notice a dashboard shows stale data. How do you debug it?
97. A Spark job is failing intermittently in production. Walk me through your approach.
98. How do you balance innovation (evaluating new technologies) with reliability?
99. Describe a time you collaborated with cross-functional teams on a data challenge. What was your contribution?
100. Why do you want to work on HPE's edge-to-cloud data platform, onsite?

---