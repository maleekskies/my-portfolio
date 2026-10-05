# maleekskies: Portfolio

Personal portfolio site for **maleekskies**, a full stack developer building AI automation, with software testing & QA and content writing experience across Web3, AI, and practical software.

**Live site:** [maleekskies.vercel.app](https://maleekskies.vercel.app)

## About

This is a static HTML portfolio, no build step, no framework, no dependencies. All markup, styles, and scripts live in `index.html`.

The site covers:

- **About**: background, current focus, and core stats
- **What I Do**: 4 core skill areas (Full Stack Development, AI Automation, Software Testing & QA, Content Writer), shown as a tabbed single-view, one at a time
- **Featured projects**: 4 highlighted projects (VAULT 01, ChessHatch, Huntboard, OZ Handcrafted Footwear) on an interactive 3D ring carousel of compact cards; tapping a card opens a details panel with the full description, tech stack, links, and a swipeable gallery of screenshots
- **My Work**: a hub with four in-page views, with Full Stack Development and AI Automation first:
  - **Full Stack Development**: all 9 projects with screenshots, descriptions, tech stacks, live links, and repo links
  - **AI Automation**: the Skies Realty AI lead-management case study, with a pipeline diagram
  - **Content Writing**: published threads and articles
  - **Research & Docs**: sourced research documents
- **Tools I Use**: tech stack organized by category (frontend, backend, AI, tools & design), each with its logo
- **What Drives Me**: 4 short values behind the work
- **Contact**: email, X, Telegram, LinkedIn, and Discord

## Features

- Light/dark theme toggle (preference saved locally)
- Dynamic background: a multi-column scrolling code effect in dark mode (brass/forest palette, glow, depth layering), an interactive particle network in light mode that particles gently drift toward the cursor
- 3D ring carousel for featured projects: drag, swipe, arrow buttons, or arrow keys to rotate; the front card tilts and catches a light glare following the mouse; clicking a side card brings it forward
- Project details panel: a bottom sheet on mobile and a centered window on desktop, with a screenshot gallery (swipe, arrows, or arrow keys), closing with the X, the Escape key, or a tap outside
- 3D tilt effect on skill and tool cards, following the mouse
- Skies Realty case study with a pipeline diagram (form, n8n, scoring, local AI summary, CRM, Telegram alert)
- Mobile header auto-hides on scroll down, reappears on scroll up
- In-page navigation between sections and views without full page reloads
- CV download link, in the header on desktop and in the mobile menu on smaller screens
- Custom favicon and social link preview image
- Fully responsive, including a dedicated mobile menu
- Scroll-triggered animations; the 3D motion and orbit animation respect the "reduce motion" accessibility setting

## Tech Stack

- HTML5, CSS3, vanilla JavaScript
- CSS 3D transforms for the project carousel, Canvas API for the particle network background
- Google Fonts (Space Grotesk, IBM Plex Mono, Inter)
- Tool icons loaded from devicon and Simple Icons via CDN, with graceful fallback if any icon fails to load
- No build tools, no package manager required

## Editing the projects

Each project is written once, as a hidden card inside the `projectStore` block near the bottom of `index.html`. The home-page ring, the details panel, and the full projects list are all built from those cards, so editing a project there updates every place it appears. The four ring projects and their order are set by the `featured` list at the top of the "Featured projects" script.

## Adding pictures to a project's gallery

Screenshots live in the `images` folder. In the same script, find the `GALLERY` list: each project has lines like `['images/huntboard-inbox.jpg', 'Caption shown under the picture']`. Add a line for each new picture (the word `cover` means the project's existing card image). A project with no entry just shows its card image, with no arrows. For fast loading, keep screenshots around 800px wide and save them as JPEG.

## Adding screenshots to the Skies Realty case study

Find the `SCREENSHOTS` comment inside the case study (the AI Automation page) in `index.html`. It contains a ready-made block: add your images to the `images` folder, uncomment the block, and point each `src` at your file. Blur or replace any real names, phone numbers, or emails first.

## Files

- `index.html`: the site itself
- `cv.pdf`: linked from the CV button in the nav
- `favicon.ico`, `favicon-32.png`, `favicon-192.png`: browser tab icon, multiple sizes
- `preview.jpg`: the image shown when the site link is shared on social platforms or messaging apps
- `images/`: screenshots shown in the project details panel
- `README.md`: this file

## Deployment

This is a static site, so it can be deployed anywhere that serves static files. Upload all the files above together, in the same folder (including the `images` folder), since `index.html` links to several of them by relative path and they'll break if separated.

- **Netlify Drop**: drag and drop the folder at [app.netlify.com/drop](https://app.netlify.com/drop)
- **Vercel**: create a project and upload the folder
- **GitHub Pages**: push the files to this repo, then enable Pages in Settings > Pages, pointing to the main branch

No build command or install step is needed. `index.html` just needs to stay named that so it's served as the homepage.

## Local Preview

Open `index.html` directly in any browser. No server required.

## Contact

- Email: maleekskies@gmail.com
- X: [@maleekskies](https://x.com/maleekskies)
- Telegram: [@maleekskies](https://t.me/maleekskies)
- LinkedIn: [maleekskies](https://www.linkedin.com/in/maleekskies/)
- Discord: @maleekskies (copy the handle from the site, Discord doesn't support a direct profile link by username alone)
