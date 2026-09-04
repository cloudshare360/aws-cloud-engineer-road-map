---
layout: default
---

# AWS Cloud Engineer - Learning Roadmap Diagrams

This document contains visual diagrams for the 33-week learning roadmap. These diagrams render natively in GitHub, GitLab, and most Markdown viewers.

---

## Learning Path Flowchart

```mermaid
flowchart TD
    Start([Start: Fresher with No Programming Background]) --> Phase1[Phase 1: MEAN Stack<br/>Weeks 1-4<br/>MongoDB, Express.js, Angular, Node.js]
    
    Phase1 --> Phase2[Phase 2: MERN Stack<br/>Weeks 5-8<br/>MongoDB, Express.js, React.js, Node.js]
    
    Phase2 --> Phase3[Phase 3: Python Fundamentals<br/>Weeks 9-10<br/>Python, Flask, FastAPI]
    
    Phase3 --> Phase4[Phase 4: Java Fundamentals<br/>Weeks 11-12<br/>Java, Spring Boot]
    
    Phase4 --> Phase5[Phase 5: .NET / C# Fundamentals<br/>Weeks 13-14<br/>C#, ASP.NET Core]
    
    Phase5 --> Phase6[Phase 6: Testing Fundamentals<br/>Weeks 15-17<br/>Jest, Mocha, Chai, Sinon, Cucumber, Playwright]
    
    Phase6 --> Phase7[Phase 7: Frontend Development<br/>Weeks 18-21<br/>Angular, React/Next.js, Vue.js]
    
    Phase7 --> Phase8[Phase 8: AWS Fundamentals & Serverless<br/>Weeks 22-25<br/>Lambda, API Gateway, DynamoDB, S3, RDS, SNS, SQS, SES, Step Functions]
    
    Phase8 --> Phase9[Phase 9: AWS Advanced Services<br/>Weeks 26-29<br/>EC2, Docker, App Runner, ECS, EKS, IAM, CloudWatch, X-Ray, OpenSearch, Athena]
    
    Phase9 --> Phase10[Phase 10: Infrastructure as Code<br/>Weeks 30-31<br/>CloudFormation, AWS CDK, Terraform, OpenTofu]
    
    Phase10 --> Phase11[Phase 11: CI/CD & DevOps<br/>Weeks 32-33<br/>GitLab CI/CD, Jenkins, GitHub Actions]
    
    Phase11 --> MultiCloud[Multi-Cloud Expansion<br/>Post-AWS Mastery<br/>Azure, GCP, Multi-Cloud Architecture]
    
    MultiCloud --> End([End: Full-Stack AWS Cloud Serverless Engineer<br/>Ready for Production Delivery])
    
    style Start fill:#4CAF50,color:#fff
    style End fill:#2196F3,color:#fff
    style Phase8 fill:#FF9800,color:#fff
    style Phase9 fill:#FF9800,color:#fff
    style Phase10 fill:#9C27B0,color:#fff
    style Phase11 fill:#9C27B0,color:#fff
    style MultiCloud fill:#00BCD4,color:#fff
```

---

## 33-Week Timeline Gantt Chart

```mermaid
gantt
    title AWS Cloud Engineer - 33-Week Learning Roadmap
    dateFormat  YYYY-MM-DD
    section Fullstack Foundations
    MEAN Stack                          :a1, 2026-01-05, 4w
    MERN Stack                          :a2, after a1, 4w
    section Backend Languages
    Python Fundamentals                 :b1, after a2, 2w
    Java Fundamentals                   :b2, after b1, 2w
    .NET / C# Fundamentals              :b3, after b2, 2w
    section Testing
    Unit & Integration Testing          :c1, after b3, 3w
    section Frontend Mastery
    Angular Advanced                    :d1, after c1, 1w
    React / Next.js Advanced            :d2, after d1, 1w
    Vue.js Fundamentals                 :d3, after d2, 1w
    Frontend Testing & Integration      :d4, after d3, 1w
    section AWS Core
    AWS Fundamentals & Serverless       :e1, after d4, 4w
    section AWS Advanced
    Containers, EC2, VPC                :f1, after e1, 4w
    Monitoring, Databases, GraphQL      :f2, after f1, 4w
    section IaC & DevOps
    Infrastructure as Code              :g1, after f2, 2w
    CI/CD & DevOps                      :g2, after g1, 2w
    section Expansion
    Multi-Cloud (Azure, GCP)            :h1, after g2, 2w
```

---

## Technology Stack Mindmap

