# Entry to Mid-Level AWS Cloud Engineer Roadmap

> **Target Audience**: Fresher from college with NO programming background
> **Duration**: 44 Weeks (~11 months)
> **Goal**: Become a job-ready AWS Cloud Engineer (entry-to-mid level, 0-3 YOE)
> **Focus**: AWS Development | DevOps | Serverless | Fullstack (Node.js, Python, Java + Angular, React) | Agentic AI & Automation

---

## Prerequisites

- A computer with 8GB+ RAM
- Stable internet connection
- AWS Free Tier account (requires credit/debit card)
- GitHub account
- 2-3 hours daily commitment

---

## Phase 0: Programming Foundations (Weeks 1-4)
**For complete beginners — build mental models before writing code**

### Week 1: How the Web Works & Computer Basics
- What is a computer program?
- How does the internet work? (HTTP, DNS, IP, browsers)
- What is a server? What is a client?
- What is an API?
- Developer tools setup: VS Code, terminal basics, browser DevTools
- HTML basics (structure, tags, forms)

**Hands-on**: Create a simple HTML portfolio page, view it locally.

### Week 2: Programming Logic & JavaScript Basics
- Variables (let, const), data types (string, number, boolean, null, undefined)
- Operators (arithmetic, comparison, logical)
- Control flow: if/else, ternary, switch
- Loops: for, while, do-while, forEach
- Functions: declarations, expressions, arrow functions, parameters, return values
- Scope: global, function, block

**Hands-on**: Build a number-guessing game in JavaScript (run in browser console).

### Week 3: Data Structures & Algorithms Basics
- Arrays: methods (push, pop, map, filter, reduce, find)
- Objects: keys, values, destructuring
- Strings: methods, template literals
- ES6+ features: spread operator, rest parameters, modules
- Basic algorithms: linear search, bubble sort, two-sum
- Problem-solving mindset

**Hands-on**: Solve 10 beginner problems on LeetCode/CodeWars (arrays and strings).

### Week 4: Asynchronous JavaScript & Git Basics
- Callbacks, call stack
- Promises: then/catch/finally
- Async/await syntax
- Error handling: try/catch/finally
- Git basics: init, add, commit, push, pull
- GitHub: repos, README, branches, PRs

**Hands-on**: Create a GitHub repo, push HTML portfolio, write a professional README.

**Phase 0 Deliverables**:
- [ ] HTML portfolio page hosted on GitHub Pages
- [ ] 10 LeetCode problems solved
- [ ] Active GitHub profile with 2 repos
- [ ] Terminal comfort with 20+ commands

---

## Phase 1: Backend Development — Node.js (Weeks 5-8)
**Primary backend language for serverless and fullstack**

### Week 5: Node.js Runtime & npm
- What is Node.js? Event loop, non-blocking I/O
- Installation and version management (nvm)
- npm: init, install, scripts, semantic versioning
- File System (fs) module: readFile, writeFile
- Path module
- Environment variables: dotenv
- Process module: env, argv

**Hands-on**: Build a CLI tool that reads a file and counts word frequency.

### Week 6: Express.js & REST APIs
- Express setup: app, middleware, routing
- Request/response objects (req, res)
- Middleware: custom, third-party (cors, helmet, morgan)
- RESTful API design (GET, POST, PUT, DELETE, PATCH)
- Status codes, JSON responses
- Validation basics (Joi/Zod)

**Hands-on**: Build a CRUD API for a "Task Manager" with in-memory storage.

### Week 7: Databases & Data Modeling
- SQL vs NoSQL concepts
- PostgreSQL: installation, psql, basic queries (SELECT, INSERT, UPDATE, DELETE)
- DynamoDB: tables, items, attributes, partitions, sort keys
- ORMs: Prisma (for SQL), Mongoose (for NoSQL)
- Connecting databases to Express
- Connection pooling

**Hands-on**: Add PostgreSQL to Task Manager API. Migrate to DynamoDB and compare.

