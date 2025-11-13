# Devhub Actions

## Description

This repository contains actions—TypeScript actions, composite actions, and workflows—used across DevHub's organization. These help automate CI/CD, code quality checks, deployments, and other development processes.

### Typescript Actions

Custom GitHub Actions written in TypeScript for advanced automation tasks. These can interact with APIs, perform complex logic, or integrate with external services.

**Usage Example:**
```yaml
- uses: DevHub-xs/devhub-actions/actions/<action-name>@v1
  with:
    # action inputs
```

### Composite Actions

Composite actions combine multiple steps (shell scripts, other actions) into a single reusable unit. Use these to simplify workflows and share common processes.

**Usage Example:**
```yaml
- uses: DevHub-xs/devhub-actions/composite/<action-name>@v1
```

### Workflows

Workflow templates provide ready-to-use automation for common DevHub tasks, such as building, testing, and deploying projects. Reference or copy these workflows to standardize processes.

**Usage Example:**
```yaml
name: CI
on: [push]
jobs:
  build:
    uses: DevHub-xs/devhub-actions/workflows/<workflow-name>@v1
```

