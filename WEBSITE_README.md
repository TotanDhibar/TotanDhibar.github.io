# SD Build - Industrial Contractor Website

A clean, modern, and responsive website for SD Build, an industrial contractor specializing in boiler maintenance, AMC, mill overhauling, and comprehensive industrial solutions.

## 🌟 Features

- **Fully Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern Industrial Theme**: Professional blue and steel color scheme
- **No Backend Required**: Pure HTML, CSS, and JavaScript - works completely offline
- **Easy to Edit**: All content clearly marked with `<!-- EDIT -->` comments
- **Smooth Animations**: Fade-in effects and smooth scrolling
- **Mobile Menu**: Hamburger menu for mobile devices
- **Contact Form**: Client-side form validation (can be connected to a backend later)
- **SEO Friendly**: Proper meta tags and semantic HTML

## 📁 File Structure

```
root/
├── index.html          # Home page
├── about.html          # About the company
├── services.html       # Full service list
├── projects.html       # Project gallery and clients
├── certificates.html   # Certificates and downloads
├── contact.html        # Contact form and information
├── style.css           # All styling (responsive)
├── script.js           # JavaScript functionality
└── assets/             # Images and resources
    ├── hero-bg.svg     # Hero background image
    └── placeholder-info.txt
```

## 🎨 Pages Overview

### 1. **index.html** - Home Page
- Hero section with call-to-action
- About summary
- Services preview (6 cards)
- Client list
- Call-to-action section

### 2. **about.html** - About Us
- Company overview
- Mission, vision, and values
- Partnership details
- Infrastructure information
- Company information block
- Why choose us section

### 3. **services.html** - Services
- 8 detailed service cards:
  - Boiler Maintenance
  - Annual Maintenance Contract (AMC)
  - Mill Overhauling
  - AHP (Air Heater Preheater)
  - ESP (Electrostatic Precipitator)
  - APH (Air Preheater)
  - Hoist Services
  - Manpower Supply
- Additional specialized services
- Service benefits

### 4. **projects.html** - Projects
- Project gallery (9 placeholder items)
- Major clients showcase (12 clients)
- Project statistics
- Featured project highlights

### 5. **certificates.html** - Certificates
- Certificate download list (8 certificates)
- Compliance information
- Professional memberships
- Certification features

### 6. **contact.html** - Contact
- Contact information cards
- Contact form with validation
- Location section
- Business hours
- Regional offices
- FAQ section

## ✏️ How to Edit Content

### Easy Editing Guide

All important content is marked with clear comments like this:
```html
<!-- EDIT COMPANY NAME HERE -->
<h1>SD Build</h1>
<!-- END EDIT COMPANY NAME -->
```

### What You Can Edit:

1. **Company Information**
   - Company name: Look for `<!-- EDIT COMPANY NAME -->`
   - Tagline: Look for `<!-- EDIT COMPANY NAME AND TAGLINE -->`
   - Address: Look for `<!-- EDIT CONTACT ADDRESS -->`
   - Phone numbers: Look for `<!-- EDIT CONTACT PHONE -->`
   - Email addresses: Look for `<!-- EDIT CONTACT EMAIL -->`

2. **Services**
   - Each service is in its own card with `<!-- EDIT SERVICE X -->`
   - Add new services by copying the card template
   - Modify service descriptions, lists, and details

3. **Client List**
   - Found in `index.html` and `projects.html`
   - Look for `<!-- EDIT CLIENT LIST -->`
   - Add/remove clients as needed

4. **Certificates**
   - Each certificate has `<!-- EDIT CERTIFICATE X -->`
   - Update PDF links: `<!-- EDIT: Add PDF link here -->`
   - Add new certificates by copying the template

5. **About Content**
   - Company overview: `<!-- EDIT COMPANY OVERVIEW -->`
   - Mission/Vision: `<!-- EDIT MISSION CARD -->`
   - Infrastructure: `<!-- EDIT INFRASTRUCTURE DETAILS -->`

6. **Colors** (in style.css)
   - Look for `:root` section at the top of `style.css`
   - Change `--primary-blue`, `--secondary-blue`, `--steel-gray`, etc.

## 🎨 Color Scheme

The website uses a professional industrial color scheme:

