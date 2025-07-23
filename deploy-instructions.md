# Manual Deployment Instructions

This guide will help you deploy your TikTok landing page manually to various hosting platforms.

## 🚀 Quick Deploy Options

### Option 1: Netlify (Recommended)
1. **Build the project locally:**
   ```bash
   npm install
   npm run build
   ```

2. **Deploy via drag-and-drop:**
   - Go to [netlify.com](https://netlify.com)
   - Drag the `dist` folder to the deployment area
   - Your site will be live instantly!

3. **Deploy via Netlify CLI:**
   ```bash
   npm install -g netlify-cli
   netlify login
   netlify deploy --prod --dir=dist
   ```

### Option 2: Vercel
1. **Build the project:**
   ```bash
   npm install
   npm run build
   ```

2. **Deploy via Vercel CLI:**
   ```bash
   npm install -g vercel
   vercel --prod
   ```

3. **Or drag-and-drop:**
   - Go to [vercel.com](https://vercel.com)
   - Import your GitHub repository or drag the `dist` folder

### Option 3: GitHub Pages
1. **Build the project:**
   ```bash
   npm install
   npm run build
   ```

2. **Create gh-pages branch:**
   ```bash
   git checkout --orphan gh-pages
   git rm -rf .
   cp -r dist/* .
   git add .
   git commit -m "Deploy to GitHub Pages"
   git push origin gh-pages
   ```

3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Select `gh-pages` branch as source

### Option 4: Other Static Hosts

The built files in the `dist` folder can be deployed to any static hosting service:

- **Firebase Hosting**
- **AWS S3 + CloudFront**
- **DigitalOcean App Platform**
- **Surge.sh**
- **Render**

## 📋 Pre-Deployment Checklist

Before deploying, ensure:

- [ ] All referral links point to: `https://tiktok.pxf.io/fkv5`
- [ ] Site builds without errors: `npm run build`
- [ ] Linting passes: `npm run lint`
- [ ] All images load correctly
- [ ] Mobile responsiveness works
- [ ] All buttons link to the referral URL

## 🔧 Build Commands

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Run linter
npm run lint
```

## 📁 Deployment Files

After running `npm run build`, deploy these files from the `dist` folder:

```
dist/
├── index.html          # Main HTML file
├── assets/
│   ├── index-[hash].js # JavaScript bundle
│   └── index-[hash].css # CSS bundle
└── vite.svg           # Favicon
```

## 🌐 Domain Configuration

### Custom Domain Setup:
1. **Netlify**: Add custom domain in site settings
2. **Vercel**: Add domain in project settings
3. **GitHub Pages**: Add CNAME file with your domain

### DNS Configuration:
- **A Record**: Point to hosting provider's IP
- **CNAME**: Point to hosting provider's domain
- **SSL**: Most providers offer free SSL certificates

## 📊 Analytics & Monitoring

Consider adding:
- **Google Analytics** for traffic monitoring
- **Hotjar** for user behavior analysis
- **Google Search Console** for SEO monitoring

## 🔒 Security Headers

The `netlify.toml` file includes security headers:
- X-Frame-Options
- X-XSS-Protection
- X-Content-Type-Options
- Referrer-Policy

For other hosts, configure these headers in your hosting platform.

## 🚨 Troubleshooting

### Common Issues:

1. **404 on refresh**: Configure your host to serve `index.html` for all routes
2. **Assets not loading**: Check if base URL is configured correctly
3. **Build fails**: Ensure Node.js version 18+ is used

### Support:
- Check the GitHub Issues for common problems
- Review hosting provider documentation
- Test locally with `npm run preview` before deploying

## 📈 Performance Optimization

The build is already optimized with:
- ✅ Code splitting
- ✅ Asset compression
- ✅ Tree shaking
- ✅ Minification
- ✅ Image optimization

Your site should achieve 95+ Lighthouse scores! 🎉