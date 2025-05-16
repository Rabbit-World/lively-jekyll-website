# GitHub Pages Deployment Verification

This document helps verify that your Jekyll site is properly configured for GitHub Pages deployment.

## Required Files and Directories

The following files and directories are essential for proper GitHub Pages deployment:

- ✅ `_config.yml`: Contains site configuration and GitHub Pages settings
- ✅ `Gemfile`: Includes the github-pages gem and other dependencies
- ✅ `.nojekyll`: (Optional) Tells GitHub Pages to not run Jekyll processing
- ✅ `_layouts/default.html`: Main layout template
- ✅ `_includes/`: Directory for reusable components
- ✅ `_data/`: Directory for site data (translations, etc.)
- ✅ `assets/`: Directory for static assets
- ✅ `index.html`: Main page
- ✅ `404.html`: Custom 404 error page
- ✅ `robots.txt`: Instructions for search engine crawlers
- ✅ `sitemap.xml`: Site map for search engines

## GitHub Pages Configuration

1. Repository should be named: `lively-jekyll-website`
2. GitHub Pages should be enabled from the main branch
3. The site will be available at: `https://rabbit-world.github.io/lively-jekyll-website/`

## Local Testing

Run the following commands to test locally:

```bash
cd lively-jekyll-static
bundle install
bundle exec jekyll serve
```

Then open your browser to: http://localhost:4000/lively-jekyll-website/

## Common Issues and Solutions

### Site Not Building

If your site is not building on GitHub Pages:

1. Check the build logs in the GitHub repository settings
2. Ensure the `github-pages` gem is in your Gemfile
3. Verify that your _config.yml has the correct baseurl and url settings

### CSS/JS Not Loading

If your CSS or JavaScript files are not loading:

1. Check that paths use `{{ site.baseurl }}` prefix
2. Verify that assets are not excluded in _config.yml

### Multilingual Support Issues

If language switching is not working:

1. Verify that language files are in the correct location
2. Check that the language switcher is properly implemented in the header
3. Ensure that _config.yml has the correct language settings