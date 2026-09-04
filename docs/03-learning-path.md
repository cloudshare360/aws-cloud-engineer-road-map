---
layout: default
---

# AWS Cloud Engineer - Detailed Learning Path

## Overview
This document provides a comprehensive 33-week learning path with **three parallel tracks**:

- **Track A: Fullstack Development** — MEAN/MERN, Python, Java, .NET, Frontend
- **Track B: Git & Version Control** — GitHub/GitLab workflows, branching, PRs, portfolio building
- **Track C: CI/CD & DevOps** — GitLab CI, Jenkins, GitHub Actions, automated pipelines

**Key Principle**: Every hands-on lab is committed to GitHub and automated through CI/CD. You learn by building and shipping code, not just watching tutorials.

---

## Week 1-2: Foundations

### Track A: MEAN Stack — MongoDB & Node.js
- MongoDB basics: documents, collections, CRUD operations
- Node.js architecture and event loop
- npm and package management
- File system (fs) module
- Environment variables: dotenv
- Connecting Node.js to MongoDB with Mongoose

**Hands-on**: Build a Node.js CLI that connects to MongoDB and performs CRUD operations.

### Track B: Git & GitHub
- What is Git? Why version control matters
- Git installation and configuration
- Git basics: init, add, commit, push, pull
- GitHub account setup and first repository
- README.md best practices
- .gitignore essentials

**Hands-on**: Create GitHub account. Initialize first repo. Push Node.js CLI lab with professional README.

### Track C: CI/CD Fundamentals
- What is CI/CD? Why automate?
- GitHub Actions basics
- Your first workflow file (.github/workflows)
- Understanding jobs, steps, and actions
- Running tests automatically on push

**Hands-on**: Create first GitHub Actions workflow that runs on every push. Automate linting.

---

## Week 3-4: MEAN Stack + Git Branching

### Track A: MEAN Stack — Express.js & REST APIs
- Express setup: app, middleware, routing
- Request/response objects (req, res)
- Middleware: custom, third-party (cors, helmet, morgan)
- RESTful API design (GET, POST, PUT, DELETE, PATCH)
- Status codes, JSON responses
- Validation basics (Joi/Zod)

**Hands-on**: Build a CRUD API for "Task Manager" with MongoDB storage. Push to GitHub.

### Track B: Git Branching & Collaboration
- Branching strategies: GitFlow, GitHub Flow, Trunk-Based
- Creating and switching branches
- Pull requests and code reviews
- Merge vs rebase
- Resolving merge conflicts
- GitHub: Issues, Projects

**Hands-on**: Create feature branches for Task Manager API. Open PRs. Practice merge conflict resolution.

### Track C: Testing in CI/CD
- Introduction to testing: unit vs integration vs E2E
- Jest setup and configuration
- Writing test cases for Node.js
- Running tests in GitHub Actions
- Code coverage reporting

**Hands-on**: Add Jest tests to Task Manager API. Configure CI to run tests automatically.

---

## Week 5-6: MERN Stack + Portfolio Building

### Track A: MERN Stack — React.js Fundamentals
- JSX, components, props
- State: useState, useEffect
- Component lifecycle (useEffect cleanup)
- Conditional rendering, lists/keys
- Forms and controlled components
- React Router: BrowserRouter, Routes, Route, Link
- Axios for API calls
- Error boundaries

**Hands-on**: Build React frontend for Task Manager API. Push to GitHub.

### Track B: Portfolio Development
- GitHub profile optimization
- Pinned repositories
- Project documentation standards
- Writing great READMEs: description, installation, usage, screenshots
- LinkedIn profile creation

**Hands-on**: Update portfolio READMEs with screenshots and deployment links. Create LinkedIn profile.

### Track C: Build Automation
- Building applications in CI
- Creating Docker images
- Dockerfile best practices
- Pushing to Docker Hub or GitHub Container Registry
- Multi-stage builds

**Hands-on**: Automate Docker image build for Task Manager API. Push to container registry.

---

## Week 7-8: MERN Integration + Advanced Git

### Track A: MERN Stack — Integration & State Management
- Connecting React to Express/MongoDB backend
- Authentication flow in React
- Protected routes
- File upload with Multer
- Error handling and loading states
- Redux Toolkit for state management
- React Query for server state

**Hands-on**: Complete MERN stack application with auth and file upload. Deploy to production.

### Track B: Advanced Git
- Advanced Git: cherry-pick, bisect, reflog, stash
- Git hooks (Husky) for pre-commit linting
- Semantic versioning and tags
- Release management on GitHub/GitLab
- CODEOWNERS and branch protection rules

