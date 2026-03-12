# BRIGHT Lab Website

A professional website for the BRIGHT (Biophotonics Research In Intelligent Global Health Technologies) Laboratory at IIT Roorkee.

## Overview

This website showcases the research, team, facilities, and publications of Dr. Rishikesh Pandey's laboratory in the Department of Biosciences & Bioengineering at IIT Roorkee.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, professional design with smooth animations
- **Multiple Pages**:
  - Home: Lab overview and mission
  - News: Latest updates and events
  - Facilities: Research equipment and capabilities
  - Team: PI, PhD scholars, and students
  - Publications: Research papers and impact metrics
  - Contact: Get in touch and collaboration information

## Files Included

- `index.html` - Homepage
- `news.html` - News and updates page
- `facilities.html` - Research facilities page
- `team.html` - Team members page
- `publications.html` - Publications listing
- `contact.html` - Contact information and form
- `styles.css` - All styling and responsive design
- `script.js` - Interactive functionality and animations

## How to Use

### Option 1: Simple Local Testing
1. Download all files to a folder on your computer
2. Open `index.html` in any web browser
3. Navigate through the site using the menu

### Option 2: Deploy to Web Hosting
1. Upload all files to your web hosting service (cPanel, FTP, etc.)
2. Make sure all files are in the root directory or a subdirectory
3. Access your domain to view the live site

### Option 3: Deploy to Free Hosting Services

**GitHub Pages:**
1. Create a GitHub repository
2. Upload all files
3. Go to Settings → Pages
4. Select main branch and save
5. Your site will be live at `https://yourusername.github.io/repository-name`

**Netlify:**
1. Create account at netlify.com
2. Drag and drop your folder or connect to GitHub
3. Site will be live immediately with auto-deploy on updates

**Vercel:**
1. Create account at vercel.com
2. Import project from GitHub or upload files
3. Deploy with one click

## Customization Guide

### 1. Adding Your Logo Images
Replace the logo placeholders in the navigation:
- Edit line ~25 in each HTML file
- Replace the placeholder divs with actual `<img>` tags:
```html
<img src="images/bright-lab-logo.png" alt="BRIGHT Lab Logo" height="50">
<img src="images/iit-roorkee-logo.png" alt="IIT Roorkee Logo" height="50">
```

### 2. Adding Photos
Create an `images` folder and add:
- `pi-photo.jpg` - Dr. Pandey's photo
- `team-member-1.jpg`, etc. - Team member photos
- `news-1.jpg`, etc. - News/event images
- `research-1.jpg` - Research/lab images

Then replace placeholders in HTML files with:
```html
<img src="images/your-image.jpg" alt="Description">
```

### 3. Updating Content
- **Team Members**: Edit `team.html` - duplicate the team-member div and update details
- **Publications**: Edit `publications.html` - add new publication-item divs
- **News**: Edit `news.html` - add new news-card divs
- **Facilities**: Edit `facilities.html` - modify facility-item sections
- **Contact Info**: Update email and phone numbers in all files

### 4. Changing Colors
Edit the CSS variables in `styles.css` (lines 9-19):
```css
:root {
    --primary-color: #1e40af;  /* Main blue color */
    --secondary-color: #3b82f6;  /* Lighter blue */
    --accent-color: #60a5fa;  /* Accent blue */
    /* ... etc */
}
```

### 5. Adding Google Maps
In `contact.html`, replace the map placeholder (around line 120) with:
```html
<iframe 
    src="https://www.google.com/maps/embed?pb=YOUR_EMBED_CODE" 
    width="100%" 
    height="400" 
    style="border:0; border-radius: 12px;" 
    allowfullscreen="" 
    loading="lazy">
</iframe>
```

Get the embed code from Google Maps:
1. Search for IIT Roorkee on Google Maps
2. Click "Share" → "Embed a map"
3. Copy the iframe code

### 6. Adding Social Media Links
Update the social media links in `contact.html` with actual URLs:
```html
<a href="https://scholar.google.com/YOUR_PROFILE">Google Scholar</a>
<a href="https://www.researchgate.net/YOUR_PROFILE">ResearchGate</a>
<!-- etc -->
```

### 7. Making the Contact Form Work
The contact form currently shows an alert. To make it functional:

**Option A: Use FormSubmit (Free, No Backend Required)**
```html
<form action="https://formsubmit.co/your@email.com" method="POST">
    <input type="hidden" name="_subject" value="New Contact Form Submission">
    <input type="hidden" name="_captcha" value="false">
    <!-- Your form fields -->
</form>
```

**Option B: Use EmailJS**
1. Sign up at emailjs.com
2. Get your service ID, template ID, and public key
3. Add EmailJS script to contact.html
4. Update the form submission handler in script.js

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Technical Details

- **Framework**: Pure HTML5, CSS3, JavaScript (No dependencies)
- **Fonts**: Google Fonts (Playfair Display, Roboto)
- **Icons**: Unicode emoji icons (no external icon library needed)
- **Responsive**: Mobile-first design with CSS media queries
- **Performance**: Optimized for fast loading

## Future Enhancements

Consider adding:
- Research blog section
- Photo gallery of lab activities
- Publication search/filter functionality
- Automated publication import from Google Scholar
- Newsletter subscription
- Member login area
- Research project pages with details

## Support

For questions or issues:
1. Check the code comments in each file
2. Test in different browsers
3. Validate HTML at validator.w3.org
4. Validate CSS at jigsaw.w3.org/css-validator

## Credits

Website designed and developed for BRIGHT Lab, IIT Roorkee
Department of Biosciences & Bioengineering

---

**Note**: Remember to replace all placeholder content (XXX-XXXXXXX for phone numbers, sample publications, team member names, etc.) with actual information before deploying to production.
