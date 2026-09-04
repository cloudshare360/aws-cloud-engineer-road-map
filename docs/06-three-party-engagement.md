# AWS Cloud Engineer - Three-Party Engagement Model

## Executive Summary

This document defines the committed engagement model involving **three distinct parties**:

1. **Employer (Client)** — Organization requiring cloud engineering resources
2. **Technical Support / Training Company (Vendor)** — Provider of skilled engineers and expert support
3. **Associate (Engineer)** — Mid-level AWS Cloud Engineer deployed to the client

The associate is presented as a **mid-level developer with 6 years of experience**, backed by a technical expert support layer from the training company to ensure successful task execution and continuous skill development.

---

## Party Definitions & Responsibilities

### Party 1: Employer (Client)

#### Role
The Employer is the end-client organization that requires cloud engineering expertise to build, deploy, and maintain AWS-based applications and infrastructure.

#### Responsibilities
- Provide project requirements, task definitions, and sprint goals
- Grant necessary system access, credentials, and tooling
- Designate a technical lead / engineering manager as primary point of contact
- Provide onboarding documentation, architecture diagrams, and codebase access
- Conduct regular feedback sessions (weekly/bi-weekly)
- Ensure associate has clear deliverables and priorities
- Review and approve work deliverables
- Provide performance feedback to the vendor

#### Expectations
- Clear and well-defined task requirements
- Timely feedback on delivered work
- Access to necessary environments and stakeholders
- Supportive environment for the associate to succeed

---

### Party 2: Technical Support / Training Company (Vendor)

#### Role
The Technical Support / Training Company is the service provider responsible for supplying the skilled associate and maintaining a technical expert support layer.

#### Responsibilities

##### Resource Provisioning
- Recruit, vet, and onboard qualified AWS Cloud Engineers
- Ensure associate meets stated experience and skill requirements
- Provide associate with necessary tools, equipment, and software licenses
- Handle associate employment, benefits, and administrative matters

##### Technical Expert Support Layer
- Maintain a pool of senior/principal engineers as expert support
- Provide architectural guidance and code review oversight
- Bridge skill gaps through training, pair programming, and mentoring
- Escalate and resolve complex technical challenges
- Ensure code quality and adherence to best practices
- Conduct regular technical reviews and quality audits

##### Training & Development
- Design and deliver structured learning path (20-week roadmap)
- Provide access to learning resources, certifications, and courses
- Track associate progress against learning milestones
- Conduct skill assessments and provide feedback
- Update training materials based on emerging technologies and client needs

##### Engagement Management
- Assign a dedicated engagement manager as single point of contact
- Conduct regular health checks with the employer
- Address any concerns or issues promptly
- Ensure SLA compliance and service quality
- Manage contract terms, timelines, and deliverables

#### Guarantees
- Associate will meet the stated experience level (6 YOE, mid-level)
- Technical expert support will be available as needed
- Structured learning and development plan will be followed
- Code quality and delivery standards will be maintained

---

### Party 3: Associate (AWS Cloud Engineer)

#### Role
The Associate is a **mid-level AWS Cloud Engineer with 6 years of professional experience**, deployed to the employer's team to execute development tasks, build cloud infrastructure, and contribute to product delivery.

#### Experience Profile
- **6 years** of professional software development experience
- **3+ years** focused on AWS cloud engineering and serverless architectures
- Proven track record of delivering production-grade backend services and cloud infrastructure

#### Technical Competencies

##### Backend Development
- Node.js, Express.js, Python — Advanced
- RESTful API design and implementation
- Microservices and event-driven architectures
- Database design (SQL & NoSQL)

##### AWS Cloud Engineering
- Serverless architectures (Lambda, API Gateway, Step Functions)
- Infrastructure as Code (AWS CDK, CloudFormation, Terraform)
- Containerization (Docker, ECS, EKS, App Runner)
- Data services (DynamoDB, RDS, S3, OpenSearch, Athena)
- Integration services (SNS, SQS, SES, AppSync)
- Security & Identity (IAM, Secrets Manager)
- Monitoring & Observability (CloudWatch, X-Ray)

##### DevOps & CI/CD
- GitLab, GitHub, Jenkins
- Automated testing and deployment
- Infrastructure automation
- Environment management

##### Frontend Awareness
- Angular (with Karma)
- ReactJS / Next.js
- Fullstack integration patterns

#### Core Responsibilities
- Execute assigned development tasks independently
- Build and maintain backend services and APIs
- Design and deploy AWS infrastructure using IaC
- Set up and maintain CI/CD pipelines
- Write unit and integration tests
- Participate in code reviews (both giving and receiving)
- Collaborate with employer's engineering team
- Seek expert support when facing knowledge gaps
- Document work and share learnings
- Participate in agile ceremonies (standups, sprint planning, retrospectives)