```mermaid
mindmap
    root((AWS Cloud Engineer))
        Fullstack Foundations
            MEAN Stack
                MongoDB
                Express.js
                Angular
                Node.js
            MERN Stack
                MongoDB
                Express.js
                React.js
                Node.js
        Backend Languages
            Python
                Flask
                FastAPI
                boto3
            Java
                Spring Boot
                Maven/Gradle
            C#
                ASP.NET Core
                Entity Framework
        Testing
            Unit Testing
                Jest
                Mocha
                Chai
                Sinon
            Integration Testing
                Cucumber
                Gherkin
            Functional Testing
                Playwright
                POM
        Frontend Frameworks
            Angular
                RxJS
                NgRx
                Material
            React
                Next.js
                Redux Toolkit
                React Query
            Vue.js
                Vue Router
                Pinia
                Composition API
        AWS Core Services
            Compute
                Lambda
                EC2
                App Runner
                ECS
                EKS
            Storage
                S3
                EBS
                EFS
            Database
                DynamoDB
                RDS
                OpenSearch
                Athena
            Integration
                API Gateway
                SNS
                SQS
                SES
                Step Functions
                AppSync
            Security
                IAM
                Secrets Manager
                Cognito
                GuardDuty
            Monitoring
                CloudWatch
                X-Ray
                CloudTrail
        IaC & DevOps
            IaC Tools
                CloudFormation
                AWS CDK
                Terraform
                OpenTofu
            CI/CD
                GitLab CI
                GitHub Actions
                Jenkins
            Containers
                Docker
                Docker Compose
                ECR
        Multi-Cloud
            Azure
                Compute
                Storage
                Databases
                Networking
            GCP
                Compute Engine
                GKE
                Cloud Storage
                BigQuery
```

---

## Skill Progression Timeline

```mermaid
timeline
    title AWS Cloud Engineer Skill Progression Timeline
    
    section Weeks 1-4
        MEAN Stack : MongoDB CRUD<br/>Express.js APIs<br/>Angular Components<br/>Node.js Runtime
    section Weeks 5-8
        MERN Stack : React Hooks<br/>State Management<br/>MongoDB Integration<br/>Fullstack Deployment
    section Weeks 9-10
        Python : Flask/FastAPI<br/>boto3 AWS SDK<br/>Scripting & Automation<br/>Lambda Functions
    section Weeks 11-12
        Java : Spring Boot<br/>JPA/Hibernate<br/>REST Controllers<br/>Build Tools
    section Weeks 13-14
        .NET/C# : ASP.NET Core<br/>Entity Framework<br/>Dependency Injection<br/>Web APIs
    section Weeks 15-17
        Testing : Jest Unit Tests<br/>Mocha/Chai<br/>Sinon Mocks<br/>Cucumber BDD<br/>Playwright E2E
    section Weeks 18-21
        Frontend : Angular Advanced<br/>React/Next.js<br/>Vue.js 3<br/>State Management<br/>Testing
    section Weeks 22-25
        AWS Core : IAM & Security<br/>Lambda & API Gateway<br/>DynamoDB & S3<br/>RDS & Secrets<br/>SNS/SQS/SES<br/>Step Functions
    section Weeks 26-29
        AWS Advanced : EC2 & VPC<br/>Docker & ECS/EKS<br/>App Runner<br/>CloudWatch & X-Ray<br/>OpenSearch & Athena<br/>AppSync GraphQL
    section Weeks 30-31
        IaC : CloudFormation<br/>AWS CDK<br/>Terraform<br/>OpenTofu
    section Weeks 32-33
        DevOps : GitLab CI<br/>Jenkins<br/>GitHub Actions<br/>Blue/Green Deploy<br/>Security Scanning
    section Post-33
        Multi-Cloud : Azure Fundamentals<br/>GCP Fundamentals<br/>Multi-Cloud Patterns<br/>Cloud-Agnostic IaC
```

---

## Phase Dependency Graph

