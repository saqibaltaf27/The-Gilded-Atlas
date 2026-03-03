# The Gilded Atlas - Automated Deployment Pipeline

## Project Overview
This project implements a lightweight CI/CD pipeline using Github Actions to automatically deploy a static HTML website to Github Pages whenever changes are published to the main branch.

The goal is to eliminate manual file uploads and ensure reliable, automated, and error-free deployments.

## Technology Stack
- HTML5
- CSS3 (Responsive, Mobile-First)
- Github Actions (CI/CD)
- Github Pages (Hosting)

## CI/CD Pipeline Workflow Overiew
The automation pipeline perfroms the following steps:
1. Triggered automatically on every push to the 'main' branch.
2. Checks out the repository.
3. Verifies that 'index.html' exists.
4. Uploads the site as an aritfact.
5. Deploys the site to Github Pages.

The workflow uses the latest stable Github Actions versions:
- 'actions/checout@v4'
- 'actions/configure-pages@v4'
- 'actions/upload-pages-artifact@v3'
- 'actions/deploye-pages@v4'

## How To Trigger The Deployment Pipeline
To Trigger a deployment:
1. Open 'index.html'
2. Make Any Modification (e.g., update header text)
3. Commit Changes. 
4. Push

The Github Action will start automatically.
Deployment completes within approximately 1-3 minutes.

## How To Verify a Successful Deployment
1. Go to the repository on Github.
2. Click the Actions tab.
3. Select: Deploy Static Site to Github Pages.
4. Confirm the latest workflow run shows a green checkmark.
5. Click the run to view logs if needed.

## Live Website URL
After successful deployment, the site is available at: https://saqibaltaf27.github.io/The-Gilded-Atlas/
