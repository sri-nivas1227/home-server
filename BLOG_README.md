# Blog Template Documentation

## Overview
This is a basic, responsive blog template designed for the home server. It includes a clean, modern design with mobile-friendly layouts.

## Files Included

### 1. `index.html` - Blog Homepage
The main landing page that displays:
- Navigation bar with logo and menu links
- Hero section with welcome message
- Blog post cards showing latest articles
- Footer with copyright information

### 2. `sample-post.html` - Sample Blog Post
A complete example blog post demonstrating:
- Article header with metadata (date, category)
- Full content structure with sections
- Lists, paragraphs, and formatting examples
- Navigation back to homepage

### 3. `post-template.html` - Template for New Posts
A blank template file to copy when creating new blog posts. Includes:
- Placeholder sections marked with `[brackets]`
- Standard structure for consistency
- All necessary styling hooks

### 4. `style.css` - Stylesheet
Comprehensive CSS styling including:
- Modern, clean design with gradient accents
- Responsive layout (mobile-friendly)
- Smooth transitions and hover effects
- Typography optimized for readability
- Color scheme: Dark blue headers (#2c3e50), purple gradients, and blue accents

## How to Use

### Viewing the Blog
Simply open `index.html` in a web browser to view the blog homepage.

### Creating a New Blog Post
1. Copy `post-template.html` to a new file (e.g., `my-new-post.html`)
2. Replace all `[placeholder]` text with your content:
   - `[Date]` - Publication date
   - `[Category]` - Post category
   - `[Post Title]` - Your post title
   - `[Post subtitle]` - Brief description
3. Fill in the content sections with your text
4. Add the new post to `index.html` by creating a new post card in the "blog-posts" section

### Adding a Post to Homepage
In `index.html`, add a new article card:
```html
<article class="post-card">
    <div class="post-meta">
        <span class="post-date">Your Date</span>
        <span class="post-category">Your Category</span>
    </div>
    <h4><a href="your-post.html">Your Post Title</a></h4>
    <p>Brief excerpt or description of your post...</p>
    <a href="your-post.html" class="read-more">Read More →</a>
</article>
```

### Customization
- **Colors**: Edit the color codes in `style.css`
- **Logo/Title**: Change "Home Server Blog" in the HTML files
- **Layout**: Modify `.container` max-width in CSS for different page widths
- **Fonts**: Update the `font-family` in the `body` selector

## Features

- ✅ Responsive design (mobile, tablet, desktop)
- ✅ Clean, modern aesthetics
- ✅ Easy to customize
- ✅ No dependencies (pure HTML/CSS)
- ✅ Fast loading times
- ✅ Semantic HTML structure
- ✅ Accessible navigation

## Serving the Blog

### Option 1: Simple HTTP Server (Python)
```bash
python3 -m http.server 8000
```
Then visit `http://localhost:8000`

### Option 2: Node.js HTTP Server
```bash
npx http-server
```

### Option 3: Use with Nginx/Apache
Copy the files to your web server's document root.

## Browser Compatibility
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Future Enhancements
Consider adding:
- RSS feed generation
- Search functionality
- Comments section
- Dark mode toggle
- Tag system for posts
- Archive/category pages

## License
Free to use and modify for personal and commercial projects.