**Hands-on**: Set up Husky pre-commit hooks. Create semantic version tags. Enable branch protection.

### Track C: Deployment Automation
- Deploying to AWS (EC2, S3, Lambda)
- Environment-specific deployments
- Secrets management in CI/CD
- Rollback strategies
- Blue/Green and Canary deployments

**Hands-on**: Automate deployment of MERN app to AWS. Implement Blue/Green deployment.

---

## Week 9-10: Python + Build Automation

### Track A: Python Fundamentals
- Installation, virtual environments, pip
- Variables, data types, type hints
- Control flow, loops, functions
- Data structures: lists, dicts, sets, tuples
- List comprehensions, lambda functions
- File I/O, JSON handling
- Exception handling: try/except/finally

**Hands-on**: Build a CLI todo app in Python. Parse a CSV file and generate summary stats.

### Track A+: Python Web & AWS
- Flask basics: routes, request/response, templates
- FastAPI basics: async routes, validation, OpenAPI docs
- boto3: AWS SDK for Python
- Lambda functions in Python
- S3 operations with boto3
- SES email sending with boto3

**Hands-on**: Build a Flask/FastAPI API that uploads files to S3 and sends emails via SES.

### Track B: Monorepo Management
- What is a monorepo?
- Organizing multiple projects in one repo
- GitHub Projects for project management
- Documentation standards across projects

**Hands-on**: Organize all previous projects into a monorepo structure.

### Track C: Advanced CI/CD
- Matrix builds for multiple environments
- Caching dependencies for faster builds
- Artifact management
- Conditional workflows
- Scheduled workflows

**Hands-on**: Set up matrix build for testing on multiple Node.js versions.

---

## Week 11-12: Java + Containerization

### Track A: Java Fundamentals
- JDK installation, IDE setup (IntelliJ IDEA)
- Variables, primitives, objects
- Control flow, loops
- OOP: classes, objects, inheritance, polymorphism, encapsulation, abstraction
- Collections Framework: List, Set, Map, Queue
- Exception handling: try/catch/finally, custom exceptions
- Generics, Streams API (filter, map, collect)

**Hands-on**: Build a student management system with CRUD operations using Collections.

### Track A+: Spring Boot
- Maven/Gradle basics
- Spring Boot project setup (Spring Initializr)
- REST controllers (@RestController, @GetMapping, @PostMapping)
- Service layer, Repository pattern
- Spring Data JPA: entities, repositories
- Application properties, profiles

**Hands-on**: Build a Spring Boot REST API for "Product Catalog" with H2 database.

### Track B: Git Advanced
- Git submodules and subtrees
- Git worktree for parallel development
- Large file storage with Git LFS
- Signed commits and tags

**Hands-on**: Add Java projects to monorepo. Practice Git worktree for parallel development.

### Track C: Docker in CI/CD
- Docker fundamentals: images, containers, Dockerfile
- Multi-stage builds for optimization
- Docker Compose for multi-container apps
- Pushing images to ECR/GitHub Container Registry
- Image scanning for vulnerabilities

**Hands-on**: Create Dockerfile for Java Spring Boot app. Automate image build and push in CI.

---

## Week 13-14: .NET/C# + IaC Basics

### Track A: .NET / C# Fundamentals
- .NET SDK installation, IDE setup (Visual Studio / Rider)
- Variables, data types, nullable types
- Control flow, loops, switch expressions
- OOP: classes, interfaces, inheritance, polymorphism
- Collections: List, Dictionary, HashSet
- LINQ for data querying
- Exception handling: try/catch/finally
- File I/O and JSON serialization

**Hands-on**: Build a console-based inventory management system with file persistence.

### Track A+: ASP.NET Core
- ASP.NET Core project setup
- Controllers and routing
- Dependency Injection
- Entity Framework Core for data access
- Building RESTful APIs
- Middleware and filters
- Authentication with JWT
- Swagger/OpenAPI documentation

**Hands-on**: Build an ASP.NET Core Web API for "Order Management" with EF Core.

### Track B: GitOps & Documentation
- GitOps principles
- Documentation as code
- Automated README generation
- Changelog automation with semantic commits

**Hands-on**: Implement automated changelog generation in CI/CD pipeline.

### Track C: Infrastructure Basics
- Infrastructure as Code concepts
- CloudFormation basics: templates, stacks
- YAML/JSON template structure
- Deploying infrastructure through CI/CD

**Hands-on**: Create CloudFormation template for a simple S3 bucket. Deploy via GitHub Actions.

---

## Week 15-17: Testing Mastery

