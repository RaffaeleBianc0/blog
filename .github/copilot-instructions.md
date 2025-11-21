# Hugo Blog Copilot Instructions

## Architecture Overview

This is a **Hugo static site generator blog** (https://www.RaffaeleBianco.it/blog/) powered by the `hugo-theme-stack` theme. The site is Italian-language, single-language, with content organized by categories (music, bass, technology, etc.).

**Key structural patterns:**
- **Content hierarchy**: `content/post/<slug>/index.md` (bundle structure) and `content/page/<slug>/index.md`
- **Theme**: Custom overrides in `layouts/` and `assets/scss/` extend `hugo-theme-stack`
- **Build output**: Static HTML generated to `public/` directory
- **Configuration**: `hugo.toml` is the single source of truth (TOML format, not YAML)

## Content Creation & Structure

### Post Format
Posts use **YAML frontmatter** (despite `.toml` config), stored in nested directories:
- Location: `content/post/<slug>/index.md` 
- Required fields: `title`, `date`, `categories`
- Optional: `Image` (featured image path like `images/3-logo-knob.jpg`)
- Example (from `content/post/3percento/index.md`):
  ```yaml
  ---
  title: "3%"
  date: "2015-07-01"
  categories: 
    - "batteria"
    - "musica"
  Image: images/3-logo-knob.jpg
  ---
  ```

### URL Routing
- Posts: `/p/:slug/` (configured in `[permalinks]`)
- Pages: `/:slug/`
- Date format in site: `02/01/2006` (Italian DD/MM/YYYY)

## Custom Styling & Assets

### SCSS Customization
- Main file: `assets/scss/custom.scss`
- Pattern: Import partials, then override theme defaults
- Example: Article titles use `font-size: 5.0rem` desktop / `3.0rem` mobile with h1-h4 margin customizations
- **Important**: Responsive breakpoint at `@media (max-width: 720px)`

### Images & Media
- Assets: `assets/img/` (processed by Hugo's image processing)
- Static: `static/` (copied as-is)
- Featured images referenced relative to `content/post/<slug>/` or via absolute paths
- Avatar: `assets/img/avatar.png` (automatically resized by theme)

## Configuration Essentials

Key `hugo.toml` settings:
- **Blog title**: "Mica scrivo granché"
- **Language**: Italian (`languageCode = 'it-it'`, `DefaultContentLanguage = "it"`)
- **Main sections**: `mainSections = [ "post" ]` (homepage shows posts)
- **TOC & reading time**: Enabled (`toc = true`, `readingTime = true`)
- **License**: CC BY-NC-SA 4.0 (shown on articles)
- **Comments**: Disabled (`enabled = false`)
- **Color scheme**: Toggle enabled, defaults to `"auto"`
- **Image processing**: Cover and content image optimization enabled

### Categories Configuration
Homepage widgets display:
- Search widget
- Categories (limit: 10)
- Archives (limit: 4, most recent 4 months)

## Extending the Theme

### Partial Templates
- Location: `layouts/partials/`
- Override theme by creating files here (e.g., `footer/include.html`, `sidebar/left.html`)
- Base layout: `layouts/_default/baseof.html` defines main container structure

### Shortcodes
- Location: `layouts/shortcodes/`
- Examples provided: `bottone.html`, `soundcloud.html`, `spotify.html`
- Use in posts: `{{< shortcode_name param="value" >}}`

## Development & Build

### Hugo Commands
- **Local preview**: `hugo server` (watches changes, rebuilds on save)
- **Build for production**: `hugo` (generates `public/` directory)
- **Draft mode**: Set `draft: false` in frontmatter to publish

### Markdown Processing
- **Syntax highlighting**: Enabled with Chroma (line numbers in tables by default)
- **Unsafe HTML**: Enabled (`unsafe = true`) - allows raw HTML in markdown
- **Table of Contents**: Auto-generated from h1-h4 headings, ordered list format

## Common Tasks

**Add a new post:**
1. Create folder: `content/post/<new-slug>/`
2. Create `index.md` with frontmatter (title, date, categories)
3. Add content and any images to same directory
4. Set `draft: false` when ready
5. Build: `hugo` and commit `public/` directory

**Customize styling:**
- Edit `assets/scss/custom.scss` (avoid modifying theme files directly)
- Use responsive breakpoints `@media (max-width: 720px)`
- Hugo pipes handle SCSS compilation automatically

**Add social links:**
- Edit `[[menu.social]]` sections in `hugo.toml`
- Currently: Facebook, Instagram, YouTube, YouTube Music, LinkedIn
- Each entry needs: `identifier`, `name`, `url`, and `icon` parameter

## Known Patterns & Quirks

- **Category system**: Posts are organized by categories like "batteria", "musica", "musica", "produzione", "chitarra", "tecnologia", "altro"
- **Date format inconsistency**: Config uses TOML but frontmatter uses YAML (both supported by Hugo)
- **Theme inheritance**: `hugo-theme-stack` provides base templates; custom overrides take precedence
- **Nested permalinks**: Articles appear at `/p/slug/` (with trailing slash) due to Hugo's directory-based URL generation