#### Expected Performance
- **Week 1-2**: Onboarding, environment setup, codebase familiarization
- **Week 3-4**: First deliverables with expert pairing
- **Month 2**: Independent delivery of medium-complexity features
- **Month 3+**: Full productivity, minimal supervision required

---

## Engagement Model

### Resource Deployment
- The associate is embedded within the employer's engineering team
- Works alongside employer's engineers as a full team member
- Reports to employer's engineering manager / technical lead for day-to-day tasks
- Maintains dotted-line reporting to vendor's engagement manager for administrative and training matters

### Technical Expert Support Flow

```
Employer Task → Associate Execution → Expert Support (if needed)
                                    ↓
                            Code Review & Guidance
                                    ↓
                            Knowledge Transfer
                                    ↓
                            Associate Delivers
```

#### Expert Support Activation
- **Self-Service First**: Associate attempts to resolve using documentation and resources
- **Peer Support**: Associate asks team members or vendor peers
- **Expert Escalation**: Associate requests expert support through vendor's engagement manager
- **Priority Levels**:
  - **P1 (Critical)**: Production incident, security issue — Immediate expert response
  - **P2 (High)**: Complex architecture decision — Expert response within 4 hours
  - **P3 (Medium)**: Implementation guidance — Expert response within 24 hours
  - **P4 (Low)**: Learning and development — Scheduled office hours

### Training & Learning Integration
- Associate follows the structured 20-week learning roadmap
- Training is conducted during non-project hours or designated learning time
- Expert support is integrated into learning—experts provide guidance on hands-on exercises
- Progress is tracked and reported to the employer

---

## Communication Structure

### Daily
- **Standups**: Associate participates in employer's daily standups
- **Slack/Teams**: Associate available on employer's communication channels

### Weekly
- **Sprint Planning**: Associate participates in sprint planning
- **Weekly Sync**: Vendor's engagement manager checks in with associate and employer
- **Code Reviews**: Regular code reviews with employer's tech leads and vendor experts

### Monthly
- **Performance Review**: Vendor reviews associate's performance with employer
- **Training Progress**: Vendor reports learning progress and skill development
- **Health Check**: Vendor and employer discuss engagement health and adjustments

### Quarterly
- **Business Review**: Comprehensive review of deliverables, quality, and engagement
- **Skill Assessment**: Evaluate associate's growth against learning roadmap
- **Contract Review**: Discuss renewal, extension, or changes to engagement

---

## SLA & Service Guarantees

### Availability
- Associate available during employer's business hours (typically 40 hours/week)
- Time off requests coordinated through vendor with advance notice

### Code Quality
- All code reviewed by senior engineers (employer's or vendor's)
- Test coverage maintained at > 80%
- Adherence to coding standards and best practices

### Expert Response Times
- P1 issues: Immediate / within 1 hour
- P2 issues: Within 4 business hours
- P3 issues: Within 24 business hours
- P4 issues: Scheduled during office hours

### Knowledge Transfer
- All work documented and knowledge shared with employer's team
- Code comments, READMEs, and architecture docs maintained
- Regular knowledge sharing sessions

---

## Risk Management

### Risks & Mitigations

| Risk | Party Responsible | Mitigation |
|------|------------------|------------|
| Skill gaps in specific technologies | Vendor | Expert support layer, training programs, pre-vetting |
| Integration challenges with existing systems | Both | Pair programming, expert guidance, phased onboarding |
| Communication gaps | Vendor | Dedicated engagement manager, regular syncs |
| Quality issues | Both | Code reviews, testing standards, QA processes |
| Turnover / resource change | Vendor | Backfill guarantee, knowledge documentation, transition plan |

### Escalation Path
1. Associate → Employer's Tech Lead → Vendor's Engagement Manager → Vendor's Technical Director

---

## Success Metrics

### For the Associate
- Completion of 20-week learning roadmap milestones
- Code quality metrics (review approval rate, test coverage, bug rate)
- Sprint velocity and delivery consistency
- Peer feedback and team integration

### For the Employer
- Feature delivery on time and within scope
- Code quality and maintainability
- System reliability and performance
- Knowledge transfer to internal team

### For the Vendor
- Client satisfaction scores
- Associate retention and growth
- SLA compliance
- Successful engagement renewals

---

## Revenue Model

### Shared Compensation Structure

The Employer pays a **single consolidated rate** to the Vendor. The Vendor then distributes the compensation across all three parties as follows:

#### Compensation Distribution