### Week 8: Authentication, Security & Advanced Node.js
- Authentication vs Authorization
- JWT (JSON Web Tokens): sign, verify, structure
- Password hashing: bcrypt
- OAuth2 basics (Google/GitHub login)
- Security headers: Helmet, CORS
- Rate limiting, input sanitization
- Logging: Winston, Morgan
- Error handling best practices

**Hands-on**: Add JWT auth to Task Manager API. Implement Google OAuth.

**Phase 1 Deliverables**:
- [ ] Production-ready REST API (Node.js + Express)
- [ ] PostgreSQL + DynamoDB integration
- [ ] JWT + OAuth2 authentication
- [ ] API documented with Swagger/OpenAPI
- [ ] Deployed to Render/Railway/AWS EC2

---

## Phase 2: Backend Development — Python (Weeks 9-10)
**Essential for scripting, AWS automation, and data engineering**

### Week 9: Python Fundamentals
- Installation, virtual environments, pip
- Variables, data types, type hints
- Control flow, loops, functions
- Data structures: lists, dicts, sets, tuples
- List comprehensions, lambda functions
- File I/O, JSON handling
- Exception handling: try/except/finally

**Hands-on**: Build a CLI todo app in Python. Parse a CSV file and generate summary stats.

### Week 10: Python for AWS & Web
- Flask basics: routes, request/response, templates
- boto3: AWS SDK for Python
- Lambda functions in Python
- S3 operations with boto3
- SES email sending with boto3
- Python packaging and modules

**Hands-on**: Build a Flask API that uploads files to S3 and sends confirmation emails via SES.

**Phase 2 Deliverables**:
- [ ] Python CLI tool with file I/O
- [ ] Flask API with boto3 AWS integration
- [ ] Script to automate AWS resource tagging

---

## Phase 3: Backend Development — Java (Weeks 11-12)
**Enterprise-grade backend and Spring ecosystem**

### Week 11: Java Fundamentals
- JDK installation, IDE setup (IntelliJ IDEA)
- Variables, primitives, objects
- Control flow, loops
- OOP: classes, objects, inheritance, polymorphism, encapsulation, abstraction
- Collections Framework: List, Set, Map, Queue
- Exception handling: try/catch/finally, custom exceptions
- Generics, Streams API (filter, map, collect)

**Hands-on**: Build a student management system with CRUD operations using Collections.

### Week 12: Spring Boot & Build Tools
- Maven/Gradle basics
- Spring Boot project setup (Spring Initializr)
- REST controllers (@RestController, @GetMapping, @PostMapping)
- Service layer, Repository pattern
- Spring Data JPA: entities, repositories
- Application properties, profiles
- Lombok for boilerplate reduction

**Hands-on**: Build a Spring Boot REST API for "Product Catalog" with H2 database.

**Phase 3 Deliverables**:
- [ ] Java OOP project with Collections
- [ ] Spring Boot REST API with JPA
- [ ] Understanding of build tools (Maven/Gradle)

---

## Phase 4: Testing Mastery (Weeks 13-15)
**Unit, integration, and functional testing across stacks**

### Week 13: Unit Testing — Jest, Mocha & Sinon
- Testing concepts: unit vs integration vs E2E
- Jest setup: describe, it, expect, matchers
- Async testing with Jest
- Mocha: BDD/TDD style, Chai assertions (expect, should, assert)
- Sinon: spies, stubs, mocks, fake timers
- Code coverage: Istanbul/NYC
- Test-driven development (TDD) workflow

**Hands-on**: Write comprehensive unit tests for Task Manager API (Node.js) using Jest + Sinon. Write tests for Python CLI app using pytest.

### Week 14: API Integration Testing — Cucumber
- Behavior-Driven Development (BDD)
- Gherkin syntax: Feature, Scenario, Given, When, Then
- Cucumber setup with Node.js/Python/Java
- Step definitions and hooks
- API testing with Cucumber + Axios/SuperTest
- Data tables and scenario outlines
- Cucumber reports

**Hands-on**: Write Cucumber tests for REST API endpoints. Generate HTML reports.

