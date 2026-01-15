# 🚀 GitHub Actions Learning Repository

Welcome to your hands-on learning journey with **GitHub Actions**! This repository is designed for beginners and intermediate developers who want to master CI/CD automation.

<p align="center">
    <img src="images/banner.png" alt="GitHub for Beginners banner" />
</p>

[![Follow me on GitHub](https://img.shields.io/github/followers/nisalgunawardhana?label=Follow&style=social)](https://github.com/nisalgunawardhana)
[![Star this repo](https://img.shields.io/github/stars/nisalgunawardhana/github-actions-learnin?style=social)](https://github.com/nisalgunawardhana/github-actions-learning/stargazers)

## 📚 What You'll Learn

- ✅ GitHub Actions fundamentals (workflows, jobs, steps)
- ✅ Automating builds and tests
- ✅ CI/CD pipeline creation
- ✅ Deploying applications to Azure App Service
- ✅ Working with secrets and environment variables
- ✅ Real-world workflow examples

## 🎯 Target Audience

- Beginners to CI/CD
- Developers wanting to automate their workflows
- Students learning DevOps practices
- Anyone interested in GitHub Actions

## 📋 Prerequisites & Setup

### Requirements
- A GitHub account
- Git installed locally
- Node.js v16+ installed
- (Optional) Azure account for deployment tasks

### Quick Setup (5 minutes)

1. **Fork this repository**
   ```bash
   # Click "Fork" button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/github-actions-learning.git
   cd github-actions-learning
   ```

3. **Install dependencies for sample app**
   ```bash
   cd sample-app
   npm install
   npm start
   ```
   Visit `http://localhost:3000` - you should see the welcome page!

4. **Run tests locally**
   ```bash
   npm test
   ```
   All tests should pass ✅

---

## 📚 Learning Content & Documentation

### 1️⃣ Start Here: Quick Start (5 minutes)

**Getting started immediately:**
- Fork the repository
- Clone: `git clone https://github.com/YOUR-USERNAME/github-actions-learning.git`
- Install: `cd sample-app && npm install`
- Run: `npm start` (visit http://localhost:3000)
- Test: `npm test`

### 2️⃣ Read Documentation (45-60 minutes)

Go through these in order in the `docs/` folder:

1. [01-what-is-github-actions.md](docs/01-what-is-github-actions.md) - Concepts & basics (10 min)
2. [02-workflow-basics.md](docs/02-workflow-basics.md) - YAML syntax & structure (15 min)
3. [03-triggers-and-events.md](docs/03-triggers-and-events.md) - When workflows run (10 min)
4. [04-jobs-and-steps.md](docs/04-jobs-and-steps.md) - Execution model (15 min)
5. [05-secrets-and-env.md](docs/05-secrets-and-env.md) - Security & configuration (10 min)
6. [06-build-and-test.md](docs/06-build-and-test.md) - CI/CD patterns (15 min)
7. [07-deploy-to-azure.md](docs/07-deploy-to-azure.md) - Cloud deployment (10 min)

### 3️⃣ Complete All Tasks (2-4 hours)

Follow [TASKS.md](TASKS.md) for 10+ hands-on exercises organized by difficulty:

| Level | Tasks | Time | Skills |
|-------|-------|------|--------|
| 🌟 **Beginner** | 1-3 | 30 min | Fundamentals & basics |
| ⭐⭐ **Intermediate** | 4-7 | 1-2 hours | Workflow creation & automation |
| ⭐⭐⭐ **Advanced** | 8-10 | 2-3 hours | Production-ready patterns |

### 4️⃣ Example Workflows

Three production-ready workflows to learn from:

- **[hello-world.yml](.github/workflows/hello-world.yml)** - Basic workflow, manual triggers
- **[build-test.yml](.github/workflows/build-test.yml)** - CI/CD pipeline with matrix testing
- **[deploy-azure-app-service.yml](.github/workflows/deploy-azure-app-service.yml)** - Production deployment

---

## 🏅 Earn Digital Badges

Complete tasks at each level and submit your work to earn prestigious badges!

### 🌟 Beginner Badge
**Complete Tasks 1-3**

**Steps:**
1. Complete all Beginner tasks in [TASKS.md](TASKS.md#beginner-tasks-)
2. Take screenshots of successful workflow runs
3. Fork the repo → Create branch `working-beginner-yourname`
4. Create file `.github/submissions/beginner-yourname.md` with evidence
5. Commit → Push → Create Pull Request
6. Submit link via [🎖️ Badge Submission issue](.github/ISSUE_TEMPLATE/badge_submission.md) (select "Beginner")
7. Automatic labels applied: `submission`, `beginner`, `pending-review`
8. Auto-assigned to reviewer for approval

**Proof needed:**
- Task 1: Hello World workflow running ✅
- Task 2: Workflow triggered by push event ✅
- Task 3: Local tests passing with npm test ✅

---

### ⭐⭐ Intermediate Badge
**Complete Tasks 4-7**

**Steps:**
1. Complete all Intermediate tasks in [TASKS.md](TASKS.md#intermediate-tasks-)
2. Gather workflow execution screenshots and logs
3. Fork the repo → Create branch `working-intermediate-yourname`
4. Create file `.github/submissions/intermediate-yourname.md` with evidence
5. Commit → Push → Create Pull Request
6. Submit link via [🎖️ Badge Submission issue](.github/ISSUE_TEMPLATE/badge_submission.md) (select "Intermediate")
7. Automatic labels applied: `submission`, `intermediate`, `pending-review`
8. Auto-assigned to reviewer for approval

**Proof needed:**
- Task 4: Custom workflow running on develop branch ✅
- Task 5: Environment variables displaying in logs ✅
- Task 6: GitHub secrets access (masked in logs) ✅
- Task 7: Matrix testing across 3 Node versions in parallel ✅

---

### ⭐⭐⭐ Advanced Badge
**Complete Tasks 8-10**

**Steps:**
1. Complete all Advanced tasks in [TASKS.md](TASKS.md#advanced-tasks-)
2. Gather comprehensive screenshots and workflow logs
3. Fork the repo → Create branch `working-advanced-yourname`
4. Create file `.github/submissions/advanced-yourname.md` with evidence
5. Commit → Push → Create Pull Request
6. Submit link via [🎖️ Badge Submission issue](.github/ISSUE_TEMPLATE/badge_submission.md) (select "Advanced")
7. Automatic labels applied: `submission`, `advanced`, `pending-review`
8. Auto-assigned to reviewer for approval

**Proof needed:**
- Task 8: Artifacts uploaded & downloaded between jobs ✅
- Task 9: Conditional execution (deploy on main only) ✅
- Task 10: PR created with template & issue using template ✅

---

## 🎯 Submission Process Simplified

### One Simple Way to Submit

1. **Fork the repo** (click Fork button)

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/github-actions-learning.git
   cd github-actions-learning
   ```

3. **Create working branch** (use this naming: `working-<level>-<yourname>`)
   ```bash
   git checkout -b working-beginner-john
   ```

4. **Complete your tasks** from TASKS.md and gather evidence (screenshots)

5. **Create submission file** in `.github/submissions/`
   ```bash
   # Create this folder if it doesn't exist
   mkdir -p .github/submissions
   
   # Create file: beginner-john.md (for Beginner)
   # or: intermediate-john.md (for Intermediate)
   # or: advanced-john.md (for Advanced)
   ```

6. **Add evidence to your file** (screenshots, workflow links, etc.)

7. **Commit your changes**
   ```bash
   git add .github/submissions/beginner-john.md
   git commit -m "feat: add beginner badge submission"
   git push origin working-beginner-john
   ```

8. **Create Pull Request** on GitHub with your branch

9. **Submit Tracking Issue** via [🎖️ Badge Submission](https://github.com/YOUR-USERNAME/your-repo/issues/new?assignees=nisalgunawardhana&labels=submission%2Cpending-review&template=badge_submission.md&title=Badge+Submission)
   - Select your level (Beginner/Intermediate/Advanced)
   - Paste your PR link
   - Labels & assignment happen automatically!

**That's it!** 🎉 Automatic labels and assignment handle the rest.

---

## ✅ What Happens After Submission

| Step | Automatic | Manual |
|------|-----------|--------|
| **Level Selection** | N/A | You choose in issue |
| **Labels Added** | ✅ Auto (submission + level) | N/A |
| **Assignment** | ✅ Auto (@nisalgunawardhana) | N/A |
| **Review** | Manual (2-5 days) | Reviewer checks evidence |
| **Feedback** | Comments on PR | If revisions needed |
| **Approval** | Issue closed | Badge awarded! 🏅 |

---

## 📋 Submission File Template

Create a simple markdown file with your evidence:

```markdown
# Beginner Badge Submission - Your Name

**Date:** January 2026
**Status:** Submitted for Review

## Tasks Completed

- [x] Task 1: Run Your First Workflow
- [x] Task 2: Understand Workflow Triggers
- [x] Task 3: Build and Test Locally

## Evidence

### Task 1: Hello World Workflow
[Screenshot showing successful workflow run]

### Task 2: Push Trigger
[Screenshot showing workflow triggered automatically on push]

### Task 3: Local Tests
[Screenshot showing npm test output - all passing]

## Notes
Any challenges faced or additional context.

---

Submitted & ready for review! ✅
```

That's all you need! No complex templates, just clear evidence.

---

## 🗂️ Repository Structure

```
github-actions-learning/
├── README.md                          # Main guide (this file)
├── TASKS.md                           # All learning tasks (10+)
├── CONTRIBUTING.md                    # How to contribute
├── LICENSE                            # MIT License
│
├── docs/                              # Learning documentation
│   ├── 01-what-is-github-actions.md
│   ├── 02-workflow-basics.md
│   ├── 03-triggers-and-events.md
│   ├── 04-jobs-and-steps.md
│   ├── 05-secrets-and-env.md
│   ├── 06-build-and-test.md
│   └── 07-deploy-to-azure.md
│
├── images/                            # Digital badges
│   ├── Beginner.png
│   ├── Intermediate.png
│   └── Advanced.png
│
├── .github/
│   ├── workflows/                     # Example workflows
│   │   ├── hello-world.yml
│   │   ├── build-test.yml
│   │   └── deploy-azure-app-service.yml
│   ├── submissions/                   # Your badge submissions go here
│   ├── ISSUE_TEMPLATE/
│   │   ├── badge_submission.md        # 🎖️ Submit badge (auto-labels & assigns!)
│   │   ├── bug_report.md              # Report bugs
│   │   ├── feature_request.md         # Suggest improvements
│   │   ├── documentation.md           # Improve docs
│   │   └── question.md                # Ask questions
│   └── PULL_REQUEST_TEMPLATE.md       # PR template
│
└── sample-app/                        # Sample Node.js app
    ├── src/server.js
    ├── tests/server.test.js
    ├── package.json
    └── README.md
```

---

## 🔄 Learning & Development Workflow

### For Self-Paced Learning

1. **Preparation** (5 min)
   - Fork repository
   - Clone to your machine
   - Setup sample app

2. **Study** (45-60 min)
   - Read documentation in docs/ folder
   - Understand concepts
   - Review example workflows

3. **Practice** (2-4 hours)
   - Complete TASKS.md exercises
   - Run workflows
   - Modify and experiment

4. **Submit** (10 min)
   - Create submission file with evidence
   - Push to GitHub
   - Create PR and submit tracking issue
   - Auto-labels and auto-assigns!

5. **Review** (2-5 days)
   - Reviewer checks your work
   - Feedback if needed
   - Badge awarded! 🏅

### For Team/Classroom Use

1. **Setup**
   - Clone this repository to your organization
   - Share link with team/students

2. **Students Fork & Learn**
   - Each student forks the repo
   - Creates `working-*` branch
   - Completes tasks locally

3. **Submit via PR**
   - Creates submission file
   - Opens PR on main repo
   - Submits tracking issue with level selection

4. **Auto-Organization**
   - Labels apply automatically (`submission`, `beginner`/`intermediate`/`advanced`)
   - Assignment automatic
   - Reviewers can focus on quality

5. **Feedback & Approval**
   - Reviewer provides feedback
   - Student makes revisions if needed
   - Badge awarded on approval

---

## 🎓 Complete Task List

### 🌟 Beginner Tasks (30 min total)

| # | Task | Time | What You Learn |
|-|------|------|---|
| 1 | [Run Your First Workflow](TASKS.md#task-1-run-your-first-workflow) | 5 min | Trigger workflows manually, read logs |
| 2 | [Understand Workflow Triggers](TASKS.md#task-2-understand-workflow-triggers) | 10 min | Automatic triggers on push |
| 3 | [Build and Test Locally](TASKS.md#task-3-build-and-test-locally) | 15 min | Run app & tests locally |

**Submit:** [🎖️ Beginner Badge Issue](.github/ISSUE_TEMPLATE/badge_submission.md) → Select "Beginner" → Auto-labels & assigns!

---

### ⭐⭐ Intermediate Tasks (1-2 hours total)

| # | Task | Time | What You Learn |
|-|------|------|---|
| 4 | [Create a Custom Workflow](TASKS.md#task-4-create-a-custom-workflow) | 15 min | Build workflows from scratch |
| 5 | [Add Environment Variables](TASKS.md#task-5-add-environment-variables) | 10 min | Configure with env vars |
| 6 | [Use GitHub Secrets](TASKS.md#task-6-use-github-secrets) | 10 min | Handle sensitive data securely |
| 7 | [Matrix Testing](TASKS.md#task-7-matrix-testing) | 15 min | Test multiple Node versions |

**Submit:** [🎖️ Intermediate Badge Issue](.github/ISSUE_TEMPLATE/badge_submission.md) → Select "Intermediate" → Auto-labels & assigns!

---

### ⭐⭐⭐ Advanced Tasks (2-3 hours total)

| # | Task | Time | What You Learn |
|-|------|------|---|
| 8 | [Upload and Download Artifacts](TASKS.md#task-8-upload-and-download-artifacts) | 20 min | Share data between jobs |
| 9 | [Conditional Execution](TASKS.md#task-9-conditional-execution) | 15 min | Run steps conditionally |
| 10 | [Create a PR and Use Issue Templates](TASKS.md#task-10-create-a-pr-and-use-issue-templates) | 20 min | Contribute to projects |

**Submit:** [🎖️ Advanced Badge Issue](.github/ISSUE_TEMPLATE/badge_submission.md) → Select "Advanced" → Auto-labels & assigns!

---

### 🏆 Bonus Challenges

- [Challenge 1: Deploy to Azure](TASKS.md#challenge-1-deploy-to-azure-optional) - Production deployment
- [Challenge 2: Add Code Coverage](TASKS.md#challenge-2-add-code-coverage-reports) - Quality metrics
- [Challenge 3: Custom Action](TASKS.md#challenge-3-create-a-custom-action) - Reusable automation

---

## 🔧 Example Workflows Explained

### 1. Hello World Workflow
**File:** [.github/workflows/hello-world.yml](.github/workflows/hello-world.yml)

```yaml
name: Hello World
on: push
jobs:
  hello:
    runs-on: ubuntu-latest
    steps:
      - run: echo "Hello, GitHub Actions!"
```

**Learn:** Basic workflow structure, triggers, steps  
**Related Tasks:** [Task 1](TASKS.md#task-1-run-your-first-workflow), [Task 2](TASKS.md#task-2-understand-workflow-triggers)

---

### 2. Build & Test Workflow
**File:** [.github/workflows/build-test.yml](.github/workflows/build-test.yml)

Uses matrix testing across Node versions, installs dependencies, runs tests.

**Learn:** Matrix strategies, dependencies, caching  
**Related Tasks:** [Task 3](TASKS.md#task-3-build-and-test-locally), [Task 7](TASKS.md#task-7-matrix-testing)

---

### 3. Deploy to Azure Workflow
**File:** [.github/workflows/deploy-azure-app-service.yml](.github/workflows/deploy-azure-app-service.yml)

Builds and deploys app to Azure App Service.

**Learn:** Production deployment, secrets, conditional execution  
**Related Tasks:** [Task 6](TASKS.md#task-6-use-github-secrets), [Challenge 1](TASKS.md#challenge-1-deploy-to-azure-optional)

---

## 📚 Documentation Overview

| Doc | Topics | Duration | Level |
|-----|--------|----------|-------|
| [01-what-is-github-actions.md](docs/01-what-is-github-actions.md) | What & why GitHub Actions | 10 min | Beginner |
| [02-workflow-basics.md](docs/02-workflow-basics.md) | Workflow structure & YAML | 15 min | Beginner |
| [03-triggers-and-events.md](docs/03-triggers-and-events.md) | When workflows run | 10 min | Beginner |
| [04-jobs-and-steps.md](docs/04-jobs-and-steps.md) | Jobs, steps, runners | 15 min | Intermediate |
| [05-secrets-and-env.md](docs/05-secrets-and-env.md) | Configuration & security | 10 min | Intermediate |
| [06-build-and-test.md](docs/06-build-and-test.md) | CI/CD pipelines | 15 min | Intermediate |
| [07-deploy-to-azure.md](docs/07-deploy-to-azure.md) | Azure deployment | 10 min | Advanced |

**Total Learning Time:** ~1.5 hours of documentation  
**Total Task Time:** 3-6 hours of hands-on practice

---

## 💡 Tips for Success

### Learning Tips
1. **Start sequentially** - Don't skip around
2. **Read the docs first** - Foundation matters
3. **Run the examples** - See it in action
4. **Modify workflows** - Experiment & break things
5. **Read the logs** - GitHub Actions logs tell you everything
6. **Add comments** - Document what you learn

### Task Completion Tips
1. **Screenshot everything** - For badge submission
2. **Take your time** - Quality > Speed
3. **Experiment with modifications** - "What if I..."
4. **Get stuck?** - Create a [Question issue](.github/ISSUE_TEMPLATE/question.md)
5. **Found a problem?** - Report [Bug report](.github/ISSUE_TEMPLATE/bug_report.md)

### Submission Tips
1. **Create clear submission files** - Organize evidence well
2. **Use descriptive commit messages** - Help reviewers understand
3. **Follow branch naming** - `working-level-yourname`
4. **Set level in issue** - Triggers auto-labels
5. **Link your PR** - Include it in submission issue

---

## 🤝 How to Contribute

If you find issues or have improvements:

1. **Report Issues**
   - Use [bug_report.md](.github/ISSUE_TEMPLATE/bug_report.md)
   - Use [feature_request.md](.github/ISSUE_TEMPLATE/feature_request.md)
   - Use [documentation.md](.github/ISSUE_TEMPLATE/documentation.md)

2. **Contribute Code**
   - Fork repository
   - Create branch: `feature/your-feature`
   - Make changes
   - Create PR using [PULL_REQUEST_TEMPLATE.md](.github/PULL_REQUEST_TEMPLATE.md)
   - See [CONTRIBUTING.md](CONTRIBUTING.md) for details

3. **Share Knowledge**
   - Improve documentation
   - Create clearer examples
   - Help others in issues

---

## 📞 Support & Questions

### Getting Help

1. **Check Documentation** - Start with [docs/](docs/) folder
2. **Review Examples** - Look at workflows in [.github/workflows/](.github/workflows/)
3. **Check TASKS.md** - Find similar examples
4. **Create Issue** - Use [question.md](.github/ISSUE_TEMPLATE/question.md) template
5. **Contact Maintainer** - [@nisalgunawardhana](https://github.com/nisalgunawardhana)

### Common Issues

**Q: My workflow isn't running?**  
A: Check the trigger event. See [03-triggers-and-events.md](docs/03-triggers-and-events.md)

**Q: How do I use secrets safely?**  
A: See [05-secrets-and-env.md](docs/05-secrets-and-env.md)

**Q: How do I deploy to Azure?**  
A: See [07-deploy-to-azure.md](docs/07-deploy-to-azure.md) and [Challenge 1](TASKS.md#challenge-1-deploy-to-azure-optional)

---

## 🎖️ Badge Submission Tracking

### Submission Flow

```
Start → Learn → Complete Tasks → Create Branch → Submit File 
  → Push PR → Submit Issue → Auto-Labels & Assign → Review → Badge! 🏅
```

### Automatic Workflow

1. **You choose level** in badge submission issue
2. **System auto-adds labels** - `submission`, `beginner`/`intermediate`/`advanced`
3. **System auto-assigns** - @nisalgunawardhana
4. **Reviewer reviews** - 2-5 days
5. **Feedback or approval** - You're notified
6. **Badge awarded!** - Congratulations! 🎉

### No Manual Labeling Needed! ✨

Just select your level in the issue → Everything else is automatic!

---

## 📊 Repository Statistics

- 📚 **7 Learning Modules** in docs/
- 🔧 **3 Example Workflows** ready to use
- 📝 **10+ Hands-On Tasks** organized by level
- 💻 **Sample Node.js App** with tests
- 📄 **Multiple Issue Templates** for contributions
- 🎖️ **Badge System** with auto-organization

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⭐ Show Your Support

- ⭐ Star this repository
- 🔀 Share with friends/colleagues
- 📢 Tell others about it
- 🤝 Contribute improvements
- 💬 Provide feedback

---

**Ready to get started? Begin with setup above or jump to [TASKS.md](TASKS.md)!** 🚀

**Questions?** Create an [❓ Question Issue](.github/ISSUE_TEMPLATE/question.md)

**Happy Learning!** 🎓

Learning GitHub Actions 🚀



