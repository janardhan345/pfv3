# Portfolio Template

A documentation-style portfolio website with Flexoki theme colors. Features a left sidebar for navigation, main content area, and right sidebar for page outlines.

## File Structure

```
├── index.html      # Main HTML file with all sections
├── styles.css      # Styling with Flexoki color palette
├── script.js       # Navigation, routing, and theme logic
└── README.md       # This file
```

## Features

- 📱 **Responsive Design** - Works on desktop, tablet, and mobile
- 🎨 **Flexoki Theme** - Beautiful color palette inspired by Flexoki
- 🌙 **Dark Mode** - Toggle between light and dark modes (saved to localStorage)
- 📑 **Dynamic Outline** - Right sidebar auto-generates from page headings
- ⚡ **Hash-based Routing** - Client-side routing without server
- 🎯 **Active States** - Visual indicators for current page and outline section
- ✨ **Smooth Animations** - Page transitions and hover effects

## Sections

The template includes 5 main sections (routes):

1. **About** - Your introduction and bio
2. **Skills** - Skills organized by category
3. **Projects** - Portfolio projects with cards
4. **Blog** - Blog posts with dates and excerpts
5. **Contact** - Contact methods and links

## How to Customize

### 1. Edit Content

Open `index.html` and replace the placeholder text in each section with your own content.

**About Section:**
```html
<section id="about" class="page-section active">
    <h1>About Me</h1>
    <p>Your bio here...</p>
</section>
```

**Skills Section:**
Add your skills by modifying the skill categories:
```html
<div class="skill-category">
    <h3>Your Skill Category</h3>
    <ul>
        <li>Skill 1</li>
        <li>Skill 2</li>
    </ul>
</div>
```

**Projects Section:**
Update project cards:
```html
<div class="project-card">
    <h3>Your Project Title</h3>
    <p>Project description</p>
    <a href="your-link.com" class="project-link">View Project →</a>
</div>
```

**Blog Section:**
Add blog posts:
```html
<article class="blog-item">
    <h3>Your Blog Title</h3>
    <span class="blog-date">Your Date</span>
    <p>Blog excerpt...</p>
    <a href="#" class="read-more">Read more →</a>
</article>
```

**Contact Section:**
Update contact links:
```html
<a href="mailto:your@email.com" class="contact-link">Email</a>
<a href="https://github.com/yourprofile" class="contact-link">GitHub</a>
```

### 2. Customize Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --accent: var(--blue);  /* Change this to var(--purple), var(--green), etc. */
}
```

Available colors:
- `--red`, `--orange`, `--yellow`, `--green`
- `--cyan`, `--blue`, `--purple`, `--magenta`

Or define custom colors:
```css
:root {
    --accent: #your-color;
}
```

### 3. Add Sections

To add a new section/route:

1. Add to HTML:
```html
<section id="new-section" class="page-section">
    <h2>New Section</h2>
    <p>Content here...</p>
</section>
```

2. Add to left sidebar navigation:
```html
<li><a href="#new-section" class="nav-link">New Section</a></li>
```

The outline and routing will work automatically!

### 4. Add Images

Place images in the project folder and reference them:
```html
<img src="image.jpg" alt="Description" width="600">
```

For better styling, wrap in a div:
```html
<div class="image-container">
    <img src="project-screenshot.png" alt="Project Screenshot">
</div>
```

Add CSS for styling:
```css
.image-container {
    margin: 2rem 0;
    border-radius: 8px;
    overflow: hidden;
}

.image-container img {
    width: 100%;
    height: auto;
}
```

### 5. Update Portfolio Info

- Change the logo text in `.logo h1`
- Update the page title in `<title>` tag
- Modify colors in the `:root` CSS variables
- Adjust spacing by modifying `padding` and `margin` values

## Theme Colors (Flexoki)

**Light Mode:**
- Background: `#fffcf0`
- Text: `#2a2724`
- Accent: `#286983` (Blue)

**Dark Mode:**
- Background: `#2a2724`
- Text: `#fffcf0`
- Accent: `#7ab5d1` (Light Blue)

## Browser Support

Works on all modern browsers:
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

## Tips

1. **SEO**: Add meta tags in `<head>`:
   ```html
   <meta name="description" content="Your portfolio description">
   <meta name="keywords" content="developer, designer, portfolio">
   ```

2. **Deploy**: Serve the folder with any static host (Netlify, Vercel, GitHub Pages, etc.)

3. **Performance**: Compress images before adding them

4. **Mobile Testing**: Use browser DevTools to test responsive design

## License

Free to use and modify for your portfolio!
