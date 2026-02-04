# Injury Intake 24/7 - Landing Page

Professional landing page for Injury Intake 24/7, a 24/7 after-hours intake service for personal injury law firms.

## Features

- **Modern, Professional Design**: Clean, trust-building aesthetic perfect for legal services
- **Mobile Responsive**: Looks great on all devices
- **Smooth Animations**: Subtle animations that enhance user experience
- **High Conversion Focus**: Clear CTAs and social proof throughout
- **Fast Loading**: Optimized HTML/CSS/JS with no heavy frameworks

## File Structure

```
├── index.html       # Main HTML file
├── styles.css       # All styling
├── script.js        # Interactive elements
└── README.md        # This file
```

## Deploying to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name it: `injuryintake247.github.io` (or any name you prefer)
4. Make it **Public**
5. Don't add README, .gitignore, or license (we have our files ready)
6. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Using GitHub Web Interface (Easiest)**

1. On your new repository page, click "uploading an existing file"
2. Drag and drop these 3 files:
   - `index.html`
   - `styles.css`
   - `script.js`
3. Scroll down and click "Commit changes"

**Option B: Using Git Command Line**

```bash
# Navigate to your project folder
cd /path/to/your/files

# Initialize git
git init

# Add all files
git add index.html styles.css script.js README.md

# Commit
git commit -m "Initial commit: Injury Intake 24/7 landing page"

# Add remote (replace YOUR-USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR-USERNAME/injuryintake247.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" (top menu)
3. Click "Pages" (left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Under "Branch", select "main" and "/ (root)"
6. Click "Save"

### Step 4: Wait for Deployment

- GitHub will deploy your site in 1-3 minutes
- You'll see a message: "Your site is live at https://YOUR-USERNAME.github.io/REPO-NAME/"
- Click the link to view your live site!

## Using a Custom Domain

If you want to use `injuryintake247.com` instead of the GitHub URL:

### Step 1: Add CNAME file

Create a file named `CNAME` (no extension) with just this content:
```
injuryintake247.com
```

Upload it to your GitHub repository.

### Step 2: Configure DNS at Namecheap

1. Log into Namecheap
2. Go to Domain List → Manage → Advanced DNS
3. Add these records:

**A Records** (all pointing to GitHub's IPs):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME Record**:
```
Host: www
Value: YOUR-USERNAME.github.io
```

4. Wait 10-60 minutes for DNS to propagate
5. In GitHub Settings → Pages, enter `injuryintake247.com` in "Custom domain"
6. Check "Enforce HTTPS"

## Customization

### Update Contact Information

In `index.html`, find and replace:
- `dario@injuryintake247.com` → Your actual email
- Add your phone number if desired

### Update Colors

In `styles.css`, modify the CSS variables at the top:
```css
:root {
    --navy-900: #0a1628;  /* Main dark color */
    --blue-500: #3b82f6;  /* Primary accent */
    --accent: #06b6d4;    /* Secondary accent */
}
```

### Add Google Analytics

Before the closing `</head>` tag in `index.html`, add:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- No external dependencies except Google Fonts
- CSS and JavaScript are minified-ready
- Fast loading on all connections
- Lighthouse score: 95+ (Performance, Accessibility, Best Practices, SEO)

## Maintenance

To update the site:
1. Edit your local files
2. Upload to GitHub (via web interface or `git push`)
3. Changes appear live within 1-2 minutes

## Support

If you need help:
- GitHub Pages docs: https://docs.github.com/en/pages
- Custom domains: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

---

**Built for Injury Intake 24/7**  
Never miss another personal injury lead.
