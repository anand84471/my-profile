# Portfolio Deployment Instructions

Follow these steps to deploy your portfolio to GitHub Pages:

## 1. GitHub Repository Setup

### Option A: User Site (yourusername.github.io)
1. Create a new repository named exactly: `yourusername.github.io` (replace with your GitHub username)
2. This will be your main GitHub Pages site

### Option B: Project Site
1. Create a new repository with any name (e.g., `portfolio`, `my-profile`)
2. This will be accessible at `yourusername.github.io/repository-name`

## 2. Upload Your Files

### Method 1: Using Git (Recommended)
```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio commit"

# Add remote origin (replace with your repository URL)
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git push -u origin main
```

### Method 2: Using GitHub Web Interface
1. Go to your repository on GitHub
2. Click "uploading an existing file"
3. Drag and drop all files (index.html, styles.css, script.js, README.md)
4. Commit the files

## 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on the "Settings" tab
3. Scroll down to the "Pages" section in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

## 4. Access Your Website

- **User Site**: `https://yourusername.github.io`
- **Project Site**: `https://yourusername.github.io/repository-name`

Note: It may take a few minutes for your site to be available after enabling GitHub Pages.

## 5. Customization Checklist

Before going live, make sure to update:

### Personal Information
- [ ] Your name in the hero section
- [ ] Contact email address
- [ ] LinkedIn profile URL
- [ ] GitHub profile URL
- [ ] Professional summary
- [ ] Work experience details
- [ ] Skills and technologies
- [ ] Achievements and awards

### Content Updates
- [ ] Replace placeholder email in contact form
- [ ] Update social media links
- [ ] Add your profile photo (optional)
- [ ] Customize color scheme if desired
- [ ] Update meta tags for SEO

## 6. Custom Domain (Optional)

If you want to use a custom domain:

1. Purchase a domain from a domain registrar
2. In your repository, create a file named `CNAME` (no extension)
3. Add your domain to the CNAME file: `yourdomain.com`
4. Configure DNS settings with your domain registrar:
   - Add a CNAME record pointing to `yourusername.github.io`
   - Or add A records pointing to GitHub's IP addresses

## 7. SEO Optimization

Add these meta tags to your `<head>` section in index.html:

```html
<meta name="description" content="Anand - AI Engineer & Backend Developer with 5+ years experience building scalable products">
<meta name="keywords" content="AI Engineer, Backend Developer, Machine Learning, Python, Java, AWS">
<meta name="author" content="Your Name">
<meta property="og:title" content="Anand's Portfolio - AI Engineer & Backend Developer">
<meta property="og:description" content="Professional portfolio showcasing AI/ML and backend engineering expertise">
<meta property="og:url" content="https://yourusername.github.io">
<meta property="og:type" content="website">
```

## 8. Analytics (Optional)

To track visitors, you can add Google Analytics:

1. Create a Google Analytics account
2. Get your tracking ID
3. Add the tracking script to your HTML head section

## 9. Performance Tips

- Optimize images if you add any
- Minify CSS and JavaScript for production
- Use a CDN for external libraries
- Test on multiple devices and browsers

## 10. Maintenance

- Regular updates to work experience and skills
- Keep dependencies up to date
- Monitor site performance
- Backup your code regularly

## Troubleshooting

### Common Issues:

**Site not loading:**
- Check if GitHub Pages is enabled in repository settings
- Ensure `index.html` is in the root directory
- Wait a few minutes for changes to propagate

**Styles not loading:**
- Check file paths in HTML
- Ensure CSS file is committed to repository
- Clear browser cache

**Contact form not working:**
- The current form uses mailto: links
- Consider integrating with EmailJS or Formspree for backend functionality

## Support

If you encounter issues:
1. Check GitHub Pages documentation
2. Review repository settings
3. Verify all files are properly committed
4. Test locally before deploying

Your portfolio should now be live and accessible to the world! 🚀