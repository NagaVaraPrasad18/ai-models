# AI Models Hosting Cabinet

This repository is used to host large LLM models for the Classic Notepad chat feature. 

### Why a separate repo?
By hosting models here, your main Notepad application stays small and deploys instantly. The 830MB model download is only performed once when you manually trigger the deployment in this repository.

## Setup Instructions

1. **Create a New Repository** on GitHub named `ai-models`.
2. **Push these files** to that repository:
   ```bash
   git init
   git add .
   git commit -m "Add model deployment workflow"
   git remote add origin https://github.com/YOUR_USERNAME/ai-models.git
   git push -u origin main
   ```
3. **Enable GitHub Pages**:
   - Go to `Settings` -> `Pages`.
   - Under "Build and deployment", set **Source** to `GitHub Actions`.
4. **Trigger the Download**:
   - Go to the `Actions` tab.
   - Select the `Deploy Models to GitHub Pages` workflow.
   - Click **Run workflow**.

Once complete, your models will be available at `https://YOUR_USERNAME.github.io/ai-models/`.