```css
--primary-blue: #1e3a8a;      /* Dark blue for headers */
--secondary-blue: #3b82f6;    /* Bright blue for accents */
--steel-gray: #64748b;        /* Steel gray for text */
--light-gray: #f1f5f9;        /* Light background */
--white: #ffffff;             /* White backgrounds */
--dark-text: #1e293b;         /* Dark text color */
```

To change colors, edit the `:root` section in `style.css`.

## 📱 Responsive Design

The website is fully responsive:
- **Desktop**: Full layout with horizontal navigation
- **Tablet**: Adjusted card grids and spacing
- **Mobile**: Hamburger menu, single column layout

## 🖼️ Adding Images

### Hero Background
Replace `assets/hero-bg.svg` with your own image (recommended: 1920x1080 px)

### Project Photos
1. Add images to the `assets/` folder
2. Replace the placeholder divs in `projects.html`:
```html
<!-- Replace this: -->
<div class="gallery-placeholder">...</div>

<!-- With this: -->
<img src="assets/project-1.jpg" alt="Project description">
```

### Client Logos
Add client logos to the `assets/` folder and update the client grid in `projects.html`.

## 📄 Adding PDF Certificates

1. Place PDF files in the `assets/` folder (or use `/mnt/data/` path)
2. Update the download links in `certificates.html`:
```html
<a href="assets/your-certificate.pdf" class="download-btn" download>📥 Download</a>
```

## 🔧 Technical Details

### Browser Support
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

### No External Dependencies
- No jQuery
- No Bootstrap
- No CDN links
- Works completely offline

### JavaScript Features
- Mobile menu toggle
- Smooth scrolling
- Fade-in animations on scroll
- Contact form validation
- Back-to-top button
- Active navigation highlighting

## 🚀 Deployment

### GitHub Pages
1. The site is ready to deploy to GitHub Pages
2. Push to the `main` branch
3. Enable GitHub Pages in repository settings
4. Your site will be live at `https://yourusername.github.io`

### Other Hosting
Simply upload all files to your web server. The site works with any static hosting:
- Netlify
- Vercel
- AWS S3
- Traditional web hosting

## 📝 Customization Tips

### Adding a New Page
1. Copy an existing HTML file
2. Update the `<title>` and meta tags
3. Keep the header and footer sections
4. Add your content in between
5. Update navigation links in all files

### Adding a New Service
1. Go to `services.html`
2. Find the `<!-- EDIT: ADD MORE SERVICES HERE -->` section
3. Copy a service card template
4. Paste and edit the content

### Changing Fonts
Edit the `font-family` in `style.css`:
```css
body {
    font-family: 'Your Font', 'Segoe UI', sans-serif;
}
```

## 📞 Contact Form

The contact form currently:
- Validates input client-side
- Shows a success message
- Stores submissions in browser's localStorage (for demo)

To connect to a backend:
1. Edit the form submission handler in `script.js`
2. Replace the localStorage code with your API call
3. Or use a service like Formspree, EmailJS, or Netlify Forms

## 🔒 Security Notes

- No sensitive data is stored
- Client-side form validation only
- All external links open in new tabs
- No cookies or tracking

## 📱 Testing

To test the website locally:
```bash
# Using Python
python3 -m http.server 8080

# Using Node.js
npx http-server -p 8080

# Then visit: http://localhost:8080
```

## 🎯 Next Steps

1. **Replace Placeholder Content**
   - Update company name and contact details
   - Add real client names
   - Add actual project photos

2. **Add Real Certificates**
   - Upload PDF certificates to `assets/`
   - Update links in `certificates.html`

3. **Customize Colors**
   - Adjust color scheme in `style.css`
   - Match your brand colors

4. **Connect Contact Form**
   - Set up backend or use form service
   - Update form handler in `script.js`

5. **SEO Optimization**
   - Update meta descriptions for each page
   - Add social media meta tags
   - Create sitemap.xml

## 📄 License

This website template is created for SD Build. Feel free to modify and use as needed.

## 🆘 Support

For questions or modifications needed, look for the `<!-- EDIT -->` comments throughout the HTML files. Everything is clearly marked for easy editing without touching the layout code.

---

**Built with ❤️ for SD Build - Industrial Excellence Since 2010**
