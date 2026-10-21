# Synthetic Promoter Strength Predictor — deployment package

This package contains the current single-file website prepared for static hosting on Render.

## Files
- `index.html` — website UI and client-side code.
- `render.yaml` — Render Blueprint configuration for a static site.
- `.gitignore` — ignores local secrets and common local files.

## Deploy with GitHub + Render
1. Extract this ZIP.
2. Create a new **private** GitHub repository.
3. Upload the contents of this folder to the repository root (make sure `index.html` is at the root, not inside another nested folder).
4. In Render, choose **New + → Blueprint** and connect the GitHub repository containing `render.yaml`.
5. Review the service and deploy. Render will publish the static site and provide a URL.
6. Open the URL on mobile and desktop and test all navigation and prediction/report features.

## Important limitations
- This is a static deployment of the supplied HTML file; it does not add a backend or database.
- Accounts/history stored in browser `localStorage` are local to that browser/device and are not secure server-side accounts. Do not use real passwords or sensitive lab data with this demo authentication.
- If the website needs shared accounts, password reset, secure authentication, or history synchronized across devices, it needs a backend/database package and a security review before public use.
- The page references Google Fonts and an external iGEM promoter catalog URL, so those external services require internet access.
