# Quick Start Guide for Lxya Blog

## 🏁 Get Started in 5 Minutes

### Step 1: Preview Your Site
```bash
hugo server
```
Visit http://localhost:1313 to see your blog in action!

### Step 2: Create a New Blog Post
```bash
hugo new posts/my-new-post.md
```

Edit the file in `content/posts/my-new-post.md` and set `draft = false` when ready to publish.

### Step 3: Add Your Content
1. Update [content/about.md](content/about.md) with your information
2. Add your logo to `static/images/logo.png`
3. Add your profile photo to `static/images/profile.jpg`

### Step 4: Build for Production
```bash
hugo
```

Your website is now in the `public/` folder, ready to deploy!

## 📁 Project Structure

```
myblog/
├── content/           # Your blog posts and pages
│   ├── about.md      # About Me page
│   ├── search.md     # Search page
│   └── posts/        # Blog posts go here
├── layouts/          # Custom templates
│   ├── posts/        # Blog post templates
│   └── partials/     # Reusable components
├── assets/           # CSS and JavaScript
│   └── css/
│       └── extended/ # Your custom styles
├── static/           # Images, fonts, files
│   └── images/       # Store all images here
├── hugo.toml         # Main configuration file
└── SETUP-GUIDE.md    # Detailed instructions
```

## ✏️ Writing Your First Post

1. Create a new post:
   ```bash
   hugo new posts/getting-started.md
   ```

2. Open the file and you'll see a template with all SEO fields

3. Write your content using proper headings:
   - **H1** (title) - Automatically from front matter
   - **H2** (##) - Main sections
   - **H3** (###) - Subsections

4. Add images:
   ```markdown
   ![Alt text describing image](/images/my-image.jpg)
   ```

5. Set `draft = false` when ready to publish

## 🎨 Customization

### Change Colors
Edit `assets/css/extended/custom.css`:
```css
:root {
    --primary-color: #your-color;
    --secondary-color: #your-color;
}
```

### Update Site Info
Edit `hugo.toml`:
- Change `title`, `description`, `author`
- Update social media links
- Add Google Analytics ID

### Add Logo
1. Save your logo as `static/images/logo.png`
2. In `hugo.toml`, add:
```toml
[params.label]
icon = "/images/logo.png"
iconHeight = 35
```

## 🚀 Deployment

### GitHub Pages
1. Push your code to GitHub
2. Set up GitHub Actions for Hugo
3. Deploy to `username.github.io`

### Netlify
1. Connect your GitHub repo
2. Build command: `hugo`
3. Publish directory: `public`

### Vercel
1. Import your GitHub repo
2. Select Hugo framework
3. Deploy automatically

## 📊 SEO Checklist

For every post:
- [ ] Write compelling title with keywords
- [ ] Add meta description (150-160 chars)
- [ ] Use proper heading hierarchy (H1 → H2 → H3)
- [ ] Add featured image with alt text
- [ ] Include relevant tags
- [ ] Write 1200+ words for important topics
- [ ] Add internal links to related posts
- [ ] Optimize all images (under 200KB)

## 🆘 Common Issues

**Images not showing?**
- Ensure images are in `static/images/`
- Use absolute path: `/images/name.jpg`
- Check file name capitalization

**CSS not applying?**
- Run `hugo server` with `--disableFastRender`
- Clear browser cache

**Build errors?**
- Check front matter syntax (must use `+++` or `---`)
- Ensure all required fields are present
- Verify image paths are correct

## 📚 Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [PaperMod Theme Docs](https://github.com/adityatelange/hugo-PaperMod)
- [SEO Guide](SETUP-GUIDE.md)
- [Markdown Syntax](https://www.markdownguide.org/)

## 💡 Next Steps

1. **Content First**: Write 5-10 quality posts before heavy promotion
2. **SEO Setup**: Submit sitemap to Google Search Console
3. **Email List**: Set up Mailchimp or ConvertKit
4. **Social Media**: Share posts on Twitter, LinkedIn
5. **Analytics**: Monitor what content performs best
6. **Consistency**: Publish on a regular schedule

Need help? Check [SETUP-GUIDE.md](SETUP-GUIDE.md) for detailed instructions!

Happy blogging! 🎉
