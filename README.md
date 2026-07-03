# Mohammed Raheem CK — CV Website

## How to deploy on GitHub Pages

1. Create a new **public** GitHub repository (any name, e.g. `Raheem_ck`).
2. Upload these files to the **root** of the repo, keeping the folder structure:
   - `index.html`
   - `Mohammed_Raheem_CK_Resume.pdf`
   - `.github/workflows/deploy.yml`  ← must stay in this exact path
3. Go to **Settings → Pages**.
4. Under **Build and deployment → Source**, select **GitHub Actions**.
5. Go to the **Actions** tab — the "Deploy to GitHub Pages" workflow will run automatically.
   Once it finishes with a green check, your site is live at:
   `https://<your-username>.github.io/<repo-name>/`

## Updating the site later

Any time you push changes to the `main` branch (or re-upload files via the GitHub website),
the workflow re-runs automatically and redeploys the site — no manual steps needed.

## Troubleshooting

- **Workflow fails immediately**: check *Settings → Actions → General → Workflow permissions*
  is set to "Read and write permissions."
- **404 on the live URL**: confirm `index.html` is in the repo root (not inside a subfolder)
  and that Pages source is set to "GitHub Actions."
- **Résumé download button doesn't work**: `Mohammed_Raheem_CK_Resume.pdf` must sit in the
  same folder as `index.html`.
