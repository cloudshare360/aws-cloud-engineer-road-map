---
layout: default
---

# AWS Cloud Engineer Roadmap

## Parallel Learning Tracks

This roadmap uses **four parallel tracks** that run simultaneously from Week 1:

- **Track A: Fullstack Development** — MEAN/MERN, Python, Java, .NET, Frontend
- **Track B: Git & Developer Tooling** — Git/GitHub workflows, Markdown, VS Code, Codespaces, GitHub Pages
- **Track C: CI/CD & DevOps** — GitLab CI, Jenkins, GitHub Actions, automated pipelines
- **Track D: Agile, Process & Architecture** — Scrum, Kanban, sprint ceremonies, task-based learning, progress tracking, software architecture, microservices, micro frontends

> **Key Principle**: Every hands-on lab is committed to GitHub and automated through CI/CD. You learn by building and shipping code, not just watching tutorials. From day one, you act like a professional developer in a real team environment.

---

## Track A: Fullstack Development (Weeks 1-21)

### MEAN Stack (Weeks 1-4)
- MongoDB
- Express.js
- Angular
- Node.js
- REST API concepts

### MERN Stack (Weeks 5-8)
- MongoDB
- Express.js
- React.js
- Node.js
- REST API concepts

### Python Fundamentals (Weeks 9-10)
- Python fundamentals
- Flask
- FastAPI
- Scripting for automation

### Java Fundamentals (Weeks 11-12)
- Java fundamentals
- Spring Boot basics

### .NET / C# Fundamentals (Weeks 13-14)
- C# fundamentals
- ASP.NET basics

### Testing Fundamentals (Weeks 15-17)
- Jest
- Chai
- Mocha
- Sinon
- Cucumber
- Playwright

### Frontend Development (Weeks 18-21)

#### Angular
- Angular CLI & Project Structure
- Components & Templates
- Data Binding & Directives
- Pipes & Custom Pipes
- Services & Dependency Injection
- RxJS & Reactive Programming
- Reactive Forms & Validation
- Angular Routing & Guards
- HTTP Client & API Integration
- State Management (NgRx)
- Lazy Loading & Performance
- Angular Testing (Jasmine, Karma)
- Build Optimization & Deployment

#### React / Next.js
- React fundamentals
- Next.js framework
- Components & Props
- State Management
- API Routes & SSR
- Deployment & Optimization

#### Vue.js
- Vue.js 3 Composition API
- Vue CLI and project structure
- Components, props, and emits
- Reactive data with ref and reactive
- Vue Router for navigation
- State management with Pinia
- Axios for API integration

---

## Track B: Git & Developer Tooling (Weeks 1-33)
**Parallel from Day 1 — professional development environment and workflow**

### Weeks 1-2: Git Foundations & IDE Setup
- Git installation and configuration
- Git basics: init, add, commit, push, pull, clone
- GitHub account setup and first repository
- VS Code setup: extensions, terminal, debugger
- GitHub Codespaces: cloud development environment
- Markdown basics: syntax, README.md, GitHub-flavored Markdown
- .gitignore and repository hygiene
- **Commit discipline**: commit at least once per learning session, never lose work

**Hands-on**: Create GitHub account. Set up VS Code with extensions. Create first repo. Push "Hello World" Node.js script with professional README.md. Open first Codespace. Make first commit within 30 minutes of starting.

### Weeks 3-4: Branching, Collaboration & GitHub Pages
- Branching strategies: GitFlow, GitHub Flow, Trunk-Based
- Creating and switching branches
- Pull requests and code reviews
- Merge vs rebase
- Resolving merge conflicts
- GitHub: Issues, Projects, Wiki
- GitHub Pages: hosting static sites and portfolios
- Markdown advanced: tables, images, links, task lists

**Hands-on**: Create feature branches for each lab. Open PRs. Practice merge conflict resolution. Deploy GitHub Pages portfolio.

