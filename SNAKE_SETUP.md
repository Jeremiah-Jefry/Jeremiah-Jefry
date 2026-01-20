# GitHub Profile Snake Setup Guide

## What Changed? 🎉

1. **Header Background** - Changed from gradient to a vibrant cyan-purple gradient (`0:00D9FF,50:667EEA,100:764BA2`) for better visibility
2. **Contribution Snake** - Replaced static contribution graph with an animated snake that eats your contributions!

## How to Enable the Snake Animation 🐍

Follow these steps to get your contribution snake working:

### Step 1: Push to GitHub
```bash
git add .
git commit -m "Add contribution snake animation"
git push origin main
```

### Step 2: Enable GitHub Actions
1. Go to your repository: `https://github.com/Jeremiah-Jefry/Jeremiah-Jefry`
2. Click on **Settings** tab
3. In the left sidebar, click **Actions** → **General**
4. Under "Workflow permissions", select **Read and write permissions**
5. Check ✅ **Allow GitHub Actions to create and approve pull requests**
6. Click **Save**

### Step 3: Run the Workflow
1. Go to the **Actions** tab in your repository
2. Click on "Generate Snake" workflow in the left sidebar
3. Click **Run workflow** → **Run workflow**
4. Wait 1-2 minutes for it to complete

### Step 4: Verify
- Once complete, you should see a new `output` branch in your repository
- The snake animation will appear on your profile README!

## How It Works 🔧

- The GitHub Actions workflow runs **automatically every 24 hours**
- It also runs whenever you **push to main branch**
- You can **manually trigger** it anytime from the Actions tab
- The snake animation shows your actual GitHub contributions being "eaten" by the snake

## Troubleshooting 🔍

**If the snake doesn't appear:**
1. Make sure the workflow ran successfully (check Actions tab)
2. Verify the `output` branch was created
3. Check that the snake SVG files are in the `output` branch
4. Wait a few minutes and refresh your profile

**Common Issues:**
- If you get a permissions error, make sure you enabled "Read and write permissions" in Settings → Actions
- If the images show 404, the workflow hasn't run yet - trigger it manually

## Customization Options 🎨

You can customize the snake in `.github/workflows/snake.yml`:
- Change colors by modifying the `palette` parameter
- Adjust generation frequency by changing the cron schedule
- Add different color schemes for light/dark mode

Enjoy your animated contribution snake! 🐍✨
