# Personal Portfolio Website

This is Minh Pham's personal portfolio website featuring projects, research, and professional information.

## Website Structure

```
/
├── index.html           # Main landing page
├── styles.css           # Global styles
├── research-styles.css  # Research page specific styles
├── cybersecurity.html   # Cybersecurity research page
├── pl.html             # Programming languages research page
├── randy_pausch.html   # Randy Pausch lecture insights
├── research-template.html # Template for new research pages
└── pkg/                # Tetris WASM game files
```

## Adding New Research

### Method 1: Using the Template (Recommended)

1. **Copy the template**
   ```bash
   cp research-template.html your-research-name.html
   ```

2. **Edit the new file** and update:
   - Page title in `<title>` tag
   - Research title in `<h1>`
   - Date and category in the meta section
   - Your content in the `research-content` div

3. **Add to main page**
   - Open `index.html`
   - Find the research grid section
   - Add a new research card:
   ```html
   <article class="research-card">
       <div class="research-icon">📊</div>
       <h3>Your Research Title</h3>
       <p>Brief description of your research...</p>
       <a href="your-research-name.html" class="research-link">Read More →</a>
   </article>
   ```

### Method 2: Using Markdown

1. **Create a markdown file**
   ```
   your-research.md
   ```

2. **Write your content** using standard markdown syntax

3. **Convert to HTML** manually or using a script:
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Your Title - Minh Pham</title>
       <link rel="stylesheet" href="styles.css">
       <link rel="stylesheet" href="research-styles.css">
       <link rel="preconnect" href="https://fonts.googleapis.com">
       <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
       <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
   </head>
   <body>
       <nav class="navbar">
           <div class="nav-container">
               <div class="nav-brand"><a href="index.html">Minh Pham</a></div>
               <ul class="nav-menu">
                   <li><a href="index.html#about">About</a></li>
                   <li><a href="index.html#projects">Projects</a></li>
                   <li><a href="index.html#research">Research</a></li>
                   <li><a href="index.html#contact">Contact</a></li>
               </ul>
               <div class="nav-toggle" id="mobile-menu">
                   <span class="bar"></span>
                   <span class="bar"></span>
                   <span class="bar"></span>
               </div>
           </div>
       </nav>

       <main class="research-main">
           <article class="research-article">
               <header class="research-header">
                   <h1>Your Title</h1>
                   <div class="research-meta">
                       <span class="research-date">2024</span>
                       <span class="research-category">Category</span>
                   </div>
               </header>

               <div class="research-content">
                   <!-- Your markdown content converted to HTML -->
               </div>

               <footer class="research-footer">
                   <a href="index.html#research" class="back-link">← Back to Research</a>
               </footer>
           </article>
       </main>

       <footer class="footer">
           <div class="container">
               <p>&copy; 2024 Minh Pham. All rights reserved.</p>
           </div>
       </footer>

       <script>
           const mobileMenu = document.getElementById('mobile-menu');
           const navMenu = document.querySelector('.nav-menu');
           mobileMenu.addEventListener('click', () => {
               navMenu.classList.toggle('active');
               mobileMenu.classList.toggle('active');
           });
       </script>
   </body>
   </html>
   ```

4. **Add the research card to index.html** (same as Method 1, step 3)

## Styling Guide

- Research pages automatically inherit styles from `research-styles.css`
- Available HTML elements with built-in styling:
  - `<h2>` - Major sections (with accent bar)
  - `<h3>` - Subsections
  - `<p>` - Paragraphs
  - `<ul>`, `<ol>` - Lists
  - `<blockquote>` - Quotes
  - `<code>` - Inline code
  - `<pre><code>` - Code blocks
  - `<a>` - Links (automatically styled)

## Icons for Research Cards

Choose an appropriate emoji for the `research-icon` div:
- 🔒 Security/Privacy
- 💻 Programming/Development
- 📊 Data/Analytics
- 🎯 Goals/Productivity
- 🧠 AI/Machine Learning
- 🌐 Web/Network
- 📱 Mobile
- 🎨 Design/UI/UX
- 🚀 Innovation/Startups
- 📚 Education/Learning

## Development

To test your changes locally:
1. Open `index.html` in a web browser
2. For the Tetris game to work, you may need to run a local server:
   ```bash
   python -m http.server 8000
   # or
   npx http-server
   ```

## Notes

- All research pages are responsive and mobile-friendly
- Navigation is consistent across all pages
- The template includes all necessary scripts and styles
- Keep research summaries on the main page brief (2-3 sentences)