```mermaid
flowchart LR
    subgraph Phase1[Phase 1: MEAN Stack]
        P1_M[MongoDB]
        P1_E[Express.js]
        P1_A[Angular]
        P1_N[Node.js]
    end
    
    subgraph Phase2[Phase 2: MERN Stack]
        P2_M[MongoDB]
        P2_E[Express.js]
        P2_R[React.js]
        P2_N[Node.js]
    end
    
    subgraph Phase3[Phase 3: Python]
        P3_Py[Python]
        P3_F[Flask]
        P3_Fa[FastAPI]
        P3_B[boto3]
    end
    
    subgraph Phase4[Phase 4: Java]
        P4_J[Java]
        P4_SB[Spring Boot]
        P4_JPA[JPA]
    end
    
    subgraph Phase5[Phase 5: .NET]
        P5_C[C#]
        P5_ASPNET[ASP.NET Core]
        P5_EF[Entity Framework]
    end
    
    subgraph Phase6[Phase 6: Testing]
        P6_J[Jest]
        P6_M[Mocha/Chai]
        P6_S[Sinon]
        P6_C[Cucumber]
        P6_P[Playwright]
    end
    
    subgraph Phase7[Phase 7: Frontend]
        P7_A[Angular Advanced]
        P7_R[React/Next.js]
        P7_V[Vue.js]
    end
    
    subgraph Phase8[Phase 8: AWS Core]
        P8_L[Lambda]
        P8_AG[API Gateway]
        P8_D[DynamoDB]
        P8_S3[S3]
        P8_RDS[RDS]
        P8_SNS[SNS/SQS/SES]
        P8_SF[Step Functions]
    end
    
    subgraph Phase9[Phase 9: AWS Advanced]
        P9_EC2[EC2]
        P9_Docker[Docker]
        P9_ECS[ECS/EKS]
        P9_IAM[IAM]
        P9_CW[CloudWatch]
    end
    
    subgraph Phase10[Phase 10: IaC]
        P10_CF[CloudFormation]
        P10_CDK[AWS CDK]
        P10_TF[Terraform]
        P10_OT[OpenTofu]
    end
    
    subgraph Phase11[Phase 11: DevOps]
        P11_GL[GitLab CI]
        P11_JK[Jenkins]
        P11_GH[GitHub Actions]
    end
    
    Phase1 --> Phase2
    Phase2 --> Phase3
    Phase3 --> Phase4
    Phase4 --> Phase5
    Phase5 --> Phase6
    Phase6 --> Phase7
    Phase7 --> Phase8
    Phase8 --> Phase9
    Phase9 --> Phase10
    Phase10 --> Phase11
    
    P8_L -.-> P10_CDK
    P8_D -.-> P10_CF
    P9_ECS -.-> P11_GL
    P6_P -.-> P7_A
    P6_P -.-> P7_R
    P6_P -.-> P7_V
```

---

## Role Focus Areas

```mermaid
graph TB
    subgraph Core[Full-Stack AWS Cloud Serverless Engineer]
        direction TB
        
        subgraph FE[Frontend - Angular First]
            Angular[Angular]
            RxJS[RxJS]
            NgRx[NgRx]
            Material[Angular Material]
        end
        
        subgraph BE[Backend - Node.js First]
            NodeJS[Node.js]
            Express[Express.js]
            TypeScript[TypeScript]
            Python[Python]
            Flask[Flask/FastAPI]
            Java[Java/Spring Boot]
            DotNet[C#/ASP.NET]
        end
        
        subgraph Cloud[AWS Cloud - First Focus]
            Lambda[AWS Lambda]
            APIGW[API Gateway]
            DynamoDB[DynamoDB]
            RDS[RDS]
            S3[S3]
            SNS[SNS/SQS/SES]
            StepFn[Step Functions]
        end
        
        subgraph Containers[Containers]
            Docker[Docker]
            AppRunner[App Runner]
            ECS[ECS]
            EKS[EKS]
        end
        
        subgraph IaC[Infrastructure as Code]
            CF[CloudFormation]
            CDK[AWS CDK]
            TF[Terraform]
            OT[OpenTofu]
        end
        
        subgraph DevOps[CI/CD & DevOps]
            GitLab[GitLab CI/CD]
            Jenkins[Jenkins]
            GH[GitHub Actions]
        end
        
        subgraph Testing[Testing]
            Jest[Jest]
            Mocha[Mocha/Chai]
            Cucumber[Cucumber]
            Playwright[Playwright]
        end
        
        subgraph Expansion[Post-AWS Expansion]
            Azure[Azure]
            GCP[GCP]
            MultiCloud[Multi-Cloud]
        end
    end
    
    FE --> Cloud
    BE --> Cloud
    Cloud --> Containers
    Cloud --> IaC
    IaC --> DevOps
    Testing --> FE
    Testing --> BE
    DevOps --> Cloud
    Cloud --> Expansion
    
    style Core fill:#1976D2,color:#fff
    style Cloud fill:#FF9800,color:#fff
    style IaC fill:#9C27B0,color:#fff
    style DevOps fill:#9C27B0,color:#fff
    style Expansion fill:#00BCD4,color:#fff
```

---

## How to Use These Diagrams

### In GitHub/GitLab
These Mermaid diagrams render automatically in Markdown files on GitHub and GitLab.

### In VS Code
Install the [Markdown Preview Mermaid](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid) extension to preview diagrams.

### Export as Image
Use the [Mermaid CLI](https://github.com/mermaid-js/mermaid-cli) to export diagrams:
```bash
npx @mermaid-js/mermaid-cli mmdc -i diagram-file.md -o output.png
```

### Edit Diagrams
Use the [Mermaid Live Editor](https://mermaid.live) for interactive editing.

---

## Continue To

- **[02-roadmap](./02-roadmap.html)** — 33-week structured learning roadmap
- **[03-learning-path](./03-learning-path.html)** — Detailed week-by-week curriculum with objectives and deliverables
- **[01-role-description](./01-role-description.html)** — Role responsibilities and success criteria
