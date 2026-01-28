# 🎖️ Badge Submission Guide

Welcome to the GitHub Actions Learning Badge Program! This guide will help you submit your completed tasks and earn your digital badges.

## 📋 Before You Submit

Make sure you have:
- ✅ Completed all tasks for your desired level
- ✅ Taken clear screenshots or gathered evidence
- ✅ Read the [README.md](../../README.md) badge requirements
- ✅ Forked this repository (if you're contributing)

## 🏅 Three Badge Levels

### 🌟 Beginner Badge
**Tasks:** 1, 2, 3  
**Estimated Time:** 30 minutes  
**Submission File:** `beginner-badge-YOURNAME.md`

### ⭐⭐ Intermediate Badge
**Tasks:** 4, 5, 6, 7  
**Estimated Time:** 50 minutes  
**Submission File:** `intermediate-badge-YOURNAME.md`

### ⭐⭐⭐ Advanced Badge
**Tasks:** 8, 9, 10  
**Estimated Time:** 55 minutes  
**Submission File:** `advanced-badge-YOURNAME.md`

---

## 📝 How to Submit Your Badge

### Step 1: Fork & Clone
```bash
# Fork the repository on GitHub

# Clone your fork
git clone https://github.com/YOUR-USERNAME/github-actions-learning.git
cd github-actions-learning
```

### Step 2: Create a Submission Branch
```bash
# For Beginner Badge
git checkout -b submission/beginner-badge-yourname

# For Intermediate Badge
git checkout -b submission/intermediate-badge-yourname

# For Advanced Badge
git checkout -b submission/advanced-badge-yourname
```

### Step 3: Create Your Submission File
Create a new file in this folder (`.github/submissions/`) with your submission:

**Example:** `.github/submissions/beginner-badge-john-doe.md`

Use the appropriate template from [README.md](../../README.md):
- [Beginner Template](../../README.md#beginner-submission-template)
- [Intermediate Template](../../README.md#intermediate-submission-template)
- [Advanced Template](../../README.md#advanced-submission-template)

### Step 4: Add Your Evidence

Inside your submission file, add screenshots or proof for each task:
- Take screenshots of your workflow runs
- Show successful test outputs
- Demonstrate working implementations
- Include workflow YAML snippets if relevant
### Step 5: Commit & Push
```bash
git add .github/submissions/your-file.md
git commit -m "Add beginner badge submission for <your-name>"
git push origin submission/beginner-badge-yourname
```

### Step 6: Create a Pull Request

1. Go to the original repository: https://github.com/nisalgunawardhana/github-actions-learning
2. Click "Pull requests" → "New pull request"
3. Select "compare across forks"
4. Choose your fork and branch
5. Add a title with the badge emoji: **"🎖️ [BEGINNER] Badge Submission - Your Name"**
   - Make sure to include `🎖️` emoji
   - Include the level: `[BEGINNER]`, `[INTERMEDIATE]`, or `[ADVANCED]`
6. Select the **Badge Submission** template (if available)
7. Fill in all sections with your evidence

### Step 7: Automatic Assignment & Labels ⚡
**Don't worry - this happens automatically!**

When you create your PR with:
- ✅ The 🎖️ emoji in the title
- ✅ The level specified: BEGINNER/INTERMEDIATE/ADVANCED

Our automation workflow will automatically:
- 🤖 **Assign** the PR to `@nisalgunawardhana` for review
- 🤖 **Add labels:**
  - `submission` - Marks it as a submission
  - `pending-review` - Shows it's waiting for review
  - `beginner` / `intermediate` / `advanced` - Your badge level
- 🤖 **Post a welcome comment** thanking you for your submission
- 🤖 **Set status** as Pending Review

**No manual work needed from you!** Just create the PR with the correct format.

### Step 8: Wait for Review
Your submission will be reviewed within 2-5 days. The reviewer will:
- ✅ Verify all tasks are completed
- ✅ Check evidence quality
- ✅ Provide feedback if needed
- ✅ Approve and award your badge!

---

## ✨ What Makes a Great Submission

### ✅ DO:
- Take clear, focused screenshots
- Show full workflow runs with logs
- Include timestamps in evidence
- Write clear notes about your implementation
- Ask questions if unclear
- Double-check your work before submitting

### ❌ DON'T:
- Submit without completing all tasks
- Use blurry or unclear screenshots
- Leave placeholder text in templates
- Submit multiple times for the same level
- Forget to add labels and assignee

---

## 🎯 Review Timeline

| Level | Average Review Time | Status |
|-------|-------------------|--------|
| Beginner | 2-3 days | Pending Review |
| Intermediate | 2-3 days | Pending Review |
| Advanced | 3-5 days | Pending Review |

---

## ❓ Troubleshooting

### "My submission was rejected"
- Review the feedback provided in the PR comments
- Make the suggested improvements
- Push new commits to the same PR
- It will be re-reviewed

### "I don't have clear screenshots"
- Re-run your workflows
- Use the Actions tab to view logs
- Take new screenshots with visible task completion
- Update your submission

### "I'm unsure about evidence quality"
- Ask in the PR comments before submitting
- Reference specific tasks
- The reviewer will guide you

### "How do I know if my workflow is working?"
- Check the Actions tab in your GitHub repo
- Look for ✅ or ❌ indicators
- Read the workflow logs for details
- Feel free to ask for help in Issues

---

## 🏆 After You Earn Your Badge

Once approved:
- ✅ Your badge will be displayed in the README Hall of Fame
- ✅ You can display the badge in your portfolio
- ✅ You'll be recognized as a GitHub Actions learner!
- ✅ You can move on to the next level

---

## 🤖 Automated Features

Our submission process is powered by GitHub Actions automation! Here's what happens automatically:

### PR Auto-Assignment & Labeling
When you create a PR with:
- 🎖️ emoji in the title
- Badge level: BEGINNER/INTERMEDIATE/ADVANCED

**Automatic Actions:**
1. ✅ **Assigned to @nisalgunawardhana** - The reviewer receives your submission
2. ✅ **Labels Added Automatically:**
   - `submission` - Identifies as a badge submission
   - `pending-review` - Shows review status
   - `beginner`/`intermediate`/`advanced` - Your badge level
3. ✅ **Welcome Comment Posted** - We thank you for your submission
4. ✅ **Review Initiated** - Reviewer notified immediately

### Issue Auto-Assignment & Labeling
When you create a badge submission issue:
- ✅ **Assigned to @nisalgunawardhana**
- ✅ **Labels Added:** `submission`, `pending-review`, `[level]`
- ✅ **Welcome Comment Posted**
- ✅ **Tracking Issue Created**

### Correct PR Title Format

**✅ CORRECT:**
- `🎖️ [BEGINNER] Badge Submission - John Doe`
- `🎖️ [INTERMEDIATE] Badge Submission - Jane Smith`
- `🎖️ [ADVANCED] Badge Submission - Alex Johnson`

**❌ INCORRECT:**
- `Badge Submission` (missing emoji and level)
- `Beginner Badge` (missing emoji)
- `PR for Badge` (missing structure)

### What Gets Created Automatically

When your PR is opened:

| Item | Auto-Assigned | Auto-Labeled | Auto-Commented |
|------|---|---|---|
| **Reviewers** | ✅ @nisalgunawardhana | N/A | ✅ Welcome message |
| **Labels** | N/A | ✅ submission, pending-review, [level] | N/A |
| **Assignees** | ✅ @nisalgunawardhana | N/A | N/A |
| **Comments** | N/A | N/A | ✅ Confirmation |

---

1. **Check Documentation:** [README.md](../../README.md) & [TASKS.md](../../TASKS.md)
2. **Read Learning Docs:** [docs/](../../docs/)
3. **Create an Issue:** [Ask a Question](.github/ISSUE_TEMPLATE/question.md)
4. **Review Examples:** Check `.github/workflows/` for examples

---

## 📚 Learning Resources

- [GitHub Actions Docs](https://docs.github.com/en/actions)
- [Workflow Syntax](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions)
- [Actions Marketplace](https://github.com/marketplace?type=actions)

---

**Good luck! 🚀 We can't wait to see your submissions!**

For questions: [@nisalgunawardhana](https://github.com/nisalgunawardhana)