### Weeks 5-8: Portfolio Development & Advanced Git
- GitHub profile optimization
- Pinned repositories
- Project documentation standards
- LinkedIn profile creation
- Advanced Git: cherry-pick, bisect, reflog, stash
- Git hooks (Husky) for pre-commit linting
- Semantic versioning and tags
- Release management on GitHub/GitLab
- CODEOWNERS and branch protection rules

**Hands-on**: Build 2-3 portfolio projects with complete READMEs, screenshots, and deployment links. Set up Husky hooks. Create semantic version tags.

### Weeks 9-14: Monorepo & Advanced Tooling
- Monorepo management with npm workspaces or Turborepo
- Git submodules and subtrees
- Git worktree for parallel development
- Large file storage with Git LFS
- Signed commits and tags
- GitHub Projects for project management
- GitHub Actions badges and status indicators
- Open source contribution basics

**Hands-on**: Organize all previous projects into a monorepo structure. Contribute to open source.

### Weeks 15-21: Documentation & Knowledge Sharing
- Technical writing best practices
- Blog posts with Markdown
- GitHub profile README with stats
- Documentation sites with MkDocs or Docusaurus
- Creating demo videos and GIFs
- Writing case studies for projects

**Hands-on**: Write blog post about learning journey. Create documentation site for projects.

### Weeks 22-33: Production-Grade Practices
- CODEOWNERS and branch protection
- Automated README generation
- Changelog automation with semantic commits
- Security scanning in Git workflows
- GitOps principles for infrastructure
- Automated dependency updates (Dependabot)

**Hands-on**: Implement automated changelog generation. Set up Dependabot. Enforce branch protection.

---

## Track C: CI/CD & DevOps (Weeks 1-33, intensifies after Week 22)
**Parallel from Day 1 — automate every lab and project**

### Weeks 1-4: CI/CD Foundations
- Understand CI/CD concepts: build, test, deploy
- GitHub Actions basics: workflows, jobs, steps
- GitLab CI basics: .gitlab-ci.yml, stages
- YAML syntax for pipelines
- Secrets management in CI

**Hands-on**: Create first GitHub Actions workflow that runs on every push. Automate linting.

### Weeks 5-8: Testing in CI/CD
- Running unit tests in CI
- Code coverage reporting
- Linting and formatting automation
- Automated PR checks
- Status badges in README

**Hands-on**: Add Jest/Mocha tests to CI pipeline. Add code coverage badge to README.

### Weeks 9-14: Build & Package Automation
- Building applications in CI
- Creating Docker images
- Pushing to registries (Docker Hub, ECR)
- Semantic versioning in pipelines
- Artifact management

**Hands-on**: Automate Docker image build and push for backend projects.

### Weeks 15-21: Deployment Automation
- Deploying to AWS (EC2, S3, Lambda)
- Environment-specific deployments
- Secrets management in CI/CD
- Rollback strategies
- Blue/Green and Canary deployments

**Hands-on**: Automate deployment of fullstack app to AWS. Implement Blue/Green deployment.

### Weeks 22-33: Production-Grade DevOps
- Infrastructure provisioning in CI/CD
- Security scanning in pipelines
- Performance testing automation
- Monitoring and alerting setup
- Multi-environment pipelines (dev/staging/prod)

**Hands-on**: Build complete CI/CD pipeline for serverless AWS app. Implement IaC deployment through CI/CD.

---

## Track D: Agile, Process & Architecture (Weeks 1-33)
**Parallel from Day 1 — learn to work and architect like a professional**

### Weeks 1-2: Software Development Process & Task-Based Learning
- What is Agile? Values and principles
- Scrum vs Kanban: when to use which
- Task-based learning: breaking down concepts into actionable tasks
- GitHub Projects for task tracking
- Setting up a Kanban board
- Sprint goals and backlog
- **Software Development Life Cycle (SDLC)**: planning → requirements → design → implementation → testing → deployment → maintenance
- **Requirements gathering**: user stories, acceptance criteria, functional vs non-functional requirements
- **Solution design**: turning requirements into technical approach
- **Data structures fundamentals**: arrays, linked lists, stacks, queues, hash tables, trees, graphs
- **Algorithm basics**: Big O notation, sorting, searching, recursion

