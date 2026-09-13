# Responsive Dashboard

A multi-page admin dashboard built with plain HTML, CSS, and a bit of vanilla JavaScript. All pages share a single stylesheet and the same sidebar/header layout, so navigation feels like one cohesive product rather than separate pages.

## Pages

| File | Description |
|---|---|
| `index.html` | Home — KPI cards (Users, Revenue, Orders, Growth), a sales chart panel, a recent activity feed, and a user data table |
| `analytics.html` | Analytics — stat cards (Total Users, Active Users, New Users, Bounce Rate) and a labeled weekly bar chart |
| `users.html` | Users — full directory table with Name, Email, Role, Status, and Joined date |
| `settings.html` | Settings — account preferences with working toggle switches, a language select, and a save button |
| `style.css` | Shared stylesheet used by every page |

## Features

- **Consistent layout** — CSS Grid shell (sidebar + header + main content) reused across all pages
- **Responsive design** — breakpoints at 1024px (tablet), 768px (mobile), and 480px (small mobile)
- **Active nav highlighting** — each page marks its own sidebar item as active
- **Interactive settings** — toggle switches update state and `aria-pressed` on click; Save button confirms changes
- **Reusable components** — cards, panels, tables, and growth indicators (positive/negative) are shared classes used across pages

## Getting started

No build step required. Open `index.html` directly in a browser, or serve the folder with any static file server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## File structure

```
.
├── index.html
├── analytics.html
├── users.html
├── settings.html
└── style.css
```

## Browser support

Uses CSS Grid and Flexbox; works in all modern evergreen browsers (Chrome, Firefox, Safari, Edge).