### Track A: Testing Across Stacks
- Testing concepts: unit vs integration vs E2E
- Jest setup: describe, it, expect, matchers
- Mocha: BDD/TDD style, Chai assertions
- Sinon: spies, stubs, mocks, fake timers
- Code coverage: Istanbul/NYC
- Cucumber: BDD, Gherkin syntax
- Playwright: browser automation, POM

**Hands-on**: Write comprehensive test suites for Node.js, Python, and Java projects.

### Track B: Portfolio Expansion
- Creating project showcases
- Writing technical blog posts
- GitHub profile README with stats and contributions
- Contributing to open source

**Hands-on**: Write blog post about testing journey. Contribute to an open source project.

### Track C: Test Automation in CI/CD
- Running all test types in CI
- Parallel test execution
- Test reporting and artifacts
- Flaky test detection and retry
- Performance testing basics

**Hands-on**: Configure CI to run unit, integration, and E2E tests in parallel. Generate test reports.

---

## Week 18-21: Frontend Mastery

### Track A: Angular Advanced
- Angular Services & Dependency Injection
- RxJS fundamentals (Observables, Operators)
- Reactive Forms and validation
- Angular Router configuration
- Route guards (CanActivate, CanDeactivate)
- Lazy loading modules
- NgRx for state management
- Material Design / Angular Material

**Hands-on**: Build complete Angular app with NgRx state management and Material UI.

### Track A+: React Advanced & Next.js
- Context API for global state
- Redux Toolkit for state management
- React Query / TanStack Query for server state
- Next.js framework (SSR, SSG, API Routes)
- Routing with Next.js
- Data fetching strategies
- Deployment and optimization

**Hands-on**: Build Next.js application with API routes, SSR, and deployment.

### Track A++: Vue.js Fundamentals
- Vue.js 3 Composition API
- Vue CLI and project structure
- Components, props, and emits
- Reactive data with ref and reactive
- Vue Router for navigation
- State management with Pinia
- Axios for API integration

**Hands-on**: Build Vue.js application with Pinia state management and routing.

### Track B: Frontend Portfolio
- Deploying frontend apps to production
- Creating demo videos
- Writing case studies for projects
- GitHub Pages for frontend projects

**Hands-on**: Deploy Angular, React, and Vue apps. Create demo videos and case studies.

### Track C: Frontend CI/CD
- Building frontend apps in CI
- Running frontend tests in CI
- Deploying to S3/CloudFront/Amplify
- Preview deployments for PRs
- Cache optimization for faster builds

**Hands-on**: Set up CI/CD for Angular, React, and Vue apps with preview deployments.

---

## Week 22-25: AWS Fundamentals & Serverless

### Track A: AWS Core Services
- AWS Free Tier setup and cost guardrails
- IAM: users, groups, roles, policies, MFA, least privilege
- AWS Lambda: runtime, handler, layers, environment variables
- Amazon API Gateway: REST APIs, HTTP APIs, stages, deployments
- Amazon DynamoDB: tables, partitions, sort keys, GSI/LSI
- Amazon S3: buckets, objects, versioning, lifecycle policies
- Amazon RDS: PostgreSQL setup, parameter groups, backups
- Secrets Manager: storing DB credentials

**Hands-on**: Build serverless CRUD API with Lambda, API Gateway, and DynamoDB.

### Track A+: Integration & Messaging
- Amazon SNS: topics, subscriptions, FIFO topics
- Amazon SQS: queues, message visibility, dead-letter queues
- Amazon SES: sending emails, templates, configurations
- AWS Step Functions: state machines, standard vs express
- EventBridge: event buses, rules, schema registry

**Hands-on**: Build an order processing workflow with Step Functions. Trigger Lambda from S3 upload and send email via SES.

### Track B: Git for Infrastructure
- Git workflow for infrastructure code
- Branching strategies for IaC
- Code review process for infrastructure
- Environment branches (dev/staging/prod)

**Hands-on**: Set up Git workflow for AWS infrastructure code.

### Track C: CI/CD for AWS
- Deploying to AWS via CI/CD
- AWS credentials in CI/CD
- Deploying Lambda functions via CI/CD
- Deploying infrastructure via CI/CD
- Rollback automation

**Hands-on**: Automate deployment of serverless app to AWS using GitHub Actions.

---

## Week 26-29: AWS Advanced Services

### Track A: Containers & Advanced Compute
- Docker fundamentals: images, containers, Dockerfile
- Amazon ECR: registries, repositories, image scanning
- Amazon App Runner: simplified container deployment
- Amazon ECS: task definitions, services, Fargate
- Amazon EKS: clusters, node groups, kubectl basics
- Amazon EC2: instances, AMIs, key pairs, security groups
- Amazon VPC: subnets, route tables, NAT gateways, IGW