**Hands-on**: Set up GitHub Project board for learning. Create tasks for Week 1-2. Write user stories for "Hello World" app. Solve 5 beginner problems on LeetCode (arrays and strings).

### Weeks 3-4: Scrum Ceremonies & Sprint Execution
- Scrum framework: roles, events, artifacts
- Sprint Planning: defining sprint goals and backlog
- Daily Standup: progress updates and blockers
- Sprint Review: demo and feedback
- Sprint Retrospective: continuous improvement
- Product Backlog refinement
- Story points and estimation
- **Architecture basics**: monolithic architecture, layers of a monolith, when monolith is appropriate

**Hands-on**: Run 2-week Scrum sprint. Conduct sprint planning, daily standups, review, and retrospective. Design a simple monolith architecture for Task Manager.

### Weeks 5-6: Kanban Method & Monolith Decomposition
- Kanban principles: visualize, limit WIP, manage flow
- Kanban board setup: To Do, In Progress, Review, Done
- WIP limits and cycle time
- Cumulative Flow Diagrams
- Lead time vs cycle time
- When to use Kanban vs Scrum
- **From monolith to services**: identifying bounded contexts, service boundaries, shared kernel
- **When NOT to microservice**: team size, domain complexity, operational maturity, observability costs

**Hands-on**: Switch to Kanban for 2 weeks. Track cycle time. Analyze Task Manager monolith and identify potential service boundaries.

### Weeks 7-8: Hybrid Agile & Microservices Introduction
- Combining Scrum and Kanban (Scrumban)
- Personal Agile: applying Agile to individual learning
- Timeboxing and Pomodoro technique
- Weekly reviews and planning
- Metrics: velocity, burndown, cumulative flow
- **Microservices fundamentals**: single responsibility, independent deployability, decentralized data management
- **Microservices trade-offs**: operational complexity, network latency, data consistency, testing challenges
- **Right-sizing microservices**: bounded context alignment, team ownership, avoiding nano-services, determining optimal service granularity
- **Micro frontends introduction**: when to split frontend, module federation, iframe vs web components

**Hands-on**: Create personal Agile system. Track velocity and burndown. Design microservices architecture for a simple app.

### Weeks 9-14: Advanced Architecture & Design
- User stories and acceptance criteria
- INVEST criteria for user stories
- Definition of Done (DoD)
- Definition of Ready (DoR)
- Test-Driven Development (TDD) as part of Agile
- Pair programming and mob programming
- Code reviews as quality gates
- **Domain-Driven Design (DDD)**: bounded contexts, aggregates, entities, value objects
- **API design**: REST, GraphQL, gRPC, versioning strategies
- **Event-driven architecture**: events, commands, CQRS, event sourcing
- **Micro frontend patterns**: module federation, single-spa, micro-apps, composition patterns
- **Design patterns**: Singleton, Factory, Observer, Strategy, Decorator, Adapter, Repository, Unit of Work
- **SOLID principles**: Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion

**Hands-on**: Write user stories for all projects. Implement DoD checklist. Design event-driven architecture for order processing system. Apply design patterns in backend projects.

### Weeks 15-21: Architecture in Practice & Team Processes
- Cross-functional teams
- Stakeholder communication
- Sprint goals and OKRs
- Agile estimation techniques (Planning Poker, T-shirt sizes)
- Handling technical debt in Agile
- Continuous improvement practices
- **Observability in microservices**: distributed tracing, correlation IDs, structured logging, metrics
- **Service mesh**: Istio, AWS App Mesh, traffic management, resilience
- **Micro frontend frameworks**: Single-SPA, Module Federation, web components
- **When microservices fail**: too many services, debugging complexity, team overhead, when to consolidate

**Hands-on**: Simulate team sprint with peers. Practice estimation. Build microservices with observability. Implement micro frontend pattern.

