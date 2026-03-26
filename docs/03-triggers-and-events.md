# Triggers and Events

## What is a Trigger?

A **trigger** (or event) tells GitHub Actions **when to run** a workflow. Without a trigger, your workflow never runs!

## Common Triggers

### 1. Push Events

Trigger when code is pushed to a branch:

```yaml
on: push
```

Trigger only on specific branches:

```yaml
on:
  push:
    branches:
      - main
      - develop
```

Trigger only when specific files change:

```yaml
on:
  push:
    paths:
      - "src/**"
      - "package.json"
```

Ignore specific branches or files:

```yaml
on:
  push:
    branches-ignore:
      - "hotfix/**"
    paths-ignore:
      - "README.md"
      - "docs/**"
```

### 2. Pull Request Events

Trigger when a PR is created or updated:

```yaml
on: pull_request
```

Trigger on specific PR branches:

```yaml
on:
  pull_request:
    branches: [main]
    types: [opened, synchronize, reopened]
```

PR action types:

- `opened` - PR is opened
- `synchronize` - New commits pushed to PR
- `reopened` - PR is reopened
- `closed` - PR is closed
- `edited` - PR title or description changed

### 3. Scheduled Events (Cron)

Cron patterns are used in GitHub Actions (and Linux cron jobs) to schedule workflows at specific times ⏰

#### 🔹 Cron Format (5 fields)

```
* * * * *
│ │ │ │ │
│ │ │ │ └── Day of week (0–7) (Sun = 0 or 7)
│ │ │ └──── Month (1–12)
│ │ └────── Day of month (1–31)
│ └──────── Hour (0–23)
└────────── Minute (0–59)
```

#### Basic Syntax

Run workflows on a schedule:

```yaml
on:
  schedule:
    - cron: "0 0 * * *" # Daily at midnight UTC
```

#### 🔹 Common Examples

**✅ Every 5 minutes**

```yaml
"*/5 * * * *"
```

**✅ Every hour**

```yaml
"0 * * * *"
```

**✅ Every day at midnight**

```yaml
"0 0 * * *"
```

**✅ Every day at 9 AM**

```yaml
"0 9 * * *"
```

**✅ Every Monday at 10 AM**

```yaml
"0 10 * * 1"
```

**✅ Every 1st day of month**

```yaml
"0 0 1 * *"
```

### 4. Manual Trigger

Allow manual workflow runs:

```yaml
on: workflow_dispatch
```

You can also accept inputs:

```yaml
on:
  workflow_dispatch:
    inputs:
      environment:
        description: "Environment to deploy to"
        required: true
        default: "staging"
      version:
        description: "Version to deploy"
        required: true
```

Access inputs in your workflow:

```yaml
steps:
  - name: Deploy to environment
    run: echo "Deploying ${{ github.event.inputs.environment }}"
```

### 5. Release Events

Trigger when releases are published:

```yaml
on:
  release:
    types: [published, created, edited]
```

### 6. Issues Events

Trigger on issue activity:

```yaml
on:
  issues:
    types: [opened, edited, closed, reopened]
```

### 7. Watch Events

Trigger when someone stars your repo:

```yaml
on: watch
```

### 8. Fork Events

Trigger when someone forks your repo:

```yaml
on: fork
```

### 9. Discussion Events

Trigger on discussion activity:

```yaml
on: discussions
```

## Multiple Triggers

Combine multiple triggers:

```yaml
on:
  push:
    branches: [main]
  pull_request:
    branches: [main]
  schedule:
    - cron: "0 0 * * 0" # Weekly
  workflow_dispatch:
```

## Advanced Trigger Conditions

### Using `if` Conditions

```yaml
on: push

jobs:
  test:
    runs-on: ubuntu-latest
    if: github.ref == 'refs/heads/main'
    steps:
      - run: npm test
```

### Exclude Branches

```yaml
on:
  push:
    branches:
      - "**" # All branches
      - "!gh-pages" # Except gh-pages
```

### Workflow Run Trigger

Trigger one workflow from another:

```yaml
on:
  workflow_run:
    workflows: [Build]
    types: [completed]
```

## Real-World Examples

### CI/CD Pipeline

```yaml
on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]
```

### Nightly Builds

```yaml
on:
  schedule:
    - cron: "0 2 * * *" # 2 AM daily
  workflow_dispatch:
```

### Deployment Workflow

```yaml
on:
  release:
    types: [published]
  workflow_dispatch:
    inputs:
      environment:
        description: "Environment"
        required: true
```

### Auto-Update Dependencies

```yaml
on:
  schedule:
    - cron: "0 0 * * 1" # Every Monday
```

## Best Practices

✅ Use **specific branches** instead of all branches  
✅ Use **paths** filters to avoid unnecessary runs  
✅ Use **scheduled workflows** for maintenance tasks  
✅ Use **workflow_dispatch** for manual operations  
✅ **Document** why workflows trigger when they do

## Common Mistakes

❌ Making workflows trigger too frequently  
❌ Not filtering branches (runs on all branches)  
❌ Setting cron jobs at the same time (GitHub might throttle)  
❌ Forgetting UTC timezone for scheduled runs  
❌ Too broad `paths` filters causing unnecessary runs

## Context Variables

Access trigger information in your workflow:

```yaml
steps:
  - name: Check branch
    run: echo "Branch: ${{ github.ref }}"

  - name: Check event
    run: echo "Event: ${{ github.event_name }}"

  - name: Check actor
    run: echo "Actor: ${{ github.actor }}"
```

## Next Steps

- [Jobs and Steps](04-jobs-and-steps.md) - Deep dive into execution
- [Secrets and Environment Variables](05-secrets-and-env.md) - Secure configuration
- [Build and Test](06-build-and-test.md) - Practical examples

---

**You now understand when workflows run! Next, let's dive deeper into jobs and steps.**
