# AWS Cloud Engineer — Committed Role Program

A 20-week training program placing a mid-level AWS Cloud Engineer (6 YOE) into a committed, full-time role backed by a technical expert support layer.

> **New here?** Start with the [Quick Start Guide](./docs/04-quick-start-guide.md) or jump to the [20-week Roadmap](./docs/02-roadmap.md).

---

## Table of Contents

- [Role Overview](#role-overview)
- [Who Should Read What](#who-should-read-what)
- [Training & Ramp-Up](#training--ramp-up)
- [Placement Model](#placement-model)
- [Repository Structure](#repository-structure)
- [Document Index](#document-index)
- [Key Highlights](#key-highlights)

---

## Role Overview

An **AWS Cloud Engineer** designs, builds, deploys, and maintains scalable, secure, and cost-effective cloud infrastructure on AWS. This role combines backend development expertise with cloud infrastructure knowledge to create robust serverless and containerized applications.

### Key Responsibilities

- Build backend services using Node.js, Express.js, and Python
- Build serverless applications using AWS Lambda, API Gateway, and DynamoDB
- Implement infrastructure as code using AWS CDK, CloudFormation, Terraform, and OpenTofu
- Set up CI/CD pipelines using GitLab, GitHub Actions, and Jenkins
- Containerize applications using Docker and orchestrate with ECS/EKS
- Monitor and optimize cloud resources using CloudWatch and X-Ray
- Ensure security and compliance using IAM, Secrets Manager, and AWS best practices
- Collaborate with frontend teams to integrate Angular/React applications

### Technical Skills

| Domain | Technologies |
|--------|-------------|
| **Languages** | JavaScript/TypeScript, Python, Node.js |
| **Backend** | Express.js, AWS Lambda |
| **Frontend** | Angular, React/Next.js |
| **Cloud** | Lambda, API Gateway, DynamoDB, S3, SNS, SQS, SES, Step Functions, RDS, OpenSearch, Athena, AppSync, EC2, ECS, EKS, IAM, Secrets Manager, CloudWatch, X-Ray |
| **IaC** | AWS CDK, CloudFormation, Terraform, OpenTofu |
| **DevOps/CI/CD** | GitLab, GitHub Actions, Jenkins |
| **Testing** | Jest, Chai, Mocha, Sinon |

---

## Who Should Read What

| Reader | Start With | Then Read |
|--------|-----------|-----------|
| **Employer / Client** | [01-role-description.md](./docs/01-role-description.md), [06-three-party-engagement.md](./docs/06-three-party-engagement.md), [07-staff-augmentation-proposal.md](./docs/07-staff-augmentation-proposal.md) | [02-roadmap.md](./docs/02-roadmap.md), [03-learning-path.md](./docs/03-learning-path.md) |
| **Associate / Engineer** | [04-quick-start-guide.md](./docs/04-quick-start-guide.md), [03-learning-path.md](./docs/03-learning-path.md), [02-roadmap.md](./docs/02-roadmap.md) | [05-resources.md](./docs/05-resources.md) |
| **Vendor / Training Company** | [07-staff-augmentation-proposal.md](./docs/07-staff-augmentation-proposal.md), [06-three-party-engagement.md](./docs/06-three-party-engagement.md) | [01-role-description.md](./docs/01-role-description.md), [03-learning-path.md](./docs/03-learning-path.md) |

---

## Training & Ramp-Up

The associate follows a structured **20-week learning roadmap**:

| Weeks | Focus Area | Key Technologies |
|-------|-----------|-----------------|
| 1-4 | Backend Development Foundations | JavaScript, TypeScript, Node.js, Express.js, REST APIs, Python |
| 5-6 | Testing Fundamentals | Jest, Chai, Mocha, Sinon |
| 5-8 | Portfolio Marketing (ongoing) | GitHub, LinkedIn, open source, personal branding |
| 7-8 | Frontend Technologies | Angular, Karma, ReactJS |
| 9-12 | AWS Services | Lambda, API Gateway, DynamoDB, SNS, SQS, SES, Step Functions, S3, RDS, OpenSearch, Athena, AppSync, EC2, Docker, ECS, EKS, IAM, Secrets Manager, CloudWatch, X-Ray |
| 13-14 | Infrastructure as Code | AWS CDK, CloudFormation, Terraform, OpenTofu |
| 15-16 | CI/CD & DevOps | GitLab, GitHub, Jenkins |
| 17-20 | Angular or React/Next.js | Angular Core + Advanced or React/Next.js (client-driven) |

---

## Placement Model

This is a **three-party committed engagement**:

| Party | Role |
|-------|------|
| **Employer (Client)** | Provides project requirements, access, and feedback |
| **Vendor (Training/Support Company)** | Supplies the associate, expert support layer, and training infrastructure |
| **Associate (6 YOE Engineer)** | Delivers development tasks with expert backup and continuous learning |

The associate is embedded in the employer's team as a full member, with technical experts available for architectural guidance, code reviews, and gap remediation. See [06-three-party-engagement.md](./docs/06-three-party-engagement.md) for full details.

---

## Repository Structure

```
.
├── readme.md                         # Root index (this file)
├── docs/                             # GitHub Pages (01-07*.md + index.html + README.md)
├── .kilo/                            # Agent config (skills, memory, tasks, kilo.json)
├── .devcontainer/                     # Codespaces config
├── .github/workflows/pages.yml       # Pages deployment
└── aws-cloud-engineer/
    ├── node-js/                     # Node.js learning path
    ├── angular/                     # Frontend resources
    ├── react/                       # Frontend resources
    ├── dev-ops/                     # DevOps learning materials
    │   ├── ci-cd/                   # GitLab, GitHub Actions, Jenkins
    │   └── iac/                     # CloudFormation, CDK, Terraform, OpenTofu
    └── aws-services/                # 82 AWS services organized by domain
        ├── analytics/
        │   ├── athena
        │   ├── datapipeline
        │   ├── emr
        │   ├── glue
        │   ├── kinesis
        │   ├── kinesis-data-analytics
        │   ├── kinesis-firehose
        │   ├── kinesis-video-streams
        │   ├── opensearch
        │   ├── quicksight
        │   └── timestream
        ├── application-integration/
        │   ├── api-gateway
        │   ├── appsync
        │   ├── eventbridge
        │   ├── mq
        │   ├── ses
        │   ├── sns
        │   ├── sqs
        │   └── stepfunction
        ├── compute/
        │   ├── ec2
        │   └── lambda
        ├── containers/
        │   ├── appmesh
        │   ├── ecr
        │   ├── ecs
        │   └── eks
        ├── database/
        │   ├── documentdb
        │   ├── dynamodb
        │   ├── elasticache
        │   ├── keyspaces
        │   ├── neptune
        │   ├── rds
        │   └── redshift
        ├── developer-tools/
        │   ├── cloud9
        │   ├── cloudformation
        │   ├── cloudshell
        │   ├── codebuild
        │   ├── codecommit
        │   ├── codedeploy
        │   └── codepipeline
        ├── iot/
        │   ├── iot-analytics
        │   ├── iot-core
        │   └── iot-device-defender
        ├── machine-learning/
        │   ├── bedrock
        │   ├── comprehend
        │   ├── forecast
        │   ├── lookout
        │   ├── polly
        │   ├── rekognition
        │   ├── sagemaker
        │   ├── textract
        │   ├── transcribe
        │   └── translate
        ├── management-governance/
        │   ├── cloudwatch
        │   ├── config
        │   ├── systems-manager
        │   └── trustedadvisor
        ├── migration-transfer/
        │   ├── application-discovery-service
        │   ├── database-migration-service
        │   ├── migration-hub
        │   ├── server-migration-service
        │   └── transfer-family
        ├── networking-content-delivery/
        │   ├── acm
        │   ├── cloud-map
        │   ├── cloudfront
        │   ├── direct-connect
        │   ├── elb
        │   ├── global-accelerator
        │   ├── route53
        │   └── vpc
        ├── security-identity-compliance/
        │   ├── cloudtrail
        │   ├── cognito
        │   ├── guardduty
        │   ├── iam
        │   ├── inspector
        │   ├── kms
        │   ├── organizations
        │   ├── secrets-manager
        │   ├── shield
        │   ├── vpn-cloudhsm
        │   └── waf
        ├── serverless-application-repository/
        └── storage/
            └── s3
```

---

## Document Index

| # | Document | Purpose | Reading Order |
|---|----------|---------|---------------|
| 01 | [Role Description](./docs/01-role-description.md) | Responsibilities, skills, and success criteria | Employer → Vendor → Associate |
| 02 | [Roadmap](./docs/02-roadmap.md) | 20-week learning roadmap and skill progression | After 01 |
| 03 | [Learning Path](./docs/03-learning-path.md) | Detailed week-by-week curriculum and deliverables | After 02 |
| 04 | [Quick Start Guide](./docs/04-quick-start-guide.md) | Daily routine, project ideas, and success metrics | Associate start here |
| 05 | [Resources](./docs/05-resources.md) | Tools, learning resources, best practices, and interview prep | After 03 |
| 06 | [Three-Party Engagement](./docs/06-three-party-engagement.md) | Engagement model, SLA, responsibilities, shared compensation | Employer/Vendor start here |
| 07 | [Staff Augmentation Proposal](./docs/07-staff-augmentation-proposal.md) | Executive proposal for resource engagement | Decision-makers |

### Recommended Reading Paths

- **Associate**: 04 → 03 → 02 → 05
- **Employer**: 01 → 06 → 07 → 02
- **Vendor**: 07 → 06 → 01 → 03

---

## Key Highlights

| Attribute | Details |
|-----------|---------|
| **Experience Level** | Mid-level developer with 6 years of professional experience |
| **Engagement Type** | Committed, full-time role with long-term growth path |
| **Support Model** | Technical expert layer for architectural guidance, code reviews, and gap remediation |
| **Training** | Structured 20-week learning roadmap with weekly milestones |
| **Delivery** | Backend-first, then AWS services, then frontend based on client needs |
| **Tools** | Node.js, Express.js, Python, Angular/React, AWS CDK, Terraform, OpenTofu, GitLab/GitHub/Jenkins |

---

*GitHub Pages documentation hosted at `/docs`. See [.github/workflows/pages.yml](./.github/workflows/pages.yml) for deployment configuration.*
