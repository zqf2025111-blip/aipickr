# AIPickr Website Framework

This is a Jekyll-based website framework for AIPickr, an AI tool comparison and review site optimized for GitHub Pages.

## How to Deploy to GitHub Pages

### Option 1: Using GitHub Web Interface (Easiest)
1. Create a new repository on GitHub named `aipickr`.
2. Upload all files from the `aipickr-site` folder to the root of your repository.
3. Edit `_config.yml`: Replace `[GITHUB_USERNAME]` with your actual GitHub username.
4. Go to **Settings** > **Pages**.
5. Under **Build and deployment** > **Source**, select **GitHub Actions**.
6. GitHub will automatically detect the Jekyll site and deploy it.

### Option 2: Using Command Line (Git)
1. Initialize git and push to your repo:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR_USERNAME/aipickr.git
   git push -u origin main
   ```
2. Follow step 3-6 from Option 1.

## Local Development
If you have Ruby and Jekyll installed locally:
1. Install dependencies: `bundle install`
2. Run the server: `bundle exec jekyll serve`
3. View at: `http://localhost:4000`

## Structure
- `_posts/`: Comparison articles and reviews.
- `_layouts/`: Page and post templates.
- `_includes/`: Reusable components (CTA, Header, Footer).
- `assets/css/`: Main stylesheet.
- `index.md`: Homepage content.
