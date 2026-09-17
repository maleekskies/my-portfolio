# maleekskies: Portfolio

Personal portfolio site for **maleekskies**, a full stack developer, product manager, and content writer working across Web3, AI, and practical software.

**Live site:** [maleekskies.vercel.app](https://maleekskies.vercel.app)

## About

This is a static HTML portfolio, no build step, no framework, no dependencies. All markup, styles, and scripts live in `index.html`.

The site covers:

- **About**: background, current focus, and core stats
- **What I Do**: 5 core skill areas (full stack development, software testing, AI evaluation, content writing, visual storytelling), shown as a tabbed single-view, one skill at a time
- **Projects that I have built**: 8 featured projects, tabbed single-view with screenshots, descriptions, tech stacks, live links, and repo links
- **My Work**: a hub with four in-page views:
  - **Content Writing**: published threads and articles
  - **AI Video Content**: produced video work
  - **Research & Docs**: sourced research documents
  - **Ambassador Work**: content collaborations with VIZO Exchange, Ozak AI, and MegPrimePay
- **Tools I Use**: tech stack organized by category (frontend, backend, AI, tools & design), each with its logo
- **What Drives Me**: 4 short values behind the work
- **Contact**: email, X, Telegram, LinkedIn, and Discord

## Features

- Light/dark theme toggle (preference saved locally)
- Dynamic background: a multi-column scrolling code effect in dark mode (brass/forest palette, glow, depth layering), an interactive particle network in light mode that particles gently drift toward the cursor
- 3D tilt effect on project and tool cards, following the mouse
- Project image carousels (arrows and thumbnail strip), ready for multiple screenshots per project
- Mobile header auto-hides on scroll down, reappears on scroll up
- In-page navigation between sections without full page reloads
- CV download link, in the header on desktop and in the mobile menu on smaller screens
- Custom favicon and social link preview image
- Fully responsive, including a dedicated mobile menu
- Scroll-triggered animations, respecting the "reduce motion" accessibility setting for larger entrance effects

## Tech Stack

- HTML5, CSS3, vanilla JavaScript
- Canvas API for the particle network background
- Google Fonts (Space Grotesk, IBM Plex Mono, Inter)
- Tool icons loaded from devicon and Simple Icons via CDN, with graceful fallback if any icon fails to load
- No build tools, no package manager required

## Files

- `index.html`: the site itself
- `cv.pdf`: linked from the CV button in the nav
- `favicon.ico`, `favicon-32.png`, `favicon-192.png`: browser tab icon, multiple sizes
- `preview.jpg`: the image shown when the site link is shared on social platforms or messaging apps
- `README.md`: this file

## Deployment

This is a static site, so it can be deployed anywhere that serves static files. Upload all the files above together, in the same folder, since `index.html` links to several of them by relative path and they'll break if separated.

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