| Party | Share | Description |
|-------|-------|-------------|
| **Employer (Client)** | 20% | **Savings** compared to hiring directly — the Employer pays less than a full-time market rate for equivalent expertise |
| **Associate (Engineer) + Vendor (Training/Support Company)** | 80% | Shared between the associate and the vendor organization |

### Example Model (Illustrative)

| Component | Amount (Monthly) | Percentage |
|-----------|------------------|------------|
| Employer Payment (Total) | $10,000 | 100% |
| Associate Compensation | $5,500 | 55% |
| Vendor Service Fee | $2,000 | 20% |
| Employer Net Savings | $2,500 | 25% |

### Benefits to Each Party

#### Employer
- **Cost Efficiency**: Pay less than direct hire market rate for mid-level talent
- **Risk Mitigation**: Expert support layer included without additional cost
- **Flexibility**: Easy scaling up/down without full-time hiring overhead
- **No Administrative Burden**: Vendor handles payroll, benefits, compliance

#### Associate
- **Competitive Compensation**: Market-rate salary with benefits
- **Structured Growth**: 20-week learning roadmap and continuous skill development
- **Expert Mentorship**: Access to senior engineers for guidance and career growth
- **Stable Employment**: Committed role with clear career progression

#### Vendor
- **Service Revenue**: Fee for providing skilled resources and support infrastructure
- **Long-term Partnership**: Recurring revenue from committed engagements
- **Expert Utilization**: Senior engineers contribute across multiple clients, maximizing their impact
- **Talent Development**: Build a bench of skilled engineers through the training program

### Payment Terms
- **Billing Cycle**: Monthly in advance
- **Payment Terms**: Net 30 days from invoice date
- **Rate Adjustments**: Annual review based on market rates and performance
- **Expert Support**: Included in the base rate — no additional charges for standard expert consultations

### Value Proposition Summary

| Party | Key Value |
|-------|-----------|
| **Employer** | Access to 6 YOE mid-level talent + expert support, at reduced cost and risk |
| **Associate** | Competitive pay, structured growth, mentorship, and stable employment |
| **Vendor** | Service revenue, talent development, and long-term client relationships |

This shared-pay model aligns incentives across all parties: the Employer gets cost-effective expertise, the Associate receives fair compensation with growth opportunities, and the Vendor earns a sustainable margin while delivering quality service.

---

## Contractual Terms

### Engagement Duration
- Initial commitment: 6 months
- Extension: Mutually agreed upon based on performance and needs
- Notice period: 2 weeks from either party

### Termination Clauses
- **For Cause**: Immediate termination for breach of contract, misconduct, or consistent underperformance
- **For Convenience**: Either party may terminate with 2 weeks notice
- **Knowledge Transfer**: Upon termination, associate will document and hand over all work

### Intellectual Property
- All work produced belongs to the Employer
- Associate agrees not to disclose confidential information
- Vendor retains rights to training materials and learning roadmap

---

## Onboarding Checklist

### Week 1: Setup
- [ ] AWS account and IAM access provisioned
- [ ] Development environment configured
- [ ] Codebase cloned and running locally
- [ ] Communication tools (Slack, email) set up
- [ ] Security and compliance training completed

### Week 2: Familiarization
- [ ] Architecture diagrams reviewed
- [ ] Codebase tour with senior engineer
- [ ] Sprint planning participation
- [ ] First small task assigned with expert pairing

### Week 3-4: First Deliverables
- [ ] First feature delivered and reviewed
- [ ] Tests written for delivered features
- [ ] Documentation updated
- [ ] Regular code review participation

---

## Contact Information

### Employer
- **Primary Contact**: [Employer's Engineering Manager]
- **Email**: [Employer's contact email]
- **Slack**: [Employer's Slack channel]

### Vendor (Technical Support / Training Company)
- **Engagement Manager**: [Vendor's Engagement Manager Name]
- **Email**: [Vendor's contact email]
- **Phone**: [Vendor's contact number]
- **Slack**: [Vendor's Slack channel]

### Associate
- **Name**: [Associate's Name]
- **Email**: [Associate's work email]
- **Slack**: [Associate's Slack handle]
- **GitHub**: [Associate's GitHub profile]

---

## Document Control

| Version | Date | Changes | Author |
|---------|------|---------|--------|
| 1.0 | 2026-08-25 | Initial document | Engagement Manager |

---

*This document defines the committed engagement model and is binding upon acceptance by all three parties.*

---

## Continue To

- **[07-staff-augmentation-proposal.md](./07-staff-augmentation-proposal.md)** — Executive proposal for resource engagement
- **[01-role-description.md](./01-role-description.md)** — Review role responsibilities and success criteria
- **[03-learning-path.md](./03-learning-path.md)** — Detailed week-by-week curriculum with objectives and deliverables
