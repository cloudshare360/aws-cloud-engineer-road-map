# AWS Serverless Developer Roadmap

This folder contains the learning roadmap for becoming an **AWS Serverless Developer**. The path focuses on building production-grade serverless applications using AWS services, infrastructure as code, and modern development practices.

---

## Target Role

**AWS Serverless Developer** — A specialist who designs, builds, deploys, and maintains serverless applications on AWS using Lambda, API Gateway, DynamoDB, Step Functions, and related services.

### Key Responsibilities
- Build serverless APIs and microservices
- Design event-driven architectures
- Implement workflows with Step Functions
- Optimize serverless applications for performance and cost
- Deploy using IaC and CI/CD pipelines
- Monitor and troubleshoot production serverless systems

---

## Prerequisites

- Basic programming knowledge (JavaScript/Node.js recommended)
- AWS Free Tier account
- Familiarity with cloud computing concepts
- 2-3 hours daily commitment

---

## 16-Week Learning Roadmap

### Phase 1: Serverless Foundations (Weeks 1-4)
- AWS account setup and cost management
- IAM fundamentals for serverless
- Lambda deep dive: runtime, handler, layers, concurrency
- API Gateway: REST APIs, HTTP APIs, stages, deployments
- Building first serverless function

### Phase 2: Data & Storage (Weeks 5-6)
- DynamoDB: tables, partitions, sort keys, GSI/LSI, transactions
- S3: buckets, objects, versioning, lifecycle, event notifications
- RDS Proxy for serverless database connections
- Secrets Manager for credentials

### Phase 3: Integration & Messaging (Weeks 7-8)
- SNS: topics, subscriptions, FIFO topics
- SQS: queues, message visibility, dead-letter queues
- SES: sending emails, templates, configurations
- EventBridge: event buses, rules, schema registry
- Step Functions: state machines, standard vs express

### Phase 4: Advanced Serverless (Weeks 9-12)
- AppSync: GraphQL APIs, resolvers, data sources
- Lambda@Edge and CloudFront Functions
- S3 Select and Glacier
- AWS Amplify for fullstack serverless
- Serverless Framework vs SAM vs CDK

### Phase 5: IaC & CI/CD (Weeks 13-14)
- AWS SAM: templates, commands, local testing
- AWS CDK: constructs, stacks, pipelines
- Serverless Framework: configuration, plugins, stages
- CI/CD for serverless: GitHub Actions, GitLab CI

### Phase 6: Observability & Production (Weeks 15-16)
- CloudWatch: metrics, logs, alarms, dashboards
- X-Ray: tracing, service map, annotations
- Distributed tracing best practices
- Performance optimization and cost monitoring

---

## Roadmap Diagram

See [roadmap-diagram.md](./roadmap-diagram.md) for the visual Mermaid diagram.

---

## Tools & Services

### Core AWS Services
- AWS Lambda
- Amazon API Gateway
- Amazon DynamoDB
- Amazon S3
- Amazon SNS
- Amazon SQS
- Amazon SES
- AWS Step Functions
- Amazon EventBridge
- AWS AppSync
- Amazon RDS Proxy
- AWS Secrets Manager
- Amazon CloudFront
- AWS Amplify

### IaC & Deployment
- AWS SAM
- AWS CDK
- Serverless Framework
- AWS CloudFormation

### CI/CD
- GitHub Actions
- GitLab CI
- AWS CodePipeline

### Observability
- Amazon CloudWatch
- AWS X-Ray
- AWS CloudTrail

---

## Recommended Learning Path

1. Start with [AWS Serverless Developer Guide](https://docs.aws.amazon.com/serverless/)
2. Complete [AWS Serverless Workshop](https://serverlessworkshops.com/)
3. Build projects using [AWS Serverless Hero examples](https://github.com/aws-samples/aws-serverless-workshops)
4. Practice on [AWS Free Tier](https://aws.amazon.com/free/)

---

## Continue To

- **[02-roadmap.md](../docs/02-roadmap.md)** — Full 33-week AWS Cloud Engineer roadmap
- **[03-learning-path.md](../docs/03-learning-path.md)** — Detailed week-by-week curriculum
- **[05-resources.md](../docs/05-resources.md)** — Tools, learning resources, and best practices