### Weeks 22-29: Cloud Architecture & Enterprise Patterns
- AWS Well-Architected Framework
- Design principles for cloud applications
- High availability and fault tolerance
- Scalability and elasticity
- Cost optimization strategies
- Security best practices
- **Serverless architecture**: function as a service, event-driven, pay-per-use
- **Serverless patterns**: API Gateway + Lambda, Step Functions, event sourcing
- **Container orchestration**: Kubernetes, ECS, service discovery, load balancing
- **Data architecture**: database per service, CQRS, event sourcing, saga pattern

**Hands-on**: Plan AWS projects using Agile. Deploy infrastructure in sprints. Implement serverless and containerized microservices.

### Weeks 30-33: Production Architecture & Scaling
- Kubernetes deeper dive (Helm, Operators, Service Mesh)
- AWS Security: IAM advanced, Security Hub, GuardDuty
- Data engineering: EMR, Glue, Redshift
- Machine Learning: SageMaker, Bedrock Agents
- Cost optimization and FinOps
- **Anti-patterns**: distributed monolith, chatty services, shared databases, tight coupling
- **Refactoring strategies**: strangler fig pattern, anti-corruption layer, branch by abstraction
- **Governance**: API contracts, schema registry, contract testing, canary deployments

**Hands-on**: Create architecture review checklist. Implement canary deployment. Document anti-patterns avoided in projects.

---

## Track D: Progress Tracking & Task-Based Learning

### Progress Tracking Methods

#### GitHub-Based Tracking
- GitHub Projects: task boards with Kanban view
- GitHub Issues: granular task tracking
- GitHub Milestones: phase-level progress
- GitHub Insights: contribution graphs, traffic, dependency graph
- GitHub Actions: automated progress reports

#### Personal Tracking
- Daily commit log: track daily progress via Git commits
- Weekly blog posts: document learning journey
- Learning journal: Markdown-based journal in repo
- Skills matrix: track proficiency in technologies
- Time tracking: Toggl, Clockify, or manual logs

#### Metrics to Track
- Commits per day/week
- Pull requests opened/merged
- Projects completed
- Test coverage percentage
- Deployment frequency
- Cycle time for features
- Learning hours invested

### Task-Based Learning Framework

#### How to Break Down Learning

1. **Choose a Technology** (e.g., "Learn React")
2. **Break into Tasks**:
   - Task 1: Set up React development environment
   - Task 2: Create first React component
   - Task 3: Understand JSX syntax
   - Task 4: Implement state with useState
   - Task 5: Build a complete feature
3. **Estimate Effort**: Small (<1 hour), Medium (1-2 hours), Large (2+ hours)
4. **Create GitHub Issues**: One issue per task
5. **Link to Milestone**: Group tasks into milestones
6. **Track Progress**: Move tasks across Kanban board

#### Example: Learning Express.js

```
Milestone: Express.js Basics
├── Issue 1: Install Express and create server (Small)
├── Issue 2: Understand middleware concept (Medium)
├── Issue 3: Build GET endpoint (Small)
├── Issue 4: Build POST endpoint with body parsing (Medium)
├── Issue 5: Implement error handling middleware (Medium)
├── Issue 6: Add validation with Joi (Medium)
└── Issue 7: Build complete CRUD API (Large)
```

---

## Integrated Learning Example: Week 1 Flow

```
Morning: Learn Node.js basics from tutorial
         ↓
Afternoon: Build "Hello World" server with Express
         ↓
Create GitHub repo and push code
         ↓
Write README.md with setup instructions
         ↓
Create GitHub Actions workflow for linting
         ↓
Evening: Commit daily progress to learning journal
         ↓
Update GitHub Project board
         ↓
Plan tomorrow's tasks in Sprint Backlog
```

---

## Weekly Rhythm: How to Learn

### Daily Routine
1. **Morning (30 mins)**: Plan day's tasks from GitHub Project board
2. **Learning (1 hour)**: Watch tutorials, read docs
3. **Hands-on (1-2 hours)**: Code the lab
4. **Git Ritual (15 mins)**: Commit code, push to GitHub, update project board
5. **CI/CD Check (5 mins)**: Verify pipeline status, fix failures
6. **Evening (15 mins)**: Update learning journal, plan next day

