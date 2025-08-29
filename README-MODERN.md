# Oregon Software Website - Modernized with Tailwind CSS

A modern, responsive website for Oregon Software built with Tailwind CSS, featuring contemporary design patterns and enhanced user experience.

## 🚀 Features

- **Modern Design**: Clean, professional design using Tailwind CSS utility classes
- **Fully Responsive**: Optimized for all devices (mobile, tablet, desktop)
- **Fast Loading**: Lightweight and optimized for performance
- **Accessible**: Built with accessibility best practices
- **SEO Optimized**: Proper meta tags and structured content
- **Analytics Ready**: Google Analytics (GA4) integration included
- **Interactive Elements**: Smooth animations and hover effects
- **Portfolio Filtering**: Dynamic portfolio filtering with smooth transitions
- **Mobile-First**: Designed with mobile-first approach

## 📁 Project Structure

```
website/
├── index.html              # Homepage (modernized)
├── portfolio.html          # Portfolio page (modernized)
├── team.html              # Team page (modernized)
├── CNAME                  # GitHub Pages domain configuration
├── README.md              # This file
├── assets/
│   ├── css/
│   │   ├── style.css      # Original CSS (legacy)
│   │   └── modern-style.css # Additional modern styles
│   ├── img/               # Images and logos
│   ├── js/                # JavaScript files
│   ├── portfolio/         # Portfolio images
│   └── vendor/            # Third-party libraries (legacy)
```

## 🎨 Design System

### Colors
- **Primary Oregon Green**: `#596808` (oregon-600)
- **Light Oregon**: `#eff4dc` (oregon-100)
- **Dark Oregon**: `#414d06` (oregon-800)
- **Neutral Grays**: Standard Tailwind gray palette

### Typography
- **Headings**: Poppins font family
- **Body Text**: Inter font family
- **Responsive Text**: Scales appropriately across devices

### Components
- **Cards**: Modern card design with hover effects
- **Buttons**: Rounded, accessible button styles
- **Navigation**: Fixed header with smooth transitions
- **Footer**: Comprehensive footer with social links

## 🔧 Setup Instructions

### 1. Clone or Download
```bash
git clone [repository-url]
cd oregon-software/website
```

### 2. Analytics Setup
Replace `YOUR_MEASUREMENT_ID` in all HTML files with your actual Google Analytics 4 Measurement ID:

```html
<!-- Find this in the <head> section of each HTML file -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_MEASUREMENT_ID');
</script>
```

### 3. Local Development
You can serve the website locally using any web server:

**Using Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js (if you have it installed):**
```bash
npx serve .
```

**Using PHP:**
```bash
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

### 4. Deployment
The website is ready for deployment to any static hosting service:

- **GitHub Pages**: Push to a repository and enable GitHub Pages
- **Netlify**: Drag and drop the `website` folder
- **Vercel**: Import the repository
- **AWS S3**: Upload files to an S3 bucket configured for static hosting

## 🎯 Analytics Integration Options

### Google Analytics 4 (GA4) - Recommended
1. Create a GA4 property at [analytics.google.com](https://analytics.google.com)
2. Get your Measurement ID (format: G-XXXXXXXXXX)
3. Replace `YOUR_MEASUREMENT_ID` in all HTML files

### Google Tag Manager (Alternative)
If you prefer Google Tag Manager:
1. Create a GTM container
2. Replace the GA4 code with GTM code
3. Configure tracking through GTM interface

### Other Analytics Services
The code can be easily modified to support:
- Facebook Pixel
- Hotjar
- Mixpanel
- Custom analytics solutions

## 📱 Responsive Design

The website is built with a mobile-first approach:

- **Mobile (< 768px)**: Single column layout, collapsible navigation
- **Tablet (768px - 1023px)**: Two-column layouts where appropriate
- **Desktop (1024px+)**: Multi-column layouts, enhanced interactions

## ⚡ Performance Optimizations

- **CDN Resources**: Tailwind CSS and fonts loaded from CDN
- **Optimized Images**: Proper image sizing and formats
- **Minimal JavaScript**: Only essential JavaScript for functionality
- **CSS Purging**: Production builds should purge unused Tailwind classes

## 🔧 Customization

### Colors
To change the brand colors, update the Tailwind configuration in each HTML file:

```javascript
tailwind.config = {
  theme: {
    extend: {
      colors: {
        'oregon': {
          500: '#YOUR_PRIMARY_COLOR',
          600: '#YOUR_PRIMARY_COLOR_DARK',
          700: '#YOUR_PRIMARY_COLOR_DARKER',
        }
      }
    }
  }
}
```

### Fonts
Update the Google Fonts import and Tailwind font configuration:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@300;400;500;600;700&display=swap" rel="stylesheet">
```

### Content
- Update company information in all HTML files
- Replace images in the `assets/img/` directory
- Modify portfolio items in `portfolio.html`
- Update team member information in `team.html`

## 🌟 Modern Features Implemented

### Interactive Elements
- Smooth scrolling navigation
- Hover effects on cards and buttons
- Portfolio filtering with animations
- Mobile-responsive hamburger menu
- Back-to-top button with smooth scroll

### Accessibility
- Proper heading hierarchy
- Alt text for images
- Focus states for keyboard navigation
- ARIA labels where appropriate
- Color contrast compliance

### SEO Optimization
- Semantic HTML structure
- Meta descriptions and keywords
- Open Graph tags ready for implementation
- Structured data markup ready for implementation

## 🔍 Browser Support

- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile Browsers**: iOS Safari, Chrome Mobile, Samsung Browser
- **Fallbacks**: Graceful degradation for older browsers

## 📞 Support

For questions or support with the modernized website:
- Review the documentation above
- Check browser developer tools for any console errors
- Ensure all file paths are correct for your hosting environment

## 📈 Next Steps

### Recommended Enhancements
1. **SEO**: Add structured data markup
2. **Performance**: Implement lazy loading for images
3. **PWA**: Add service worker for offline functionality
4. **Forms**: Implement contact forms with backend integration
5. **CMS**: Consider headless CMS integration for content management

### Production Optimizations
1. **CSS Purging**: Remove unused Tailwind classes
2. **Image Optimization**: Compress and convert images to modern formats
3. **CDN**: Implement CDN for static assets
4. **Caching**: Configure proper cache headers
5. **Monitoring**: Set up performance monitoring

---

## 📄 License

This project is for Oregon Software. All rights reserved.

## 🤝 Contributing

For modifications or improvements, please follow the established code structure and maintain the responsive design principles.
