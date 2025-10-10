# GitHub Pages Site with Dynamic Page Loading

This site uses client-side routing to load HTML pages from the `/pages` folder.

## Structure

- `index.html` - Main entry point with navigation and routing logic
- `/pages/` - Individual HTML page content
- `/static/` - Static assets (images, etc.)

## Adding New Pages

1. Create a new HTML file in the `/pages` folder (e.g., `mypage.html`)
2. Add the page to the `PAGES` array in `index.html`:
   \`\`\`javascript
   { name: 'My Page', file: 'mypage.html' }
   \`\`\`
3. The page will be accessible at `/mypage`

## Deployment to GitHub Pages

1. Push this repository to GitHub
2. Go to Settings → Pages
3. Set source to the branch you want to deploy (usually `main` or `gh-pages`)
4. Your site will be available at `https://username.github.io/repository-name/`

## URL Access

- Home: `/` or `/index.html`
- Directory: `/directory`
- Any page: `/pagename` (e.g., `/about`, `/contact`)

The `.nojekyll` file ensures GitHub Pages doesn't process the site with Jekyll.
