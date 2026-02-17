# GitHub Pages Setup Instructions

This repository is configured to automatically deploy to GitHub Pages using GitHub Actions. However, GitHub Pages must be enabled in the repository settings first.

## Setup Steps

### 1. Enable GitHub Pages

1. Go to the repository settings: https://github.com/gmcdonald-sfg/ai-for-research/settings/pages
2. Under "Build and deployment":
   - **Source**: Select "GitHub Actions" from the dropdown menu
3. Save the settings

### 2. Trigger Deployment

Once GitHub Pages is enabled, the deployment will happen automatically:

- **Automatic**: Any push to the `main` branch will trigger the workflow
- **Manual**: Go to Actions tab and manually run the "Publish Quarto to GitHub Pages" workflow

### 3. Access Your Site

After successful deployment, your site will be available at:
https://gmcdonald-sfg.github.io/ai-for-research/

## Current Status

The GitHub Actions workflow is already configured and ready to deploy:
- ✅ Workflow file: `.github/workflows/publish.yml`
- ✅ Proper permissions configured
- ✅ HTML content rendered in `docs/` directory
- ❌ GitHub Pages needs to be enabled (see step 1 above)

## Troubleshooting

If the workflow fails with a 404 error mentioning "Ensure GitHub Pages has been enabled", it means step 1 above hasn't been completed yet.

### Recent Workflow Runs

You can check the status of workflow runs at:
https://github.com/gmcdonald-sfg/ai-for-research/actions/workflows/publish.yml

### Error: "Failed to create deployment (status: 404)"

This error indicates GitHub Pages is not enabled. Follow step 1 above to resolve.