### Week 15: Functional & E2E Testing — Playwright
- Playwright setup (Node.js/Python/Java)
- Browser automation basics
- Selectors, locators
- Assertions and auto-waiting
- Page Object Model (POM)
- Cross-browser testing (Chrome, Firefox, Safari)
- Visual regression testing basics
- CI integration with Playwright

**Hands-on**: Automate login flow and CRUD operations for a web app using Playwright. Run tests in CI.

**Phase 4 Deliverables**:
- [ ] Jest/Mocha test suite with >80% coverage
- [ ] Cucumber BDD test suite with reports
- [ ] Playwright E2E test suite with POM
- [ ] Testing strategy document for a sample project

---

## Phase 5: Frontend Development (Weeks 16-19)
**Fullstack capability — React first, Angular second**

### Week 16: React.js Fundamentals
- JSX, components, props
- State: useState, useEffect
- Component lifecycle (useEffect cleanup)
- Conditional rendering, lists/keys
- Forms and controlled components
- React Router: BrowserRouter, Routes, Route, Link
- Axios for API calls
- Error boundaries

**Hands-on**: Build a React frontend for Task Manager API. Implement routing, CRUD, and auth.

### Week 17: React Advanced & State Management
- Custom hooks
- Context API for global state
- Redux Toolkit (optional but recommended)
- React Query / TanStack Query for server state
- Performance: React.memo, useMemo, useCallback
- Code splitting and lazy loading

**Hands-on**: Refactor Task Manager frontend with Redux Toolkit + React Query.

### Week 18: Angular Fundamentals
- Angular CLI, project structure, modules
- Components, templates, data binding
- Directives: ngIf, ngFor, ngSwitch
- Pipes: built-in and custom
- Services and Dependency Injection
- RxJS basics: Observables, subscribe, pipe
- HttpClient for API integration

**Hands-on**: Build Angular version of Task Manager. Implement services and HTTP client.

### Week 19: Angular Advanced
- Reactive Forms and validation
- Template-driven forms
- Routing: RouterModule, route guards, lazy loading
- NgRx: actions, reducers, selectors, effects
- Authentication flow in Angular
- Material Design / Angular Material
- Build optimization and deployment

**Hands-on**: Complete Angular app with NgRx state management, guards, and Material UI.

**Phase 5 Deliverables**:
- [ ] React fullstack app deployed
- [ ] Angular fullstack app deployed
- [ ] Understanding of component architecture
- [ ] State management implementation (Redux/NgRx)

---

## Phase 6: AWS Fundamentals & Serverless (Weeks 20-23)
**Cloud foundation before deep dives**

### Week 20: AWS Account Setup & Core Services
- AWS Free Tier setup and cost guardrails (budget alerts)
- AWS Global Infrastructure (Regions, AZs, Edge Locations)
- IAM: users, groups, roles, policies, MFA, least privilege
- AWS Organizations and SCPs
- CloudWatch basics: metrics, logs, alarms
- AWS Config for compliance

**Hands-on**: Create IAM users/groups/roles. Set up budget alerts. Configure CloudWatch alarms.

### Week 21: Serverless Compute & APIs
- AWS Lambda: runtime, handler, layers, environment variables
- Lambda triggers and integrations
- Amazon API Gateway: REST APIs, HTTP APIs, stages, deployments
- Request/response mapping templates
- CORS configuration
- Lambda authorizers

**Hands-on**: Build a serverless REST API (Lambda + API Gateway) replacing Express backend.

### Week 22: Data & Storage Services
- Amazon DynamoDB: tables, partitions, sort keys, GSI/LSI
- DynamoDB operations and transactions
- Amazon S3: buckets, objects, versioning, lifecycle policies
- S3 event notifications
- Amazon RDS: PostgreSQL setup, parameter groups, backups
- Secrets Manager: storing DB credentials

**Hands-on**: Build serverless CRUD API with DynamoDB. Implement file upload to S3.

