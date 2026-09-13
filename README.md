# Admin Dashboard

A responsive admin dashboard layout built as a practice project for **[The Odin Project](https://www.theodinproject.com/)** curriculum, using CSS Grid to structure a real-world, multi-panel application UI.

> **Disclaimer:** This project is **frontend only**, built purely in compliance with The Odin Project's coursework. There is no backend, no real data, no authentication, and no live functionality behind buttons, search, or navigation links. All content (projects, announcements, trending users) is static placeholder data.

## Live Demo

**[https://carnocentaurus.github.io/admin-dashboard/](https://carnocentaurus.github.io/admin-dashboard/)**

## Overview

The dashboard is composed of four main regions, all arranged with CSS Grid:

- **Sidebar** — brand icon and a vertical navigation menu (Home, Profile, Messages, History, Tasks, Communities, Settings, Support, Privacy).
- **Header** — a two-row bar containing a search input, notification bell, user greeting with avatar, and quick-action buttons (New, Upload, Share).
- **Projects panel** — a responsive grid of project cards, each with a title, description, and interactive icon row (favorite, watch, fork).
- **Right sidebar** — an Announcements panel and a Trending panel showing user avatars, usernames, and their project names.

## Features

- Full-page layout built with **CSS Grid** (`grid-template-columns`, `grid-template-rows`, and explicit `grid-area` placement) rather than Flexbox, to practice complex 2D layout structuring.
- Custom `@font-face` declaration for Roboto with `woff2`/`woff` fallbacks and `font-display: swap`, plus font preloading via `<link rel="preload">`.
- SVG icons recolored dynamically using CSS `filter` values (converted from hex colors to `invert()`/`sepia()`/`hue-rotate()` filter chains) instead of shipping multiple icon color variants.
- Hover states throughout — icons shift color, buttons darken, profile images gain a colored border, and text links underline or change color.
- CSS custom properties (`:root` variables) for a consistent color palette and reusable filter values.
- Semantic sectioning with clear HTML comments marking header, dashboard/sidebar, and main content regions.

## Built With

- **HTML5** — semantic structure, no JavaScript
- **CSS3** — Grid layout, custom properties, `filter`, pseudo-classes (`:hover`, `:focus`)
- No frameworks, libraries, or build tools

## Project Structure

```
.
├── index.html
├── style.css
├── fonts/
│   └── Roboto-Regular.woff2 / .woff
├── icons/
│   ├── magnify.svg, bell-ring-outline.svg, star-plus-outline.svg,
│   │   eye-plus-outline.svg, source-fork.svg
│   └── dashboard-icons/
│       ├── view-dashboard.svg, home.svg, account.svg, message.svg,
│       │   clock-outline.svg, file-multiple-outline.svg,
│       │   account-group.svg, cog.svg, help-box.svg, shield-check.svg
├── profile-images/
│   ├── carnocentaurus.png
│   └── Multiavatar-elvio.png, Multiavatar-gilmar.png,
│       Multiavatar-ligeia.png, Multiavatar-morgan.png
└── README.md
```

## Getting Started

This is a static site with no dependencies:

1. Clone or download this repository.
2. Ensure the `fonts/`, `icons/`, and `profile-images/` folders are present alongside `index.html`.
3. Open `index.html` in your browser, or serve it locally (e.g. VS Code's "Live Server" extension) for the best experience with font preloading.

No installation or build step is required — or simply visit the [live demo](https://carnocentaurus.github.io/admin-dashboard/).

## 🧩 What This Project Does *Not* Do

- ❌ No backend or server — the search bar, buttons, and nav links are not wired to any functionality
- ❌ No real user accounts, authentication, or data persistence
- ❌ No JavaScript — interactivity is limited to CSS hover states
- ❌ Project/announcement/trending content is placeholder (Lorem ipsum) data, not real information

## Credits

- Icons courtesy of [Material Design Icons](https://pictogrammers.com/library/mdi/)
- Avatar images generated with [Multiavatar](https://multiavatar.com/)
- Project brief and guidance from [The Odin Project](https://www.theodinproject.com/) curriculum

## License

This project was built for educational purposes as part of The Odin Project coursework and is free to reference or reuse for learning purposes.