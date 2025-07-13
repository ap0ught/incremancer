# GitHub Pages Setup Instructions

## Automatic Setup (Recommended)

This repository now includes a GitHub Actions workflow that will automatically deploy your site to GitHub Pages when you push to the master branch.

### To Enable GitHub Pages:

1. **Go to your repository settings:**
   - Navigate to `https://github.com/ap0ught/incremancer/settings/pages`
   - Or go to your repository → Settings → Pages (in the left sidebar)

2. **Configure the source:**
   - Under "Source", select **"GitHub Actions"**
   - This will use the workflow file at `.github/workflows/pages.yml`

3. **Save the configuration**
   - Click "Save" if prompted
   - GitHub will automatically deploy your site when you push changes to master

### Your site will be available at:
- **Primary URL:** `https://ap0ught.github.io/incremancer/`
- **Custom domain:** `https://chalice12.github.io/incremancer/` (if CNAME is configured)

## Manual Setup (Alternative)

If you prefer to use the traditional method:

1. Go to repository Settings → Pages
2. Under "Source", select **"Deploy from a branch"**
3. Choose **"master"** branch
4. Choose **"/ (root)"** folder
5. Click "Save"

## Verification

After enabling GitHub Pages:
- Check the "Actions" tab to see deployment status
- Visit your site URL to confirm it's working
- The game should load exactly as it does locally

## Notes

- The CNAME file is already configured for `chalice12.github.io/incremancer/`
- All development files (package.json, node_modules, etc.) are properly excluded
- The site is fully static and compatible with GitHub Pages
- No build process is required - it deploys the files directly