**Hands-on**: Containerize Task Manager API. Deploy to ECS Fargate and App Runner.

### Track A+: Monitoring & Databases
- Amazon CloudWatch: metrics, logs, alarms, dashboards
- AWS X-Ray: service map, traces, annotations
- Amazon OpenSearch: indices, queries, Kibana
- AWS Glue: ETL basics, crawlers
- AWS Athena: querying S3 with SQL
- AWS AppSync: GraphQL APIs, resolvers, data sources

**Hands-on**: Set up CloudWatch dashboard for Lambda metrics. Enable X-Ray tracing. Query S3 data with Athena.

### Track B: Advanced Git Workflows
- Trunk-based development
- Feature flags in Git
- Git bisect for bug hunting
- Automated release notes
- Git tags for versioning

**Hands-on**: Implement trunk-based development with feature flags. Automate release notes.

### Track C: Advanced CI/CD
- Multi-stage pipelines
- Matrix builds for multi-AZ deployments
- Automated security scanning (Trivy, Snyk)
- Performance testing in CI
- Notification integrations (Slack, Teams)

**Hands-on**: Implement security scanning in CI/CD pipeline. Add Slack notifications for deployments.

---

## Week 30-31: Infrastructure as Code

### Track A: IaC Tools
- CloudFormation: templates, stacks, change sets
- AWS CDK: constructs, stacks, apps
- CDK Pipelines for CI/CD
- Terraform: HCL syntax, providers, resources
- OpenTofu: Terraform alternative

**Hands-on**: Deploy VPC + ECS + RDS using CloudFormation, CDK, Terraform, and OpenTofu.

### Track B: GitOps for IaC
- GitOps principles and workflows
- Automated IaC deployment from Git
- Drift detection and remediation
- Infrastructure testing in CI

**Hands-on**: Implement GitOps workflow for infrastructure changes. Automate drift detection.

### Track C: IaC in CI/CD
- Automating infrastructure deployment
- Infrastructure testing in pipelines
- Policy as Code (OPA, Checkov)
- Automated rollback for infrastructure failures

**Hands-on**: Build CI/CD pipeline that deploys infrastructure and runs policy checks.

---

## Week 32-33: Production DevOps

### Track A: DevOps Practices
- Multi-stage deployments
- Blue/Green and Canary deployments
- Infrastructure provisioning automation
- Security scanning in pipelines
- Monitoring and alerting in CI/CD

**Hands-on**: Build complete CI/CD pipeline: lint → test → build → deploy to AWS.

### Track B: Portfolio Finalization
- GitHub profile final polish
- Writing case studies for all projects
- Recording demo videos
- Blog posts about learnings
- Resume and LinkedIn updates

**Hands-on**: Record demo videos for 3 major projects. Publish blog post about CI/CD journey.

### Track C: Production-Grade CI/CD
- Complete CI/CD pipeline for a project
- Automated deployment to AWS
- Automated testing in pipeline
- Security scanning in pipeline
- Documentation of deployment process

**Hands-on**: Complete production-grade CI/CD pipeline with all quality gates.

---

## Integrated Learning Flow

```
Week 1-4: MEAN Stack
├── Learn: MongoDB, Express, Angular, Node.js
├── Git: Init repo, commit after each concept, push daily
├── CI/CD: First workflow, automated linting
└── Deploy: Render/Railway/AWS

Week 5-8: MERN Stack
├── Learn: React, Redux, MERN integration
├── Git: Feature branches, PRs, code reviews
├── CI/CD: Test automation, coverage reports
└── Deploy: Production deployment with Blue/Green

Week 9-14: Backend Languages
├── Learn: Python, Java, .NET
├── Git: Monorepo, advanced workflows, GitOps
├── CI/CD: Docker builds, matrix builds, IaC
└── Deploy: Multi-language deployments

Week 15-21: Testing & Frontend
├── Learn: Jest, Mocha, Cucumber, Playwright, Angular, React, Vue
├── Git: Hooks, semantic versioning, releases
├── CI/CD: Test automation, frontend CI/CD, preview deployments
└── Deploy: Frontend apps with CDN

Week 22-29: AWS Cloud
├── Learn: Lambda, API Gateway, DynamoDB, S3, RDS, SNS, SQS, SES, Step Functions, EC2, ECS, EKS
├── Git: Infrastructure as Code workflows
├── CI/CD: AWS deployment automation, security scanning
└── Deploy: Serverless apps, containers, VPC

Week 30-33: IaC & DevOps
├── Learn: CloudFormation, CDK, Terraform, OpenTofu
├── Git: GitOps, drift detection, automated releases
├── CI/CD: Multi-env pipelines, production-grade automation
└── Deploy: Multi-environment infrastructure
```

