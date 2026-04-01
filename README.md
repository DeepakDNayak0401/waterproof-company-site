# ShieldRoof Waterproofing Website

A high-performance, accessible, and responsive single-page website designed for a professional waterproofing company. Built with HTML5, Tailwind CSS, and Vanilla JavaScript.

## 🌟 Features

- **🎨 Modern UI/UX:** Bold design with high-contrast colors (Safety Orange & Deep Blue) for a professional industrial look.
- **🌙 Dark/Light Mode:** Fully functional theme toggle that respects user system preferences and saves choices locally.
- **♿ Accessibility (A11y) Compliant:** 
  - WCAG 2.1 AA standards.
  - Skip-to-content links.
  - High visibility focus states for keyboard navigation.
  - Reduced motion support for vestibular disorders.
  - Semantic HTML5 structure.
- **🌍 Global Compliance:** 
  - GDPR/CCPA Cookie Consent Banner.
  - Legal placeholder links (Privacy Policy, Terms).
- **📱 Fully Responsive:** Optimized for Mobile, Tablet, and Desktop views.
- **⚡ Performance:** No heavy frameworks. Uses Tailwind CSS via CDN for easy deployment (can be optimized for production).
- **🆘 Emergency Contact:** Floating Action Button (FAB) for immediate calling on mobile devices.

## 📂 Folder Structure

```text
waterproofing-site/
│
├── index.html                # Main HTML structure
├── README.md                 # Project documentation
│
├── css/
│   └── style.css             # Custom CSS & Accessibility overrides
│
├── js/
│   └── script.js             # Dark mode, Menu, and Cookie logic
│
└── assets/
    └── images/
        ├── hero-bg.jpg       # Main banner image
        ├── project1.jpg      # Portfolio images
        ├── project2.jpg
        └── project3.jpg

## 🚀 Getting Started

### Prerequisites

- Any modern web browser (Chrome, Firefox, Safari, Edge).
- A code editor (VS Code, Sublime Text, etc.) for customization.

### Installation & Running

Since this is a static website, no build process is required to run it locally.

1. **Clone or Download** the project folder.
2. **Open** `index.html` in your web browser.
   - _Recommended:_ Use a local server (like VS Code "Live Server" extension) to avoid CORS issues with local assets, though direct file opening works for this setup.

## 🛠 Customization

### 1. Changing Colors

The color scheme is configured within the `<script>` tag in `index.html` (Tailwind Config).

```html
<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          brand: {
            500: "#0ea5e9", // Change Primary Blue here
          },
          accent: {
            500: "#f97316", // Change Safety Orange here
          },
        },
      },
    },
  };
</script>
```

### 2. Updating Images

1. Place your images in the `assets/images/` folder.
2. Open `index.html`.
3. Search for `<img>` tags and update the `src` attribute.
   ```html
   <!-- Example -->
   <img src="assets/images/hero-bg.jpg" alt="Description" />
   ```

### 3. Contact Information

Update the phone numbers and email addresses in the **Contact Section** and the **Emergency FAB** (bottom right) in `index.html`.

```html
<!-- Example -->
<a href="tel:+1234567890">...</a>
<a href="mailto:info@shieldroof.com">...</a>
```

### 4. Cookie Consent

The cookie banner logic is in `js/script.js`. To change the text, edit the HTML inside the `#cookie-banner` div in `index.html`.

## 🌐 Deployment

This site can be hosted on any static hosting provider.

1. **Netlify / Vercel:** Drag and drop the project folder into their dashboard.
2. **GitHub Pages:** Push the code to a repository and enable GitHub Pages in settings.
3. **cPanel / Shared Hosting:** Upload all files to the `public_html` directory via FTP.

## ♿ Accessibility Notes

- **Focus States:** All interactive elements have a visible orange outline when navigated via keyboard (Tab key).
- **Screen Readers:** ARIA labels are added to buttons (e.g., "Toggle Dark Mode", "Emergency Call").
- **Motion:** Users with "Reduce Motion" enabled in their OS will see animations disabled automatically.

## 📄 License

This project is proprietary software created for the client. All rights reserved.

## 🤝 Support

For technical issues or further customization, please contact the development team.

```

```
