# Portfolio Website - Chekoti Praneeth Sai

A modern, responsive portfolio website featuring a dark theme, interactive animations, and smooth user experience. Built with pure HTML, CSS, and JavaScript.

![Portfolio Preview](https://img.shields.io/badge/Status-Live-brightgreen) ![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🌟 Features

- **Modern Dark Theme** - Sleek black design with elegant white accents
- **Fully Responsive** - Optimized for desktop, tablet, and mobile devices
- **Interactive Animations** - Canvas-based particle effects and smooth transitions
- **Loading Screen** - Animated loading screen with progress indicator
- **Smooth Scrolling** - Seamless navigation between sections
- **Contact Form** - Integrated EmailJS for direct email communication
- **Progress Indicator** - Real-time scroll progress tracking
- **Interactive Elements** - Cursor-following eyes, click explosions, and hover effects
- **Mobile Menu** - Hamburger menu for mobile navigation
- **PWA Ready** - Web manifest included for Progressive Web App support

## 🛠️ Technologies & Tools

### Core Technologies
- **HTML5** - Semantic markup and structure
- **CSS3** - Advanced styling with animations and responsive design
- **JavaScript (ES6+)** - Vanilla JavaScript for interactivity
- **Canvas API** - Particle animations and visual effects

### External Services
- **EmailJS** - Contact form email service
- **Google Fonts** - Inter font family

### Development Tools
- **Git** - Version control
- **Netlify** - Hosting and deployment

## 📁 Project Structure

```
portfolio latest/
├── index.html              # Main HTML file
├── education.html          # Education page (standalone)
├── styles.css              # All CSS styles and animations
├── MOBILE_FIXES.css        # Mobile-specific CSS fixes
├── site.webmanifest        # PWA manifest file
├── logo.jpeg              # SSEV SOFTSOLS logo
├── profilepic.jpeg        # Profile photo
├── pslogo.jpeg            # PS logo (favicon)
├── video/
│   └── footer.mp4         # Skills section background video
├── README.md              # This file
├── DEPLOY_STEPS.md        # Deployment instructions
├── NETLIFY_DEPLOYMENT.md  # Netlify deployment guide
└── DEPLOYMENT_GUIDE.md    # General deployment guide
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A code editor (VS Code, Sublime Text, etc.)
- Git (optional, for version control)
- Netlify account (for deployment)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/portfolio.git
   cd portfolio
   ```

2. **Open the project**
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     ```

3. **Configure EmailJS** (for contact form)
   - Sign up at [EmailJS](https://www.emailjs.com/)
   - Get your Public Key and Service ID
   - Update the EmailJS configuration in `index.html`:
     ```javascript
     emailjs.init("YOUR_PUBLIC_KEY");
     emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', formData)
     ```

## 📱 Sections

1. **Home** - Introduction with animated particles
2. **About Me** - Professional background and experience
3. **Education** - Academic qualifications and timeline
4. **Skills** - Technical skills and expertise
5. **Certifications** - Professional certifications
6. **Projects** - Portfolio of projects with descriptions
7. **Contact** - Contact form and information

## 🎨 Customization

### Changing Colors
Edit the color scheme in `styles.css`:
```css
body {
    background-color: #000000; /* Main background */
    color: #ffffff;             /* Text color */
}
```

### Adding Projects
Add new project cards in the Projects section of `index.html`:
```html
<a class="project-card" href="#" target="_blank" rel="noopener" data-project>
    <div class="project-card-inner">
        <div class="project-accent"></div>
        <h3 class="project-title">Your Project</h3>
        <p class="project-desc">Project description</p>
        <div class="project-tags">
            <span class="tag">Technology</span>
        </div>
    </div>
</a>
```

### Updating Personal Information
- Edit personal details in `index.html`
- Update profile picture: Replace `profilepic.jpeg`
- Modify social links in the Home section

## 🚢 Deployment

### Deploy to Netlify (Recommended)

#### Method 1: Drag & Drop
1. Go to [Netlify](https://app.netlify.com)
2. Drag and drop your project folder
3. Wait for deployment (1-2 minutes)
4. Your site is live!

#### Method 2: Git Integration
1. Push your code to GitHub
2. In Netlify, click "Add new site" → "Import an existing project"
3. Connect to GitHub and select your repository
4. Deploy automatically on every push

### Custom Domain
1. In Netlify Dashboard → Domain settings
2. Click "Add custom domain"
3. Follow DNS configuration instructions
4. Free SSL certificate provided automatically

For detailed deployment instructions, see [NETLIFY_DEPLOYMENT.md](./NETLIFY_DEPLOYMENT.md)

## 📊 Performance

- **Lightweight** - No heavy frameworks or libraries
- **Fast Loading** - Optimized assets and minimal dependencies
- **Mobile Optimized** - Responsive design with touch-friendly interactions
- **SEO Friendly** - Semantic HTML structure

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Chekoti Praneeth Sai**

- LinkedIn: [praneethsai4596](https://www.linkedin.com/in/praneethsai4596/)
- GitHub: [gitpr4596](https://github.com/gitpr4596)
- Email: praneethsai4596@gmail.com

## 🙏 Acknowledgments

- [EmailJS](https://www.emailjs.com/) for contact form service
- [Google Fonts](https://fonts.google.com/) for Inter font family
- [Netlify](https://www.netlify.com/) for hosting platform

## 📈 Future Enhancements

- [ ] Add blog section
- [ ] Implement dark/light theme toggle
- [ ] Add more interactive animations
- [ ] Integrate analytics
- [ ] Add project filtering
- [ ] Implement lazy loading for images

---

⭐ If you find this project helpful, please consider giving it a star!
