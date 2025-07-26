# WordPress Development Proposal Site

A Docsify-powered static site for presenting WordPress development proposals. The site features a professional design with custom typography and is deployed via GitHub Pages.

## Quick Start

### Local Development

1. **Open in VS Code:** Navigate to the `docs/` folder
2. **Start Live Server:** Right-click `index.html` → "Open with Live Server"
3. **Auto-reload:** Live Server will automatically refresh on file changes

### File Structure

```
docs/
├── index.html          # Docsify configuration and setup
├── _coverpage.md       # Landing page cover content
├── _sidebar.md         # Navigation sidebar
├── README.md           # This file (not shown to visitors)
├── styles.css          # Custom styling and typography
├── .nojekyll          # Disables Jekyll processing
└── slides/            # Proposal content sections
    ├── 01-introduction.md
    ├── 02-deliverables.md
    ├── 03-ongoing-costs.md
    └── 04-exclusions.md
```

## Configuration

### Docsify Settings
- **`onlyCover: true`** - Shows only cover page initially
- **Plugins enabled:** Search, Copy Code, Pagination

### Theming
- **Base theme:** Vue theme with custom overrides
- **Typography:** Cormorant Garamond (headings), Open Sans (body), Raleway (accents)
- **Custom styles:** Defined in `styles.css`

### Content Management
- Edit proposal sections in `slides/` directory
- Update navigation in `_sidebar.md`
- Modify cover page in `_coverpage.md`
- Customize styling in `styles.css`

## Deployment

### GitHub Pages Setup
1. **Repository Settings** → **Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main`
4. **Folder:** `/docs` (important!)

### Why `/docs` folder?
- GitHub Pages serves underscore files (`_sidebar.md`, `_coverpage.md`) correctly
- No need for `.nojekyll` in root (though we include one for safety)
- Cleaner separation of site files from project files


## Troubleshooting

**Site shows "Loading..."**
- Check browser console for 404 errors
- Ensure GitHub Pages is set to `/docs` folder
- Verify `.nojekyll` file exists in `docs/`

**Search not working**
- Search plugin requires serving over HTTP (not file://)
- Use local server for testing search functionality
