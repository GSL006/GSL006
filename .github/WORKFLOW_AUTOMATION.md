# 🤖 Workflow Automation Guide

## ✅ Automatic vs Manual

All workflows are configured to run **AUTOMATICALLY**. Here's how each one works:

---

## 🐍 Snake Game Workflow (`snake.yml`)

### Automatic Triggers:
- ✅ **On push to main branch** - Runs immediately when you push
- ✅ **Every 6 hours** - Scheduled automatic updates
- ✅ **Manual trigger** - Optional via Actions tab

### What It Does:
- Generates animated snake game from your GitHub contributions
- Creates SVG and GIF files in `output/` directory
- Automatically commits the files back to your repo

### Setup Required:
- **None!** Just push the files and it works

---

## 📈 Activity Update Workflow (`update-activity.yml`)

### Automatic Triggers:
- ✅ **Every 6 hours** - Scheduled automatic updates
- ✅ **Manual trigger** - Optional via Actions tab
- ❌ Does NOT run on push (only schedule/manual)

### What It Does:
- Updates the "Coding Activity" section in your README
- Shows recent commits, PRs, and issues

### Setup Required:
- **None!** Uses built-in `GITHUB_TOKEN` automatically

---

## 🎯 Summary

| Workflow | Auto on Push | Auto Schedule | Manual Trigger | Setup Required |
|----------|-------------|---------------|----------------|----------------|
| Snake Game | ✅ Yes | ✅ Every 6h | ✅ Yes | ❌ None |
| Activity Update | ❌ No | ✅ Every 6h | ✅ Yes | ❌ None |

---

## 🚀 First Time Setup

**Just push your files!**

```bash
git add .
git commit -m "Add GitHub profile workflows"
git push origin main
```

That's it! The workflows will:
1. Run automatically on push
2. Continue running every 6 hours
3. Update your profile automatically

---

## 🔍 Checking Workflow Status

1. Go to your repository on GitHub
2. Click the **Actions** tab
3. You'll see all workflow runs and their status
4. Green checkmark = Success ✅
5. Red X = Failed (check logs) ❌

---

## ⚙️ Workflow Permissions

All workflows have `contents: write` permission, which means they can:
- ✅ Commit files back to your repository
- ✅ Update your README automatically
- ✅ Create/update files in `output/` directory

This is safe and expected behavior for profile README workflows.

---

## 🐛 Troubleshooting

### Workflows Not Running?

1. **Check Actions are enabled:**
   - Repo Settings → Actions → General
   - Ensure "Allow all actions and reusable workflows" is selected

2. **Check branch name:**
   - Workflows trigger on `main` branch
   - If your default branch is `master`, update the workflow files

3. **Check workflow files location:**
   - Must be in `.github/workflows/` directory
   - Files must have `.yml` or `.yaml` extension

### Snake Game Not Appearing?

- Wait 1-2 minutes after push
- Check Actions tab for workflow completion
- Verify `output/` directory exists in your repo
- Check README path matches: `output/github-contribution-grid-snake.svg`

---

## 💡 Pro Tips

1. **First push triggers everything** - All workflows run on your first push
2. **Check Actions tab** - See real-time progress of all workflows
3. **Manual trigger anytime** - Use "Run workflow" button if needed
4. **No maintenance needed** - Once set up, everything runs automatically

---

**Enjoy your automatically updating GitHub profile! 🎉**

