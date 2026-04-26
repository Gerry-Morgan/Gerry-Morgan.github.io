# Gerry Morgan — Hugo Website

Official website for **Gerry Morgan**, Canadian songwriter, author, educator, and software designer. Powered by [Hugo](https://gohugo.io/) and the custom **Geezer** theme.

## Quick Start

```bash
# Install Hugo (if needed)
# See: https://gohugo.io/installation/

# Run the dev server
hugo server -D

# Build for production
hugo --minify
```

The site will be available at `http://localhost:1313/`.

## Site Structure

```
├── hugo.toml                  # Main site configuration
├── archetypes/                # Templates for new content
│   ├── blog.md                # Blog post template
│   ├── music.md               # Music entry template
│   └── default.md             # Default template
├── content/
│   ├── _index.md              # Homepage
│   ├── about.md               # Professional bio
│   ├── contact.md             # Contact information
│   ├── blog/
│   │   ├── _index.md          # Blog listing page
│   │   └── *.md               # Daily Innovation Reports
│   ├── music/
│   │   ├── _index.md          # Music catalogue page
│   │   └── *.md               # Individual songs/albums
│   └── pantokrator/
│       └── _index.md          # Rock opera dedicated page
├── themes/geezer/             # Custom theme
│   ├── layouts/
│   │   ├── _default/
│   │   │   ├── baseof.html    # Base template
│   │   │   ├── single.html    # Single page/post
│   │   │   └── list.html      # List/archive pages
│   │   ├── partials/
│   │   │   ├── header.html    # Site header & nav
│   │   │   └── footer.html    # Site footer
│   │   └── index.html         # Homepage template
│   └── static/css/
│       └── style.css          # Complete stylesheet
└── static/
    ├── css/                   # Additional stylesheets
    ├── images/                # Site images (add og-default.jpg, favicon.ico)
    └── js/                    # JavaScript files
```

## Adding Content

### New Blog Post (Daily Innovation Report)
```bash
hugo new blog/2026-04-27-title-of-post.md
```

### New Song/Album Entry
```bash
hugo new music/song-title.md
```

## Key Pages

| Page | URL | Description |
|------|-----|-------------|
| Home | `/` | Hero + featured sections + recent posts |
| About | `/about/` | Full professional biography |
| Music | `/music/` | Catalogue of 900+ songs |
| Pantokrator | `/pantokrator/` | Rock opera dedicated page |
| Blog | `/blog/` | Daily Innovation Reports |
| Contact | `/contact/` | Email and social links |

## Customization

- **Site settings**: Edit `hugo.toml` (title, author, social links, contact email)
- **Styling**: Edit `themes/geezer/static/css/style.css`
- **Layout**: Edit templates in `themes/geezer/layouts/`

## TODO

- [ ] Add real profile/hero images to `static/images/`
- [ ] Add favicon (`static/images/favicon.ico`)
- [ ] Add Open Graph image (`static/images/og-default.jpg`)
- [ ] Fill in social media links in `hugo.toml`
- [ ] Populate music catalogue with real song entries
- [ ] Complete Pantokrator track listing and act structure
- [ ] Set up mailing list integration
- [ ] Configure deployment (Netlify, Vercel, or similar)

## Label

**Geezer Records** — Independent music label by Gerry Morgan.

## License

Content copyright Gerry Morgan. Theme code MIT.
