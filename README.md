# nutrii - Android App

Generated from web app using Capacitor.

## 🚀 QUICK START GUIDE (Follow Exactly!)

### Step 1: Create Repository (CRITICAL - Do This Right!)
1. Go to https://github.com/new
2. **Name:** Enter any name (e.g., "my-android-app")
3. **Visibility:** Select **PUBLIC** (required for free GitHub Actions)
4. ✅ **CHECK:** "Add a README file" (This creates the main branch!)
5. Click **"Create repository"**

### Step 2: Enable Workflow Permissions (REQUIRED!)
**⚠️ If you skip this, the workflow won't work!**

1. In your new repo, click the **Settings** tab (top right)
2. In the left sidebar, click **Actions** → **General**
3. Scroll down to **"Workflow permissions"**
4. Select **"Read and write permissions"**
5. Click **Save**

### Step 3: Upload Your Files
1. **Extract** the ZIP file you downloaded from the converter tool
2. In your GitHub repo, click **"Add file"** → **"Upload files"**
3. **Drag and drop ALL files** from the extracted folder:
   - package.json
   - capacitor.config.json
   - ionic.config.json
   - src/ folder (with your web app)
   - .github/workflows/build-android.yml
4. **Important:** At the bottom, select **"Commit directly to the main branch"**
5. Click **"Commit changes"**

### Step 4: Wait for Auto-Build
1. Immediately click the **Actions** tab at the top
2. You should see **"Build Android APK"** running automatically!
3. If you see "Get started with GitHub Actions", wait 10 seconds and refresh
4. Wait 3-5 minutes for the green checkmark ✅

### Step 5: Download APK
1. Click the completed workflow run
2. Scroll to **Artifacts** section
3. Download **app-debug.apk**
4. Install on your Android device!

---

## 🔧 Troubleshooting Guide

### Problem: "Get started with GitHub Actions" appears instead of workflow
**Causes & Solutions:**
- **Didn't check "Add README" when creating repo?** → Create any file first to initialize main branch
- **Committed to a new branch instead of main?** → Merge that branch to main or commit directly to main
- **Actions disabled?** → Settings → Actions → General → Allow all actions
- **Workflow file in wrong location?** → Ensure it's at ".github/workflows/build-android.yml"

**Quick Fix:**
1. Go to your repo's main page
2. Click the file "README.md"
3. Click the ✏️ (edit) icon
4. Add a space anywhere, then click **"Commit changes"**
5. This should trigger the workflow!

### Problem: Workflow runs but no APK artifact appears
**Solution:**
1. Check you enabled **"Read and write permissions"** in Step 2
2. Click the failed workflow run
3. Look at the logs - likely missing "index.html" in src/ folder

### Problem: APK installs but app shows blank screen
**Solution:**
- Ensure your web app uses **relative paths** (`./style.css` not "/style.css")
- Check that "index.html" is directly in src/ folder (not in a subfolder)
- Open browser DevTools in the app to see errors (if you know how)

### Problem: Build fails with "capacitor.config.json not found"
**Solution:**
- Make sure you uploaded "capacitor.config.json" to the root of the repository
- Don't rename it or change its contents

---

## 📱 Detected Features
- Basic WebView

## 🔄 Making Updates
Every time you update files in GitHub and commit to main, the APK will rebuild automatically!

---
*Generated with ❤️ by Web to Android Converter*  
*Final Fixed Version - March 2025*  
*Workflow auto-triggers on upload - no manual trigger needed!*