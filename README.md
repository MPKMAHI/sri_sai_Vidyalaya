# Sri Sai Vidyalaya High School (SSVHS) — Official Web Ecosystem & SSV SchoolSphere

> **Official Website:** [https://srisaividyalaya.in/](https://srisaividyalaya.in/)  
> **School Management Portal / Mobile App:** [https://srisaividyalaya.in/app/](https://srisaividyalaya.in/app/)  
> **Location:** Noonevari Palli Road, Rajampet, Andhra Pradesh 516115, India  
> **Tagline:** *Every Student. Every Update. One Connected School.*

---

## 📁 Repository Structure

```
.
├── CNAME                    # Custom domain mapping (srisaividyalaya.in)
├── index.html               # Main public school portal & website
├── style.css                # Official website styles & animations
├── script.js                # Official website scripts & interactions
├── 404.html                 # Zero-mistake SPA routing fallback for GitHub Pages
├── _redirects               # Host redirect rules (Cloudflare / Netlify)
├── vercel.json              # Host rewrite rules (Vercel)
├── sitemap.xml              # SEO search engine sitemap
├── images/                  # School photographs, campus gallery, and official logos
│   ├── logo.jpeg            # High-resolution official school crest
│   ├── mahidhar.jpg         # Mahidhar profile photo
│   └── ...
│
├── app/                     # 🚀 DEPLOYED PRODUCTION APPLICATION (srisaividyalaya.in/app/)
│   ├── index.html           # Application entrypoint
│   ├── manifest.json        # Mobile PWA manifest (Install to Home Screen)
│   ├── mahidhar.jpg         # Profile image
│   ├── images/logo.jpeg     # App icon
│   └── assets/              # Optimized CSS & JS bundles
│       ├── index-CKsb86Pw.js
│       └── index-GLhz6DYr.css
│
├── screenshare/             # P2P screen sharing & remote pointer utility
│   └── index.html
│
└── school-app-source/       # 💻 DEVELOPER SOURCE CODE (React + TypeScript + Tailwind)
    ├── package.json
    ├── vite.config.ts
    ├── tailwind.config.js
    ├── tsconfig.json
    ├── src/
    ├── public/
    └── tests/
```

---

## 🚀 How to Publish to GitHub

Open a terminal inside this folder:

```bash
# 1. Initialize git if not already initialized
git init

# 2. Add your GitHub repository remote (if not already linked)
git remote add origin https://github.com/<YOUR_USERNAME>/<YOUR_REPOSITORY>.git

# 3. Stage all files
git add .

# 4. Commit changes
git commit -m "Deploy Sri Sai Vidyalaya High School website and SSV SchoolSphere app"

# 5. Push to GitHub
git branch -M main
git push -u origin main
```

---

## 🌐 GitHub Pages Configuration

1. In your GitHub repository, navigate to **Settings** > **Pages**.
2. Under **Build and deployment**:
   - **Source:** Deploy from a branch
   - **Branch:** `main` / `root`
3. Under **Custom domain**:
   - Domain is already declared as `srisaividyalaya.in` via the `CNAME` file.
   - Check **Enforce HTTPS**.

Once deployed:
- **`https://srisaividyalaya.in/`** serves the school website.
- **`https://srisaividyalaya.in/app`** (or `/app/`) serves the SSV SchoolSphere mobile and desktop app.
- Mobile users in Chrome or Safari can tap **"Add to Home Screen"** to install it as a native full-screen app.

---

## 🛠️ Modifying the Application

To make changes to the app code:
1. Navigate into `school-app-source/`:
   ```bash
   cd school-app-source
   npm install
   npm run dev
   ```
2. Build and update the production `../app/` folder:
   ```bash
   npm run build:deploy
   ```