### Week 23: Integration, Messaging & Workflows
- Amazon SNS: topics, subscriptions, FIFO topics
- Amazon SQS: queues, message visibility, dead-letter queues
- Amazon SES: sending emails, templates, configurations
- AWS Step Functions: state machines, standard vs express
- Error handling and retries in Step Functions
- EventBridge (EventBus) for event-driven architecture

**Hands-on**: Build an order processing workflow with Step Functions. Trigger Lambda from S3 upload and send email via SES.

**Phase 6 Deliverables**:
- [ ] Serverless backend (Lambda + API Gateway + DynamoDB)
- [ ] File upload service with S3
- [ ] Messaging pipeline (SNS + SQS + SES)
- [ ] Step Functions workflow
- [ ] AWS architecture diagram

---

## Phase 7: AWS Advanced Services (Weeks 24-27)
**Containers, monitoring, and advanced compute**

### Week 24: Containers & Orchestration
- Docker fundamentals: images, containers, Dockerfile, volumes
- Docker Compose for multi-container apps
- Amazon ECR: registries, repositories, image scanning
- Amazon ECS: task definitions, services, Fargate
- Amazon EKS: clusters, node groups, kubectl basics
- Load Balancers: ALB, NLB basics

**Hands-on**: Containerize Task Manager API. Deploy to ECS Fargate. Set up EKS cluster.

### Week 25: EC2, VPC & Networking
- Amazon EC2: instances, AMIs, key pairs, security groups
- Amazon VPC: subnets, route tables, NAT gateways, IGW
- Elastic Load Balancing: ALB, target groups
- Route 53: hosted zones, record sets, routing policies
- CloudFront: distributions, origins, cache behaviors

**Hands-on**: Deploy app to EC2. Set up VPC with public/private subnets. Configure Route 53.

### Week 26: Monitoring, Tracing & Advanced Databases
- Amazon CloudWatch: custom metrics, dashboards, log insights
- AWS X-Ray: service map, traces, annotations
- Amazon OpenSearch: indices, queries, Kibana
- AWS Glue: ETL basics, crawlers
- AWS Athena: querying S3 with SQL
- Amazon Kinesis: data streams basics

**Hands-on**: Set up CloudWatch dashboard for Lambda metrics. Enable X-Ray tracing. Query S3 data with Athena.

### Week 27: GraphQL, Caching & Additional Services
- AWS AppSync: GraphQL APIs, resolvers, data sources
- Amazon ElastiCache: Redis/Memcached basics
- AWS AppConfig for feature flags
- AWS Systems Manager Parameter Store
- AWS CodeStar connections

**Hands-on**: Build a GraphQL API with AppSync connected to DynamoDB.

**Phase 7 Deliverables**:
- [ ] Containerized app on ECS/EKS
- [ ] VPC architecture diagram and deployment
- [ ] Monitoring dashboard (CloudWatch + X-Ray)
- [ ] GraphQL API with AppSync

---

## Phase 8: Infrastructure as Code (IaC) (Weeks 28-29)
**Automate everything — repeatable, versioned infrastructure**

### Week 28: CloudFormation & AWS CDK
- CloudFormation: templates, stacks, change sets
- YAML/JSON template structure
- Intrinsic functions (Ref, Fn::GetAtt, Sub)
- AWS CDK: constructs, stacks, apps
- CDK with TypeScript/Python/Java
- CDK Pipelines for CI/CD

**Hands-on**: Deploy serverless app using CloudFormation. Re-deploy using CDK.

### Week 29: Terraform & OpenTofu
- Terraform installation, HCL syntax
- Providers, resources, data sources
- Variables, outputs, locals
- State management (local, S3, DynamoDB locking)
- Modules for reusability
- Workspaces for environments (dev/staging/prod)
- OpenTofu as Terraform alternative (compatibility, licensing)

**Hands-on**: Deploy VPC + ECS + RDS using Terraform. Deploy same with OpenTofu.

**Phase 8 Deliverables**:
- [ ] Infrastructure deployed with CloudFormation
- [ ] Infrastructure deployed with AWS CDK
- [ ] Infrastructure deployed with Terraform
- [ ] Infrastructure deployed with OpenTofu
- [ ] Multi-environment setup (dev/staging/prod)

