# AGENTS.md

AWS Cloud Engineer Committed Role Program — 20-week training placing a mid-level AWS Cloud Engineer (6 YOE) with technical expert support layer.

## Repository Structure

```
.
├── readme.md                    # Root index
├── docs/                        # GitHub Pages (01-07*.md + index.html + README.md)
├── .kilo/                       # Agent config
├── .devcontainer/devcontainer.json
├── .github/workflows/pages.yml
├── aws-cloud-engineer/          # Role root
│   ├── node-js/                 # Node.js learning path
│   ├── angular/                 # Frontend resources
│   ├── react/                   # Frontend resources
│   ├── dev-ops/                 # DevOps learning materials
│   │   ├── ci-cd/               # GitLab, GitHub Actions, Jenkins
│   │   └── iac/                 # CloudFormation, CDK, Terraform, OpenTofu
│   └── aws-services/            # 82 AWS services organized by domain
│       ├── analytics/             # athena, datapipeline, emr, glue, kinesis, opensearch, timestream, etc.
│       ├── application-integration/  # api-gateway, appsync, sns, sqs, ses, stepfunction, etc.
│       ├── compute/               # ec2, lambda
│       ├── containers/            # ecr, ecs, eks, appmesh
│       ├── database/              # dynamodb, rds, documentdb, neptune, elasticache, etc.
│       ├── developer-tools/       # cloud9, cloudformation, codebuild, codecommit, etc.
│       ├── iot/                   # iot-core, iot-analytics, iot-device-defender
│       ├── machine-learning/      # sagemaker, bedrock, rekognition, polly, etc.
│       ├── management-governance/ # cloudwatch, config, systems-manager, trustedadvisor
│       ├── migration-transfer/    # dms, migration-hub, transfer-family, etc.
│       ├── networking-content-delivery/  # cloudfront, route53, vpc, elb, etc.
│       ├── security-identity-compliance/  # iam, cognito, guardduty, kms, etc.
│       ├── serverless-application-repository/
│       └── storage/               # s3
```

## Conventions

- Markdown: ATX headings, ≤120 chars, relative paths
- Docs: `NN-name.md` format, case-sensitive
- Commits: Conventional (`feat:`, `fix:`, `docs:`, `chore:`)
- Pages: `/docs` folder, `index.html` entry, `.nojekyll`

## Agent System

- Skills: `.kilo/skills/`
- Memory: `.kilo/memory/`
- Tasks: `.kilo/tasks/`

## Environment

```bash
KILO_MODE=code
KILO_MODEL=kilo/kilo-auto/free
```

Devcontainer: Node.js LTS, Python, Java, AWS CLI, Kilo CLI
