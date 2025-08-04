# GitHub Pages Deployment

This repository is configured with automated deployment to GitHub Pages. The deployment happens automatically when code is pushed to the `main` branch.

## How it works

1. **Trigger**: The workflow runs on every push to the `main` branch
2. **Build**: Uses Bun to install dependencies and run the build process (`bun ./build.ts`)
3. **Deploy**: Deploys only the contents of the `build/` directory to GitHub Pages

## Manual Configuration Required

To enable GitHub Pages for this repository, a repository administrator needs to:

1. Go to repository Settings → Pages
2. Set Source to "GitHub Actions"
3. The site will be available at `https://<username>.github.io/<repository-name>/`

## Build Process

The build process:
- Installs Bun runtime
- Runs `bun install` to install dependencies
- Executes `bun ./build.ts` to build the static files
- Uploads only the `build/` directory contents to GitHub Pages

The build creates a single minified HTML file with all CSS and JavaScript inlined, along with any static resources like robots.txt and favicon.ico.