---

## Phase 9: CI/CD & DevOps (Weeks 30-31)
**Automate build, test, and deployment**

### Week 30: Git, GitHub & GitLab
- Advanced Git: rebase, cherry-pick, bisect, reflog
- Branching strategies: GitFlow, GitHub Flow, Trunk-Based
- GitHub: Actions, Packages, Codespaces, Projects
- GitLab: CI/CD pipelines, Auto DevOps, Package Registry
- Pull request templates, CODEOWNERS
- Git hooks (Husky) for pre-commit linting

**Hands-on**: Set up monorepo with GitHub Actions. Set up GitLab CI for multi-environment deploy.

### Week 31: CI/CD Pipelines & Deployment Strategies
- Pipeline concepts: build, test, scan, deploy
- GitHub Actions: workflows, jobs, matrix, caching
- GitLab CI: .gitlab-ci.yml, stages, artifacts
- Jenkins: freestyle vs pipeline, Jenkinsfile
- Deployment strategies: Rolling, Blue/Green, Canary
- Secrets management in CI (GitHub Secrets, GitLab Variables)
- Trunk-based development and feature flags

**Hands-on**: Build complete CI/CD pipeline: lint → test → build → deploy to AWS. Implement Blue/Green deployment.

**Phase 9 Deliverables**:
- [ ] Production-grade CI/CD pipeline (GitHub Actions or GitLab CI)
- [ ] Automated testing in pipeline (unit, integration, E2E)
- [ ] Automated deployment to AWS
- [ ] Blue/Green deployment strategy
- [ ] Security scanning in pipeline

---

## Phase 10: Agentic Development & AI Automation (Weeks 32-36)
**Build intelligent agents that automate end-to-end workflows**

### Week 32: Generative AI & AI Tools for Developers
- What is Generative AI? LLMs, transformers, tokenization
- AI coding assistants: GitHub Copilot, Claude Code, Codex CLI
- Prompt engineering basics: context, constraints, examples
- Using AI for code generation, refactoring, and review
- AI for documentation and debugging
- Ethical considerations and limitations

**Hands-on**: Use Copilot/Claude to build a full feature. Use AI to refactor legacy code.

### Week 33: Agentic AI Concepts & Frameworks
- What is Agentic AI? Autonomous agents vs chatbots
- Agent components: tools, memory, reasoning, planning
- LangChain/LangGraph basics: chains, agents, tools
- CrewAI: multi-agent orchestration
- AutoGen: conversational multi-agent patterns
- Building a simple agent with tool use

**Hands-on**: Build a research agent that searches web and summarizes findings.

### Week 34: RAG — Retrieval Augmented Generation
- What is RAG and why it matters
- Vector databases: Pinecone, Weaviate, pgvector, Chroma
- Embeddings: OpenAI, Cohere, Amazon Titan, HuggingFace
- Chunking strategies: recursive, semantic, sliding window
- Retrieval strategies: dense, sparse, hybrid
- AWS Kendra for enterprise search
- Evaluation metrics: recall, precision, faithfulness

**Hands-on**: Build a RAG chatbot for company documentation using LangChain + Pinecone.

### Week 35: MCP (Model Context Protocol) & AWS Bedrock
- What is MCP? Standardizing AI-tool integrations
- MCP architecture: client, server, transport
- Building MCP servers and clients
- AWS Bedrock: managed foundation models
- Bedrock models: Claude, Titan, Llama, Mistral
- Bedrock Agents: action groups, knowledge bases
- Amazon Bedrock Flows for agent orchestration

**Hands-on**: Build an MCP server for a custom tool. Create a Bedrock agent with knowledge base.

### Week 36: Building Production Agents & Automation Workflows
- Agent design patterns: ReAct, Plan-and-Execute, Reflexion
- Memory: short-term (conversation), long-term (vector store)
- Tool use: API calls, database queries, file operations
- Human-in-the-loop patterns
- Error handling and fallback strategies
- Observability: LangSmith, tracing, logging
- End-to-end automation case study

