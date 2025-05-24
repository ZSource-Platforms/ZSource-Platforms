# ZSource-Platforms

A scalable, Twitter-like backend system built as an academic proof-of-concept.

## Overview

ZSource-Platforms demonstrates a fault-tolerant, high-throughput microservice architecture for social-media style “tweet” ingestion and retrieval. It showcases:

- **Serverless Ingestion:** AWS SQS publish new messages into AWS Lambda functions.
- **Decoupled Processing:** Create (write) and Read operations run on separate EC2 instances behind ELBs for isolation and scalability.
- **Caching Layer:** Redis accelerates timeline reads and hot data access, reducing load on the primary database.
- **NoSQL Storage:** DynamoDB tables were used and sample data was generated via public APIs and pre-seeded into the database to simulate real-world workloads.
- **API Fronting:** Express API Gateway and Elastic Load Balancers handle RESTful traffic at scale.
- **Load-Tested Performance:** Validated for 10,000 requests/sec throughput under test.

## Architecture

![ZSource-Platforms Architecture](https://github.com/user-attachments/assets/00b64d0f-3c97-46eb-a3eb-a00d3d0989ff)

## Academic Project

This implementation was developed as part of an academic coursework. The codebase is available upon request, please open an issue or contact the author for access.
