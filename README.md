# Termux Web - Professional Termux Website

A comprehensive, modern website for the Termux project - providing documentation, tutorials, FAQ, and community support for Linux on Android users.

## 🎯 Features

- **Home Page** - Beautiful landing page with features showcase
- **Documentation** - Comprehensive guides covering:
  - Installation & Setup
  - Basic Commands
  - Package Management
  - Development Tools (Python, Node.js, Git)
  - Networking & Web Servers
  - Scripting & Automation
  - Advanced Configuration
  
- **FAQ** - Interactive accordion-style FAQ with 25+ questions covering:
  - Getting Started
  - Installation & Configuration
  - Usage & Development
  - Troubleshooting
  - Advanced Topics
  - Real-time search functionality

- **About** - Project information, history, use cases, and resources

- **Contact** - Contact form and multiple communication channels

## 🚀 Quick Start

### Local Development
1. Clone the repository:
```bash
git clone https://github.com/Kode-Santai/termux-web.git
cd termux-web
```

2. Open with a local server (optional but recommended):
```bash
# Python 3
python -m http.server 8000

# Or Node.js
npx http-server

# Or PHP
php -S localhost:8000
```

3. Open `http://localhost:8000` in your browser

### View the Website
- **Live URL:** https://kode-santai.github.io/termux-web/
- **Main Page:** `index.html`
- **Documentation:** `documentation.html`
- **FAQ:** `faq.html`
- **About:** `about.html`
- **Contact:** `contact.html`

## 📁 File Structure

```
termux-web/
├── index.html                 # Home page
├── documentation.html         # Complete documentation
├── faq.html                  # Interactive FAQ
├── about.html                # About project
├── contact.html              # Contact page
├── README.md                 # This file
└── .github/
    └── workflows/
        └── pages.yml         # GitHub Pages deployment config
```

## 🎨 Design Features

- **Modern Dark Theme** - Professional dark mode with green accents
- **Responsive Design** - Fully responsive on mobile, tablet, and desktop
- **Interactive Elements** - Accordion FAQs, search functionality, smooth animations
- **Accessibility** - Semantic HTML, proper heading hierarchy, good contrast
- **Fast Loading** - Static HTML files with no external dependencies (except fonts)

## 📱 Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🚢 Deployment

### GitHub Pages (Automatic)

The website is automatically deployed to GitHub Pages when you push to the `main` branch. The deployment workflow is configured in `.github/workflows/pages.yml`.

**Steps:**
1. Push changes to GitHub: `git push origin main`
2. GitHub Actions automatically deploys to GitHub Pages
3. Site will be live at: `https://kode-santai.github.io/termux-web/`

### Manual Deployment

To deploy to other hosting services:

1. **Netlify:**
   - Connect your GitHub repository
   - Set build command to: (leave empty)
   - Set publish directory to: `.` (root)

2. **Vercel:**
   - Import from GitHub
   - No build step needed

3. **Self-Hosted:**
   - Copy all HTML files to your web server
   - Ensure proper MIME types are set for `.html` files

## 📝 Content Management

### Adding New Pages

1. Create a new HTML file (e.g., `tutorial.html`)
2. Copy the header and footer from an existing page
3. Update navigation links in all pages to include the new page
4. Add to footer links
5. Commit and push to GitHub

### Updating Navigation

Edit the `<nav>` section in each HTML file:

```html
<ul>
    <li><a href="index.html#features">Features</a></li>
    <li><a href="documentation.html">Documentation</a></li>
    <li><a href="faq.html">FAQ</a></li>
    <li><a href="about.html">About</a></li>
    <li><a href="contact.html">Contact</a></li>
</ul>
```

### Adding FAQ Items

Edit `faq.html` and add new items to the appropriate category:

```html
<div class="faq-item">
    <div class="faq-question" onclick="toggleFAQ(this)">
        <span>Your question here?</span>
        <span class="faq-toggle">▼</span>
    </div>
    <div class="faq-answer">
        <p>Your answer here...</p>
    </div>
</div>
```

## 🎯 Use Cases

This website serves:
- **New Users** - Complete guides to get started with Termux
- **Developers** - Documentation for using dev tools
- **System Admins** - Advanced configuration guides
- **Enthusiasts** - Community resources and links
- **Contributors** - Contact and contribution information

## 🔗 Related Links

- **Official Termux:** https://termux.dev
- **Termux Wiki:** https://wiki.termux.com
- **GitHub Repository:** https://github.com/termux/termux-app
- **Gitter Chat:** https://gitter.im/termux/community
- **Reddit:** https://reddit.com/r/termux

## 📄 License

This website content is provided as-is for the Termux project community. Please refer to the Termux project for licensing information.

## 🤝 Contributing

Want to improve this website? You can:

1. **Report Issues** - Found a bug or have suggestions? Create an issue
2. **Improve Content** - Submit pull requests with documentation improvements
3. **Add Sections** - Suggest new pages or content sections
4. **Fix Bugs** - Help improve the design and functionality

### How to Contribute

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Make your changes
4. Commit: `git commit -m "Add your message"`
5. Push: `git push origin feature/your-feature`
6. Open a Pull Request

## ✨ Features Completed

- ✅ Professional home page
- ✅ Comprehensive documentation (7 sections)
- ✅ Interactive FAQ with search (25+ questions)
- ✅ About page with project info
- ✅ Contact page with form and channels
- ✅ Responsive mobile design
- ✅ GitHub Pages deployment
- ✅ Automated deployment workflow

## 🗓️ Version History

- **v1.0** (2025-12-29) - Initial release
  - Home page
  - Documentation page
  - FAQ page
  - About page
  - Contact page
  - GitHub Pages deployment

## 📧 Contact

For questions about this website, please:

1. Use the **Contact Form** on the website
2. Open an **Issue** on GitHub
3. Join our community on **Gitter** or **Reddit**

---

**Made with ❤️ for the Termux Community**

*This website aims to provide comprehensive resources for Termux users and developers.*
