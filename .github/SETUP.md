# GitHub Profile Setup Guide

## 🐍 Snake Game Setup

**✅ AUTOMATIC - No Manual Setup Required!**

The snake game workflow runs automatically:
- **On push to main branch** - Runs immediately when you push the workflow files
- **Every 6 hours** - Scheduled automatic updates
- **Manual trigger** - Optional, via Actions tab → "Run workflow"

**First Time Setup:**
1. Just commit and push all files to your repository
2. The workflow will run automatically on the first push
3. Wait 1-2 minutes for it to complete
4. The snake animation will appear in your README

**To manually trigger (optional):**
1. Go to the **Actions** tab in your repository
2. Select **Generate Snake Game** workflow
3. Click **Run workflow** → **Run workflow**

## 📊 GitHub Stats

The GitHub stats use the `github-readme-stats` API. If you see errors:

1. **Rate Limiting**: The API may be rate-limited. Wait a few minutes and refresh.
2. **Cache**: Stats are cached for 24 hours (`cache_seconds=86400`) to reduce API calls.
3. **Private Repos**: Set `count_private=false` if you don't want private repo stats.

## 🔧 Troubleshooting

### Snake Game Not Showing
- Check if the `output/` directory exists in your repo
- Verify the workflow ran successfully in the Actions tab
- Ensure the file path in README matches: `output/github-contribution-grid-snake.svg`

### Stats Not Loading
- The API might be temporarily down - wait and refresh
- Check your username is correct: `GSL006`
- Try accessing the API URL directly in your browser

### Workflow Errors
- Ensure repository has Actions enabled
- Check that the workflow has write permissions
- Verify you're on the `main` branch

## 🚀 Quick Start

**Everything runs automatically! Just follow these steps:**

1. **Commit and push** all files to your repository
   - The workflows will trigger automatically on push
2. **Wait 1-2 minutes** for workflows to complete
   - Check the Actions tab to see progress
3. **Refresh your profile** to see all animations

**That's it!** No manual setup needed. The workflows will continue running automatically every 6 hours.

## 📝 Notes

- The snake game updates every 6 hours automatically
- Stats cache for 24 hours to reduce API load
- All workflows run on GitHub's free tier

