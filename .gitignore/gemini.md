
# Gemini Guidelines for letsgoai.co.uk

This document provides guidelines for Gemini (and other AI assistants) on how to interact with the `letsgoai.co.uk` static website project.

## Project Overview

This is a static HTML/CSS/JavaScript website. The main pages are:
- `index.html`: The main landing page for Let's Go AI.
- `markmywordspro.html`: The product page for MarkMy.words Pro.
- `markmywordspro_privacy.html`: The privacy policy for MarkMy.words Pro.

The site uses inlined CSS and JavaScript. There are no build steps or package management tools used.

## Development Workflow

### Running the Website Locally

To preview the website, you can open the HTML files directly in your web browser.

For a better development experience, it is recommended to use a local web server with live reload capabilities. If you have Node.js installed, you can use the `live-server` package:

1. Install `live-server` globally:
   ```bash
   npm install -g live-server
   ```
2. Run `live-server` from the project root:
   ```bash
   live-server
   ```

This will start a local server and open the website in your default browser. The page will automatically reload when you make changes to the files.

### Making Changes

- **Content:** To change the text or structure of a page, edit the corresponding `.html` file.
- **Styling:** All CSS is located within `<style>` tags in the `<head>` of each HTML file. Modify the CSS rules there to change the appearance of the site.
- **Functionality:** All JavaScript is located within `<script>` tags at the end of the `<body>` of each HTML file.
- **Images:** Add new images to the `images/` directory and reference them using a relative path.
- **Icons:** Favicons and app icons are in the `icons/` directory.

### Adding a New Page

1. Create a new `.html` file.
2. You can copy the structure from an existing file (e.g., `markmywordspro.html`) to maintain a consistent header and footer.
3. Add a link to the new page in the navigation or other relevant sections of the existing pages.

## Deployment

This is a static website. To deploy it, you can copy the files to any static web hosting service (e.g., GitHub Pages, Netlify, Vercel, AWS S3).

The `CNAME` file is used by GitHub Pages to configure the custom domain.

## Best Practices

- **Keep it simple:** This is a simple static site. Avoid adding unnecessary complexity, libraries, or build tools unless absolutely necessary.
- **Maintain consistency:** When adding new elements or pages, follow the existing style and structure.
- **Optimize assets:** Before adding new images, make sure they are optimized for the web to ensure fast loading times.
- **Privacy first:** As demonstrated by the `markmywordspro.html` page, the brand values privacy. Do not add any tracking scripts or third-party services that could compromise user privacy, unless explicitly asked.