**Hands-on**: Build a flight booking agent that:
- Asks user preferences (min/max cost, dates, times, meal preferences)
- Researches flight options via API
- Compares and summarizes options
- Proceeds to booking flow with payment integration

**Phase 10 Deliverables**:
- [ ] AI-assisted development workflow (Copilot/Claude)
- [ ] Simple agent with tool use
- [ ] RAG chatbot with vector database
- [ ] MCP server implementation
- [ ] AWS Bedrock agent with knowledge base
- [ ] End-to-end automation agent (flight booking use case)

---

## Phase 11: Capstone Project & Job Preparation (Weeks 37-40)
**Synthesize all skills into portfolio-ready projects**

### Week 37: Capstone Project — Part 1
- Choose a complex, real-world problem
- Design system architecture
- Plan AWS infrastructure
- Set up repositories and CI/CD
- Implement backend (Node.js/Python/Java)

### Week 38: Capstone Project — Part 2
- Implement frontend (React/Angular)
- Add comprehensive testing (unit, integration, E2E)
- Containerize and deploy
- Add monitoring and observability

### Week 39: Capstone Project — Part 3
- Automate infrastructure with IaC
- Add AI/Agentic features (optional)
- Document thoroughly
- Record demo video
- Write blog post/tutorial

### Week 40: Job Preparation
- Resume tailoring for Cloud Engineer roles
- LinkedIn optimization
- Portfolio website
- Mock interviews (system design, coding, behavioral)
- AWS certification prep (Solutions Architect Associate or Developer Associate)
- Job application strategy

**Phase 11 Deliverables**:
- [ ] Complete capstone project deployed
- [ ] GitHub portfolio with 5+ projects
- [ ] Resume and LinkedIn updated
- [ ] AWS certification attempt
- [ ] Job applications submitted

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

### AI & Agentic Tools
- GitHub Copilot
- Claude (Anthropic)
- AWS Bedrock
- LangChain
- LangSmith
- Pinecone/Chroma
- MCP SDK

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
- GitHub Actions
- GitLab CI
- Jenkins

### Frontend
- React
- Angular
- Next.js
- Redux Toolkit
- NgRx

### Backend
- Node.js
- Express
- Python
- Flask
- Java
- Spring Boot

---

## Assessment Criteria

### Weekly Assessments
- Code reviews
- Project submissions
- Knowledge quizzes
- Practical assignments

### Milestone Projects
- Phase 0: HTML portfolio + Git workflow
- Phase 1: REST API with authentication
- Phase 2: Python automation script
- Phase 3: Spring Boot API
- Phase 4: Complete test suite
- Phase 5: Fullstack application
- Phase 6: Serverless AWS application
- Phase 7: Containerized app + monitoring
- Phase 8: IaC deployments (4 tools)
- Phase 9: Complete CI/CD pipeline
- Phase 10: AI automation agent
- Phase 11: Capstone project

### Final Assessment
- Complete cloud-native application
- Infrastructure deployed with IaC
- CI/CD pipeline implemented
- AI/Agentic features integrated
- Documentation and presentation

---

## Tips for Success

1. **Practice Daily**: Code every day, even if it's just 30 minutes
2. **Build Projects**: Apply learning through real projects
3. **Document Everything**: Keep notes and write blog posts
4. **Join Communities**: Engage with other learners and professionals
5. **Stay Updated**: Follow AWS blogs and AI/agentic trends
6. **Get Certified**: Pursue AWS certifications to validate skills
7. **Seek Feedback**: Share code for reviews and improve continuously
8. **Teach Others**: Explain concepts to reinforce understanding
9. **Experiment with AI**: Use Copilot, Claude, and Bedrock in daily work
10. **Think in Agents**: Design solutions as autonomous, goal-driven systems

---

## Next Steps After Completion
- Pursue AWS certifications
- Contribute to open source projects
- Build agentic AI solutions
- Network with industry professionals
- Apply for Cloud Engineer positions
- Continue learning advanced topics (security, ML, etc.)
