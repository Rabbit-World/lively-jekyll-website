# Lively Wallpaper - Static Jekyll Template

This is a Jekyll template for the Lively Wallpaper website with multilingual support (English and Italian).

## Features

- Static HTML structure preserved from the original site
- Multilingual support (English and Italian)
- Configured for GitHub Pages deployment
- Preserves all styling, images, and functionality of the original site

## Deployment Instructions

### Local Development

1. Install Ruby and Jekyll (if not already installed):
   ```
   gem install bundler jekyll
   ```

2. Install dependencies:
   ```
   cd lively-jekyll-website
   bundle install
   ```

3. Run the development server:
   ```
   bundle exec jekyll serve
   ```

4. Open your browser and navigate to `http://localhost:4000/lively-jekyll-website/`

### GitHub Pages Deployment

1. Create a new GitHub repository named `lively-jekyll-website`

2. Push this template to the repository:
   ```
   git init
   git add .
   git commit -m "Initial commit"
   git remote add origin https://github.com/YOUR-USERNAME/lively-jekyll-website.git
   git push -u origin main
   ```

3. Configure GitHub Pages:
   - Go to your repository settings
   - Navigate to "Pages"
   - Select "main" branch as the source
   - Save the settings

4. Your site will be published at `https://YOUR-USERNAME.github.io/lively-jekyll-website/`

## Structure

- `_config.yml`: Jekyll configuration
- `_layouts/`: Layout templates
- `_includes/`: Reusable components
- `_data/`: Data files for translations
- `_i18n/`: Language-specific content
- `assets/`: Static assets (CSS, JS, images)
- `index.html`: Main page (English)
- `it.html`: Italian version of the main page

## Multilingual Support

The site supports English and Italian languages. The language switcher is included in the header.

## GitHub Pages Configuration

The site is configured to be deployed on GitHub Pages with the following settings:
- Base URL: `/lively-jekyll-website`
- URL: `https://rabbit-world.github.io`

These settings can be modified in the `_config.yml` file.