### Weekly Rhythm
- **Weekdays**: Learn concepts, build labs, commit daily
- **Weekend**: 
  - Saturday: Review week's progress, deploy projects, write blog post
  - Sunday: Plan next week's tasks, conduct weekly retrospective

### Git Ritual (Every Day)
- Commit at least once per learning session
- Write meaningful commit messages
- Push to GitHub before end of day
- Check CI/CD pipeline status
- Update GitHub Project board
- **Never let code live uncommitted for more than 2 hours**
- Commit small, logical chunks — one concept or fix per commit
- Use branches for experiments; merge only working code

### Agile Ritual
- **Daily**: Update task board, note blockers
- **Weekly**: Sprint review and retrospective
- **Bi-weekly**: Sprint planning and goal setting

---

## Developer Environment Setup

### Required Tools
- **IDE**: Visual Studio Code (primary), GitHub Codespaces (cloud)
- **Browser**: Chrome/Firefox with DevTools
- **Terminal**: VS Code integrated terminal or iTerm2/WT
- **Git**: Git CLI with Git Credential Manager
- **Node.js**: nvm for version management
- **Python**: pyenv for version management
- **Docker**: Docker Desktop
- **AWS CLI**: AWS CLI v2

### VS Code Extensions
- ESLint, Prettier
- GitLens
- Thunder Client / REST Client
- Markdown Preview Enhanced
- Docker
- AWS Toolkit
- Angular Language Service
- ESLint for React/Vue

### GitHub Codespaces
- Pre-configured development environments
- Consistent environment across machines
- Browser-based development
- Secrets and environment variables
- Port forwarding for local development

---

## Phase Deliverables Summary

| Phase | Weeks | Track A: Fullstack | Track B: Git/IDE/Pages | Track C: CI/CD | Track D: Agile/Architecture |
|-------|-------|-------------------|------------------------|----------------|----------------------------|
| 1 | 1-4 | MEAN Stack | Git basics, VS Code, Markdown, first Codespace | First CI workflow | Task board setup, SDLC, requirements, monolith design |
| 2 | 5-8 | MERN Stack | Portfolio, GitHub Pages, advanced Git | Test automation | Scrum sprints, monolith decomposition, service boundaries |
| 3 | 9-10 | Python | Monorepo, Git worktree, LFS | Build automation | Kanban, microservices intro, when NOT to microservice |
| 4 | 11-12 | Java | CODEOWNERS, releases, changelog | Docker in CI | Scrumban, DDD, API design, event-driven architecture |
| 5 | 13-14 | .NET/C# | GitOps, documentation as code | IaC deployment | Micro frontends, module federation, composition patterns |
| 6 | 15-17 | Testing | Open source, blog posts, docs site | Test automation | Observability, distributed tracing, service mesh |
| 7 | 18-21 | Frontend | Demo videos, case studies | Frontend CI/CD | Team sprints, micro frontend frameworks, when microservices fail |
| 8 | 22-25 | AWS Core | Infrastructure Git workflow | AWS deployment | Serverless architecture, patterns, anti-patterns |
| 9 | 26-29 | AWS Advanced | Git for containers/images | Security scanning | Container orchestration, data architecture, saga pattern |
| 10 | 30-31 | IaC | GitOps, drift detection | IaC automation | Refactoring strategies, strangler fig, anti-corruption |
| 11 | 32-33 | DevOps | Dependabot, automation | Multi-env pipelines | Governance, API contracts, canary deployments |

---

## Core AWS Knowledge
- AWS architecture-level understanding
- AWS developer-level understanding
- Latest agentic development practices on AWS

## Multi-Cloud Expansion (Post-AWS Mastery)
- Azure fundamentals and core services
- Google Cloud Platform (GCP) fundamentals
- Multi-cloud architecture patterns
- Cloud-agnostic IaC and deployment strategies

---

## Continue To

- **[03-learning-path](./03-learning-path.html)** — Detailed week-by-week curriculum with parallel track objectives
- **[01-role-description](./01-role-description.html)** — Review role responsibilities and success criteria
