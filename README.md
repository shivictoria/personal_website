# Personal Website

A personal website built with Jekyll using the Hyde theme. Features a blog, portfolio, and resume sections.

## Features

- **Blog**: Write and publish blog posts in Markdown
- **Portfolio**: Showcase your projects and work
- **Resume**: Professional experience and skills
- **About**: Personal information and contact details
- **Responsive Design**: Works on desktop and mobile devices
- **Clean Theme**: Based on the Hyde Jekyll theme

## Prerequisites

Before you can run this website locally, you need to install:

1. **Ruby** (version 2.5 or higher)
   - Download from [ruby-lang.org](https://www.ruby-lang.org/en/downloads/)
   - Or use a version manager like [rbenv](https://github.com/rbenv/rbenv) or [rvm](https://rvm.io/)

2. **Jekyll and Bundler**
   ```bash
   gem install jekyll bundler
   ```

## Getting Started

1. **Navigate to the project directory**
   ```bash
   cd personal_website
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Start the local server**
   ```bash
   bundle exec jekyll serve
   ```

4. **Open your browser**
   - Go to `http://localhost:4000`
   - Your website should now be running locally!

## Customization

### Personal Information

Edit `_config.yml` to update:
- Your name and contact information
- Site title and description
- Social media links
- URL settings

### Content

- **Blog Posts**: Add new posts in `_posts/` directory
- **Portfolio**: Add projects in `_projects/` directory
- **Pages**: Edit `about.md`, `resume.md`, etc.

### Theme

The website uses the Hyde theme with a reverse layout. You can:
- Change the color theme by modifying the body class in `_layouts/default.html`
- Customize CSS in `public/css/hyde.css`
- Add your own images and assets

## File Structure

```
personal_website/
├── _config.yml          # Site configuration
├── _layouts/            # HTML templates
├── _includes/           # Reusable components
├── _posts/              # Blog posts
├── _projects/           # Portfolio projects
├── public/              # Static assets (CSS, images)
├── about.md             # About page
├── resume.md            # Resume page
├── blog/                # Blog index
├── portfolio/           # Portfolio index
└── index.html           # Homepage
```

## Deployment

### GitHub Pages (Recommended)

1. Push your site to a GitHub repository
2. Go to Settings > Pages
3. Select your source branch (usually `main` or `master`)
4. Your site will be available at `https://username.github.io/repository-name`

### Other Hosting Options

- **Netlify**: Drag and drop the `_site` folder
- **Vercel**: Connect your GitHub repository
- **Any static hosting service**: Upload the generated `_site` folder

## Adding Content

### New Blog Post

Create a new file in `_posts/` with the format `YYYY-MM-DD-title.md`:

```markdown
---
layout: post
title: "Your Post Title"
date: 2024-01-15
categories: [category1, category2]
excerpt: "Brief description of your post."
---

Your content here...
```

### New Portfolio Project

Create a new file in `_projects/` with the format `project-name.md`:

```markdown
---
layout: project
title: "Project Name"
technologies: "React, Node.js, MongoDB"
github: "https://github.com/username/project"
---

Project description here...
```

## Troubleshooting

### Common Issues

1. **Ruby version issues**: Make sure you have Ruby 2.5+ installed
2. **Bundle install fails**: Try `gem update bundler` first
3. **Port already in use**: Change the port with `bundle exec jekyll serve --port 4001`

### Getting Help

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Hyde Theme](https://github.com/poole/hyde)
- [GitHub Pages](https://pages.github.com/)

## License

This project is based on the Hyde theme, which is licensed under the MIT License.