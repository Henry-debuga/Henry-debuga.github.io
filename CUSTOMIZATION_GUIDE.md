# Portfolio Customization Guide

Welcome to your professional portfolio website! This guide will help you customize it with your own information.

## 🚀 Quick Start

Your portfolio is now live at: **https://henry-debuga.github.io**

## 📝 How to Customize

### 1. Update Your Profile Information (index.html)

**Profile Picture:**
- Replace the placeholder image URL on line ~55
- Current: `https://via.placeholder.com/200`
- Replace with your image URL or upload to the repo

**Hero Section (lines 52-67):**
```html
<h1>Henry Debuga</h1>  <!-- Change to your name -->
<p class="subtitle">Full-Stack Programmer & Creative Designer</p>  <!-- Your title -->
<p class="description">Your description here</p>  <!-- Your tagline -->
```

**Contact Information (lines 247-265):**
```html
<p>henry@example.com</p>  <!-- Your email -->
<p>+1 (555) 123-4567</p>  <!-- Your phone -->
<p>San Francisco, CA</p>  <!-- Your location -->
```

### 2. Update About Section (lines 96-118)

Replace the placeholder text with your actual bio. Add 2-3 paragraphs about:
- Your background and experience
- Your skills and expertise
- Your passion and goals

**Statistics (lines 121-135):**
Update the numbers and labels to match your experience:
```html
<div class="stat">
    <h3>5+</h3>  <!-- Change number -->
    <p>Years Experience</p>  <!-- Change label -->
</div>
```

### 3. Update Skills Section (lines 138-186)

Add or remove skill tags:
```html
<span class="skill-tag">JavaScript</span>
<span class="skill-tag">Your Skill Here</span>
```

Categories included:
- Programming
- Design
- Tools & Technologies

Feel free to add more categories by copying the `skill-category` div.

### 4. Update Blog Section (lines 189-240)

Replace blog placeholders with your actual articles:

**For each blog post (lines 199-220):**
```html
<article class="blog-card">
    <div class="blog-image">
        <img src="your-image-url" alt="Blog Post">
    </div>
    <div class="blog-content">
        <span class="blog-category">Your Category</span>
        <h3>Your Article Title</h3>
        <p>Article preview/summary</p>
        <a href="your-article-url" class="blog-link">Read More →</a>
    </div>
</article>
```

### 5. Update Footer (lines 293-310)

**Social Links:** Add your social media profiles
```html
<a href="https://github.com/yourprofile" target="_blank"><i class="fab fa-github"></i></a>
<a href="https://linkedin.com/in/yourprofile" target="_blank"><i class="fab fa-linkedin"></i></a>
<!-- Add more social links as needed -->
```

## 🎨 Customizing Colors

Edit `style.css` lines 8-15 to change the color scheme:

```css
:root {
    --primary-color: #6366f1;      /* Main color */
    --secondary-color: #ec4899;    /* Accent color */
    --dark-bg: #0f172a;            /* Dark background */
    --light-bg: #f8fafc;           /* Light background */
    --text-dark: #1e293b;          /* Dark text */
    --text-light: #64748b;         /* Light text */
}
```

## 📧 Setting Up Contact Form

The contact form uses Formspree for free email delivery. To enable it:

1. Go to [formspree.io](https://formspree.io)
2. Sign up and create a new form
3. Copy your form ID
4. In `script.js` line 33, replace `YOUR_FORM_ID` with your actual form ID:

```javascript
const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
```

Example: `https://formspree.io/f/xyzabc123`

## 🖼️ Adding Your Profile Picture

**Option 1: Use an Image URL**
- Use any online image URL
- Replace placeholder in index.html line 55

**Option 2: Upload to Repository**
1. Click "Add file" → "Upload files" on your repo
2. Upload your image (e.g., `profile.jpg`)
3. Update the src: `<img src="profile.jpg" alt="Profile Picture">`

## 🔗 Adding Project Links

You can add project showcase by creating a new section or linking from blog posts/skills to your GitHub projects.

## 📱 Mobile Responsiveness

Your portfolio is fully responsive! It automatically adapts to:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (480px - 767px)

Breakpoints defined in `style.css` starting at line 306.

## 🚀 Deployment

Your site is automatically deployed to GitHub Pages. 

**To update:**
1. Make changes to files in your repository
2. Commit and push to `main` branch
3. Changes appear within 1-2 minutes at https://henry-debuga.github.io

## 📚 File Structure

```
henry-debuga.github.io/
├── index.html          # Main HTML file
├── style.css           # Styling and layout
├── script.js           # JavaScript interactivity
├── README.md           # This file
└── profile.jpg         # (Optional) Your profile image
```

## 🎯 Next Steps

1. ✅ Update your profile information
2. ✅ Add your profile picture
3. ✅ Update skills and about section
4. ✅ Add your blog articles or projects
5. ✅ Set up contact form with Formspree
6. ✅ Add social media links
7. ✅ Test on mobile devices

## 💡 Tips

- Keep content concise and professional
- Use high-quality images
- Regularly update blog with new articles
- Test form submissions
- Monitor your email for contact form submissions

## 🆘 Troubleshooting

**Contact form not working?**
- Verify Formspree form ID is correct
- Check browser console for errors (F12)
- Ensure email address is valid

**Images not showing?**
- Check image URL is accessible
- Ensure correct file path if uploading to repo
- Try different image format (jpg, png, webp)

**Mobile menu not working?**
- Clear browser cache
- Ensure script.js is loaded (check console)

## 📞 Support

For GitHub Pages issues, visit: [GitHub Pages Documentation](https://docs.github.com/en/pages)

---

Happy customizing! 🎉 Your portfolio is now ready to showcase your amazing work!