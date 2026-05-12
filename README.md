# Harshita Umesh - Portfolio Website

A professional portfolio website for Harshita Umesh, Advertising Producer based in Bangalore, India.

## About

This portfolio showcases Harshita's work producing print and digital advertising campaigns for major Indian brands including PUMA, Titan, Tata Tea, Allen Solly, Ikea, and many more.

## Features

- Clean, professional design focused on showcasing work
- Fully responsive (mobile, tablet, desktop)
- Smooth scrolling navigation
- Animated project cards with staggered loading
- Ready for Heroku deployment
- SEO optimized

## Local Development

1. Install dependencies:
```bash
cd ~/claude-projects/portfolio
npm install
```

2. Run the development server:
```bash
npm run dev
```

3. Open your browser and visit `http://localhost:3000`

## Project Structure

```
portfolio/
├── public/
│   ├── index.html      # Main HTML with all content
│   ├── styles.css      # Professional styling
│   └── script.js       # Smooth animations & interactions
├── server.js           # Express server
├── package.json        # Node.js dependencies
├── Procfile           # Heroku configuration
└── README.md          # This file
```

## Deploying to GitHub Pages

### Quick Deploy

1. Create a new repo on GitHub (e.g., `harshita-portfolio`)

2. Push your code:
```bash
git remote add origin https://github.com/YOUR_USERNAME/harshita-portfolio.git
git add .
git commit -m "Initial portfolio"
git branch -M main
git push -u origin main
```

3. Enable GitHub Pages:
   - Go to repo Settings → Pages
   - Source: Deploy from branch
   - Branch: `main` / folder: `/ (root)`
   - Save

4. Your site will be live at: `https://YOUR_USERNAME.github.io/harshita-portfolio/`

### Alternative: Use `gh-pages` branch

```bash
# Install gh-pages package
npm install --save-dev gh-pages

# Add to package.json scripts:
# "deploy": "gh-pages -d public"

# Then deploy:
npm run deploy
```

## Customization Guide

### Adding Project Images

Replace the placeholder divs in `public/index.html` with actual images:

```html
<!-- Before -->
<div class="placeholder-image">Project Name</div>

<!-- After -->
<img src="path/to/image.jpg" alt="Project Name">
```

### Updating Content

1. **Personal Information**: Edit `public/index.html`
   - Update name, bio, location in relevant sections
   - Add actual email address in the contact section
   - Verify all social media links

2. **Projects**: Add or remove projects in the work grid
   - Each project follows the same `.project-card` structure
   - Add `data-category` attributes for filtering (future feature)

3. **Colors**: Modify `public/styles.css`
   - Change CSS variables in `:root` section
   - Primary color: `--primary-color`
   - Accent color: `--accent-color` (currently orange)

### Adding a Project

```html
<div class="project-card" data-category="campaign">
    <div class="project-image">
        <img src="project-image.jpg" alt="Project Name">
    </div>
    <div class="project-info">
        <h3>Project Name</h3>
        <p class="project-category">Campaign Type</p>
    </div>
</div>
```

## Technologies Used

- **Backend**: Node.js, Express
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Deployment**: Heroku
- **Design**: Minimalist, portfolio-focused aesthetic

## Future Enhancements

- [ ] Add project detail pages/modals
- [ ] Implement filtering by project category
- [ ] Add testimonials section
- [ ] Integrate with Behance API to pull projects dynamically
- [ ] Add contact form with email backend
- [ ] Add blog/insights section
- [ ] Implement dark mode toggle

## Links

- **Behance**: https://www.behance.net/harshitaumesh
- **Instagram**: https://www.instagram.com/crayon.pictures
- **LinkedIn**: https://www.linkedin.com/in/harshita-umesh/

## License

MIT License - feel free to use this template for your own portfolio.

---

Built with ☕ for showcasing creative advertising work.
