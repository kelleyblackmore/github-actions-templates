# GitHub Actions Templates

A comprehensive collection of 50 GitHub Actions workflow templates showcasing various CI/CD patterns, automation, and best practices.

## 📋 Table of Contents

- [Overview](#overview)
- [Workflow Categories](#workflow-categories)
- [Quick Start](#quick-start)
- [Workflow List](#workflow-list)
- [Configuration Files](#configuration-files)
- [Usage](#usage)
- [Contributing](#contributing)

## Overview

This repository contains 50 ready-to-use GitHub Actions workflow templates covering:

- **Multi-language CI/CD** - Node.js, Python, Go, Java, .NET, Rust, Ruby
- **Cloud Deployments** - AWS, Azure, Google Cloud
- **Container Workflows** - Docker build, push, and Kubernetes deployments
- **Security Scanning** - CodeQL, Trivy, dependency review
- **Automation** - PR labeling, stale issue management, auto-merge
- **Testing** - Unit, integration, E2E with Playwright/Cypress
- **Notifications** - Slack, Discord integrations
- **Release Management** - Semantic release, changelog generation

## Workflow Categories

### 🔨 CI/CD Basics (1-10)
| # | Workflow | Description |
|---|----------|-------------|
| 01 | [Basic CI](/.github/workflows/01-ci-basic.yml) | Simple Node.js CI pipeline |
| 02 | [Multi Node Versions](/.github/workflows/02-multi-node-versions.yml) | Test across multiple Node.js versions |
| 03 | [Multi OS Testing](/.github/workflows/03-multi-os.yml) | Test on Linux, Windows, macOS |
| 04 | [Python CI](/.github/workflows/04-python-ci.yml) | Python project CI pipeline |
| 05 | [Go CI](/.github/workflows/05-go-ci.yml) | Go project CI pipeline |
| 06 | [Java Maven CI](/.github/workflows/06-java-maven.yml) | Java project with Maven |
| 07 | [Java Gradle CI](/.github/workflows/07-java-gradle.yml) | Java project with Gradle |
| 08 | [.NET CI](/.github/workflows/08-dotnet-ci.yml) | .NET project CI pipeline |
| 09 | [Rust CI](/.github/workflows/09-rust-ci.yml) | Rust project CI pipeline |
| 10 | [Ruby CI](/.github/workflows/10-ruby-ci.yml) | Ruby project CI pipeline |

### 🐳 Docker & Containers (11)
| # | Workflow | Description |
|---|----------|-------------|
| 11 | [Docker Build Push](/.github/workflows/11-docker-build-push.yml) | Multi-platform Docker builds with GHCR |

### 🔍 Code Quality (12-14)
| # | Workflow | Description |
|---|----------|-------------|
| 12 | [ESLint Prettier](/.github/workflows/12-eslint-prettier.yml) | JavaScript/TypeScript linting and formatting |
| 13 | [CodeQL Security](/.github/workflows/13-codeql-security.yml) | Automated security scanning |
| 14 | [Dependency Review](/.github/workflows/14-dependency-review.yml) | PR dependency vulnerability check |

### 📦 Publishing (15-17)
| # | Workflow | Description |
|---|----------|-------------|
| 15 | [npm Publish](/.github/workflows/15-npm-publish.yml) | Publish to npm registry |
| 16 | [PyPI Publish](/.github/workflows/16-pypi-publish.yml) | Publish to Python Package Index |
| 17 | [GitHub Pages](/.github/workflows/17-github-pages.yml) | Deploy static site to GitHub Pages |

### 💬 Notifications (18)
| # | Workflow | Description |
|---|----------|-------------|
| 18 | [Slack Notifications](/.github/workflows/18-slack-notifications.yml) | Build status to Slack |

### 🤖 Automation (19-20)
| # | Workflow | Description |
|---|----------|-------------|
| 19 | [Auto Label PRs](/.github/workflows/19-auto-label-prs.yml) | Label PRs based on file changes |
| 20 | [Stale Issues](/.github/workflows/20-stale-issues.yml) | Mark and close stale issues/PRs |

### ☁️ Infrastructure & Cloud (21-25)
| # | Workflow | Description |
|---|----------|-------------|
| 21 | [Terraform](/.github/workflows/21-terraform.yml) | Infrastructure as Code workflow |
| 22 | [Kubernetes Deploy](/.github/workflows/22-kubernetes-deploy.yml) | Deploy to Kubernetes cluster |
| 23 | [AWS S3 Deploy](/.github/workflows/23-aws-s3-deploy.yml) | Static site to S3 + CloudFront |
| 24 | [Azure Web App](/.github/workflows/24-azure-web-app.yml) | Deploy to Azure App Service |
| 25 | [Google Cloud Run](/.github/workflows/25-gcp-cloud-run.yml) | Deploy to Cloud Run |

### 🏷️ Release Management (26-27)
| # | Workflow | Description |
|---|----------|-------------|
| 26 | [Semantic Release](/.github/workflows/26-semantic-release.yml) | Automated versioning and changelog |
| 27 | [Release Drafter](/.github/workflows/27-release-drafter.yml) | Draft releases from merged PRs |

### 🧪 Testing (28-31)
| # | Workflow | Description |
|---|----------|-------------|
| 28 | [Coverage Report](/.github/workflows/28-coverage-report.yml) | Test coverage with Codecov |
| 29 | [Lighthouse CI](/.github/workflows/29-lighthouse-ci.yml) | Performance auditing |
| 30 | [Playwright E2E](/.github/workflows/30-playwright-e2e.yml) | End-to-end testing with Playwright |
| 31 | [Cypress E2E](/.github/workflows/31-cypress-e2e.yml) | End-to-end testing with Cypress |

### ⏰ Scheduled Tasks (32)
| # | Workflow | Description |
|---|----------|-------------|
| 32 | [Scheduled Backup](/.github/workflows/32-scheduled-backup.yml) | Automated database backups |

### 🔧 Advanced Patterns (33-40)
| # | Workflow | Description |
|---|----------|-------------|
| 33 | [Dependabot Auto-Merge](/.github/workflows/33-dependabot-auto-merge.yml) | Auto-merge Dependabot PRs |
| 34 | [Monorepo CI](/.github/workflows/34-monorepo-ci.yml) | CI for monorepo with path filters |
| 35 | [Caching Dependencies](/.github/workflows/35-caching-dependencies.yml) | Various caching strategies |
| 36 | [Artifacts Handling](/.github/workflows/36-artifacts-handling.yml) | Upload/download artifacts between jobs |
| 37 | [Environment Variables](/.github/workflows/37-environment-variables.yml) | Env vars and secrets usage |
| 38 | [Conditional Jobs](/.github/workflows/38-conditional-jobs.yml) | Conditional job execution |
| 39 | [Reusable Workflows](/.github/workflows/39-reusable-workflow-caller.yml) | Calling reusable workflows |
| 40 | [Manual Dispatch](/.github/workflows/40-manual-dispatch.yml) | Manually triggered with inputs |

### 🎯 Specialized Workflows (41-50)
| # | Workflow | Description |
|---|----------|-------------|
| 41 | [Composite Action](/.github/workflows/41-composite-action-usage.yml) | Using composite actions |
| 42 | [Database Migrations](/.github/workflows/42-database-migrations.yml) | Run database migrations |
| 43 | [PR Size Labeler](/.github/workflows/43-pr-size-labeler.yml) | Label PRs by size |
| 44 | [Branch Protection](/.github/workflows/44-branch-protection.yml) | Required status checks |
| 45 | [Trivy Security](/.github/workflows/45-trivy-security.yml) | Container security scanning |
| 46 | [API Documentation](/.github/workflows/46-api-documentation.yml) | Generate API docs |
| 47 | [Discord Notifications](/.github/workflows/47-discord-notifications.yml) | Build status to Discord |
| 48 | [Performance Benchmarking](/.github/workflows/48-performance-benchmarking.yml) | Track performance metrics |
| 49 | [Changelog Generation](/.github/workflows/49-changelog-generation.yml) | Auto-generate changelog |
| 50 | [Full CI/CD Pipeline](/.github/workflows/50-full-cicd-pipeline.yml) | Complete end-to-end pipeline |

## Configuration Files

This repository includes supporting configuration files:

| File | Purpose |
|------|---------|
| [.github/labeler.yml](/.github/labeler.yml) | PR labeling configuration |
| [.github/release-drafter.yml](/.github/release-drafter.yml) | Release drafter configuration |
| [.github/actions/setup-build/action.yml](/.github/actions/setup-build/action.yml) | Composite action example |

## Quick Start

1. **Copy a workflow** to your repository's `.github/workflows/` directory
2. **Update the workflow** with your specific settings (secrets, environment variables, etc.)
3. **Push changes** and watch the workflow run

### Example: Adding Basic CI

```bash
# Create workflows directory
mkdir -p .github/workflows

# Copy the basic CI workflow
curl -o .github/workflows/ci.yml \
  https://raw.githubusercontent.com/kelleyblackmore/github-actions-templates/main/.github/workflows/01-ci-basic.yml
```

## Usage

### Required Secrets

Most workflows require secrets to be configured. Common secrets include:

| Secret | Used By | Description |
|--------|---------|-------------|
| `GITHUB_TOKEN` | Most workflows | Automatically provided by GitHub |
| `NPM_TOKEN` | 15, 26 | npm registry authentication |
| `CODECOV_TOKEN` | 28 | Codecov coverage upload |
| `SLACK_WEBHOOK_URL` | 18 | Slack incoming webhook |
| `DISCORD_WEBHOOK` | 47 | Discord webhook URL |
| `AWS_ACCESS_KEY_ID` | 21-23, 32 | AWS access credentials |
| `AWS_SECRET_ACCESS_KEY` | 21-23, 32 | AWS secret credentials |
| `AZURE_CREDENTIALS` | 24 | Azure service principal |
| `WIF_PROVIDER` | 25 | GCP Workload Identity |
| `WIF_SERVICE_ACCOUNT` | 25 | GCP service account |

### Environment Configuration

Some workflows use GitHub Environments for deployment protection:

```yaml
jobs:
  deploy:
    environment: production  # Requires approval
```

Configure environments in your repository settings under **Settings > Environments**.

## Best Practices

### 1. Security
- Never commit secrets to the repository
- Use GitHub Secrets for sensitive data
- Enable Dependabot for dependency updates
- Run security scans (CodeQL, Trivy) regularly

### 2. Performance
- Use caching for dependencies
- Only run jobs when relevant files change (path filters)
- Use matrix builds sparingly
- Cancel in-progress runs on new pushes

### 3. Reliability
- Pin action versions (e.g., `@v4` not `@main`)
- Add timeouts to prevent runaway jobs
- Use `continue-on-error` for non-critical steps
- Implement proper error handling

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/new-workflow`)
3. Commit your changes (`git commit -m 'Add new workflow'`)
4. Push to the branch (`git push origin feature/new-workflow`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

---

⭐ If you find these templates helpful, please consider giving this repository a star!