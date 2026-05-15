# Deployment Guide - Global Free IPTV

Quick deployment instructions for various platforms.

## 📱 Instant Testing (No Deployment Needed)

Simply open `index.html` in any web browser. That's it! The app works completely offline once loaded.

---

## 🚀 GitHub Pages (Recommended - FREE)

**Time Required**: 5 minutes  
**Cost**: Free  
**URL**: `https://yourusername.github.io/repository-name`

### Step-by-Step:

1. **Create GitHub Account** (if you don't have one)
   - Go to https://github.com
   - Sign up for free

2. **Create New Repository**
   - Click the "+" icon → "New repository"
   - Name: `iptv-app` (or any name you prefer)
   - Make it Public
   - Click "Create repository"

3. **Upload Files**
   
   **Option A: Web Upload (Easiest)**
   - Click "uploading an existing file"
   - Drag and drop all project files
   - Click "Commit changes"

   **Option B: Git Command Line**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/iptv-app.git
   git push -u origin main
   ```

4. **Enable GitHub Pages**
   - Go to repository "Settings"
   - Click "Pages" in left sidebar
   - Under "Source", select "main" branch
   - Click "Save"

5. **Access Your Site**
   - Wait 1-2 minutes for deployment
   - Visit: `https://yourusername.github.io/iptv-app/`

✅ **Done!** Your IPTV app is now live!

---

## 🎯 Netlify (Easiest - Drag & Drop)

**Time Required**: 2 minutes  
**Cost**: Free  
**URL**: `https://random-name.netlify.app` (customizable)

### Step-by-Step:

1. **Visit Netlify Drop**
   - Go to https://app.netlify.com/drop

2. **Drag & Drop**
   - Drag the entire project folder onto the page
   - Wait for upload to complete

3. **Get Your URL**
   - Instant live site!
   - URL like: `https://magical-unicorn-123456.netlify.app`

4. **Optional: Custom Domain**
   - Sign up for free account
   - Go to Site settings → Domain management
   - Add custom domain

✅ **Done!** Fastest deployment ever!

---

## ⚡ Vercel (Fast & Modern)

**Time Required**: 3 minutes  
**Cost**: Free  
**URL**: `https://your-app.vercel.app`

### Step-by-Step:

**Option A: Web Upload**
1. Go to https://vercel.com
2. Click "New Project"
3. Import your GitHub repository (or drag & drop)
4. Click "Deploy"

**Option B: CLI**
```bash
# Install Vercel CLI
npm install -g vercel

# Navigate to project folder
cd path/to/global-free-iptv

# Deploy
vercel

# Follow prompts, then get instant URL
```

✅ **Done!** Lightning-fast deployment!

---

## 🌐 Cloudflare Pages

**Time Required**: 4 minutes  
**Cost**: Free  
**URL**: `https://your-app.pages.dev`

### Step-by-Step:

1. **Go to Cloudflare Pages**
   - Visit https://pages.cloudflare.com
   - Sign in or create account

2. **Create a Project**
   - Click "Create a project"
   - Connect GitHub repository

3. **Configure Build**
   - Build command: (leave empty)
   - Build output directory: `/`
   - Click "Save and Deploy"

4. **Get Your URL**
   - Site available at: `https://your-app.pages.dev`

✅ **Done!** Cloudflare's global CDN powers your app!

---

## 🔧 Render

**Time Required**: 5 minutes  
**Cost**: Free  
**URL**: `https://your-app.onrender.com`

### Step-by-Step:

1. Go to https://render.com
2. Click "New +" → "Static Site"
3. Connect your GitHub repository
4. Configure:
   - Build Command: (leave empty)
   - Publish Directory: `.`
5. Click "Create Static Site"

✅ **Done!** Deployed with automatic SSL!

---

## 💾 Firebase Hosting

**Time Required**: 6 minutes  
**Cost**: Free (generous limits)  
**URL**: `https://your-app.web.app`

### Step-by-Step:

1. **Install Firebase CLI**
   ```bash
   npm install -g firebase-tools
   ```

2. **Login**
   ```bash
   firebase login
   ```

3. **Initialize**
   ```bash
   cd path/to/global-free-iptv
   firebase init hosting
   ```
   - Select "Use an existing project" or create new
   - Public directory: `.` (current directory)
   - Configure as SPA: No
   - Overwrite index.html: No

4. **Deploy**
   ```bash
   firebase deploy
   ```

5. **Get URL**
   - Your app is at: `https://your-project.web.app`

✅ **Done!** Google's infrastructure powers your app!

---

## 🏠 Local Server (For Testing)

### Using Python (Built-in on Mac/Linux):

```bash
# Python 3
python3 -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Visit: `http://localhost:8000`

### Using Node.js:

```bash
# Install http-server globally
npm install -g http-server

# Run
http-server

# Or with specific port
http-server -p 8000
```

Visit: `http://localhost:8000`

### Using PHP:

```bash
php -S localhost:8000
```

Visit: `http://localhost:8000`

---

## 📲 Share on Local Network (Mobile Testing)

1. **Start Local Server** (any method above)

2. **Find Your IP Address**
   - **Windows**: `ipconfig` (look for IPv4)
   - **Mac/Linux**: `ifconfig` or `ip addr`

3. **Access from Mobile**
   - On same WiFi network
   - Visit: `http://YOUR-IP:8000`
   - Example: `http://192.168.1.100:8000`

---

## 🔐 Custom Domain

Once deployed, add a custom domain:

### For GitHub Pages:
1. Go to repository Settings → Pages
2. Enter custom domain (e.g., `iptv.yourdomain.com`)
3. Add CNAME record in your DNS:
   ```
   CNAME: iptv → yourusername.github.io
   ```

### For Netlify/Vercel/Cloudflare:
1. Go to site settings
2. Add custom domain
3. Follow DNS configuration instructions
4. Automatic SSL included!

---

## 🎯 Best Practices

### Performance Optimization:
- ✅ All CDN resources have fallbacks
- ✅ Optimized for mobile/low bandwidth
- ✅ Lazy loading implemented
- ✅ Minimal dependencies

### Security:
- ✅ HTTPS required for HLS streaming
- ✅ All platforms provide free SSL
- ✅ No sensitive data stored
- ✅ No backend required

### Maintenance:
- ✅ Update channel URLs in `index.html`
- ✅ Test streams periodically
- ✅ Monitor for broken links
- ✅ Keep dependencies updated

---

## 🆘 Troubleshooting

### Streams Not Playing After Deployment:

**Problem**: Mixed content (HTTP streams on HTTPS site)  
**Solution**: Use HTTPS deployment platforms (all above support SSL)

**Problem**: CORS errors  
**Solution**: Most free streams allow CORS. If not, use proxy service.

**Problem**: Geo-blocking  
**Solution**: Some streams only work in specific regions. Document this for users.

### GitHub Pages Not Updating:

1. Check deployment status in Actions tab
2. Clear browser cache (Ctrl+F5)
3. Wait 2-3 minutes for propagation
4. Check repository settings

### Mobile Not Loading:

1. Ensure using HTTPS
2. Check mobile data/WiFi
3. Try low bandwidth mode
4. Test on different browser

---

## 📊 Monitoring & Analytics (Optional)

Add free analytics without tracking users:

### Cloudflare Web Analytics (Privacy-First):
```html
<!-- Add before </body> -->
<script defer src='https://static.cloudflareinsights.com/beacon.min.js' 
        data-cf-beacon='{"token": "YOUR_TOKEN"}'></script>
```

### Simple Analytics (Open Source):
```html
<script async defer src="https://scripts.simpleanalyticscdn.com/latest.js"></script>
```

---

## 🎉 Success Checklist

After deployment, verify:

- [ ] Site loads on desktop
- [ ] Site loads on mobile
- [ ] HTTPS enabled (green padlock)
- [ ] Video player initializes
- [ ] At least one channel plays
- [ ] Low bandwidth mode works
- [ ] Categories filter correctly
- [ ] Responsive on different screen sizes
- [ ] No console errors
- [ ] Legal disclaimer visible

---

## 📞 Need Help?

- **GitHub Issues**: Report bugs or ask questions
- **Documentation**: Read README.md thoroughly
- **Community**: Check existing issues for solutions
- **Stack Overflow**: Tag with `iptv`, `video-js`, `hls`

---

**Happy Deploying! 🚀**

*Remember: The app works instantly from `index.html` - deployment is optional but gives you a shareable URL!*
