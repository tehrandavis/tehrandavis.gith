# GitHub Pages Setup Instructions

This repository has been configured for GitHub Pages deployment. Follow these steps to enable GitHub Pages:

## Automatic Setup (Recommended)

1. Go to your repository on GitHub: `https://github.com/tehrandavis/tehrandavis.gith`
2. Click on **Settings** tab
3. In the left sidebar, click on **Pages**
4. Under **Source**, select **GitHub Actions** (this is required for the workflow to work)
5. Save the settings

Once configured, the site will be automatically deployed when you push to the `main` branch.

## What's Included

### Files Created

- **`index.md`**: Main landing page for your GitHub Pages site
- **`_config.yml`**: Jekyll configuration with site title, description, and theme settings
- **`.github/workflows/pages.yml`**: GitHub Actions workflow for automatic deployment
- **`.gitignore`**: Excludes Jekyll build artifacts from version control

### Jekyll Configuration

The site uses the `minima` theme by default, which is a clean and simple Jekyll theme. You can customize:
- Site title and description in `_config.yml`
- Content in `index.md`
- Theme by changing the `theme` value in `_config.yml`

## Accessing Your Site

After deployment, your site will be available at:
```
https://tehrandavis.github.io/tehrandavis.gith/
```

## Customization

### Adding More Pages

Create additional Markdown files in the repository root (e.g., `about.md`, `contact.md`) with front matter:

```markdown
---
layout: default
title: About
---

# About Page Content
```

### Changing the Theme

Edit `_config.yml` and change the `theme` value to any supported GitHub Pages theme:
- minima (current)
- jekyll-theme-cayman
- jekyll-theme-minimal
- jekyll-theme-architect
- And more...

### Custom Domain

To use a custom domain:
1. Add a `CNAME` file to the repository root with your domain
2. Configure DNS settings with your domain provider
3. Update settings in GitHub Pages settings

## Troubleshooting

If the site doesn't deploy:
1. Check the Actions tab for workflow runs and error messages
2. Ensure GitHub Pages is set to use "GitHub Actions" as the source
3. Verify that the workflow has the necessary permissions in repository settings

## Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Minima Theme](https://github.com/jekyll/minima)