---

## Weekly Rhythm: How to Learn

### Daily Routine
1. **Morning (1 hour)**: Learn new concepts from tutorials/docs
2. **Afternoon (1-2 hours)**: Hands-on coding — build the lab
3. **Evening (30 mins)**: Commit code to Git, push to GitHub, review CI/CD pipeline

### Weekly Rhythm
- **Weekdays**: Learn concepts, build labs, commit daily
- **Weekend**: Review week's progress, improve README, deploy to production, plan next week

### Git Ritual (Every Day)
- Commit at least once per learning session
- Write meaningful commit messages
- Push to GitHub before end of day
- Check CI/CD pipeline status

### CI/CD Ritual (Every Project)
- Create CI workflow before writing code
- Pipeline should: lint → test → build → deploy
- Add status badges to README
- Review pipeline logs and fix failures

---

## Continuous Learning & Specializations

### AWS Certifications (Pursue in order)
1. AWS Cloud Practitioner
2. AWS Developer Associate
3. AWS Solutions Architect Associate
4. AWS DevOps Engineer Professional

### Advanced Topics
- Kubernetes deeper dive (Helm, Operators, Service Mesh)
- AWS Security: IAM advanced, Security Hub, GuardDuty
- Data engineering: EMR, Glue, Redshift
- Machine Learning: SageMaker, Bedrock Agents
- Cost optimization and FinOps

### Communities & Practice
- AWS Free Tier for experimentation
- AWS Skill Builder hands-on labs
- LeetCode for algorithms
- GitHub for open source contributions
- Reddit r/aws, r/devops, local meetups

---

## Recommended Resources

### Platforms
- AWS Free Tier
- AWS Skill Builder
- A Cloud Guru
- Udemy
- Pluralsight
- GitHub Student Pack

### Testing Tools
- Jest
- Mocha
- Chai
- Sinon
- Cucumber
- Playwright

### IaC & DevOps
- Terraform
- OpenTofu
- AWS CDK
- CloudFormation
- GitLab CI
- GitHub Actions
- Jenkins

### Frontend
- Angular
- React
- Next.js
- Vue.js
- Redux Toolkit
- NgRx
- Pinia

### Backend
- Node.js
- Express
- MongoDB
- Python
- Flask
- FastAPI
- Java
- Spring Boot
- C#
- ASP.NET Core

### Cloud
- AWS Documentation
- Azure Documentation
- GCP Documentation

---

## Assessment Criteria

### Weekly Assessments
- Code reviews
- Project submissions
- Knowledge quizzes
- Practical assignments

### Milestone Projects
- Week 4: MEAN stack application with CI/CD
- Week 8: MERN stack application with automated deployment
- Week 10: Python automation project with CI/CD
- Week 12: Spring Boot API with Docker and CI/CD
- Week 14: ASP.NET Core API with IaC
- Week 17: Complete test suite with automated reporting
- Week 21: Multi-framework frontend apps with CI/CD
- Week 25: Serverless AWS application with automated deployment
- Week 29: Containerized app with monitoring and CI/CD
- Week 31: Complete IaC with GitOps
- Week 33: Production-grade fullstack application with complete CI/CD pipeline

### Final Assessment
- Complete cloud-native fullstack application
- Infrastructure deployed with IaC
- CI/CD pipeline implemented
- GitHub portfolio with 10+ projects
- Documentation and presentation

---

## Tips for Success

1. **Practice Daily**: Code every day, even if it's just 30 minutes
2. **Build Projects**: Apply learning through real projects
3. **Commit Daily**: Push code to GitHub every day — track your progress
4. **Automate Everything**: Every project should have CI/CD from day one
5. **Document Everything**: Keep notes and write blog posts
6. **Join Communities**: Engage with other learners and professionals
7. **Stay Updated**: Follow AWS, Azure, and GCP blogs
8. **Get Certified**: Pursue AWS certifications to validate skills
9. **Seek Feedback**: Share code for reviews and improve continuously
10. **Teach Others**: Explain concepts to reinforce understanding

---

## Next Steps After Completion
- Pursue AWS certifications
- Expand to Azure and GCP
- Contribute to open source projects
- Build a strong portfolio
- Network with industry professionals
- Apply for Cloud Engineer positions
- Continue learning advanced topics (security, ML, etc.)
