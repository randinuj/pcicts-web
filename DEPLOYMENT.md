# Deployment Guide

This guide will help you deploy the PCICTS website to various hosting platforms.

## Quick Deployment Options

### 1. GitHub Pages (Recommended)

1. **Create a GitHub Repository**
   - Go to GitHub and create a new repository
   - Name it `pcicts-web` or similar

2. **Upload Your Files**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/your-username/pcicts-web.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository settings
   - Scroll down to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

4. **Your site will be available at**: `https://your-username.github.io/pcicts-web`

### 2. Netlify (Drag & Drop)

1. Go to [netlify.com](https://netlify.com)
2. Sign up/Login
3. Drag and drop your entire project folder to the deployment area
4. Your site will be live instantly with a random URL
5. You can customize the URL in site settings

### 3. Vercel

1. Go to [vercel.com](https://vercel.com)
2. Sign up/Login with GitHub
3. Click "New Project"
4. Import your GitHub repository
5. Deploy with default settings

### 4. Firebase Hosting

1. **Install Firebase CLI**
   ```bash
   npm install -g firebase-tools
   ```

2. **Login to Firebase**
   ```bash
   firebase login
   ```

3. **Initialize Firebase**
   ```bash
   firebase init hosting
   ```

4. **Deploy**
   ```bash
   firebase deploy
   ```

## Custom Domain Setup

### For GitHub Pages:
1. Go to repository settings → Pages
2. Add your custom domain in the "Custom domain" field
3. Create a CNAME record pointing to `your-username.github.io`

### For Netlify:
1. Go to site settings → Domain management
2. Add custom domain
3. Update your DNS records as instructed

### For Vercel:
1. Go to project settings → Domains
2. Add your custom domain
3. Update DNS records as instructed

## Performance Optimization

### Before Deployment:
1. **Optimize Images**
   - Use tools like TinyPNG or ImageOptim
   - Convert to WebP format if possible
   - Ensure images are appropriately sized

2. **Minify CSS and JavaScript**
   - Use online minifiers or build tools
   - Remove unused CSS

3. **Enable Compression**
   - Most hosting platforms enable this automatically
   - For custom servers, enable gzip compression

### After Deployment:
1. **Test Performance**
   - Use Google PageSpeed Insights
   - Check mobile responsiveness
   - Test loading speed

2. **Set Up Analytics**
   - Google Analytics
   - Search Console for SEO

## SSL Certificate

Most modern hosting platforms provide free SSL certificates:
- **GitHub Pages**: Automatic HTTPS
- **Netlify**: Automatic HTTPS
- **Vercel**: Automatic HTTPS
- **Firebase**: Automatic HTTPS

## Troubleshooting

### Common Issues:

1. **Images Not Loading**
   - Check file paths are correct
   - Ensure images are in the `assets/images/` folder
   - Verify file names match exactly

2. **CSS Not Loading**
   - Check CSS file paths
   - Ensure files are in `assets/css/` folder
   - Clear browser cache

3. **Fonts Not Loading**
   - Verify font files are in `assets/fonts/` folder
   - Check font-face declarations in CSS

4. **Mobile Menu Not Working**
   - Check JavaScript console for errors
   - Ensure all script tags are properly closed

### Support:
- Check browser console for errors
- Validate HTML at [validator.w3.org](https://validator.w3.org)
- Test on multiple browsers and devices

## Maintenance

### Regular Tasks:
1. **Update Content**: Keep team information current
2. **Check Links**: Ensure all external links work
3. **Monitor Performance**: Regular performance checks
4. **Backup**: Keep local backups of your files

### Updates:
1. **Content Updates**: Edit HTML files directly
2. **Style Changes**: Modify CSS files
3. **New Features**: Add JavaScript as needed

---

**Note**: Always test your website locally before deploying changes to production. 