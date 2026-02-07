# Hair Kabana Website - Documentation

## Overview
This is a complete, elegant website for **Hair Kabana** salon. The site features a sophisticated design with a warm, professional aesthetic perfect for a luxury hair salon.

---

## File Structure

```
hair-kabana-website/
│
├── index.html          (Home page)
├── about.html          (About page)
├── services.html       (Services page)
├── contact.html        (Contact page)
├── style.css           (Main stylesheet)
└── README.md           (This file)
```

---

## Features

### Design
- **Elegant & Luxe Aesthetic**: Sophisticated color palette with gold accents
- **Sticky Navigation**: Header stays at top when scrolling
- **Fully Responsive**: Works perfectly on mobile, tablet, and desktop
- **Clean Typography**: Uses Google Fonts (Playfair Display + Lato)
- **Professional Layout**: Ample white space, clear hierarchy

### Technical
- **Semantic HTML5**: Proper use of header, nav, main, section, footer
- **CSS Variables**: Easy color/spacing customization at top of CSS file
- **Mobile-First**: Responsive breakpoints at 768px and 480px
- **No Framework**: Pure HTML/CSS/JavaScript (lightweight and fast)
- **Well Commented**: Clear explanations throughout code

---

## Customization Guide

### 1. Update Contact Information

**In ALL HTML files (footer section):**
```html
<p>123 Main Street | (555) 123-4567 | hello@hairkabana.com</p>
```
Replace with your actual address, phone, and email.

**In contact.html:**
- Update phone number (lines 66-68)
- Update email (lines 73-75)
- Update physical address (lines 80-86)
- Update opening hours (lines 91-113)
- Update Instagram handle (lines 119-125)

---

### 2. Add Your Images

The site has placeholders for images. Replace these:

#### Hero Image (Home Page)
**Location**: `style.css` line 180
```css
background: url('hero-placeholder.jpg') center/cover no-repeat;
```
- Upload a high-quality image of your salon interior or styled hair
- Name it `hero-placeholder.jpg` OR update the filename in CSS
- Recommended size: 1920x1080px

#### About Image (About Page)
**Location**: `style.css` line 398
```css
background: url('about-placeholder.jpg') center/cover no-repeat;
```
- Upload a photo of your salon interior or team
- Name it `about-placeholder.jpg` OR update the filename in CSS
- Recommended size: 800x800px

---

### 3. Add Google Maps

**In contact.html** (line 139):

1. Go to [Google Maps](https://www.google.com/maps)
2. Search for your salon address
3. Click **"Share"** → **"Embed a map"**
4. Copy the `<iframe>` code
5. Replace the placeholder div with your iframe code

Example:
```html
<iframe 
    src="https://www.google.com/maps/embed?pb=YOUR_EMBED_CODE" 
    width="100%" 
    height="400" 
    style="border:0;" 
    allowfullscreen="" 
    loading="lazy">
</iframe>
```

---

### 4. Update Colors

**Location**: `style.css` lines 11-22

The color palette uses CSS variables for easy customization:

```css
:root {
    --primary-dark: #2c2c2c;        /* Change main text color */
    --primary-light: #ffffff;       /* Change background color */
    --accent-gold: #c9a961;         /* Change accent color */
    --neutral-gray: #f5f5f5;        /* Change section backgrounds */
    --mid-gray: #666666;            /* Change secondary text */
}
```

Simply update these hex codes to change the entire color scheme.

---

### 5. Add Instagram Link

**In ALL HTML files** (footer and contact page):

Find:
```html
<a href="#" aria-label="Instagram">📷</a>
```

Replace `#` with your Instagram profile URL:
```html
<a href="https://instagram.com/hairkabana" aria-label="Instagram">📷</a>
```

---

### 6. Update Services & Pricing

**In services.html:**

Each service is contained in a `<div class="service-card">`. To edit:

```html
<div class="service-card">
    <h3>Service Name</h3>
    <p>Service description goes here...</p>
    <p class="service-price">From $XX</p>
</div>
```

- Change the service name in `<h3>`
- Update the description in `<p>`
- Update pricing in `<p class="service-price">`

To add a new service, copy an entire service-card div and paste it within the services-grid.

---

### 7. Adjust Spacing

**Location**: `style.css` lines 24-29

Spacing throughout the site uses CSS variables:

```css
--spacing-xs: 0.5rem;
--spacing-sm: 1rem;
--spacing-md: 2rem;
--spacing-lg: 3rem;
--spacing-xl: 4rem;
```

Increase/decrease these values to adjust spacing globally.

---

## Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

## Deployment

### Option 1: Basic Web Hosting
1. Upload all files to your web hosting via FTP
2. Ensure `index.html` is in the root directory
3. Done! Your site is live.

### Option 2: Free Hosting (Netlify/Vercel)
1. Create account on [Netlify](https://netlify.com) or [Vercel](https://vercel.com)
2. Drag and drop the entire folder
3. Get a free URL instantly
4. Optional: Connect custom domain

---

## Page Descriptions

### Home (index.html)
- Welcoming hero section with call-to-action buttons
- Brief introduction to the salon
- Highlights of key features

### About (about.html)
- Salon story and philosophy
- Team/founder background
- Personal, authentic tone

### Services (services.html)
- Complete list of 9 services
- Descriptions and pricing
- Professional service cards layout

### Contact (contact.html)
- Phone, email, address
- Opening hours
- Map placeholder
- Social media links

---

## Maintenance Tips

### To Keep Content Fresh:
1. Update service descriptions seasonally
2. Add new services as you expand
3. Update pricing annually
4. Share new Instagram posts regularly

### To Maintain Performance:
1. Optimize images before uploading (use tinypng.com)
2. Keep file sizes under 500KB per image
3. Test on mobile devices regularly

---

## Support

For questions about customization:
- **HTML/CSS basics**: [W3Schools](https://www.w3schools.com)
- **Google Fonts**: [fonts.google.com](https://fonts.google.com)
- **CSS color picker**: [htmlcolorcodes.com](https://htmlcolorcodes.com)

---

## Credits

- **Fonts**: Google Fonts (Playfair Display, Lato)
- **Design**: Custom elegant theme
- **Framework**: None (vanilla HTML/CSS/JS)

---

**Last Updated**: February 2026
